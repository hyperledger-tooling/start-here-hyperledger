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
                PR <a href="https://github.com/hyperledger/solang/pull/1020" class=".btn">#1020</a>
            </td>
            <td>
                <b>
                    Update issue templates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add template for new issues
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-20 14:22:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1018" class=".btn">#1018</a>
            </td>
            <td>
                <b>
                    Fix AddMod and MulMod
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes three bugs in the implementation of AddMod and MulMod.

1. In Yul, `addmod` and `mulmod` were not implemented correctly, because 512-bit operations were not in use. To fix this, those builtins now call `Builtin::AddMod` and `Builtin::MulMod`.
2. `Builtin::AddMod` was calculating `(a+b)/c` instead of `(a+b)%c`.
3. `Builtin::MulMod` was calcuating `(a*b)/c` instead of `(a+b)%c`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-19 03:35:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1017" class=".btn">#1017</a>
            </td>
            <td>
                <b>
                    Post release cleanups
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Use v0.1.3 label
- Remove unused parts of workflow
- vscode extension 0.3.1 was published
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-17 10:10:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1016" class=".btn">#1016</a>
            </td>
            <td>
                <b>
                    Release v0.1.13: Genoa
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                v0.1.13 Genoa

### Changed
- Introduce sub-commands to the CLI. Now we have dedicated sub-commands for
  `compile`, `doc`, `shell-completion` and the `language-server`, which makes
  for a cleaner CLI.
  [seanyoung](https://github.com/seanyoung)
- On Solana, emitted events are encoded with Borsh encoding following the Anchor
  format.
  [LucasSte](https://github.com/LucasSte)
- The ewasm target has been removed, since ewasm is not going to implemented on
  Ethereum. The target has been reused for an new EVM target, which is not complete
  yet.
  [seanyoung](https://github.com/seanyoung)
- Substrate: Concrete contracts must now have at least one public function. A
  public function is in a contract, if it has public or external functions, if
  it has a receive or any fallback function or if it has public storage items
  (those will yield public getters). This aligns solang up with `ink!`.
  [xermicus](https://github.com/xermicus)

### Added
- Solana v1.11 is now supported.
  [seanyoung](https://github.com/seanyoung)
- On Solana, programs now use a custom heap implementation, just like on
  Substrate. As result, it is now possible to `.push()` and `.pop()` on
  dynamic arrays in memory.
  [seanyoung](https://github.com/seanyoung)
- Arithmetic overflow tests are implemented for all integer widths,
  [salaheldinsoliman](https://github.com/salaheldinsoliman)
- Add an NFT example for Solana
  [LucasSte](https://github.com/LucasSte)
- Add a wrapper for the Solana System Program
  [LucasSte](https://github.com/LucasSte)
- The selector for functions can be overriden with the `selector=hex"abcd0123"`
  syntax.
  [seanyoung](https://github.com/seanyoung)
- Shell completion is available using the `solang shell-completion` subcommand.
  [xermicus]([https://github.com/xermicus)
- Add support for the `create_program_address()` and `try_find_program_address()`
  system call on Solana
  [seanyoung](https://github.com/seanyoung)
- Substrate: The `print()` builtin is now supported and will write to the debug
  buffer. Additionally, error messages from the `require` statements will now be
  written to the debug buffer as well. The Substrate contracts pallet prints the
  contents of the debug buffer to the console for RPC ("dry-run") calls in case
  the `runtime::contracts=debug` log level is configured.
  [xermicus](https://github.com/xermicus)

### Fixed
- DocComments `/** ... */` are now permitted anywhere.
  [seanyoung](https://github.com/seanyoung)
- Function calls to contract functions via contract name are no longer possible,
  except for functions of base contracts.
  [xermicus](https://github.com/xermicus)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-16 15:46:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1015" class=".btn">#1015</a>
            </td>
            <td>
                <b>
                    Refactor emit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR refactors the emit code. The largest problem there was that `emit/mod.rs` has about 10 thousand lines, making it difficult to navigate. Here is a summary of my changes:

1. The trait `TargetRuntime` only defines an interface for behaviors that are not shared between targets. All shared implementations are now standalone functions.
2. I created a `StorageSlot` to be an interface for storage management functions for environments that depend on storage slots, like Substrate and EVM.
3. Target specific code is separated into folders. Code emission for Solana is under `emit/solana` and for Substrate, under `emit/substrate`.
4. The implementation of the `TargetRuntime` trait is located in `emit/<target>/target.rs`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-15 18:40:26 +0000 UTC
    </div>
</div>

