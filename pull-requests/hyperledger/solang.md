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
                PR <a href="https://github.com/hyperledger/solang/pull/1438" class=".btn">#1438</a>
            </td>
            <td>
                <b>
                    Create PDA hash table example
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I saw an example of a PDA hash table on [Anchor's website](https://www.anchor-lang.com/docs/pdas#hashmap-like-structures-using-pd-as). I liked it and wanted to replicate it in Solidity.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-07 15:15:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1437" class=".btn">#1437</a>
            </td>
            <td>
                <b>
                    Update roadmap
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I changed the roadmap to reflect what we are working on right now. Calling Solidity from Rust is not even in our backlog, so I removed it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-07 13:17:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1432" class=".btn">#1432</a>
            </td>
            <td>
                <b>
                    Identify externally callable functions in `sema`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The information whether a given function is supposed to be reachable via an external call to the contract is currently done directly in `codegen`. However, we need this information during the ABI generation too. This fixes a bug where inherited public functions would end up duplicated in the contract metadata.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-06 16:32:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1431" class=".btn">#1431</a>
            </td>
            <td>
                <b>
                    Remove unwanted files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These files are temporary and automatically generated during tests. They have been included in the repository.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-06 15:47:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1427" class=".btn">#1427</a>
            </td>
            <td>
                <b>
                    Do not return arguments of revert
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR solves #1152. @salaheldinsoliman has already done most of the job. I certified that the parameter string in `revert` is indeed printed and removed all returns on Solana, as they have no effect (Anchor does not decode return data when a function reverts).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 21:24:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1426" class=".btn">#1426</a>
            </td>
            <td>
                <b>
                    Avoid narrowing casts from `size_t` to `uint32_t`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I changed all occurrences of `size_t` to `uint32_t`, except for `sol_memset` from `solana_sdk.h`.
Converting from `size_t` to `uint32_t` could cause an overflow on Solana.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 18:37:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1423" class=".btn">#1423</a>
            </td>
            <td>
                <b>
                    Minor code improvements (nfc)
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
        Created At 2023-07-05 11:17:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1422" class=".btn">#1422</a>
            </td>
            <td>
                <b>
                    Add Solana minimum balance library
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add runtime function for calculating the balance required for instantiating a contract of a certain size.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 10:26:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1421" class=".btn">#1421</a>
            </td>
            <td>
                <b>
                    Bugfix: Type of `Error(string)` selectors should be `bytes4`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Avoiding using the integer type for [`Error(string)`](https://docs.soliditylang.org/en/latest/control-structures.html#panic-via-assert-and-error-via-require) selectors avoids endianess swaps resulting in the wrong value.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-04 12:27:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1420" class=".btn">#1420</a>
            </td>
            <td>
                <b>
                    `Display` our compilation targets with capitalization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As Lucas suggested on #1414
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-04 07:52:22 +0000 UTC
    </div>
</div>

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
                    Polkadot: `AssertFailure` emits revert instead trap
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

