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
                PR <a href="https://github.com/hyperledger/grid/pull/1041" class=".btn">#1041</a>
            </td>
            <td>
                <b>
                    Clarify po update error message for is_closed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The old update po error message for is_closed was ambiguous. This change
clarifies that the error is due to the closed constraint on the state
not being in sync with the is_closed payload.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-12 17:13:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1039" class=".btn">#1039</a>
            </td>
            <td>
                <b>
                    Fix pagination filters
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the logic for extracting the base URL so that filters will be passed along to paging.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-12 00:02:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1038" class=".btn">#1038</a>
            </td>
            <td>
                <b>
                    Fix po update cli command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change fixes the po update cli command by changing it to use the alternate id from the po get endpoint (which is already called earlier and therefore its result is available) instead of the unimplemented `list_alternate_ids` REST client fn.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-11 22:26:29 +0000 UTC
    </div>
</div>

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

