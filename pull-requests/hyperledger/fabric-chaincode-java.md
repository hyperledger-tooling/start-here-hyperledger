---
layout: default
title: fabric-chaincode-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-chaincode-java
---

# fabric-chaincode-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-chaincode-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/253" class=".btn">#253</a>
            </td>
            <td>
                <b>
                    Bump version to 2.5.0
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
        Created At 2022-07-19 16:56:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/252" class=".btn">#252</a>
            </td>
            <td>
                <b>
                    Bump version to 2.4.2
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
        Created At 2022-07-19 16:48:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/250" class=".btn">#250</a>
            </td>
            <td>
                <b>
                    PurgePrivateData
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implements the purgePrivateData API in the stub

Closes #240 

Fabric Issue https://github.com/hyperledger/fabric/issues/3020

Signed-off-by: fraVlaca <ocsenarf@outlook.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-15 16:08:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/249" class=".btn">#249</a>
            </td>
            <td>
                <b>
                    Swap to using the published fabric-protos libraries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Move the codebase to directly using the published protobuf libraries. The fabric-protos
repo, as well as holding the 'main' copy of the protos, also publishes packages for each language
These can then be pulled directly here; everything under version control.

Removes the need to the copies of the protobufs held locally in this repo.

Signed-off-by: fraVlaca <ocsenarf@outlook.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-15 09:57:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/248" class=".btn">#248</a>
            </td>
            <td>
                <b>
                    Fix(security): Path Traversal Bug & Arbitrary Code Execution 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes to ```/fabric-chaincode-integration-test/src/contracts/bare-maven/.mvn/wrapper/MavenWrapperDownloader.java```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-13 06:18:14 +0000 UTC
    </div>
</div>

