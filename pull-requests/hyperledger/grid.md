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
                PR <a href="https://github.com/hyperledger/grid/pull/1265" class=".btn">#1265</a>
            </td>
            <td>
                <b>
                    Add check if po doesn't have accepted version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds a check if the purchase order does not have the
`accepted_version_number` set to validate the list of versions for that
purchase order do not contain versions that exist in an
`accepted`-constrained state.

This addresses this bug: https://github.com/hyperledger/grid/issues/1246
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-25 21:43:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1263" class=".btn">#1263</a>
            </td>
            <td>
                <b>
                    Remove actix-web default features
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates the actix-web dependencies used across Grid to
disable default features. As Grid's Splinter dependency uses another
version of actix-web, multiple versions of a default compression
feature were being pulled in which caused a build error pertaining to
multiple definitions of the same things across the different versions
of the brotli compression feature. As Grid does not currently use these
default compression features, it is safe to turn these features off.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-25 16:26:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1257" class=".btn">#1257</a>
            </td>
            <td>
                <b>
                    Remove xsd files from example
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Removes xsd files used in data validation, since these will be
provided by the downloader.

Resolves: #1247

Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-20 18:55:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1256" class=".btn">#1256</a>
            </td>
            <td>
                <b>
                    Add architecture check for protoc during grid-dev builds
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
        Created At 2022-01-20 15:39:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1255" class=".btn">#1255</a>
            </td>
            <td>
                <b>
                    Fix PO migrations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the PO migrations by adding a new migrations file for the
0.3 version of the tables and reverts the original file back to its
original 0.2 state.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 21:07:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1252" class=".btn">#1252</a>
            </td>
            <td>
                <b>
                    Add `download-xsd` CLI command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add an XSD download CLI command, along with several utility methods for
downloading, extracting, and validating the files within the schema
archive.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 12:44:55 +0000 UTC
    </div>
</div>

