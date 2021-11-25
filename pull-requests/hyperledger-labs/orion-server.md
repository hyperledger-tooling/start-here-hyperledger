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
                    WIP: Re-config cluster endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">replication</span>
            </td>
            <td>
                <nil>
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/270" class=".btn">#270</a>
            </td>
            <td>
                <b>
                    Adding cryptoGen.sh documentation.
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
        Created At 2021-11-21 17:16:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/269" class=".btn">#269</a>
            </td>
            <td>
                <b>
                    Updating sdk transactions, docker documentation and broken links
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
        Created At 2021-11-21 14:22:43 +0000 UTC
    </div>
</div>

