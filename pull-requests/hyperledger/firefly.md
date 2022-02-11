---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/507" class=".btn">#507</a>
            </td>
            <td>
                <b>
                    Add "reInitEnabled" config to DX
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When enabled, FireFly will post to `/api/v1/init` on the DX connector with a list of all current nodes,
before initial connect of the websocket and before each reconnect.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-10 21:53:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/505" class=".btn">#505</a>
            </td>
            <td>
                <b>
                    Rename data exchange plugin to "ffdx"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #259

Open to other names here, but we landed on "fftokens" for the tokens plugin, so this seemed reasonable.
The name just needs to be globally unique in FireFly across all plugins, and identifiable as a data exchange plugin
vs. some other type of plugin.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-10 19:52:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/503" class=".btn">#503</a>
            </td>
            <td>
                <b>
                    Prometheus metrics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prometheus metrics for the following events:

Broadcast & Private Message:
- Submitted
- Confirmed
- Rejected
- Histogram

Token Mint, Transfer, and Burn:
- Submitted
- Confirmed
- Rejected
- Histogram
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 21:25:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/502" class=".btn">#502</a>
            </td>
            <td>
                <b>
                    Use inline ABI for all Ethconnect contract interactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates all smart contract interactions with Ethconnect so that Ethconnect no longer needs a previously deployed ABI to interact with a given contract. Instead, FireFly now has code that can convert the relevant parts of an FFI into an ABI format. The JSON ABI is used inline in each request to Ethconnect to invoke or query smart contracts or subscribe to events.

Resolves:
- https://github.com/hyperledger/firefly/issues/426
- https://github.com/hyperledger/firefly/issues/425
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 15:37:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/501" class=".btn">#501</a>
            </td>
            <td>
                <b>
                    Re-work batch logic for simplicity, efficiency, and restart recovery
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This leads on from the investigation in #421 and then #499

At the moment this is how the batching logic works:

## OLD

