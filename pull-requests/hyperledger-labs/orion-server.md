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
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/398" class=".btn">#398</a>
            </td>
            <td>
                <b>
                    Dynamic cluster - remove node tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: tohar-ayash <toharayash1@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-04 13:09:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/394" class=".btn">#394</a>
            </td>
            <td>
                <b>
                    provenance queries test: historical data api
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit covers all historical data apis
1. GetAllValues()
2. GetValueAt()
3. GetNextValues()
4. GetPreviousValues()
5. GetMostRecentValueAtOrBelow()

Signed-off-by: senthil <cendhu@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-02 03:01:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/393" class=".btn">#393</a>
            </td>
            <td>
                <b>
                    Restart after reconfig: add node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                After adding a node, and restarting the server, the block replicator needs
to avoid re-committing a block that was created during membership config changes,
but apply the 'ConfChangeV2' to the raft state machine. This may happen when:
 - existing nodes apply a config change but then restart from a snapshot prior to the config change;
 - a node joins an existing cluster, as on-boarding brings all the ledger from a remote peer, and then we start raft.

 must avoid re-committing the block,
Signed-off-by: Yoav Tock <tock@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-01 15:03:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/390" class=".btn">#390</a>
            </td>
            <td>
                <b>
                    Dynamic cluster - simple add test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: tohar-ayash <toharayash1@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-28 16:11:30 +0000 UTC
    </div>
</div>

