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
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/311" class=".btn">#311</a>
            </td>
            <td>
                <b>
                    Validate config preorder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">replication</span>
            </td>
            <td>
                Validate a config tx before proposing in to Raft.

We validate a config TX preorder to prevent a membership change to be applied to Raft, and then
have the TX marked invalid during commit. Note that ConfigTxValidator.Validate reads the current
config from the store. However, together with the code to prevent in-flight config blocks before
proposing a new one (future commit), the  config from the store should match the config stored in
the BlockReplicator.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-04 15:00:16 +0000 UTC
    </div>
</div>

