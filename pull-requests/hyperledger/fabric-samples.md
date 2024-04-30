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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1203" class=".btn">#1203</a>
            </td>
            <td>
                <b>
                    Switch microfab to hyperledger-labs version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                full-stack-asset-transfer points to an old image
that no longer exists.
Point to the hyperledger-labs microfab image instead.

Also, pass the orderer endpoint in lifecycle commands
instead of using the channel config fallback.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-30 17:22:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1202" class=".btn">#1202</a>
            </td>
            <td>
                <b>
                    GHA: Use ubuntu-20.04 for local forks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                GHA: Use ubuntu-20.04 for local forks
since local forks don't have access to fabric-ubuntu-20.04.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-30 15:54:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1200" class=".btn">#1200</a>
            </td>
            <td>
                <b>
                    test-network error message if jq not installed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                With removal of fabric-tools image, test-network
now depends on jq being installed locally.

This commit logs an error message if jq commands
fail due to jq not being installed locally.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-29 20:15:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1199" class=".btn">#1199</a>
            </td>
            <td>
                <b>
                    Update nano test network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix regression in network.sh and update peer scripts to allow chaincodeListenAddress and chaincodeAddress to be overridden if required

Also updates the nano test network readme to describe the new environment variables for the k8s builder

Fixes #1198
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-29 12:56:19 +0000 UTC
    </div>
</div>

