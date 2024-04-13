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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/548" class=".btn">#548</a>
            </td>
            <td>
                <b>
                    Fix race tests
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
        Created At 2024-04-12 08:49:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/547" class=".btn">#547</a>
            </td>
            <td>
                <b>
                    committer listener
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
        Created At 2024-04-12 07:52:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/546" class=".btn">#546</a>
            </td>
            <td>
                <b>
                    transaction filter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR does the following: It allows both orion and fabric commit pipeline to process transactions that are unknown but are accepted by the custom filters.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-11 13:04:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/543" class=".btn">#543</a>
            </td>
            <td>
                <b>
                    fabric refactor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR does the following: It refactors the fabric platform without changing its functionalities. The services are better separated and then composed in the `Network` and `Channel` interface. The committer service has been unified and cleaned up. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-10 08:09:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/542" class=".btn">#542</a>
            </td>
            <td>
                <b>
                    Fix race conditions in tests
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
        Created At 2024-04-08 09:54:13 +0000 UTC
    </div>
</div>

