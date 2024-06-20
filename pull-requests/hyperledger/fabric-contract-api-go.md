---
layout: default
title: fabric-contract-api-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-contract-api-go
---

# fabric-contract-api-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-contract-api-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-contract-api-go/pull/137" class=".btn">#137</a>
            </td>
            <td>
                <b>
                    v2 implementation based on fabric-chaincode-go/v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The v2 implementation retains wire-level compatibility with Fabric but does include the following breaking changes:

- Chaincode implementations that make direct use of fabric-protos-go will experience protocol buffer namespace conflicts (as described in https://protobuf.dev/reference/go/faq/). Any use of fabric-protos-go must be replaced by fabric-protos-go-apiv2.

Closes #102
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-19 16:57:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-contract-api-go/pull/136" class=".btn">#136</a>
            </td>
            <td>
                <b>
                    Update test dependencies to address CVE-2024-37168
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update to latest fabric-chaincode-integration to pick up new grpc-js dependency.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-13 19:06:24 +0000 UTC
    </div>
</div>

