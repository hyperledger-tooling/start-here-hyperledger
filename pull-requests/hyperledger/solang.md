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
                PR <a href="https://github.com/hyperledger/solang/pull/1455" class=".btn">#1455</a>
            </td>
            <td>
                <b>
                    Bugfix: Do not make assumptions about storage variable reads
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Contracts can get upgraded so we must not make any assumptions whether a storage variable is read or not; writes to storage variables must happen regardless whether the variable is never read.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-23 12:14:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1454" class=".btn">#1454</a>
            </td>
            <td>
                <b>
                    Bubble reverts
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
        Created At 2023-07-21 20:52:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1452" class=".btn">#1452</a>
            </td>
            <td>
                <b>
                    Bugfix: Strength reduce must not optimize mul into shl if overflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Optimizing multiplications with a SHL must not disable overflow checks.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-20 18:06:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1449" class=".btn">#1449</a>
            </td>
            <td>
                <b>
                    Polkadot: Reverts return encoded error data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a continuation of #1415. `require()`, `assert()` and `revert()` now return error data, according to the [Solidity documentation](https://docs.soliditylang.org/en/v0.8.20/control-structures.html#panic-via-assert-and-error-via-require). Additionally, many reverts inserted by the compiler now return the corresponding `Panic(uint256)`  error data, to align Solang closer with `solc`.

The error types known to the contract are added in the metadata `lang_error` field. At the moment there are only `Error` and `Panic` because we don't support custom errors yet.

Refactored revert-related code into a dedicated `codegen` module to. Refactored the `polkadot::errors` into distinct tests, made them less brittle and added assertions for the execution output.

I'm now working on a follow-up PR for bubbling up uncaught exceptions (this is why it's already included that in the documentation).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-19 17:24:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1448" class=".btn">#1448</a>
            </td>
            <td>
                <b>
                    Allow modification of AcconuntInfo lamports field
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The field `lamports` of the struct `AccountInfo` is mutable, so we should allow its modification. For this we needed two modifications:

1. lamports is of type `Type::Ref(Type::Ref(Type::Uint(64)))` after accessing the struct member, we needed to include an extra load in sema do deal with the double pointer.
2. When we have `AccountInfo ai = tx.accounts[0];`, `ai` becomes a pointer to AccountInfo. The unused variable elimination was incorrectly eliminating references to structs, so I fixed such an issue.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-18 14:44:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1447" class=".btn">#1447</a>
            </td>
            <td>
                <b>
                    Bugfix: Accessing virtual function selectors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The added test case panics in current `main` because accessing the selector of a virtual function which is not used in any other way will put the function in `all_functions` but not `virtual_functions`.  `check_inheritance` will insert the function into `all_functions` because we have this symbol, however because we only access the selector it's not a virtual function to the contract. The fix is that when we walk `all_functions` to find the externally callable ones, do not assume every function marked `virtual` is present in the `virtual_functions` of this contract.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-18 12:59:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1446" class=".btn">#1446</a>
            </td>
            <td>
                <b>
                    Add debug implementations required to print Namespace
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Derive `Debug` implementations for structs and enums required to print `struct Namespace`. This is of use when one needs to print `Namespace` struct for debugging purposes. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-18 01:29:39 +0000 UTC
    </div>
</div>

