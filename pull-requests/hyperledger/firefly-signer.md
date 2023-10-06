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
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/50" class=".btn">#50</a>
            </td>
            <td>
                <b>
                    Add wsbackend client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a JSONRPC WebSocket client.

- Provides sync `CallRPC` functionality over an async WebSocket transport
    - Manages JSON/RPC request IDs for you
    - Provides automatic reconnect, and all the other quality of life benefits of the `firefly-common` WebSocket impl
- Supports `eth_subscribe`/`eth_unsubscribe` with a higher level `Subscription` semantic
    - Automatically resubscribes if your WebSocket reconnects
    - Has a client-side ID to track your subscription, as well as the server-side ID (which changes on reconnect)
    - At-most-once delivery semantics is all you get with raw Ethereum WebSockets (it's all the `eth_` protocol supports) - you miss it, you lose it
        - If you need more than that, use the full [FireFly core](https://github.com/kaleido-io/firefly) which provides reliable check-pointed subscriptions with a higher level blockchain connector

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 20:19:44 +0000 UTC
    </div>
</div>

