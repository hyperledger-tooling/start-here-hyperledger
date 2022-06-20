---
layout: default
title: fabric-token-sdk
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-token-sdk
---

# fabric-token-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-token-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/265" class=".btn">#265</a>
            </td>
            <td>
                <b>
                    Doc Correction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sapthasurendran <saptha.surendran@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 12:55:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/263" class=".btn">#263</a>
            </td>
            <td>
                <b>
                    htlc exchange services
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 09:37:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/260" class=".btn">#260</a>
            </td>
            <td>
                <b>
                    update FSC dep to latest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the Token-SDK to the FSC version that offers enhanced discovery capabilities. (https://github.com/hyperledger-labs/fabric-smart-client/issues/293)

Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 08:20:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/259" class=".btn">#259</a>
            </td>
            <td>
                <b>
                    htlc basic integration test infrastructure
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Hagar Meir <hagar.meir@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 08:06:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/257" class=".btn">#257</a>
            </td>
            <td>
                <b>
                    Namespace is always zkat even if it was changed in the node config #256
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When invoking token.GetManagementService() without any additional option, the token-api tries to load the default TMS. What does this mean? The token-api checks if there is a default fabric or orion network configuration, if yes it consider that the default. For the channel, it is the same. For the namespace, the issue is that there can be multiple token namespaces in the same <network, channel>. So, the code currently uses the default namespace zkat.

So, the solution we can put forth is the following: The code checks the configuration and if there is a unique tuple <network, channel, namespace>, the code will use that one, otherwise it will return an error.

Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 07:22:15 +0000 UTC
    </div>
</div>

