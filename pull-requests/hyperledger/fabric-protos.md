---
layout: default
title: fabric-protos
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-protos
---

# fabric-protos <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-protos){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/112" class=".btn">#112</a>
            </td>
            <td>
                <b>
                    [WIP] Bump version to 0.1.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 11:54:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/111" class=".btn">#111</a>
            </td>
            <td>
                <b>
                    [WIP] Only tag release versions as latest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The node module should only be tagged with “latest” for released versions, and “unstable” otherwise

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 11:49:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/110" class=".btn">#110</a>
            </td>
            <td>
                <b>
                    Bump version to 0.1.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 20:14:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/109" class=".btn">#109</a>
            </td>
            <td>
                <b>
                    Allow release builds to be re-run manually
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It would be useful to rerun the release build using the workflow_dispatch event, however this does not currently work because the workflows are checking the github ref for a v* version tag.

It’s not safe to always publish for a manual build and all the language bindings at a particular version should be published from the same commit, so this PR adds a job to the ci-checks workflow to look for the required version tag on the commit being built.

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 20:03:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/107" class=".btn">#107</a>
            </td>
            <td>
                <b>
                    Allow Maven after Github fails
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 13:20:30 +0000 UTC
    </div>
</div>

