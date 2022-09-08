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
                We saw a case in a performance run, where FireFly failed to receive a batch of 3 events from EVMConnect.

What we found from the logs, is that FireFly Core had ended up in a situation where it was sending acknowledgements that were being interpreted by FFTM/EVMConnect as being for the _next_ batch after the one that had just been processed.

FFTM/EVMConnect before this PR had a very simple "acknowledge last thing you sent" system, which I can see has a window for this. There are attempts in the code to make this window very small - with the code by clearing out the go channel that passes `ack` payloads to the batch dispatcher, before delivering the batch. However, that does not eliminate the window completely.

This PR make a breaking change to the protocol such that:
- The events passed by FFTM/EVMConnect to FF Core are not just arrays, they are a structure like:
    ```js
    { "batchNumber":  12345, "events": [ ... ] }
    ```
- The `ack` payload contains a `batchNumber` and is only processed if this matches the delivered batch
- The Go routine from the WebSocket to the batch dispatcher has a length of `10`
- If spurious acks are sent on an invalid topic, or a `broadcast` topic, that exceed the channel depth, we disconnect

FF Core will need to be updated:
- To look for `{`/`[` in the payload to see whether it's old-style EthConnect or new style FFTM/EVMConnect
- If it's new style, include the `batchNumber` in the `ack`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-08 02:42:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/35" class=".btn">#35</a>
            </td>
            <td>
                <b>
                    Send update to FF Core each time there is an error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #34
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-03 02:05:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/33" class=".btn">#33</a>
            </td>
            <td>
                <b>
                    GET /status/* APIs for Liveness and Readiness Probes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding endpoints for use within K8s for liveness / readiness probes, as well as for upstream connector services like tokens. See https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/85 where we noticed we are missing these endpoints that Ethconnect did have.

TODO 
- [x] unit tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-02 18:14:00 +0000 UTC
    </div>
</div>

