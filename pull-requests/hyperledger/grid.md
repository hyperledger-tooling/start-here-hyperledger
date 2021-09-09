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
                PR <a href="https://github.com/hyperledger/grid/pull/927" class=".btn">#927</a>
            </td>
            <td>
                <b>
                    Add `list_purchase_order_versions` operation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds a `list_purchase_order_versions` operation to the purchase
order store. This operation gets a list of purchase order versions for a
gived purchase order. This also includes that version's revisions.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 16:51:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/925" class=".btn">#925</a>
            </td>
            <td>
                <b>
                    Add `buyer` and `seller` org fields to Purchase Order
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the `PurchaseOrderPayload` to remove the `org_id` field, as the organizations are now being recorded in the purchase order itself. This also updates the `CreatePurchaseOrderPayload` and `PurchaseOrder` struct in state to support a `buyer_org` and `seller_org` fields for the purchase order. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 15:28:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/924" class=".btn">#924</a>
            </td>
            <td>
                <b>
                    Add `get_purchase_order_version` operation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds a `get_purchase_order_version` operation. This fetches a PO
version and its associated revisions and returns the Grid representation
of them.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-08 21:52:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/923" class=".btn">#923</a>
            </td>
            <td>
                <b>
                    Update `add_purchase_order` operation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the `add_purchase_order` operation to properly add/update POs, versions, and revisions while avoiding unnecessary db updates.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-08 20:23:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/921" class=".btn">#921</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-2: Change keygen system default backport
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Merged to main in #885.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-07 16:29:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/920" class=".btn">#920</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-2: Update Splinter Docker Hub compose file to use 0.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-07 16:22:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/919" class=".btn">#919</a>
            </td>
            <td>
                <b>
                    Update Splinter Docker Hub compose file to use 0.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-07 16:20:54 +0000 UTC
    </div>
</div>

