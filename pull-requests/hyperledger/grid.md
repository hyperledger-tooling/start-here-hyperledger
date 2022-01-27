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
                PR <a href="https://github.com/hyperledger/grid/pull/1268" class=".btn">#1268</a>
            </td>
            <td>
                <b>
                    Check if version exists in create version command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates how the revision ID is fetched for a version being
created. As this version is being created, the revision ID should be '1'
rather than the most recent revision ID of the version. The most recent
revision ID should not exist, as a version being created should not
already exist.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-26 22:47:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1267" class=".btn">#1267</a>
            </td>
            <td>
                <b>
                    Add file checks to avoid "os error: file not found"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Checks to see if XSD and user-provided po XML files exist before attempting to read. Previously, the user would get a generic os error message, as these errors weren't mapping to ours.

Resolves: #1169 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-26 22:43:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1266" class=".btn">#1266</a>
            </td>
            <td>
                <b>
                    Add test to validate removing accepted version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Validate that the po versions are consistently not accepted with the
parent po when the po is no longer accepted.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-26 18:11:29 +0000 UTC
    </div>
</div>

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

