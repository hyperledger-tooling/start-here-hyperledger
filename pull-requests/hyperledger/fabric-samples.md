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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1186" class=".btn">#1186</a>
            </td>
            <td>
                <b>
                    Decouple fabric tools image from fabric sample
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Decouple fabric tools image from fabric sample.
change list for running on github action:
- network for orderer.
- file path for add org3.
- core.yaml missing?

The current PR seems has many code smells... but it seems works.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-20 13:40:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1185" class=".btn">#1185</a>
            </td>
            <td>
                <b>
                    Fix to configtx.yaml to enable it to work as intended with the test network and channel tutorials
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It seems the profile name was incorrectly changed to from "TwoOrgsApplicationGenesis" as the fabric tutorial requires to "ChannelUsingRafts".  This latter profile name creates an error when setting up channels using the test network and tutorials.  This update changes the profile name back to "TwoOrgsApplicationGenesis" as is required for the test network tutorials for which this file was created. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-19 15:37:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1184" class=".btn">#1184</a>
            </td>
            <td>
                <b>
                    Update go.mod
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
        Created At 2024-03-16 21:02:51 +0000 UTC
    </div>
</div>

