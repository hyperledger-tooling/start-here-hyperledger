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
                PR <a href="https://github.com/hyperledger/fabric-gateway-java/pull/118" class=".btn">#118</a>
            </td>
            <td>
                <b>
                    Use correct CryptoSuite and User context for event replay
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use the exact CryptoSuite and User context from the original HFClient when creating a new HFClient for event replay, instead of assuming that the CryptoSuite and User context are ones created using an X509IdentityProvider with the Gateway client identity.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-15 01:01:54 +0000 UTC
    </div>
</div>

