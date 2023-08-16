---
layout: default
title: solang
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1488" class=".btn">#1488</a>
            </td>
            <td>
                <b>
                    Produce error diagnostics if overflow occurs in constant folding
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The negate operator does not check for overflow, add this too.

Fixes https://github.com/hyperledger/solang/issues/1484
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-15 08:37:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1487" class=".btn">#1487</a>
            </td>
            <td>
                <b>
                    Bring import resolution in line w/ Solc's
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Solang's import resolution departs from solc's in several key ways. I've spent quite a bit of time trying to understand how solc's import system works (it's very bad), and how Solang differs. This has been both through reading code and through experimenting with both systems.

I've compiled a set of tests [here](https://github.com/BenTheKush/solc_remapping_behavior_test). These tests show differences in behavior between the import resolution (this includes filename resolution specified from CLI, remapping behavior, import path behavior, etc etc).

This PR is attempting to bring solang's implementation in line with my understanding of the solidity documentation. It's currently a draft and is rough around the edges (including debug println statements so I can figure out control flow, etc).

## Differences between Solang and Solc

### 1. Remap Targets
Solang and Solc treat the target of a remapping `map=target` very differently.

+ **Solc:** In solc, when an import statement of the form `import "map/path/to/Foo.sol";` is encountered, solc will attempt to remplace `map` with `target` and then resolve this new replaced version of the import path against the base-path and any specified include-paths.

  **Note:** from the current working director, the path specified by `target` DOES NOT NEED TO EXIST!
  
+ **Solang:** Solang [canonicalizes the target](https://github.com/hyperledger/solang/blob/90c687ecb52dd4c75adda3c52443c0b5725ab16c/src/file_resolver.rs#L43); if the target does not exist compilation immediately fails. Worse, this canonicalization may be valid but point to a _different_ target than what was expected by the developers. This could silently lead to incorrect files being imported, leading to potential security risks.

The fix is to remove the call to `.canonicalize()`

Another bug is that when a remapping applies then it _must_ be applied.

Consider the following setup:`Contract.sol` imports `import "lib/A.sol";`, which exists in `resources/node_modules/lib/A.sol`. 

+ **Solc:** Compiling with `solc Contract.sol lib=resources/node_modules/lib --base-path node_modules` fails, _even though the imported path `lib/A.sol` can be appended to the base path `resoucres/node_modules` to get the correct path `resources/node_modules/lib/A.sol`_. This is because the remapping `lib=node_modules/lib` __modifies__ the imported path `lib/A.sol` to `node_modules/lib/A.sol`, and then _this path_, not the original imported path, is used to resolve against the base-path.

+ **Solang:** Compiling with `solang --target solana Contract.sol -m lib=resources/node_modules/lib -Inode_modules` succeeds.

The fix is to apply a remapping when possible and not allow the original imported path to be used for resolution.
**EDIT:** After some experimenting with solc it appears that _the last remapping_ is always the one that is applied!
Note that these are not cumulative: each successive remapping is applied to the original import path, replacing any other remappings that applied:

```
solc a=good C.sol                 # good
solc a=good a=bad C.sol           # bad
solc a=bad a=good C.sol           # good
solc a=good a=bad a=good C.sol    # good
```

### 2. Incorrect Direct Imports

A _direct import_ is any import that doesn't start with `"./"` or `"../"` (these are relative imports). 

+ **Solc:** resolves direct imports against the `--base-path` and any specified `--include-path`s

+ **Solang:** currently attempts to [resolve an import path by canonicalizing it in the host filesystem](https://github.com/hyperledger/solang/blob/90c687ecb52dd4c75adda3c52443c0b5725ab16c/src/file_resolver.rs#L209-L213)
  ```rust
        if let Some(file) = self.try_file(filename, &path, None)? {
            return Ok(file);
        } else if path.is_absolute() {
            return Err(format!("file not found '{}'", filename.to_string_lossy()));
        }
  ```
  
  This is correct behavior only when this is a file specified from CLI, which is true iff parent is `None` (at least, according to the current implementation). The easiest solution is to change the above lines to:
  
  ```rust
    if parent.is_none(){
        if let Some(file) = self.try_file(filename, &path, None)? {
            return Ok(file);
        }
        return Err(format!("file not found '{}'", filename.to_string_lossy()));
    }
  ```
  
  **Note:** when parent is none and try_file failed we fail (as opposed to only when it was an absolute path). Why? Because a file specified from CLI is a path in the _host file system_, not the _virtual file system_. This means that if `canonicalize()` fails, it's a bad filename.

### 3. Ambiguous Imports should Fail

An ambiguous import (i.e., an import path that can be resolved multiple ways given the configuration) should fail. This is specified in solidity docs. It's also undesirable to have import map order not commute (i.e., `-I a -I b` results in a different binary than `-I b -I a`). 


The fix for this is to create a list of resolved files and then, if there is more than one, report an error and list all resolved file paths. Example from solc where I specified the same import root twice, causing multiple resolutions, once for each redundant occurance of the `.` import root:

![Screen Shot 2023-08-14 at 9 51 33 PM](https://github.com/hyperledger/solang/assets/128326394/fbe9510a-af59-437b-a71d-58da569b01c9)

### 4. Remapping's maps should support multi-path segments

A remap like `a/b/c=target` is valid according to solidity docs/solc. I've replaced the [previous `iter()`/`first()` based implementation](https://github.com/hyperledger/solang/blob/90c687ecb52dd4c75adda3c52443c0b5725ab16c/src/file_resolver.rs#L216-L218):

```rust
        let mut iter = path.iter();
        if let Some(first_part) = iter.next() {
            let relpath: &PathBuf = &iter.collect();
```

with a `strip_prefix()` based implementation.


### 5. Solc's import path specification is _non-monotonic_

By this I mean that you can add an import path (specifically `--base-path`), and previously valid imports will now become _invalid_. YUCK.

This is because the default `--base-path` is `""`, and this gets _replaced_ when you specify an import path. This is gross and leads to disgusting edge cases. I'll expand more on this later
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-15 05:00:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1486" class=".btn">#1486</a>
            </td>
            <td>
                <b>
                    Use named constants instead of magic numbers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Using magic numbers degrades code readability.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 20:51:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1485" class=".btn">#1485</a>
            </td>
            <td>
                <b>
                    Avoid overflow in transfer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `address.transfer` and `address.send` utilize `void sol_transfer` from `solana.c` under the hood, which was saving the overflowed valued to the account balance. This PR fixes such an issue.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 17:56:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1483" class=".btn">#1483</a>
            </td>
            <td>
                <b>
                    Use Ubuntu 20.04 rather than 22.04
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We've had a few users reporting that solang does not work in their environment; usually this is ubuntu 20.04 WSL.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-10 08:00:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1482" class=".btn">#1482</a>
            </td>
            <td>
                <b>
                    Polkadot: Integration tests use Polkadot v1.0.0 node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update integration tests to use the latest CI node build containing a substrate node built against `polkadot-v1.0.0`.

Some tests required changes in their weight calculations.

I allowed to take some shortcuts with upgrading the subxt tests. Because we have a student working on making the extrinsics library from cargo-contract re-usable, it'd be a waste spending too much time there (plan is to then use this in the CLI and the integration).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-09 10:58:39 +0000 UTC
    </div>
</div>

