---
layout: default
title: grid
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/grid
---

# grid <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/grid){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1220" class=".btn">#1220</a>
            </td>
            <td>
                <b>
                    Stabilize `rest-api-resources-purchase-order`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This stabilizes the `rest-api-resources-purchase-order` feature by
moving it from `experimental` to `stable`.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-03 18:12:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1219" class=".btn">#1219</a>
            </td>
            <td>
                <b>
                    Stabilize `purchase-order` in gridd
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
        Created At 2022-01-03 15:46:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1217" class=".btn">#1217</a>
            </td>
            <td>
                <b>
                    Validate alternate ID formats
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds tests to validate alt ID parsing. Enforces format of alt ID inputs.

Previously, invalid alt IDs were accepted. Also, users would receive
`status_code:500` errors when invalid alt IDs were provided.

Resolves: #1212
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-31 00:39:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1213" class=".btn">#1213</a>
            </td>
            <td>
                <b>
                    Update "update po" action in po smart contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates the "update_purchase_order" method to handle a list of versions. This also updates the method to correctly handle versions depending on the intended update state. This also updates the related tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-30 15:04:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1210" class=".btn">#1210</a>
            </td>
            <td>
                <b>
                    Update `po update` command to allow simultaneous version updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds options and flags to enable simultaneous changes to purchase orders and
versions in situations where step-wise updates would lead to invalid states.

Users may only update the components of the version workflow state that must
be changed to avoid invalid states when updating purchase orders.

Resolves: #1202, #1183

Requires: #1199
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-28 20:10:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1207" class=".btn">#1207</a>
            </td>
            <td>
                <b>
                    Update "create purchase order" action in po handler
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the structure and layout of the purchase order smart contract's create po action. This also updates the tests to be valid with the additional validation checks happening in the smart contract. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-28 16:31:23 +0000 UTC
    </div>
</div>

