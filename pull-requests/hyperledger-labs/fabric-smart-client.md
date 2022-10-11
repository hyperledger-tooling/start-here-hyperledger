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
                
            </td>
            <td>
                - Fabric: 
  - Export Envelope Service
  - Export Transaction Validation Code
- Orion:
  - Ledger Support 
  - Export Discard Tx

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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/411" class=".btn">#411</a>
            </td>
            <td>
                <b>
                    fabric ordering: retry also when establishing the connection fails
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                Currently, if getting the connection to an orderer fails the first time, no retry happens.
This PR fixes this.

Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-10 09:35:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/409" class=".btn">#409</a>
            </td>
            <td>
                <b>
                    Various bug fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                nwo:
- fix stop/start FSC node

fabric:
- if an envelope is stored for the txid, then commit it

orion:
- if an envelope is stored for the txid, then commit it
- finality fix for unknown transactions for which an envelope is stored. 

various:
- fix Committer's lister + integration test
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-07 13:16:15 +0000 UTC
    </div>
</div>

