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
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/305" class=".btn">#305</a>
            </td>
            <td>
                <b>
                    HTTPTransport reports active peers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Utilize the rafthttp transport method that reports active peers.
2. Register the raft endpoints correctly to the ServeMux.
3. Expose a new method comm.HTTPTransport.ActivePeers, this will be used in the API that reports the cluster status (future commit).
4. Correct unit tests in comm and replication in light of the fix in (2).

After registering the raft endpoints correctly (2), the nodes may connect in an asymmetric way, that is:
- say the shared cluster config defines: (node1  localhost:1001) (node2  localhost:1002) (node3 localhost:1003)
- and: node1 binds to 1001, node2 binds to 1002
- but: node3 binds to 1004
- then: the connectivity is asymmetric - node3 can reach node1 & node2 but not the other way around

This may happen when reconfiguring an endpoint: node3 from 1003 -> 1004; and if
- node3 restarts on the new port before the config-tx, or
- it is kept alive during config-tx and restarted later.

The correct procedure for node endpoint update is to stop the node, reconfigure the remaining, and start it on the new port.

The tests were updated accordingly.

Signed-off-by: Yoav Tock <tock@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-22 13:47:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/303" class=".btn">#303</a>
            </td>
            <td>
                <b>
                    Integration testing: cluster node recovery
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
        Created At 2021-12-19 14:20:02 +0000 UTC
    </div>
</div>

