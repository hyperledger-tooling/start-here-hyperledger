---
layout: default
title: firefly-transaction-manager
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-transaction-manager
---

# firefly-transaction-manager <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-transaction-manager){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/46" class=".btn">#46</a>
            </td>
            <td>
                <b>
                    Add AddressBalance() to FFCAPI and a new REST API route to call it
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The aim of this PR is to add an address balance API call to the FFCAPI interface. This makes it possible for users of of the FFCAPI (such as FireFly Transaction Manager) to query and optionally surface via their own APIs.

Under this PR I have introduced a new REST API `/gastoken/balances/{address}` which calls `AddressBalance()` for the the configured blockchain connector. The use of `gastoken` in the API path is intended to be clear that it is unrelated to token balances.

Signed-off-by: Matthew Whitehead <matthew.whitehead@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-08 13:21:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/45" class=".btn">#45</a>
            </td>
            <td>
                <b>
                    Reduce the size of websocket updates for transactions.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Subscribers can use /transactions/{txid} to provide full detail about a transaction if required.

Delivered as part of closing https://github.com/hyperledger/firefly/issues/1108

Signed-off-by: Matthew Whitehead <matthew.whitehead@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-05 12:57:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/44" class=".btn">#44</a>
            </td>
            <td>
                <b>
                    Add Errors spec support to contract deploy request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jim Zhang <jim.zhang@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-05 02:34:41 +0000 UTC
    </div>
</div>

