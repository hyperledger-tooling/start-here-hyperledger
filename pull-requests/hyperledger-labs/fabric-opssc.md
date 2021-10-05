---
layout: default
title: fabric-opssc
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-opssc
---

# fabric-opssc <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-opssc){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/14" class=".btn">#14</a>
            </td>
            <td>
                <b>
                    OpsSC v0.2.0 release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update README to release v0.2.0

This changes include:
- Support multiple endorsement policy formats for chaincode_ops
- Bump fabric version to 2.3.3 or 2.2.4
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-05 00:38:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/13" class=".btn">#13</a>
            </td>
            <td>
                <b>
                    Support chaincode deployment with private data for chaincode_ops
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR supports chaincode deployment with private data for chaincode_ops.

- The current implementation internally uses some protobuf handlers based on source code in [Fabric Operations Console (FOC)](https://github.com/hyperledger-labs/fabric-operations-console) to encode/decode private data collections definitions.
- NOTE: This PR contains minimal integration tests of the feature, but more strict tests should be added for various formats of private collections in the future.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-01 00:22:14 +0000 UTC
    </div>
</div>

