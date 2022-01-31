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
                PR <a href="https://github.com/hyperledger/grid/pull/1275" class=".btn">#1275</a>
            </td>
            <td>
                <b>
                    Fix product XSD location
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                On docker build, puts the product xsd file in /var/lib/grid/...
instead of /usr/share/grid/...

Resolves an issue in which the data validation could not find the
file.

Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-31 18:14:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1274" class=".btn">#1274</a>
            </td>
            <td>
                <b>
                    Add Grid 0.3 release notes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-28 21:09:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1273" class=".btn">#1273</a>
            </td>
            <td>
                <b>
                    Add Hyperledger code of conduct
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Required as a part of the Hyperledger common repo structure

Signed-off-by: Andrea Gunderson <agunde@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-28 18:34:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1272" class=".btn">#1272</a>
            </td>
            <td>
                <b>
                    Remove unwraps for required arguments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously required arguments were retrieved via a call to unwrap(),
which had the capacity to panic at runtime. This change removes those
unwrap() calls and replaces them with a function that sends back a
standard CliError type.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-28 18:21:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1271" class=".btn">#1271</a>
            </td>
            <td>
                <b>
                    Add in-depth instructions for download tool
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add instructions on what steps the utility specifically takes when
downloading and extracting the XSD files.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 22:29:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1270" class=".btn">#1270</a>
            </td>
            <td>
                <b>
                    Move data_validation tests to cli integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This moves the data_validation tests to the cli integration tests so
the XSD files can be downloaded using the `grid download-xsd` command.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 22:13:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1269" class=".btn">#1269</a>
            </td>
            <td>
                <b>
                    Stabilize `xsd-downloader` feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change stabilizes the `xsd-downloader` feature, which enables the
user to download XSDs using the `grid download-xsd` subcommand.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 15:28:24 +0000 UTC
    </div>
</div>

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

Testing instructions:
1. Create a PO & a PO version
2. Attempt to create the same version made previously
3. You should receive an error that that version already exists. Previously, you would receive the error I pasted in a comment below.
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

