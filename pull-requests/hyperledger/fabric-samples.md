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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/486" class=".btn">#486</a>
            </td>
            <td>
                <b>
                    updated chaincodes for asset-transfer-basic in order to show good example on how achieving determinism over json
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Show good praticse in order to make sure that data will be stored in the blockchain in a deterministic way using json
Signed-off-by: fraVlaca <ocsenarf@outlook.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-06 10:05:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/483" class=".btn">#483</a>
            </td>
            <td>
                <b>
                    Move to use the 1.4.5 rather than snapshot versions
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
        Created At 2021-09-02 10:00:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/482" class=".btn">#482</a>
            </td>
            <td>
                <b>
                    Update Compose Spec & VM Spec Version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Based on PR #449 by Brett Logan <lindluni@github.com>

Signed-off-by: Arnaud J Le Hors <lehors@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-02 08:31:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/481" class=".btn">#481</a>
            </td>
            <td>
                <b>
                    Updated dependencies for Json and fabric-chaincode-shim:2.+ in java samples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Json libraries were pulled into the project in fabric-chaincode-shim:2.+  BUT - they were declared in the project scope as compileOnly and/or testImplementation.
Fabric-chaincode-shim used to (2.2.3) declare the json dependency with scope compile. In 2.3.1 and 2.4.0-beta the transitive dependencies are declared as runtime, which means they won’t be available to the compiler.
Changed all java dependecies from 
"compileOnly 'org.hyperledger.fabric-chaincode-java:fabric-chaincode-shim:2.+'"
to
"implementation 'org.hyperledger.fabric-chaincode-java:fabric-chaincode-shim:2.+'
implementation 'org.json:json:+'"
Additionally declaration for transient dependency 'org.hyperledger.fabric.protos.common' was added
P.S. dependencies were already changed from compile only to implementatio in PR [#465](https://github.com/hyperledger/fabric-samples/pull/465) for other reason related to using fabric with microfab
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-31 16:15:38 +0000 UTC
    </div>
</div>

