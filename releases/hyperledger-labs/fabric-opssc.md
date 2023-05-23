---
layout: default
title: fabric-opssc
parent: Hyperledger Labs
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger-labs/fabric-opssc
---

# fabric-opssc <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-opssc){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v0.4.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.4.0
                </span>
            </td>
            <td>
                # OpsSC v0.4.0 release (May. 16, 2023)

## Changes in this release:
- Support both Hyperledger Fabric v2.5 and v2.2 series (Out of scope: v2.4)
- Support chaincode operations on Kubernetes (K8s) environments
  - Support for chaincode operations with External Chaincode Builder for K8s
    - [CCaaS builder ('ccaas')](https://github.com/hyperledger/fabric/releases/tag/v2.4.1) support
    - [K8s chaincode builder ('k8s')](https://github.com/hyperledger-labs/fabric-builder-k8s) support
  - Helm charts to run OpsSC on K8s
    - Helm chart for OpsSC API server
    - Helm chart for OpsSC Agent
    - Helm chart for building a chaincode image and running it as a chaincode server
  - Documents and integration tests for OpsSC on K8s
    - Environment using [fabric-samples/test-network-k8s](https://github.com/hyperledger/fabric-samples/tree/main/test-network-k8s)
    - Environment using [fabric-operator/sample-network](https://github.com/hyperledger-labs/fabric-operator/tree/main/sample-network)
  - Limitations:
    - Channel operations on K8s environments are not yet supported
    - Only support Fabric 2.5+
- Other minor improvements
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger-labs/fabric-opssc/releases/tag/v0.4.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-05-16 02:28:04 +0000 UTC
    </span>
</div>

