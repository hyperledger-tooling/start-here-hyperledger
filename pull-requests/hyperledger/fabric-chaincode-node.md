---
layout: default
title: fabric-chaincode-node
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-chaincode-node
---

# fabric-chaincode-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-chaincode-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-node/pull/377" class=".btn">#377</a>
            </td>
            <td>
                <b>
                    Fix the handling of the key endorsement policy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The nOutOf was missing.

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-24 10:27:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-node/pull/375" class=".btn">#375</a>
            </td>
            <td>
                <b>
                    GetHistoryForKey to return correct data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The 2.5 release used an updated protobuf js library; this has meant changes across the codebase to use this new library, subtly different API.. this function was sadly missed.

resolves #374 

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-20 14:12:30 +0000 UTC
    </div>
</div>

