---
layout: default
title: fablo
parent: Hyperledger Labs
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger-labs/fablo
---

# fablo <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fablo){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger-labs/fablo/issues/274" class=".btn">274</a>
            </td>
            <td>
                <b>
                    Update Node.js runtime compatibility
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span>
            </td>
            <td>
                > By default a Fabric Peer v1.4 will create a Nodejs v8 runtime, and a Fabric Peer v2.2/2.3 will create a Nodejs 12 runtime. The Fabric v2.4 will create a Nodejs 16 runtime.

see: https://github.com/hyperledger/fabric-chaincode-node/blob/main/COMPATIBILITY.md

Due to it, we need to update chaincode scripts to provide accurate warnings
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-06 12:23:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger-labs/fablo/issues/228" class=".btn">228</a>
            </td>
            <td>
                <b>
                    Fablo fails if two chaincodes have the same name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">good first issue</span>
            </td>
            <td>
                To reproduce: create a config with two chaincodes with the same name (on different channels).

The network won't start, since we do not aim (yet?) to support chaincodes with the same names (i fails with duplicate volumes).

AND when you try to prune the network, the prune operation fails as well (duplicate volumes as well).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-18 14:17:30 +0000 UTC
    </div>
</div>

