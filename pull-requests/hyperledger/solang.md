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
                PR <a href="https://github.com/hyperledger/solang/pull/1459" class=".btn">#1459</a>
            </td>
            <td>
                <b>
                    Do not overwrite accounts' signer and writer flags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When we traverse a functions to collect accounts, we may add the same account multiple times. IndexMap overwrites the entry in the table, whenever we add the same key again. We should not overwrite the writer and signer flags, however.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 21:30:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1458" class=".btn">#1458</a>
            </td>
            <td>
                <b>
                    Polkadot does not yet support catching Panics or custom errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This isn't implemented yet in codegen and it won't make it into the July release (planned for August).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-23 20:33:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1457" class=".btn">#1457</a>
            </td>
            <td>
                <b>
                    Bugfix: External functions read their variable if they are called
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
        Created At 2023-07-23 18:59:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1456" class=".btn">#1456</a>
            </td>
            <td>
                <b>
                    Remove unnecessary .into_iter() and raw string
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These are clippies in the next rust version.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-23 13:48:20 +0000 UTC
    </div>
</div>

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
                    Polkadot: Bubble up reverts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a continuation of #1415. To align Solang with `solc` further, any uncaught reverts must be bubbled up back to the caller. To do so, handling of the return code for `call`, `instantiate` and `transfer` runtime API calls is now done in codegen and no longer treated as a bool.

Parts of this PR can be tested much better after #1449 is in `main`, but it is ready for a first review round.
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

