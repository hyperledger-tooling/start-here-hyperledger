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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/475" class=".btn">#475</a>
            </td>
            <td>
                <b>
                    Catch inconsistency if chaincode name does not match
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Problem

I'm testing asset-transfer-basic/chaincode-java.

If I accidently changed rootProject.name in settings.gradle to something else, but still use 

```
 ./network.sh deployCC -ccn basic -ccp ../asset-transfer-basic/chaincode-java -ccl java 
```

for deploying the chaincode, the tool compiles the source code into  ../asset-transfer-basic/chaincode-java/build/install/newName, but deploys the outdated ../asset-transfer-basic/chaincode-java/build/install/basic to the chain.


This behavior is very likely to cause confusions for beginners when they made changes to the source code but didn't see effects on the chain because network.sh is deploying the old copy named basic while the user is changing a project named newName.

## Solution

In this PR, for a Java project, network.sh is revised to remove the install folder to clean up the residues. If the root project name does not match with `-ccn`, users will see an error so that they know there is something wrong.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-24 08:58:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/471" class=".btn">#471</a>
            </td>
            <td>
                <b>
                    kubernetes test network : initial commit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR introduces a new deployment pattern for running the fabric `test-network` on Kubernetes, focusing on a local [KIND](https://kind.sigs.k8s.io) instance to emulate a cloud-native cluster.

While the project is in early status, it provides enough functionality to illustrate the basic mechanics of launching peers, orderers, chaincode, and client applications in a virtualized environment.  No attempt has been made to streamline or script the kube descriptors into a cluster at this early stage.

This project has been verified with KIND, and runs natively on IKS with minor modifications to the PVC claims and docker registry URLs.

Ahoy!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-20 16:26:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/470" class=".btn">#470</a>
            </td>
            <td>
                <b>
                    Fix: logspec output
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If ORDERER_KAFKA_VERBOSE is true, the output of /logspec will contain
the following kafka information even if it is raft orderer.
{"spec":"orderer.consensus.kafka.sarama=debug:info"}
This PR deletes environment valiable for kafka in docker-compose.

Signed-off-by: Nao Nishijima <nao.nishijima.xt@hitachi.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-19 09:01:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/469" class=".btn">#469</a>
            </td>
            <td>
                <b>
                    Remove .env Files and Explicitly Name Network (#417)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport from main to release-2.2.

There have been lots of changes and quirks with the
docker-compose .env file, this change removes the file
and explicitly creates and assigns the networks in the
compose yaml files.

Signed-off-by: Brett Logan <lindluni@github.com>
Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 17:54:09 +0000 UTC
    </div>
</div>

