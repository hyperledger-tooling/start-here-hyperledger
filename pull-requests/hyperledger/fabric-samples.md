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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1206" class=".btn">#1206</a>
            </td>
            <td>
                <b>
                    Remove double quotes for env variables
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Double quotes have caused issues in some environments, e.g. see https://github.com/hyperledger/fabric/issues/4358
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-06 14:28:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1205" class=".btn">#1205</a>
            </td>
            <td>
                <b>
                    Fix of issue #1204
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix solution of  issue #1204 titled Test-network-k8s network script gets last version Fabric bin files instead of requested version.
When test-network-k8s is called with a specific but not the last version of Fabric hyper-ledger and the binary files are not available into ./bin folder, the script always downloaded the last version of binary files.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-01 10:34:16 +0000 UTC
    </div>
</div>

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
                full-stack-asset-transfer points to an old image.
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

