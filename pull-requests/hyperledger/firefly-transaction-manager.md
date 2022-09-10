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
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/36" class=".btn">#36</a>
            </td>
            <td>
                <b>
                    Acknowledge batches by number
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We saw a case in a performance run, where FireFly core skipped a batch of 3 events from EVMConnect.

EVMConnect believed they had been acknowledged and received, but FF Core never actually processed them.

What we found from the logs, is that FireFly Core had ended up in a situation where it was sending acknowledgements that were being interpreted by FFTM/EVMConnect as being for the _next_ batch after the one that had just been processed.

This combined with a disconnect/reconnect of the websocket, where a batch was dropped. After the reconnect - EVMConnect didn't re-send the missed batch, because it believed it already to be acknowledged.

The problem is the "acknowledge last thing you sent" protocol, combined with the fact that the WS code doesn't close the go channels through reconnects (deliberately to support multiple WS connections/reconnects). It leaves a window where an ack can be misinterpretted from before a reconnect. There are attempts in the code to make this window very small - with the code by clearing out the go channel that passes `ack` payloads to the batch dispatcher, before delivering the batch. However, that does not eliminate the window completely.

So this PR make a breaking change to the protocol to be specific about the batch being ack'd:
- Change the payload for events passed by FFTM/EVMConnect to FF Core, from a top-level array, to an object structure like:
    ```js
    { "batchNumber":  12345, "events": [ ... ] }
    ```
- Change the `ack` payload to have a `batchNumber` declaring which batch is being ack'd
- Moved "spurious" / extra ack processing from the WS side of the Go channel, to the batch manager side
- Extend the length of the go channel from `1` to `10` - because now the acks are unique, we could stall if we missed one
- If for any reason we get too many spurious acks that fill up the channel, then close the websocket rather than losing it (there really only ever should be one, after a reconnect)

FF Core and the Tokens connectors will need to be updated:
- To handle _either_ the old EthConnect flat array payloads, or the new style FFTM/EVMConnect payloads with an object containing `batchNumber` and `events`
- Include the `batchNumber` in the corresponding `ack`

> Note that the reply payloads that do _not_ require acknowledgement come over the same pipe, and this is an area that could be overall made more consistent in the future.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-08 02:42:35 +0000 UTC
    </div>
</div>

