---
layout: default
title: firefly-transaction-manager
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-transaction-manager
---

# firefly-transaction-manager <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-transaction-manager){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/37" class=".btn">#37</a>
            </td>
            <td>
                <b>
                    Move 10 depth to correct channel, for spurious ack processing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There was an unused `receive` channel on the WebSocket connection, which was updated in #36 - but the actual channel that was used to queue acks (the `receiveChannel`) that is shared between all connections on given topic, was not updated.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-11 22:20:19 +0000 UTC
    </div>
</div>

