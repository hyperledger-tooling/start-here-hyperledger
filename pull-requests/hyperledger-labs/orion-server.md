---
layout: default
title: orion-server
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/orion-server
---

# orion-server <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/orion-server){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/288" class=".btn">#288</a>
            </td>
            <td>
                <b>
                    Re-config cluster membership: peer addition
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">replication</span>
            </td>
            <td>
                Allow a config-tx to carry a membership change that adds a peer.
Test that the peer was added to the existing cluster.
Note that bootstrapping the peer is not yet supported (future commit).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-30 08:20:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/287" class=".btn">#287</a>
            </td>
            <td>
                <b>
                    Adding proofs general doc, ledger, block header, Merkle tree and MPTrie
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Gennady Laventman <gennady@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-28 18:20:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/286" class=".btn">#286</a>
            </td>
            <td>
                <b>
                    Re-config comm transport endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">replication</span>
            </td>
            <td>
                Allow the HTTPTransport to update its member peers - add peer / remove peer / change peer endpoint.
This includes both the raft http transport and the catchup client.

Note: a config TX that adds or removes peers is not yet supported (future commit).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-28 14:35:40 +0000 UTC
    </div>
</div>

