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
                PR <a href="https://github.com/hyperledger/grid/pull/1191" class=".btn">#1191</a>
            </td>
            <td>
                <b>
                    Fix revision count in `po version list`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds filter to select only revisions of the same purchase order
when listing po versions. Previously, if versions of different
purchase orders had the same version ID, the revison count would
include all revisions of versions with that name.

Resolves: #1170

Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-18 00:36:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1190" class=".btn">#1190</a>
            </td>
            <td>
                <b>
                    Stabilize `purchase-order` feature in sdk
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This stabilizes the `purchase-order` feature in the Grid SDK by moving
the feature from `experimental` to `stable`.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-17 19:06:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1189" class=".btn">#1189</a>
            </td>
            <td>
                <b>
                    Fix small typo in purchase_order/addressing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrea Gunderson <agunde@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-17 17:32:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1188" class=".btn">#1188</a>
            </td>
            <td>
                <b>
                    Update Splinter version and add authorization to ScabbardClient
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
        Created At 2021-12-16 20:38:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1187" class=".btn">#1187</a>
            </td>
            <td>
                <b>
                    Add xsd files to gridd .deb package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Including these in the package ensures they're available if the package
is copied out of the Docker image and installed elsewhere.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-16 16:43:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1186" class=".btn">#1186</a>
            </td>
            <td>
                <b>
                    Fix CLI display of many results
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes the performance of the CLI when attempting to display many purchase order results. Previously, no results would be shown until all records were fetched from storage. With this update, a special iterator is used to take advantage of the REST API's paging and cache records so the CLI can print as soon as the first result comes back. This required significant rewrites to the CLI printing functionality.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-15 22:57:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1185" class=".btn">#1185</a>
            </td>
            <td>
                <b>
                    Fix lint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change removes two empty lines. This was causing a lint error for
the main build of Grid.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-15 14:08:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1182" class=".btn">#1182</a>
            </td>
            <td>
                <b>
                    v0.2 Rust 1.57 clippy updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 Rust 1.57 clippy updates for the 0-2 branch
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-13 15:27:31 +0000 UTC
    </div>
</div>

