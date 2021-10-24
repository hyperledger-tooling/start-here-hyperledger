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
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/218" class=".btn">#218</a>
            </td>
            <td>
                <b>
                    Get last ledger block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding API to get last ledger block using /ledger/block/last URL

This API used to get ledger height and get ledger last block at once.

Signed-off-by: Gennady Laventman <gennady@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-24 14:29:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/217" class=".btn">#217</a>
            </td>
            <td>
                <b>
                    Block numbering in replicator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">replication</span>
            </td>
            <td>
                The block replicator is made in charge of numbering the blocks and setting the last header base hash.
The block replicator keeps track of the last committed block, and the last proposed block, and
updates them whe leadership is assumed and lost.

The block numbers given the block creator are provisional, and number the sequence of proposals since
the node started its current incarnation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 17:26:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/211" class=".btn">#211</a>
            </td>
            <td>
                <b>
                    Release txs replicator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">replication</span>
            </td>
            <td>
                When a leader loses its leadership, it should stop proposing blocks to raft, and drain all blocks
waiting to be proposed by calling ReleaseWithError to the PendingTxs queue.
This will eventually reject, redirect, or drop all the transactions waiting for replication.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 14:21:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/209" class=".btn">#209</a>
            </td>
            <td>
                <b>
                    MPTrie Proof data scructure comments fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                Misleading comment in state.Proof data structure.

Signed-off-by: Gennady Laventman <gennady@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-18 14:12:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/206" class=".btn">#206</a>
            </td>
            <td>
                <b>
                    Release txs in block-creator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">replication</span>
            </td>
            <td>
                When the replicator rejects a block, release TXs in the block from the PendingTxs queue.

Signed-off-by: Yoav Tock <tock@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-17 19:47:20 +0000 UTC
    </div>
</div>

