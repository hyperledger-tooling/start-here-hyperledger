---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4913" class=".btn">#4913</a>
            </td>
            <td>
                <b>
                    Update docs for Ed25519 support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update docs for Ed25519 support.
Also clarify ECDSA and RSA support.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-27 21:13:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4912" class=".btn">#4912</a>
            </td>
            <td>
                <b>
                    find and fix error in tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - For unit-test in smartbft I increased the waiting time for the desired altitude. There were cases when orders went to synchronization and there was simply not enough time and changed the heartbeat settings
- Fix the integration test in smartbft_block_deliverer_test.go
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-26 11:36:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4911" class=".btn">#4911</a>
            </td>
            <td>
                <b>
                    Disable peer.deliveryclient.blockGossipEnabled in sample core.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since v2.2 it has been recommended to configure all peers to be orgLeaders so that they pull blocks from ordering service.

In v2.4 peer.deliveryclient.blockGossipEnabled was added and recommended to be set to false so that peers don't gossip pulled blocks.

These settings simplify peer behavior and reduce communication between peers (at the expense of more connections to ordering service).

Finally in v3.0 peer.deliveryclient.blockGossipEnabled is set to false by default.

This change also updates core.yaml and documentation to make these recommendations clear and consistent.

Closes https://github.com/hyperledger/fabric/issues/3961
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-25 19:39:48 +0000 UTC
    </div>
</div>

