---
layout: default
title: fabric-smart-client
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-smart-client
---

# fabric-smart-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-smart-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/421" class=".btn">#421</a>
            </td>
            <td>
                <b>
                    nwo delete vault
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
        Created At 2022-10-18 14:31:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/420" class=".btn">#420</a>
            </td>
            <td>
                <b>
                    sample config with doc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a sample core.yaml file for fsc and fabric-driver, for discussion to add and improve the associated documentation
Signed-off-by: Dave Kelsey <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-18 08:54:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/417" class=".btn">#417</a>
            </td>
            <td>
                <b>
                    Fix npe if no core file found
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                closes #406

Signed-off-by: Dave Kelsey <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-14 12:52:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/416" class=".btn">#416</a>
            </td>
            <td>
                <b>
                    fabric: call discard for unknown tx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                Currently, when a transaction is marked is invalid by Fabric and it is unknown to the vault, no event is fired.
The point is that the node can still be aware of the transaction because it stores the corresponding envelope.

This PR, discard all transactions.

Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-12 08:13:26 +0000 UTC
    </div>
</div>

