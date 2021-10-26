---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/516" class=".btn">#516</a>
            </td>
            <td>
                <b>
                    test-network: Make the regexp of checking version more strict (backpo…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                (Backport #515)

Make the regular expression of checking version more strict in `test-network/network.sh` for comparing only the main version.

If the version string (by `'peer version'`) includes other "Version: " strings, the comparing version between `LOCAL_VERSION` and `DOCKER_IMAGE_VERSION` would be failed because of the cropping by '`head -1`'.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 12:22:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/515" class=".btn">#515</a>
            </td>
            <td>
                <b>
                    test-network: Make the regexp of checking version more strict
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Make the regular expression of checking version more strict in `test-network/network.sh` for comparing only the main version.

If the version string (by `'peer version'`) includes other "Version: " strings, the comparing version between `LOCAL_VERSION` and `DOCKER_IMAGE_VERSION` would be failed because of the cropping by '`head -1`'.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 10:01:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/513" class=".btn">#513</a>
            </td>
            <td>
                <b>
                    resolve for #512
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                resolve for #512

by adding storageClassName in PVC files

Signed-off-by: Sam Yuan <yy19902439@126.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-25 14:16:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/510" class=".btn">#510</a>
            </td>
            <td>
                <b>
                    [DO NOT MERGE] Initial REST sample
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Needs more unhappy path testing and lots of review comments!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-22 16:56:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/509" class=".btn">#509</a>
            </td>
            <td>
                <b>
                    Get label for chaincode from metadata.json
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-22 10:39:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/508" class=".btn">#508</a>
            </td>
            <td>
                <b>
                    Ignore java temp files
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
        Created At 2021-10-22 09:25:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/507" class=".btn">#507</a>
            </td>
            <td>
                <b>
                    Possible update to nano-bash network for external builders
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Pull in the external builders from an assumed location in the binary package (as per https://github.com/hyperledger/fabric/pull/2990)

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 15:55:00 +0000 UTC
    </div>
</div>

