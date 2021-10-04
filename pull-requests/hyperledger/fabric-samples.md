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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/498" class=".btn">#498</a>
            </td>
            <td>
                <b>
                    Run the fabric test network on Kubernetes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Example scripts and guide to run the Fabric test-network on Kubernetes.
- Includes a `./network kind` command to quickly bootstrap a local KIND cluster and container registry. 
- Includes a reference guide for building and launching Chaincode-as-a-Service and External Chaincode Builders. 
- Includes a reference guide for debugging chaincode locally, invoked from Fabric on Kubernetes.
- Includes a reference deployment of the [fabric-rest-sample](https://github.com/hyperledgendary/fabric-rest-sample) blockchain application. 
- Tested with KIND and IKS Kubernetes clusters. 


Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-04 11:45:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/497" class=".btn">#497</a>
            </td>
            <td>
                <b>
                    Fix ERC1155 chaincode indeterminism caused by iterating maps in Go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hi. I am the person who contributed ERC1155 in #463 . I noticed a problem with the chaincode. I fall into the trap of using map data structure in Go when developing a Fabric chaincode. The functions `BatchTransferFrom` and `BatchTransferFromMultiRecipient` in the ERC1155 chaincode sometimes give the error `ProposalResponsePayloads do not match`. This happens since iterating maps in Go is not deterministic. As a solution, I copied the keys of the map and sorted them and iterated over the sorted keys.

Signed-off-by: Baran Kılıç <baran.kilic@boun.edu.tr>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 10:01:20 +0000 UTC
    </div>
</div>

