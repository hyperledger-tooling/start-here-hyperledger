---
layout: default
title: fabric-chaincode-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-chaincode-go
---

# fabric-chaincode-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-chaincode-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/108" class=".btn">#108</a>
            </td>
            <td>
                <b>
                    v2 implementation using fabric-protos-go-apiv2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The v2 implementation retains wire-level compatibility with Fabric but does include the following breaking changes:

- Chaincode implementation that make direct use of fabric-protos-go will experience protocol buffer namespace conflicts (as described in https://protobuf.dev/reference/go/faq/). Any use of fabric-protos-go must be replaced by fabric-protos-go-apiv2.
- The Chaincode interface and Stub now use only pointers to protocol buffer messages in their API. Chaincode implementation must provide matching Init and Invoke methods.

Closes #80
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-01 14:35:23 +0000 UTC
    </div>
</div>

