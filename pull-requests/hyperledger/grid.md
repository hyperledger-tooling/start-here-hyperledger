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
                PR <a href="https://github.com/hyperledger/grid/pull/1226" class=".btn">#1226</a>
            </td>
            <td>
                <b>
                    Rename remaining `workflow_type`s to `workflow_id`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This replaces any remaining instances of `workflow_type` with the new terminology `workflow_id`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-05 19:06:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1225" class=".btn">#1225</a>
            </td>
            <td>
                <b>
                    Update permissions to use seller
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Permissions were incorrectly set to buyer. Updated to be seller.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-05 15:56:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1223" class=".btn">#1223</a>
            </td>
            <td>
                <b>
                    Add ability to add/update POs/versions by alternate ID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds the ability to update POs, add/update PO versions, and look up revisions using a PO's alternate ID.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-04 21:51:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1222" class=".btn">#1222</a>
            </td>
            <td>
                <b>
                    Update `worklow_type` to `workflow_id`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change update the `workflow_type` field in the purchase order
struct to be `workflow_id`. This makes the "create purchase order"
payload field for the `workflow_id` to match the corresponding field in
the purchase order struct.

This also updates the tests affected by this change.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-04 15:13:31 +0000 UTC
    </div>
</div>

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

