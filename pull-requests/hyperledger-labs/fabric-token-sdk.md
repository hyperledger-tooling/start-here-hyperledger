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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/251" class=".btn">#251</a>
            </td>
            <td>
                <b>
                    improve identity and wallet default cache size management
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Mathilde Ffrench <mathilde.ffrench@fr.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 16:48:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/249" class=".btn">#249</a>
            </td>
            <td>
                <b>
                    filter metadata by recipient identity #212
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
        Created At 2022-06-08 09:18:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/248" class=".btn">#248</a>
            </td>
            <td>
                <b>
                    CI go1.17
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
        Created At 2022-06-08 07:41:51 +0000 UTC
    </div>
</div>

