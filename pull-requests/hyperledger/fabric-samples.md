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

