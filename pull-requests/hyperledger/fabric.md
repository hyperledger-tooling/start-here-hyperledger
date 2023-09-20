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
                PR <a href="https://github.com/hyperledger/fabric/pull/4445" class=".btn">#4445</a>
            </td>
            <td>
                <b>
                    Add orderer backoff
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                By default, the maximum time between attempts to connect one orderer to another via grpc is 2 minutes. And the waiting time for a heartbeat message from the leader in smartbft is 1 minute.
Therefore, it is possible to choose a time interval between the start of the leader and the follower, such that the follower will leave the consensus immediately.

This hotfix adds the ability to set the maximum time between connection attempts (ORDERER_GENERAL_BACKOFF_MAXDELAY).

Recommendations: if LeaderHeartbeatTimeout is 1m, then MaxDelay 20s.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-18 21:45:12 +0000 UTC
    </div>
</div>

