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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/503" class=".btn">#503</a>
            </td>
            <td>
                <b>
                    Do not weep for the UNKIND Kubernetes test-network prototype. 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The [new one](/hyperledger/fabric-samples/tree/main/test-network-k8s) is much better.


_Farewell! thou art too dear for my possessing,
And like enough thou knowst thy estimate.
The Charter of thy worth gives thee releasing;
My bonds in thee are all determinate.
For how do I hold thee but by thy granting,
And for that riches where is my deserving?
The cause of this fair gift in me is wanting,
And so my patent back again is swerving.
Thy self thou gav'st, thy own worth then not knowing,
Or me, to whom thou gav'st it, else mistaking,
So thy great gift, upon misprision growing,
Comes home again, on better judgement making.
   Thus have I had thee as a dream doth flatter:
   In sleep a king, but waking no such matter._

  -- Bill

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 16:43:13 +0000 UTC
    </div>
</div>

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

