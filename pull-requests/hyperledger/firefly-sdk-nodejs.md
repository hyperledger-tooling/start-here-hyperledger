---
layout: default
title: firefly-sdk-nodejs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-sdk-nodejs
---

# firefly-sdk-nodejs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-sdk-nodejs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-sdk-nodejs/pull/62" class=".btn">#62</a>
            </td>
            <td>
                <b>
                    Support non-reconnecting websockets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - treat a recconectDelay of -1 as meaning do not attempt to reconnect
- reconnecting is not always desirable - for example when using firefly-sdk as a websocket proxy

Signed-off-by: Chris Bygrave <chris.bygrave@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-01 20:50:32 +0000 UTC
    </div>
</div>

