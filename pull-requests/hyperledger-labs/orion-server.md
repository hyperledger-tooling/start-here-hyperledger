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
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/244" class=".btn">#244</a>
            </td>
            <td>
                <b>
                    Solve replicator close deadlock
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                When closing the replicator, in one case, the replicator's event-loop go-routine breaks out
of the loop without broadcasting to the propose-loop sync.Cond, and the propose loop remains
waiting on it and does not exit.

The solution is to broadcast to the sync.Cond when the event-loop go-routine exits, not only
when it detects the stop signal.

Signed-off-by: Yoav Tock <tock@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 07:15:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/242" class=".btn">#242</a>
            </td>
            <td>
                <b>
                    Check TxId is a URL segment-nz
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Yoav Tock <tock@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 20:10:55 +0000 UTC
    </div>
</div>

