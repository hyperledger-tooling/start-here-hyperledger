---
layout: default
title: fabric-sdk-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-go
---

# fabric-sdk-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/206" class=".btn">#206</a>
            </td>
            <td>
                <b>
                    Get proposal response payload from chaincode action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is the correct chaincode transaction response payload location. The response payload field is intended to contain metadata but the peer currently copies the transaction response payload here for convenience. This causes failures due to gRPC message size limits for large response payloads and so may be removed in the future.

Also changed a few build scripts to honour the GO_CMD environment variable.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-02 13:59:08 +0000 UTC
    </div>
</div>

