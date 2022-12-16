---
layout: default
title: fabric-builder-k8s
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-builder-k8s
---

# fabric-builder-k8s <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-builder-k8s){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-builder-k8s/pull/77" class=".btn">#77</a>
            </td>
            <td>
                <b>
                    Add service account configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The chaincode pod service account may need image pull secrets defined to access chaincode images, which should not be added to the default service account

Add a new FABRIC_K8S_BUILDER_SERVICE_ACCOUNT option to start chaincode pods with a different service account

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-16 16:58:52 +0000 UTC
    </div>
</div>

