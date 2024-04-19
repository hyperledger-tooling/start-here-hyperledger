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
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/551" class=".btn">#551</a>
            </td>
            <td>
                <b>
                    fix finality listener
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
        Created At 2024-04-19 07:37:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/550" class=".btn">#550</a>
            </td>
            <td>
                <b>
                    Refactor/reuse vault
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvement</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-18 09:50:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/549" class=".btn">#549</a>
            </td>
            <td>
                <b>
                    add fallback option to use OrdererAddresses
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If the Orderer MSP does not have Endpoints in its channel config, this PR adds a fallback check. Another valid configuration for orderer endpoints is OrdererAddresses in the ChannelConfig, see https://hyperledger-fabric.readthedocs.io/en/latest/config_update.html.

**Orderer addresses.** A list of addresses where clients may invoke the orderer Broadcast and Deliver functions. The peer randomly chooses among these addresses and fails over between them for retrieving blocks.

The OrdererAddresses do not have TLSRootCerts. The code only uses the OrdererAddresses key if there is one OrdererMSP in the channel, so that it can use the root certs from there.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-13 13:34:25 +0000 UTC
    </div>
</div>

