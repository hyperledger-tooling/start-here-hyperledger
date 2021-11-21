---
layout: default
title: solang
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/573" class=".btn">#573</a>
            </td>
            <td>
                <b>
                    Use the latest @solana/solidity npm version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-19 12:59:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/572" class=".btn">#572</a>
            </td>
            <td>
                <b>
                    Fix contract in mappings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #557 

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-19 10:54:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/571" class=".btn">#571</a>
            </td>
            <td>
                <b>
                    Move to llvm 13.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-19 10:15:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/570" class=".btn">#570</a>
            </td>
            <td>
                <b>
                    Increase stack size on Windows to 8MB
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Both Mac and Linux already use a 8MB stack by default.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-18 15:02:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/569" class=".btn">#569</a>
            </td>
            <td>
                <b>
                    Vector to slice pass creates invalid phi nodes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If the vector to slice pass updates one incoming value for a phi node,
but not another we end up with a phi node that is invalid; one entry
is a vector and the other a slice.

This fix does the following.

1. First collect all the set instructions we are going to update.
2. For all phi nodes, check if there are any reaching definitions we
   are not updating.
3. If any reaching definition for the phi node is not updated, then do
   not update any of them.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-17 17:52:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/567" class=".btn">#567</a>
            </td>
            <td>
                <b>
                    Do not link against libffi
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                libffi is not needed and we shouldn't depend on it.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-16 14:49:02 +0000 UTC
    </div>
</div>

