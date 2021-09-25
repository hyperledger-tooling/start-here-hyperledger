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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/948" class=".btn">#948</a>
            </td>
            <td>
                <b>
                    Fix get/list role display bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes a bug where roles' `inherit_from` roles were not being
displayed correctly. This fixes it so roles now properly display their
inherited roles.

# Testing

## Create orgs

$ grid keygen alpha-agent
$ grid keygen beta-agent
$ export GRID_DAEMON_KEY="beta-agent" && grid organization create beta BetaOrg --alternate-ids gs1_company_prefix:0 --wait 10
$ export GRID_DAEMON_KEY="alpha-agent" && grid organization create alpha AlphaOrg --alternate-ids gs1_company_prefix:1 --wait 10

# Create a role for beta to inherit
$ grid role create alpha productowner --permissions schema::can-create-schema,product::can-create-product,product::can-delete-product,schema::can-update-schema,product::can-update-product --active --wait 10

# inherit role
$ export GRID_DAEMON_KEY="beta-agent"
$ $ grid role create beta alpha-po --permissions product::can-update-product --inherit-from alpha.productowner --active --wait 10

# try to list role
$ grid role list beta
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 19:15:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/946" class=".btn">#946</a>
            </td>
            <td>
                <b>
                    Add `workflow_type` to purchase order & make `accepted_version_id` optional within the SDK
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change mainly adds a string field, `workflow_type` to the purchase order object. This field addition affects the use of purchase order throughout the SDK, from the protobuf message to the store. Also, added the `workflow_type` to the purchase order that is returned by the rest API. 

This change also makes an update to make `accepted_version_number/id` optional in the purchase order protocol and store code. This updates the use of this field as it is now an `Option<String>`, rather than just `String`. 

This change also adds migration data to account for these changes to the purchase order database model.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 14:58:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/945" class=".btn">#945</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-2: Conform whitespace to calc CSS standard
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To conform to the CSS standard, plus and minus characters must be
surrounded by whitespace within the calc function. The lack of
whitespace caused the docker image build to fail when creating
grid-ui-alpha. This change fixes that by adding the appropriate
whitespace.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-21 18:12:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/944" class=".btn">#944</a>
            </td>
            <td>
                <b>
                    Add whitespace to conform to calc CSS standard
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To conform to the CSS standard, plus and minus characters must be
surrounded by whitespace within the calc function. The lack of
whitespace caused the docker image build to fail when creating
grid-ui-alpha. This change fixes that by adding the appropriate
whitespace.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-21 15:13:52 +0000 UTC
    </div>
</div>

