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
                PR <a href="https://github.com/hyperledger/grid/pull/1036" class=".btn">#1036</a>
            </td>
            <td>
                <b>
                    Improve build times
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
        Created At 2021-11-11 02:04:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1035" class=".btn">#1035</a>
            </td>
            <td>
                <b>
                    Replace `workflow_status` with `workflow_state`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This replaces all references/arguments/variables called
`workflow_status` with the name `workflow_state`. This is for
consistency and accuracy.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 22:29:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1034" class=".btn">#1034</a>
            </td>
            <td>
                <b>
                    Clean up client feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR contains several updates to the client module. These changes are intended to work towards stabilizing the `client` feature. Changes include:
 - Standardizing documentation
 - Standardizing objects to derive the same traits where applicable
 - Removing the `create_client_factory` fn in favor of creating the factories directly
 - Reorganizing the client module to group like files and simplify config
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 18:26:50 +0000 UTC
    </div>
</div>

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

