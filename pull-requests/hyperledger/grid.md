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
                PR <a href="https://github.com/hyperledger/grid/pull/1033" class=".btn">#1033</a>
            </td>
            <td>
                <b>
                    Add paging query string support, tests, and docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a rewrite of the paging module with several notable differences
from the original.

The first and most notable change is the addition of arbitary query
string support in the base URL, so we can add filters to the paging
URLs. To facilitate this, this change uses the Rust url crate for both
the external API and internal URL representation. This change also adds
the serde feature to the url library to allow the Paging object to
serialize.

The second change is to modify the returned object to make the "prev"
link optional. This mirrors "next" which was already optional.

Other notable changes include splitting up the internal structure for
ease of reading and testing, added tests to verify offset and
serialization output, and added documentation in anticipation of
Paging module stabilization.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 18:29:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1032" class=".btn">#1032</a>
            </td>
            <td>
                <b>
                    Change keygen priv key file permissions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changes private key file perms from 640 to 600. This matches
ssh-keygen (as a standard).

Resolves: #1020

Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 18:20:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1031" class=".btn">#1031</a>
            </td>
            <td>
                <b>
                    Fix CLI values of global options
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implements a fix regarding values of global options being
unavailable to subcommands.

While clap propagates global argument values down to the
subcommand level, they are not available in intermediate levels.
This is in contrast to how we must define them in the app.

Previously, the CLI tried to access global arg values at the level
that they were defined. This fix gets the values at the lowest
subcommand level.

These changes also changed the formatting required by `cargo fmt`.

Resolves: #1026

Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 21:59:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1030" class=".btn">#1030</a>
            </td>
            <td>
                <b>
                    Support `alternate_id` for PO creation and lookup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the Grid PO store, SDE, and CLI to support PO creation and lookup using a properly formatted (`<id_type>:<id>`) alternate ID. This change includes an update to the `grid create po` CLI command to update the flag for specifying an alternate ID to `--alternate-id` from the less descriptive `--id`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 20:42:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1029" class=".btn">#1029</a>
            </td>
            <td>
                <b>
                    Set explicit feature dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 19:44:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1027" class=".btn">#1027</a>
            </td>
            <td>
                <b>
                    Fix bug in cli `grid location show`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes bug related to location_id.

Resolves: #1013

Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-05 22:32:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1025" class=".btn">#1025</a>
            </td>
            <td>
                <b>
                    Remove current revision ID from update payload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change removes the `current_revision_id` from the
`UpdateVersionPayload`. This payload includes a `PayloadRevision` which
is the source of this value, otherwise the value is automatically
incremented based on the previous revision. Therefore, the payload does
not need this value.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-05 20:28:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1023" class=".btn">#1023</a>
            </td>
            <td>
                <b>
                    Backport 0-2: Update the image used by node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates the image used by node within the UI Dockerfiles,
from `lts-alpine` to `14.18.1-alpine3.11`.

This change also updates the copyright headers within the affected files
to include the current year.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-05 20:14:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1022" class=".btn">#1022</a>
            </td>
            <td>
                <b>
                    Backport 0-2: Backport adding a protocol version for Splinter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds a `SplinterProtocolVersion` to the app auth handler's registration to allow for backwards compatibility.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-05 19:29:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1021" class=".btn">#1021</a>
            </td>
            <td>
                <b>
                    Backport 0-2: Backport the cylinder-jwt-support feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change backports the updates made to add Cylinder JWT authorization to Grid, to allow it to run with current versions of Splinter.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-05 19:26:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1019" class=".btn">#1019</a>
            </td>
            <td>
                <b>
                    Remove `sawtooth-compat` from SDK
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change removes the `sawtooth-compat` feature from the SDK. The
dependencies pulled in by this feature are already pulled in based on
the `target_arch` and the `sawtooth-compat` feature itself does not
protect any code within the SDK.

This also updates the `sawtooth-support` feature in the daemon to pull
in the Sabre and Sawtooth SDKs individually.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 16:10:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1018" class=".btn">#1018</a>
            </td>
            <td>
                <b>
                    Remove `splinter` feature from CLI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change removes the experimental "splinter" feature from the Grid
CLI. Grid handles the separate backends within the Rest API and daemon.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 15:41:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1017" class=".btn">#1017</a>
            </td>
            <td>
                <b>
                    Validate payloads in `apply` method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change passes a reference to the payload, once it is converted to
the PurchaseOrderPayload, to the `validate_po_payload` function. This
function will validate the timestamp within the payload and the
associated action's payload.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 21:32:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1016" class=".btn">#1016</a>
            </td>
            <td>
                <b>
                    Update `add` method in state to consider updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates the `set_purchase_order_version` method in the
purchase order state module to consider if a purchase order version is
being updated. This means, when the po is fetched from state, the method
will now check to see if a version with the same ID exists in the list
and then it is removed and re-inserted with the updated version.
Otherwise, a new version is simply added to the end of the purchase
order's `versions` list.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 20:18:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1015" class=".btn">#1015</a>
            </td>
            <td>
                <b>
                    Validate self workflow state in `can_transition`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates the workflow state module's `can_transition` method,
which validates whether an agent has the correct permissions to
transition to a new workflow state, to check the workflow state's name.
This covers a case in which an agent is not attempting to transition a
workflow, but rather update an object. 

Previously, the `can_transition`
method would return false if it did not have it's own name within it's
transitions. Rather than add all of the workflow states as transitions
to their own state, this will check if we are staying in the same
workflow state and return `true`, as we are not transitioning.

This PR also updates a test to change the name of the workflow state used. This allows an alias' transitions to be validated, while avoiding a situation where the alias is attempting to transition to the same state.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 20:16:54 +0000 UTC
    </div>
</div>

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

