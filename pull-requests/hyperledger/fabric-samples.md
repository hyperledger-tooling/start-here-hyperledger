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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/609" class=".btn">#609</a>
            </td>
            <td>
                <b>
                    Update test-network to use org level ca-cert.pem
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Although test network scripts functionally worked, they demonstrated
some strange patterns around use of the ca cert.

This change makes it clear that the ca cert is configured and used
at the org level, and not related to any individual peer or orderer node.
Also that when connecting to individual servers, clients can pass the
org level CA cert as the root of trust when establishing TLS connections.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-01 08:16:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/608" class=".btn">#608</a>
            </td>
            <td>
                <b>
                    DRAFT Feature/k8s e2e test with cert manager DO NOT MERGE
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
DO NOT MERGE - THIS IS A DRAFT PR

Testing some E2E / CI script runs on Azure.

This build incorporates cert-manager.io as a Kube-native provider of TLS certificates for the test network.  TLS certificates are issued with cert-manager, and MSP certificates are issued with the Fabric-CA.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-31 17:36:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/607" class=".btn">#607</a>
            </td>
            <td>
                <b>
                    Minor improvement to test network docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also fix the version of prometheus and grafana being used
to ensure the queries remain compatible as well as avoid
issues whether they may not work if latest images already
exist on machine but are not at a level that will work

Signed-off-by: D <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-31 13:38:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/606" class=".btn">#606</a>
            </td>
            <td>
                <b>
                    Convert comments to tsdoc in REST sample
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-31 12:48:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/605" class=".btn">#605</a>
            </td>
            <td>
                <b>
                    Run basic-asset-transfer on the Kubernetes Test Network in an Azure CI pipeline 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a CI test case to run an E2E validation of the basic-asset-transfer chaincode and Gateway application on the Kubernetes Test Network.  This suite exercise only ONE test case, primarily as an exercise in validating the mechanics  of running the Kube Test Network on an Azure image.  After the mechanics of running on Azure have been worked out, additional tests can follow, both for additional Fabric routines (e.g. Commercial Paper) and new container orchestration runtimes (e.g. containerd / podman / nerdctl / etc.) 

The suite runs a complete E2E, including: 

- Creates a KIND Kubernetes cluster and Nginx ingress controller.

- Configures the Kubernetes Test Network (3 org: 2x peers/org + 3x orderers) using JFrog / STABLE tag Fabric images.

- Compiles and deploys asset-transfer-basic/chaincode-external Chaincode-as-a-Service.

- Creates a localhost:7051 -> service/org1-peer1:7051 port forward.

- Compiles and runs the application-gateway-typescript example on the host OS.

- Tears down the port-forward, Test Network, KIND cluster, and scrubs chaincode docker images.


Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-28 18:03:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/604" class=".btn">#604</a>
            </td>
            <td>
                <b>
                    Podman nerdctl experiement - DO NOT MERGE
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-28 16:15:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/601" class=".btn">#601</a>
            </td>
            <td>
                <b>
                    Fix markdown logical structure in asset-transfer-events/README.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fenced code blocks within a list were at the wrong level if indentation and so logically terminated the list.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 17:05:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/600" class=".btn">#600</a>
            </td>
            <td>
                <b>
                    Refactor of asset transfer events Go sample for Fabric Gateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Split boiler-plate connection code into a separate file since the basic sample already covers this aspect. The `app.go` file now only presents the main application code, making it much easier for readers to view.

Also changed the event replay code to use a different style of reading from the real-time eventing example, demonstrating the use of timeouts while reading events we expect to arrive quickly, and avoiding any possibility of the main application execution hanging indefinitely.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 12:27:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/599" class=".btn">#599</a>
            </td>
            <td>
                <b>
                    fix a bug in function [getBlockByNumber]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This bug can lead to users can't change target peer to send query operations.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 11:45:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/598" class=".btn">#598</a>
            </td>
            <td>
                <b>
                    Fix CHAINCODE_AS_A_SERVICE_TUTORIAL.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes several typos and more importantly add an instruction to
set FABRIC_CFG_PATH without which the peer command fails.

Signed-off-by: Arnaud J Le Hors <lehors@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 07:45:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/597" class=".btn">#597</a>
            </td>
            <td>
                <b>
                    Asset transfer events Go sample for Fabric Gateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-26 19:37:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/596" class=".btn">#596</a>
            </td>
            <td>
                <b>
                    Experimental Support for using podman with the test-network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Podman support

A copy of the `install_fabric.sh` script is in the `test-network` directory. This has been enhanced to support a `podman` argument; if used it will use `podman` to pull down images and tag them rather than docker. The images are the same, but need to pulled differently.

The `network.sh` script has been enhanced so that it can use `podman` and `podman-compose` instead of docker. Ensure that `CONTAINER_CLI` is set as below when running anet `network.sh` script. 

```bash
CONTAINER_CLI=podman ./network.sh up
````

As there is no Docker-Daemon in this context, only Chaincode-as-a-service is supported.

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-26 09:54:18 +0000 UTC
    </div>
</div>

