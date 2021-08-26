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
                PR <a href="https://github.com/hyperledger/grid/pull/913" class=".btn">#913</a>
            </td>
            <td>
                <b>
                    Update purchase-order specific workflow tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change makes a few updates across workflow tests implemented using purchase order objects. These changes include removing unused imports from the workflow module's tests in the purchase order smart contract. This also includes updating the workflow module's tests in the SDK to match the updated permission/aliases for purchase order based on the most updated RFC.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-26 14:23:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/912" class=".btn">#912</a>
            </td>
            <td>
                <b>
                    Add workflow-aware "Create PO" action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds an implementation to the purchase order smart contract's "create po" action. This action is implemented using the workflow-aware permission check.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-26 13:07:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/910" class=".btn">#910</a>
            </td>
            <td>
                <b>
                    BACKPORT: Fix `has_permission()` bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes a bug in the `has_permission` check. Previously, the check was not properly validating whether an inherited role was actually allowed to be inherited by its owner.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-25 19:54:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/908" class=".btn">#908</a>
            </td>
            <td>
                <b>
                    Update purchase order protos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change makes various updates to the Purchase Order smart contract's
state and payload protobuf messages, as several necessary attributes
were left out of these messages.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-25 19:33:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/907" class=".btn">#907</a>
            </td>
            <td>
                <b>
                    Add Purchase Order store struct accessors and builders
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds public accessor methods to the PurchaseOrderStore structs
and makes the structs' fields private. This also adds builders for the
structs. This brings the module in-line with the other Grid stores.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-23 22:16:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/903" class=".btn">#903</a>
            </td>
            <td>
                <b>
                    Implement some methods for Purchase Order state
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds implementations for a few methods on the Purchase Order state that are used by the smart contract actions. This pr adds implementations for the methods `get_purchase_order`, `set_purchase_order`, `get_agent`, and `get_organization`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-19 19:10:08 +0000 UTC
    </div>
</div>

