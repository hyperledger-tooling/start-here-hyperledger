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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1225" class=".btn">#1225</a>
            </td>
            <td>
                <b>
                    Update permissions to use seller
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Permissions were incorrectly set to buyer. Updated to be seller.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-05 15:56:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1223" class=".btn">#1223</a>
            </td>
            <td>
                <b>
                    Add ability to add/update POs/versions by alternate ID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds the ability to update POs, add/update PO versions, and look up revisions using a PO's alternate ID.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-04 21:51:42 +0000 UTC
    </div>
</div>

