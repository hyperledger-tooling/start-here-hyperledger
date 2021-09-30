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
                PR <a href="https://github.com/hyperledger/grid/pull/960" class=".btn">#960</a>
            </td>
            <td>
                <b>
                    Add CLI filters to DB ops
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds filters to some of the PO DB operations that correspond to the filters available in the list/show PO CLI commands.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 19:50:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/959" class=".btn">#959</a>
            </td>
            <td>
                <b>
                    Add OpenAPI validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a GitHub Action to validate the swagger file

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 22:03:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/958" class=".btn">#958</a>
            </td>
            <td>
                <b>
                    Add purchase order version REST endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a purchase order REST endpoint to retrieve a version provided a
version id and a purchase order.

Related to: https://github.com/hyperledger/grid/issues/867

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 19:53:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/957" class=".btn">#957</a>
            </td>
            <td>
                <b>
                    Add purchase order version list endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add an endpoint to obtain purchase order versions at
/purchase-order/{UUID}/versions.

Related: #866

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 16:32:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/956" class=".btn">#956</a>
            </td>
            <td>
                <b>
                    Consolidate PO DB migrations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This consolidates the PO DB migrations files down to one migration. We
    aren't currently worried about losing data as the feature is not yet
    released and consolidating will simplify the code and development.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-27 20:58:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/955" class=".btn">#955</a>
            </td>
            <td>
                <b>
                    Make `accepted_version_id` optional throughout SDK
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the `accepted_version_id` field in the purchase order object to be optional throughout the SDK. This previously was defined as a required string, however this value may not always be defined. A purchase order version must first be validated that it is able to be "accepted". Therefore, this value should be optional to allow for the cases where a purchase order does not have an accepted version (yet).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-27 19:01:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/954" class=".btn">#954</a>
            </td>
            <td>
                <b>
                    Add list/get revision operations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds database operations to the `PurchaseOrderStore` to get and list `PurchaseOrderVersionRevisions`. The list operation lists revisions filtered by `po_uid` and `version_id` and the get operation fetches a revision filtered by `po_uid`, `version_id`, and `revision_id`. This also includes migrations and updates to the revisions table to add a `purchase_order_uid` column. This is necessary to be able to properly get revisions in case of overlap in version IDs between different POs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-24 21:20:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/953" class=".btn">#953</a>
            </td>
            <td>
                <b>
                    Add `--skip` to griddle examples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These docker examples are likely to be rerun many times. The --skip
option will allow the entrypoint command to run without throwing an
error if the keys are already generated.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-24 20:44:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/952" class=".btn">#952</a>
            </td>
            <td>
                <b>
                    Test keygen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add tests to validate the behavior of key generation given various
permutations of the configuration values.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-24 20:36:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/950" class=".btn">#950</a>
            </td>
            <td>
                <b>
                    Add `workflow_status` to `CreatePurchaseOrder` payload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds a `workflow_status` field to the `CreatePurchaseOrder` payload
which brings the create payload in line with its update counterpart.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-24 16:50:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/949" class=".btn">#949</a>
            </td>
            <td>
                <b>
                    Add create version CLI command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds the create version CLI command to create a Purchase Order
    version and first revision for that version.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-23 21:36:59 +0000 UTC
    </div>
</div>