![batch_logic](https://user-images.githubusercontent.com/6660217/150621839-468e5be6-e1b5-4ac6-8086-34b4b9d73281.jpg)

- The assembly loop of each batch dispatcher is able to keep accepting work as long as the last batch has been successfully dispatched.
- The assembly loop passes work to the persistence loop, which has as many slots in its channel input as there are slots in the batch.
- The persistence loop keeps continually recording data to the database.
- The offset on the batch manager that's reading from the messages queue, is updated as soon as the assembly loop picks up the message

This design evolved from a similar design in the previous generation of Asset Trail technology.

Given this most recent issue, and some inefficiency and crash recovery challenges that exist in the design after it's port over to FireFly and evolution, I'm planning an updated design.

## NEW

This PR updates it to simplify it (even beyond the previous proposal in #421):

![batching_v2](https://user-images.githubusercontent.com/6660217/153135529-e81ff098-5266-44df-8021-849af7882fd2.jpg)

- We remove two of the loops
- Persistence only happens once for each batch in the final stage when the batch is sealed
- Dispatching is synchronous to the assembler
- The assembler only allows one batch to be in assembly before it blocks waiting for the dispatch completion
- The batch manager just has in-memory offset state, and on restart it looks from time-zero again
- We introduce a new `sent` state for messages that go into a batch
- Anything that doesn't reach that state is eligible for re-send after restart (at least once delivery)
- The manager can rewind at any time, because everything will either:
  - Be persisted with a batch ID so skipped
  - Be already in-flight
- The processor keeps track of sequences its flushing, and does duplicate detection
- The processor orders the assembly batch in sequence order


Note this means if things are appearing at once across a batch assembly window of 0.5s, it's very likely all messages will be sent in DB sequence order (even though the DB doesn't guarantee that's the order they'll become visible in).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 06:38:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/498" class=".btn">#498</a>
            </td>
            <td>
                <b>
                    Misc fixes for operations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ensure the operations for tokens and custom contracts behave as expected in success/failure scenarios.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 22:08:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/497" class=".btn">#497</a>
            </td>
            <td>
                <b>
                    Pass requestId to DX and remove backend_id from Operation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Follow the convention of all other plugins by passing a request ID into the
connector, rather than reading one from the connector response. This will be
enforced as a requirement for future connectors, so backend_id is removed from
the operations table.

Depends on https://github.com/hyperledger/firefly-dataexchange-https/pull/54
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 17:44:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/496" class=".btn">#496</a>
            </td>
            <td>
                <b>
                    Rewind when messages appear behind offset
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix for #493 

Observed reviewing the logs for #493 that the messages were never being picked up by the batch processor, and the perf tool is submitting them in a highly parallel way. My analysis is that with PSQL as used in this test (or any production ready database) parallel writing of messages to the DB could result in the commit order of the transactions, being mismatched with the sequence allocation to the rows. 

The code in the batch manager did not handle this - it would simply do a shoulder tap to re-read from the DB when a message was created, but not check if that message had appeared behind the offset and it needed to do a rewind.

This code change implements a simple rewind (like we have for the event aggregator).
Note this means that in the case of parallel REST API submission of messages, the final delivery order might not match the local sequence order. However, that's in-line with the assurances FireFly provides - as application should only be able to depend on.

- The local order they submitted in (in this case there is parallel submission, so the order is not deterministic) - but they should only rely on this for their own participation, and cannot consider this the global order across participants.
- The final order as ordered by the blockchain, when pinning is used.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 17:16:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/495" class=".btn">#495</a>
            </td>
            <td>
                <b>
                    Pass arguments from Makefile to docker build script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should fix the failing docker latest / release builds after we merge PRs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 16:09:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/494" class=".btn">#494</a>
            </td>
            <td>
                <b>
                    Compile directly with solc to avoid full Node.js npm install of Truffle
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Saves a lot of time and I/O activity during the docker build.

The `jq` command converts the `combined.json` output from `solc` in this syntax of JSON required by the CLI (which is a subset of the Truffle output):
https://github.com/hyperledger/firefly-cli/blob/680665495e45074b250e5ed5a74e8f152774254c/pkg/types/ethconnect.go#L19-L23
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 15:39:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/491" class=".btn">#491</a>
            </td>
            <td>
                <b>
                    Fix fabric event timestamp parsing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jim Zhang <jim.zhang@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 03:27:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/490" class=".btn">#490</a>
            </td>
            <td>
                <b>
                    Fix group to be constant throughout test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix for #487 

Note rename of `restclient.go` to `restclient_test.go` is to allow it to share `testState`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 03:13:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/488" class=".btn">#488</a>
            </td>
            <td>
                <b>
                    Add extra logging for message/event ids
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Notices these were missing when investigating a set of performance logs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-07 22:33:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/486" class=".btn">#486</a>
            </td>
            <td>
                <b>
                    Fix possibility for nil access in sendloop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix for #485 with a bonus fix for this timing issue I'm seeing intermittently since upgrading my laptop.

```
time="2022-02-07T13:21:00-05:00" level=info msg="API server context cancelled - shutting down"
time="2022-02-07T13:21:00-05:00" level=info msg="API server complete"
--- FAIL: TestTLSServerSelfSignedWithClientAuth (0.13s)
    http_server_test.go:197: 
                Error Trace:    http_server_test.go:197
                Error:          Received unexpected error:
                                context deadline exceeded
                Test:           TestTLSServerSelfSignedWithClientAuth
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-07 19:03:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/483" class=".btn">#483</a>
            </td>
            <td>
                <b>
                    Update aggregator batch processing to maintain in-memory pin state until OnFinalize
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix for #481 

We were failing to process multiple private messages on the same topic, within a single batch of pins that are read by the aggregator. This was a side-effect of the #462 changes - because the logic that evaluates the `NextPin` state on each message no longer had up-to-date information to read from the database.

The core fix implemented for that, was to move to in-memory processing for all state that can change during processing of a page of pins in the aggregator. So the first time we access the state on a context (context is a particular `topic`, scoped to a group if it's a private context), we read the data we need in memory and from that point on we update it in memory until the `Finalize` phase is called at the end. At that point everything is flushed.

Fixing this turned into quite a big change to the internals of the aggregator, and in doing so I did find two other less serious issues:
1. When there were multiple pins in a message (multiple topics) we would leave some of those pins with `dispatched=false` when the message was confirmed. This means potential re-processing on rewind.
2. If the pins within a message with multiple topics, spanned a page of reads from the aggregator, then when we came to the next page we could immediately re-process the message.

The fix for ^^^ was that we always mark _all_ pins associated with a message as dispatched. That can include pins outside of the page that was just read, so we calculate the start+end index of the pins within the batch for that message, and do an update in the DB scoped to that start+end range (and the batch ID).

> While enhancing the E2E I found another bug - in the automatic reply generation for webhooks, we're not setting the `topics` in the reply to match the request.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-06 00:45:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/482" class=".btn">#482</a>
            </td>
            <td>
                <b>
                    Remove extra "rejected" events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Only "message_rejected" will be emitted for rejected definition messages -
no special per-type event will be emitted.

This requires one extra lookup in syncasync to find rejected token pools,
but seems better for overall consistency.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-05 19:03:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/480" class=".btn">#480</a>
            </td>
            <td>
                <b>
                    Address some inconsistencies in Operation behavior
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Operations should all correspond to an external plugin action (only announce_pool needed a change)
- Name all operations as "plugin_action" (only contract_invoke needed a change)
- Mark operations successful after the new [synchronous forms](https://github.com/hyperledger/firefly/pull/460) of token pool creation and activation
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-04 19:38:45 +0000 UTC
    </div>
</div>

