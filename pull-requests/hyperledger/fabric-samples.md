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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/639" class=".btn">#639</a>
            </td>
            <td>
                <b>
                    test-network-k8s: High availability on application connection profiles 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Signed-off-by:** Charalarg <charalarg@gmail.com>

**Type of change:**

- New feature
- Bug fix

**Description:**

With these changes applications use the gateway-svc services in order to establish connection with any available peer on each organization rather than connecting manually to peer1. 

The service names need also to be added as dnsName in each peer TLS certificate configuration.

**Resolves:** #635 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 11:32:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/638" class=".btn">#638</a>
            </td>
            <td>
                <b>
                    Add README to asset-transfer-basic sample
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also:
- Refactor application-gateway-java slightly to reflect more idiomatic Java class structure, in line with asset-transfer-events sample.
- Correctly handle unexpected error case where key file is missing.
- Update Gradle wrapper for application-gateway-java.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 18:05:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/637" class=".btn">#637</a>
            </td>
            <td>
                <b>
                    Run a basic-asset-transfer CI test on Kubernetes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a CI test case to run an E2E validation of the basic-asset-transfer chaincode and Gateway application on the Kubernetes Test Network. This suite exercise only ONE test case, primarily as an exercise in validating the mechanics of running the Kube Test Network on an Azure image. After the mechanics of running on Azure have been worked out, additional tests can follow, both for additional Fabric routines (e.g. Commercial Paper) and new container orchestration runtimes (e.g. containerd / podman / nerdctl / etc.)

The suite runs a complete E2E, including:

- Creates a KIND Kubernetes cluster and Nginx ingress controller.

- Configures the Kubernetes Test Network (3 org: 2x peers/org + 3x orderers) using JFrog / STABLE tag Fabric images.

- Compiles and deploys asset-transfer-basic/chaincode-external Chaincode-as-a-Service.

- Creates a localhost:7051 -> service/org1-peer1:7051 port forward.

- Compiles and runs the application-gateway-typescript example on the host OS.

- Tears down the port-forward, Test Network, KIND cluster, and scrubs chaincode docker images.

Signed-off-by: Josh Kneubuhl [jkneubuh@us.ibm.com](mailto:jkneubuh@us.ibm.com)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 14:58:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/636" class=".btn">#636</a>
            </td>
            <td>
                <b>
                    Podman experimental and not native MacOs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 14:11:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/634" class=".btn">#634</a>
            </td>
            <td>
                <b>
                    Make network.sh more tolerant
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The network.sh is dependent on being executed from the test-network directory.

This PR makes it a little more tolerant, and will add a bin directory based on the location of the script - not just the PWD

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 10:18:02 +0000 UTC
    </div>
</div>

