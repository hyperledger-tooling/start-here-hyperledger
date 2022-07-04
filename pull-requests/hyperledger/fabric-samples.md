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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/784" class=".btn">#784</a>
            </td>
            <td>
                <b>
                    Fix namespace in k8s configuration files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Issues:
1. When the name of NETWORK_NAME or NS in file "network" (i.e., the namespace in k8s) is changed from "test-network", the resources in the k8s cluster cannot be created successfully when the command "./network up" is executed.
Error message: error: the namespace from the provided object "test-network" does not match the namespace "xxxxxx". You must pass '--namespace=test-network' to perform this operation.
2. org2-cc.yaml is not completed.

Fix:
1. Replace "test-network" in yaml files in folder "kube" with "${NS}".
2. Complete "org2-cc-template.yaml" by referring to "org1-cc-template.yaml".
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-04 09:53:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/782" class=".btn">#782</a>
            </td>
            <td>
                <b>
                    Fix asset-transfer-events sample Java chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - chaincode-java Gradle project name did not match the instructions or the chaincode name used by the sample application code.
- Added test of Java chaincode to CI pipeline.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 10:47:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/781" class=".btn">#781</a>
            </td>
            <td>
                <b>
                    Update secured asset transfer sample
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A recent commit added the potential buyer to an asset's state based endorsement policy.
That change was problematic because if the transfer fell through, the buyer lost control of the asset,
in that they could no longer update the asset or change the sell price or sell to somebody else.

The asset state based endorsement policy is now based on the seller only, and we document
that additional parties could be added such as a trusted third party (although no
such party exists in test network at this time).

This commit also re-adds some necessary verifications, and make other minor edits and
comments to help users understand the sample.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-29 11:39:53 +0000 UTC
    </div>
</div>

