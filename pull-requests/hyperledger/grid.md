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
                PR <a href="https://github.com/hyperledger/grid/pull/1014" class=".btn">#1014</a>
            </td>
            <td>
                <b>
                    Stabilization changes for error response
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Part of https://github.com/hyperledger/grid/issues/1012
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 17:21:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1009" class=".btn">#1009</a>
            </td>
            <td>
                <b>
                    Update po create action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addresses https://github.com/hyperledger/grid/issues/985
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 18:57:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1008" class=".btn">#1008</a>
            </td>
            <td>
                <b>
                    Add PO list/show CLI functionality
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the Grid CLI to include functionality to list and show a Grid Purchase Order. This includes changes to the Purchase Order client to update the structs and functions to align with the RFC and current discussions. It also includes updates to the version and revision list/show commands to use the new display utility functions/patterns introduced here.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 15:23:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1006" class=".btn">#1006</a>
            </td>
            <td>
                <b>
                    Update schema loading for Order.xsd
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates the loading of the schema to be done in the
directory where schemas are specified. This directory is able to be set
with the `GRID_ORDER_SCHEMA_DIR` environment variable, or it is set by
default.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-29 15:20:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1005" class=".btn">#1005</a>
            </td>
            <td>
                <b>
                    Add update version action to po smart contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds an implementation to the po smart contract for the "update version" action. 

This also makes a few small bu fixes that were found while running the unit tests for this action. Mainly, this updates the following:

- `can_transition` workflow state method, this method will now check it's `self.name` property against the desired state. If these values are the same, and we are not transitioning the po/vers to a new workflow state, `true` is returned.

- `add_purchase_order_version` in po state module, this method will now validate if the purchase order version it is adding to state is an update (as in, the version already exists for the po we fetch). Now, this method will replace the outdated vers with the updated one, rather than pushing all "new" versions it receives to the end of the list (which would result in duplicate version IDs being present and the `get_purchase_order_version` method to only return the first version it finds, which based on the functionality of iters is the first one added which would be the outdated version)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-28 21:28:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1003" class=".btn">#1003</a>
            </td>
            <td>
                <b>
                    Add simple validation for po payloads
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds a `payload` module to the purchase order smart contract
for basic validation of the various PurchaseOrderPayload`s that are
handled. These new functions validate that the payload has all the
required fields defined.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-28 17:24:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1002" class=".btn">#1002</a>
            </td>
            <td>
                <b>
                    Update the image used by node in Dockerfiles
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates the image used by node within the UI Dockerfiles,
from `lts-alpine` to `14.18.1-alpine3.11`.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-27 21:56:26 +0000 UTC
    </div>
</div>

