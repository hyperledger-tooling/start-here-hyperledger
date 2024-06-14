---
layout: default
title: fabric-gateway-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-gateway-java
---

# fabric-gateway-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-gateway-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway-java/pull/172" class=".btn">#172</a>
            </td>
            <td>
                <b>
                    Use only v2.2.x packages in test chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Newer v2.5 chaincode packages are not compatible with the v2.2 chaincode container. The test chaincode previously used the latest v2.x release of the chaincode packages. This change restricts use to only v2.2.x packages, matching the Fabric v2.2 version used for testing.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-13 18:30:26 +0000 UTC
    </div>
</div>

