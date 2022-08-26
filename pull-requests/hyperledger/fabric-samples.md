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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/820" class=".btn">#820</a>
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
                Fix minor bugs, and add network.sh script to simplify standing up the network

Note: the updated peerNadmin.sh scripts no longer create or join a channel and now only configure the environment for the relevant peer

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-26 13:57:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/818" class=".btn">#818</a>
            </td>
            <td>
                <b>
                    Cloudathon
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
        Created At 2022-08-24 16:42:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/817" class=".btn">#817</a>
            </td>
            <td>
                <b>
                    separate namespace for each organization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently all the organizations are in a single namespace. Changes are done in multiple files to create three namespaces and to separate organizations across namespaces.
- ORG0_NS, ORG1_NS, ORG3_NS are defined in network script
- $NS in the scripts are replaced with corresponding namespace

All till chaincode invoke/query is working. I'm yet to test the api server. kind was used for n/w setup, will test on Rancher also.

fixes https://github.com/hyperledger/fabric-samples/issues/644.

Signed-off-by: Basil K Y <techiebasil@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-22 13:41:55 +0000 UTC
    </div>
</div>

