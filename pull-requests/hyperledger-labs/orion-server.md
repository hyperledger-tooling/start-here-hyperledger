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
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/297" class=".btn">#297</a>
            </td>
            <td>
                <b>
                    Admin API to get last config block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">replication</span>
            </td>
            <td>
                When an admin joins a new server to the cluster, he has to provide to the new server
the last config block of the cluster. In this commit we expose an API that allows him
to get this block from the cluster.

Signed-off-by: Yoav Tock <tock@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-09 12:12:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/296" class=".btn">#296</a>
            </td>
            <td>
                <b>
                    Cluster bootstrap join in replication
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
        Created At 2021-12-08 18:11:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/295" class=".btn">#295</a>
            </td>
            <td>
                <b>
                    Cluster bootstrap join server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">replication</span>
            </td>
            <td>
                When boostrap.method is 'join' the config loads a config block from a binary file.
The boostrapping sequence of the server is changed. Instead of generating the genesis
block, from the shared-config object, the server gets a config block (a.k.a. the join-block).
The server selects from where to take the cluster config: (1) from the DB, or (2) the
join-block; depending on which is more recent. The server then starts the transport and
replication components with the most recent cluster-config, and also lets the replication
have the join-block.

Note: the functionality in the replication component that does on-boarding is not yet
implemented (future commit).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 16:56:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/294" class=".btn">#294</a>
            </td>
            <td>
                <b>
                    Cluster bootstrap join config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">replication</span>
            </td>
            <td>
                When boostrap.method is 'join' the config loads a config block from a binary file.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 16:53:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/293" class=".btn">#293</a>
            </td>
            <td>
                <b>
                    Proofs documentation and code snipplets for SDK.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span>
            </td>
            <td>
                Signed-off-by: Gennady Laventman <gennady@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-07 11:44:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/291" class=".btn">#291</a>
            </td>
            <td>
                <b>
                    Updated readme - first pr
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Hanan Singer <hanan@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-06 12:17:30 +0000 UTC
    </div>
</div>

