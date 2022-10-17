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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/415" class=".btn">#415</a>
            </td>
            <td>
                <b>
                    restructure fsc and fabric driver core to be more intuitive
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">configuration</span><span class="chip">Fabric</span>
            </td>
            <td>
                1. create a grpc section in core and move appropriate keys to be children
2. sort out tls for fabric-driver section
3. make web client configuration keys match intent

Signed-off-by: Dave Kelsey <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-11 13:48:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/414" class=".btn">#414</a>
            </td>
            <td>
                <b>
                    Extensions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">Fabric</span><span class="chip">orion</span>
            </td>
            <td>
                - Fabric: 
  - Export Envelope Service
  - Export Transaction Validation Code
  - TxIDStore stores now also busy transactions
  - Restart delivery from the last block seen, if available.
- Orion:
  - Ledger Support 
  - Export Discard Tx
  - TxIDStore stores now also busy transactions

Used by: https://github.com/hyperledger-labs/fabric-token-sdk/pull/406

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-11 11:40:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/412" class=".btn">#412</a>
            </td>
            <td>
                <b>
                    kvs/vault web browser
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
        Created At 2022-10-10 13:29:48 +0000 UTC
    </div>
</div>

