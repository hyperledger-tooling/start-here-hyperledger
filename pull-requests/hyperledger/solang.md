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
                PR <a href="https://github.com/hyperledger/solang/pull/1419" class=".btn">#1419</a>
            </td>
            <td>
                <b>
                    Add resolved files to FileResolver
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR:
1. Adds a `resolved_files: Vec<ResolvedFile>` field to `FileResolver`;
2. Populates it during the execution of `FileResolver.resolve_file()`;
3. Extends `FileResolver`'s API with `get_resolved_file(file_no: usize)` to allow access of this data.
 
Prior to this PR, the resolution root of each file is discarded after `parse_and_resolve` and has to be recomputed by a client (and this recomputation depends on implementation-specifics such as source root visit order during file resolution). This PR persists this data.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-03 20:49:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1418" class=".btn">#1418</a>
            </td>
            <td>
                <b>
                    Unbreak build updating target to Solana in solana tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Merging https://github.com/hyperledger/solang/pull/1413 broke the build as `.substrate_default()` no longer exists.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-03 20:31:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1417" class=".btn">#1417</a>
            </td>
            <td>
                <b>
                    Bump all crate dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I tried updating subxt tests, but there are breaking changes which I don't understand
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-03 13:30:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1416" class=".btn">#1416</a>
            </td>
            <td>
                <b>
                    Bump solana-rbpf crate to 0.5.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This makes it possible to use rust 1.70.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-03 13:23:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1415" class=".btn">#1415</a>
            </td>
            <td>
                <b>
                    Substrate: `AssertFailure` emits revert instead trap
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Using the `seal_return` API with the revert flag instead of just trapping the contract execution allows to return data. This is required for further alignment with [solc](https://docs.soliditylang.org/en/latest/control-structures.html#panic-via-assert-and-error-via-require). 

Closes #1292
Unblocks #916
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-03 07:23:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1414" class=".btn">#1414</a>
            </td>
            <td>
                <b>
                    Rename Substrate to Polkadot
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As per #1398 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-02 18:12:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1413" class=".btn">#1413</a>
            </td>
            <td>
                <b>
                    Ensure that doccomments still work when a function has an annotation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Annotations stop doc tags from working on functions

```solidity
contract c {
      /// comment is free
      @selector([1,2,3,4])
      function foo() public {}
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-02 15:59:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1412" class=".btn">#1412</a>
            </td>
            <td>
                <b>
                    Fix some typos in docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-01 14:37:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1411" class=".btn">#1411</a>
            </td>
            <td>
                <b>
                    Implement Goto Definition functionality in the language server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-01 13:26:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1409" class=".btn">#1409</a>
            </td>
            <td>
                <b>
                    Fix undefined variable detection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The contract I added in the tests was working properly in Solang v0.3.0, but it caused a panic in [this line](https://github.com/hyperledger/solang/blob/a84b0ad3b67a17b524ef6b7437fd4c5376833807/src/codegen/strength_reduce/expression_values.rs#L79) on the main branch. 

I couldn't identify what has changed from the release till now, but I deemed the logic for reporting undefined variables and stop optimizations erroneous.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 21:11:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1408" class=".btn">#1408</a>
            </td>
            <td>
                <b>
                    Added get_contents_of_file_no
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a public way to get the file contents from a file number. I've defaulted to a verbose function name, but happy to change that if folks like (e.g., maybe just `get_contents(file_no: usize)`, but that's a little awkward because of `set_contents(path: &str, contents: String)`... I feel like `get_XXX` and `set_XXX` should have the same type for `XXX` (in this case `file_no`'s `usize` would conflict with `path`'s `&str`)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 16:53:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1407" class=".btn">#1407</a>
            </td>
            <td>
                <b>
                    Change `log_runtime_error` call
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix for a problem resulting from merging #1400.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 14:25:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1405" class=".btn">#1405</a>
            </td>
            <td>
                <b>
                    Substrate: Distinct dispatch CFG for `call` and `deploy`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix an oversight form #1249. The dispatch logic can not be the same for `call` and `deploy` as constructors must _not_ be allowed to be accessed from the `call` function.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 00:09:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1404" class=".btn">#1404</a>
            </td>
            <td>
                <b>
                    v0.3.1: Göttingen release (aka June release)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release tests are running [here](https://github.com/LucasSte/solang/actions/runs/5395030402).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-27 22:03:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1403" class=".btn">#1403</a>
            </td>
            <td>
                <b>
                    Move stdlib build output to `target` folder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a fix for #1321.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-27 21:11:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1402" class=".btn">#1402</a>
            </td>
            <td>
                <b>
                    Ensure that a constructor cannot be run twice on the same data account
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The constructor code path was not checking that the data account magic number is not populated.

The change also exposed another issue: when a pure function is called, there should be no load of data magic number, this may result in a access violation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-27 09:22:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1401" class=".btn">#1401</a>
            </td>
            <td>
                <b>
                    Make rust analyzer work again
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This slipped in, nuke it to fix RA
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-27 08:04:01 +0000 UTC
    </div>
</div>

