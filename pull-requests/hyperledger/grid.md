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
                PR <a href="https://github.com/hyperledger/grid/pull/932" class=".btn">#932</a>
            </td>
            <td>
                <b>
                    Update PO store for updated protos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the PO store to account for the changes to the PO protobuf messages. This updates the schemas, DB models, Grid structs, DB operations, and REST API to account for the different fields in the updated messages.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 19:36:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/931" class=".btn">#931</a>
            </td>
            <td>
                <b>
                    Added the libzmq3-dev dependency for building in Debian(Ubuntu)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hi, I have added the needed pre-requisite for building Grid on Debian(Ubuntu).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 12:18:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/929" class=".btn">#929</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-2: Add GHA files
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
        Created At 2021-09-09 20:18:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/928" class=".btn">#928</a>
            </td>
            <td>
                <b>
                    Add state methods to get/set purchase order versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds implementations for `get_purchase_order_version` and `set_purchase_order_version` for `PurchaseOrderState`. This also adds tests for all of the state methods (including the newly implemented ones).  
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 20:00:10 +0000 UTC
    </div>
</div>

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

