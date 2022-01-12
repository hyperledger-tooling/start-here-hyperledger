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
                PR <a href="https://github.com/hyperledger/grid/pull/1240" class=".btn">#1240</a>
            </td>
            <td>
                <b>
                    Update version action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates to the "update version" action are dependent on the updates made for the "update po" action. (The `unaccept_versions` method is used for both of these actions). This PR will be updated as ready to be reviewed once #1213 is merged.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-12 15:43:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1239" class=".btn">#1239</a>
            </td>
            <td>
                <b>
                    Update `create_version` action in handler
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the `create_version` function in the purchase order smart
contract that handles the creation of a purchase order version. This
change updates the workflow state used to validate a user's permission
to use the workflow state specified in the payload for that version.
This also updates tests that attempted to create a version in any other
state than "create". This movement is now validated by the smart
contract and will return an err if a version is not created in the
"create" state.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-12 15:31:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1238" class=".btn">#1238</a>
            </td>
            <td>
                <b>
                    Fix numbers in proto messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes protobuf numbering to be consecutive.

Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-11 16:41:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1230" class=".btn">#1230</a>
            </td>
            <td>
                <b>
                    Use functions as opposed to pub schema const
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                All external references to the schema directory should be based on both
the base schema dir and environment variables. This change creates
functions to facilitate that, and removes the public modifier from the
schema const.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-06 16:58:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1229" class=".btn">#1229</a>
            </td>
            <td>
                <b>
                    Update schema directory to /usr/share/grid/schemas
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                XML schema files now go into /usr/share, which is for
architecture-independent shareable files.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-06 16:47:25 +0000 UTC
    </div>
</div>

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

