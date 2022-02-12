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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/641" class=".btn">#641</a>
            </td>
            <td>
                <b>
                    Issue 602
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Flow:

Check if docker network is running. 
If network is not running exit
If running, and containers are present + certs are present skip network up
If running, containers are not present then we should networkUp
If containers exist but certs don’t, bring network down and then networkUp

When containers are running but for some reason peerOrganisation dir was not present, the following error: 
`Failed to generate channel configuration transaction...` may be awkward to debug. So this is why there is a check to see if peerOrg does not exist but the containers do. 


Test Cases: 

1) Docker is not running 
```
./network.sh up createChannel -ca
Using docker and docker-compose
Creating channel 'mychannel'.
If network is not up, starting nodes with CLI timeout of '5' tries and CLI delay of '3' seconds and using database 'leveldb 
docker network is required to be running to create a channel
```

2) Docker is running but containers are not, peerOrganizations directory exists
```
./network.sh up createChannel -ca
Using docker and docker-compose
Creating channel 'mychannel'.
If network is not up, starting nodes with CLI timeout of '5' tries and CLI delay of '3' seconds and using database 'leveldb 
Bringing up network
LOCAL_VERSION=2.4.1
DOCKER_IMAGE_VERSION=2.4.1
CA_LOCAL_VERSION=1.5.2
CA_DOCKER_IMAGE_VERSION=1.5.2
WARN[0000] Found orphan containers ([ca_org2 ca_org1 ca_orderer]) for this project. If you removed or renamed this service in your compose file, you can run this command with the --remove-orphans flag to clean it up. 
[+] Running 4/4
 ⠿ Container peer0.org2.example.com  Started                                                                                                                                                                                                                               0.6s
 ⠿ Container peer0.org1.example.com  Started                                                                                                                                                                                                                               0.6s
 ⠿ Container orderer.example.com     Started                                                                                                                                                                                                                               0.6s
 ⠿ Container cli                     Started  
```
3) Containers running but  peerOrganizations directory does not exist
```
./network.sh up createChannel -ca
Using docker and docker-compose
Creating channel 'mychannel'.
If network is not up, starting nodes with CLI timeout of '5' tries and CLI delay of '3' seconds and using database 'leveldb with crypto from 'Certificate Authorities'
Decomposing compose-test-net.yaml
[+] Running 10/7
 ⠿ Container orderer.example.com          Removed                                                                                                                                                                                                                          0.2s
 ⠿ Container cli                          Removed                                                                                                                                                                                                                         10.2s
 ⠿ Container peer0.org1.example.com       Removed                                                                                                                                                                                                                          0.3s
 ⠿ Container peer0.org2.example.com       Removed                                                                                                                                                                                                                          0.3s
 ⠿ Container ca_orderer                   Removed                                                                                                                                                                                                                          0.3s
 ⠿ Container ca_org2                      Removed                                                                                                                                                                                                                          0.3s
 ⠿ Container ca_org1                      Removed                                                                                                                                                                                                                          0.3s
 ⠿ Volume compose_peer0.org2.example.com  Removed                                                                                                                                                                                                                          0.0s
 ⠿ Volume compose_peer0.org1.example.com  Removed                                                                                                                                                                                                                          0.0s
 ⠿ Volume compose_orderer.example.com     Removed                                                                                                                                                                                                                          0.0s
Decomposing compose-couch.yaml
service "peer0.org1.example.com" has neither an image nor a build context specified: invalid compose project
Decomposing compose-ca.yaml
[+] Running 1/0
 ⠿ compose  Warning: No resource found to remove                                                                                                                                                                                                                           0.0s
Error: No such volume: docker_orderer.example.com
Error: No such volume: docker_peer0.org1.example.com
Error: No such volume: docker_peer0.org2.example.com
Removing remaining containers
Removing generated chaincode docker images
"docker kill" requires at least 1 argument.
See 'docker kill --help'.

Usage:  docker kill [OPTIONS] CONTAINER [CONTAINER...]

Kill one or more running containers
Bringing up network
LOCAL_VERSION=2.4.1
DOCKER_IMAGE_VERSION=2.4.1
CA_LOCAL_VERSION=1.5.2
...
```

Signed-off-by: Kieran O Mahony [Kieran.O.Mahony1@ibm.com](mailto:Kieran.O.Mahony1@ibm.com)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-11 23:28:48 +0000 UTC
    </div>
</div>

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

