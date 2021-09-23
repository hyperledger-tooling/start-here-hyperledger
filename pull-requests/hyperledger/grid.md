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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/941" class=".btn">#941</a>
            </td>
            <td>
                <b>
                    Fix Client `ROLES_ENDPOINT` const
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates the `ROLES_ENDPOINT` const, defined for the
`ReqwestPikeClient`, to `ROLE_ENDPOINT` and updates the value from
"roles" to "role". The role endpoint is singular.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-17 21:54:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/939" class=".btn">#939</a>
            </td>
            <td>
                <b>
                    Hookup PO SDE
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This sets up the state delta export for purchase order events. This PR also adds the conversion methods to `EventError` for the purchase order store errors.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-17 18:40:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/936" class=".btn">#936</a>
            </td>
            <td>
                <b>
                    Update PO version protos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the PO version proto to reflect that a version can have multiple revisions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 18:34:46 +0000 UTC
    </div>
</div>

