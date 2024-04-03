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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1189" class=".btn">#1189</a>
            </td>
            <td>
                <b>
                    Add Go chaincode for asset-transfer-events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There were recently questions on how to emit chaincode events from Go smart contracts: hyperledger/fabric-gateway#698

This implementation is based on the asset-transfer-basic chaincode (as the README already suggests) and does not include the private data used by the other language implementations. I don't know why private data is necessary to demonstrate chaincode eventing.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 19:03:36 +0000 UTC
    </div>
</div>

