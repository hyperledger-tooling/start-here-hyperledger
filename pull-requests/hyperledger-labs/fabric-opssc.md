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
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/58" class=".btn">#58</a>
            </td>
            <td>
                <b>
                    feat(*): Initial implementation to support chaincode operations on K8s
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds an initial implementation to support chaincode operations on Kubernetes (K8s) environments.

This includes the following updates:
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
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-18 02:11:14 +0000 UTC
    </div>
</div>

