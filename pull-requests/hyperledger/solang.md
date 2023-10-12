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
                PR <a href="https://github.com/hyperledger/solang/pull/1563" class=".btn">#1563</a>
            </td>
            <td>
                <b>
                    Bugfix struct member read access (take 2)
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
        Created At 2023-10-12 11:12:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1562" class=".btn">#1562</a>
            </td>
            <td>
                <b>
                    Each call to new_scope() should be matched with leave_scope()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The try catch blocks had an additional new_scope() which is incorrect. I think the extra scope is harmless but let's clean it up.

Rename `new_scope()` to `enter_scope()` as this matches `leave_scope()` better.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-09 11:26:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1560" class=".btn">#1560</a>
            </td>
            <td>
                <b>
                    Completion
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
        Created At 2023-10-06 12:34:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1559" class=".btn">#1559</a>
            </td>
            <td>
                <b>
                    Fix clippy 1.73 warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I updated Rust in my computer and fixed the errors from clippy.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-05 22:01:10 +0000 UTC
    </div>
</div>

