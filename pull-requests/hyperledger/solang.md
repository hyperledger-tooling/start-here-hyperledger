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
                PR <a href="https://github.com/hyperledger/solang/pull/1366" class=".btn">#1366</a>
            </td>
            <td>
                <b>
                    Refactor constructor annotations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Presently, we can declare an account on a Solana constructor using the `@payer(my_account)` annotation, while `@seed(my_seed)` refers to a constructor parameter. Such a construction is confusing for the same syntax have two different meanings.

This PR limits the scope of annotation above a constructor to accept only literals as parameters (e.g. `@seed("pine_tree")`). Annotations that refer to function parameters must appear before them: `constructor (@seed bytes arg1)`. This is another in #1251.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-14 21:06:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1365" class=".btn">#1365</a>
            </td>
            <td>
                <b>
                    `wasm-opt` for Substrate 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `wasm-opt` brings some great optimizations and we should use it (`cargo contract` uses it for ink contracts). For example, the Wasm blob of our flipper example (compile `--release`) goes down from 2.2kb to 1.2kb. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-13 21:16:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1364" class=".btn">#1364</a>
            </td>
            <td>
                <b>
                    Fix codegen tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Make the failing case less brittle
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-13 18:00:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1363" class=".btn">#1363</a>
            </td>
            <td>
                <b>
                    Update Address and Hash types to ink ABI v4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This slipped through integration tests because the frontends remain backwards compatibility. I added a test that would have caught it (based of it, more can be added in the future).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-13 08:33:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1362" class=".btn">#1362</a>
            </td>
            <td>
                <b>
                    Implement `is_contract` builtin 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #1333
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-12 09:49:40 +0000 UTC
    </div>
</div>

