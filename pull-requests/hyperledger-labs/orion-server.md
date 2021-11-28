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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/285" class=".btn">#285</a>
            </td>
            <td>
                <b>
                    Re-config cluster membership: peer removal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">replication</span>
            </td>
            <td>
                Handle a config TX that carries a membership change, i.e. adding or removing a member peer.

If a config transaction carries changes to the cluster membership, i.e. add or remove a node, it is proposed
using Raft’s ProposeConfChange(), with the config-block as Context field of the proposal.
This allows consensus on the new Raft membership, while consenting on the new config-block at the same time.
If the config tx does not carry changes to the cluster membership it is proposed using the normal Propose().

Implement peer removal and addition, but test only removal.
- When a node is removed, it is recommended to shutdown the removed node prior to proposing the removal config-tx.
- If the removed node is alive, it detects its own removal after it commits and then shuts down the replication component.
- The removed server may continue to serve queries until it is shutdown.
- The removed server always reports the Leader-RaftID=0, so it cannot be used for transactions.

Adding a peer is still not supported (future commit).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-28 11:51:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/283" class=".btn">#283</a>
            </td>
            <td>
                <b>
                    queries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: senthil <cendhu@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-24 16:18:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/282" class=".btn">#282</a>
            </td>
            <td>
                <b>
                    Fix image name in README
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
        Created At 2021-11-24 15:45:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/277" class=".btn">#277</a>
            </td>
            <td>
                <b>
                    Re-config cluster endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">replication</span>
            </td>
            <td>
                Allow a config Tx that changes the endpoint of an existing PeerConfig.

Note: a config TX that adds or removes peers is not yet supported (future commit).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 15:39:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/276" class=".btn">#276</a>
            </td>
            <td>
                <b>
                    minor fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: senthil <cendhu@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 10:06:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/275" class=".btn">#275</a>
            </td>
            <td>
                <b>
                    Updated images/README.md
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
        Created At 2021-11-23 09:43:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/274" class=".btn">#274</a>
            </td>
            <td>
                <b>
                    Update docker build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Same image name both locally and in docker hub
README.md to docker hub.

Signed-off-by: Gennady Laventman <gennady@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 09:03:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/272" class=".btn">#272</a>
            </td>
            <td>
                <b>
                    ConsensusConfig reconfig rules
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">replication</span>
            </td>
            <td>
                Define the rules for updating the ConsensusConfig, in particular, the Memebrs.

The core contribution is the VerifyConsensusReConfig method, that checks the configuration changes in types.ConsensusConfig.

This method checks that the changes between one ConsensusConfig to the next are safe, because some mutations might
cause a permanent loss of quorum in the cluster, something that is very difficult to recover from.
 - Members can be added or removed (membership change) one member at a time
 - Members' endpoints cannot be changed together with a membership change
 - An existing member cannot change its Raft ID (it must be removed from the cluster and added again as a new member)
 - The Raft ID of a new member must be unique - therefore it must be larger than MaxRaftId

We assume that both the current and updated ClusterConfig are internally consistent, specifically, that the Nodes
and the ConsensusConfig.Members arrays match by NodeId in each.

Signed-off-by: Yoav Tock <tock@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-22 13:58:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/271" class=".btn">#271</a>
            </td>
            <td>
                <b>
                    Overview of ledger API
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
        Created At 2021-11-22 13:22:47 +0000 UTC
    </div>
</div>

