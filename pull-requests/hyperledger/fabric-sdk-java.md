---
layout: default
title: fabric-sdk-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-java
---

# fabric-sdk-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/261" class=".btn">#261</a>
            </td>
            <td>
                <b>
                    release-2.2 mutual tls config key and peer property key not matching #260
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I have done the changes as follows:

1. change property names from tlsClient* to client* in NetworkConfig.java; add unit test and associated fixture.
2. change from tlsClient* to client* in HFCAClient.java; add unit test and associated fixtures.
3. Refactor clientCert* and clientKey* to constant in Endpoint.java and apply the constants in Channel.java.

Closes #260
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-08 02:19:36 +0000 UTC
    </div>
</div>

