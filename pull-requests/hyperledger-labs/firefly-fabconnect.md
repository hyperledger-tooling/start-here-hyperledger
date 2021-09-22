---
layout: default
title: firefly-fabconnect
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-fabconnect
---

# firefly-fabconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-fabconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-fabconnect/pull/47" class=".btn">#47</a>
            </td>
            <td>
                <b>
                    Gateway client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added support to use the gateway implementation in the SDK (client-side gateway) that works with a Fabric peer that has the discovery service turned on, in order to minimize the required information inside the connection profile.

This works when `UserGatewayClient: true` is configured. If not set or set to `false`, then the original support of solely relying on the connection profile is used.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-21 19:38:46 +0000 UTC
    </div>
</div>

