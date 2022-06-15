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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/254" class=".btn">#254</a>
            </td>
            <td>
                <b>
                    fix AuditDB redeem bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                Currently, AuditDB fails to record redeem transactions because it does consider only the enrollment IDs of the outputs.
In a redeem, the output has no enrollment ID.
To make sure the fix works, we augment the CheckBalance function in the integration test to enforce that the holding of the party, at the auditor, is the same as the balance at the party.
We also introduce additional checks for the current spending.

Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-10 14:41:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/253" class=".btn">#253</a>
            </td>
            <td>
                <b>
                    auditdb: extend to owner wallets #247
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-10 10:32:27 +0000 UTC
    </div>
</div>

