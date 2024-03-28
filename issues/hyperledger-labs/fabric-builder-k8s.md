---
layout: default
title: fabric-builder-k8s
parent: Hyperledger Labs
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger-labs/fabric-builder-k8s
---

# fabric-builder-k8s <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-builder-k8s){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger-labs/fabric-builder-k8s/issues/102" class=".btn">102</a>
            </td>
            <td>
                <b>
                    Add resource limits configuration capabilities for the chaincode pods
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">help wanted</span>
            </td>
            <td>
                The chaincode PODS don ´t have defined the resource limits.

Those limits can be configured in:

1. Chaincode Artifacts - image.json;
2. Environment Variables;
4. etc?

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-21 11:46:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger-labs/fabric-builder-k8s/issues/100" class=".btn">100</a>
            </td>
            <td>
                <b>
                    Add liveness probe support to chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">help wanted</span><span class="chip">design</span>
            </td>
            <td>
                Based on discussions with @y12studio in #98, it would be useful to support liveness probes for chaincode containers.

I don't think there is a simple way to implement this with current Fabric capabilities since the peer<->chaincode communication is via a long-lived grpc stream, and I'm not sure what chaincode language neutral alternatives might be possible instead.

One possibility is to update the Fabric protos to add a liveness service for chaincode implementations to (optionally?) support this requirement. The peer uses a separate operations service for [health checks](https://hyperledger-fabric.readthedocs.io/en/release-2.5/operations_service.html#health-checks) but that doesn't seem like a good approach for chaincode.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-01 17:31:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger-labs/fabric-builder-k8s/issues/98" class=".btn">98</a>
            </td>
            <td>
                <b>
                    Add signal handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span>
            </td>
            <td>
                Ideally the k8s pod should be terminated if the peer is terminated. This is related to #88 however it will not always be possible to add an owner reference.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-02 19:54:22 +0000 UTC
    </div>
</div>

