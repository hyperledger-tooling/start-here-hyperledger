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
                <nil>
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
                <nil>
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1001" class=".btn">#1001</a>
            </td>
            <td>
                <b>
                    Add PO version and revision `list` and `show` CLI commands
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds CLI commands for listing and showing Grid Purchase Order versions and revisions. In support of this, the purchase order client's functions and structs are also brought up-to-date with the rest of the module's pieces.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-27 15:58:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1000" class=".btn">#1000</a>
            </td>
            <td>
                <b>
                    Fix adding a new revision to the store
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes a bug when attempting to add a revision to the store when the
version doesn't yet exist. This now proprly creates the new version
first.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 14:59:56 +0000 UTC
    </div>
</div>

