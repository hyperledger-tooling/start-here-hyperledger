---
layout: default
title: firefly-signer
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-signer
---

# firefly-signer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-signer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/53" class=".btn">#53</a>
            </td>
            <td>
                <b>
                    Fix auto reconnect for RPC WebSocket
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In the case of a reconnect the `resChl` was `nil` so sending `nil` to it ended up blocking, causing the receiver to not receive any further messages.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-30 20:29:49 +0000 UTC
    </div>
</div>

