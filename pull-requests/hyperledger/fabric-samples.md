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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/502" class=".btn">#502</a>
            </td>
            <td>
                <b>
                    Fix function comment in asset-transfer-ledger-queries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix typo in function comment.

Thanks to RobertBetschinger for finding this issue.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 02:35:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/501" class=".btn">#501</a>
            </td>
            <td>
                <b>
                    Add .env with DOCKER_SOCK variable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Aditya Hajare <aditya43@gmail.com>

Added .env file with DOCKER_SOCK variable set to Unix socket for curl requests to Docker API.
Without this variable, following error was encountered:
```
docker-compose -f docker-compose-test-net.yaml up   
WARNING: The DOCKER_SOCK variable is not set. Defaulting to a blank string.
orderer.example.com is up-to-date
Creating peer0.org2.example.com ... error
Creating peer0.org1.example.com ... 

ERROR: for peer0.org2.example.com  Cannot create container for service peer0.org2.example.com: create .: volume name is too short, names should be at least two alphanumeric chaCreating peer0.org1.example.com ... error

ERROR: for peer0.org1.example.com  Cannot create container for service peer0.org1.example.com: create .: volume name is too short, names should be at least two alphanumeric characters

ERROR: for peer0.org2.example.com  Cannot create container for service peer0.org2.example.com: create .: volume name is too short, names should be at least two alphanumeric characters

ERROR: for peer0.org1.example.com  Cannot create container for service peer0.org1.example.com: create .: volume name is too short, names should be at least two alphanumeric characters
ERROR: Encountered errors while bringing up the project.
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-06 15:01:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/500" class=".btn">#500</a>
            </td>
            <td>
                <b>
                    Update go.mod
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
        Created At 2021-10-06 14:47:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/498" class=".btn">#498</a>
            </td>
            <td>
                <b>
                    Run the fabric test network on Kubernetes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Example scripts and guide to run the Fabric test-network on Kubernetes.
- Includes a `./network kind` command to quickly bootstrap a local KIND cluster and container registry. 
- Includes a reference guide for building and launching Chaincode-as-a-Service and External Chaincode Builders. 
- Includes a reference guide for debugging chaincode locally, invoked from Fabric on Kubernetes.
- Includes a reference deployment of the [fabric-rest-sample](https://github.com/hyperledgendary/fabric-rest-sample) blockchain application. 
- Tested with KIND and IKS Kubernetes clusters. 


Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-04 11:45:08 +0000 UTC
    </div>
</div>

