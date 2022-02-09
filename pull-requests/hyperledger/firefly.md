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
                PR <a href="https://github.com/hyperledger/firefly/pull/500" class=".btn">#500</a>
            </td>
            <td>
                <b>
                    New DX events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Gabriel Indik <gabriel.indik@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 05:19:42 +0000 UTC
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
                Includes commits from #497 plus a few more fixes.
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/478" class=".btn">#478</a>
            </td>
            <td>
                <b>
                    Store all token transfer inputs on operation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since the transfer is only recorded upon success, all inputs must be stored
on the operation in order to support retries or accurately report failures.

Needed for #400 and #316
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-03 21:39:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/477" class=".btn">#477</a>
            </td>
            <td>
                <b>
                    [new-prom-metrics] prometheus metrics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 to track broadcasts, private messages, and token mint/burn/transfers

Signed-off-by: David Echelberger <david.echelberger@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-03 21:13:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/476" class=".btn">#476</a>
            </td>
            <td>
                <b>
                    Add missing test coverage in txcommon
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-03 20:49:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/475" class=".btn">#475</a>
            </td>
            <td>
                <b>
                    Use PreFinalize/Finalize in all definition handlers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Follow-up to #462
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-03 20:15:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/474" class=".btn">#474</a>
            </td>
            <td>
                <b>
                    Make the factories act like factories
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Instead of instantiating all plugins up front, instantiate them on demand.

Fixes #467
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-03 17:39:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/473" class=".btn">#473</a>
            </td>
            <td>
                <b>
                    Fix Docker build on ARM
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves https://github.com/hyperledger/firefly/issues/469
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-03 14:29:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/472" class=".btn">#472</a>
            </td>
            <td>
                <b>
                    wsReader cannot rely on `testing.T` as it might extend past test scope
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix for #471 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-03 14:21:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/470" class=".btn">#470</a>
            </td>
            <td>
                <b>
                    Set default keepalive timeout to 5s on clients for Node.js connectors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix for #468 

For keepalive timeout there's a big disparity between Go and Node.js
- Node.js default server timeout is 5s: https://nodejs.org/api/http.html#serverkeepalivetimeout
- Go default client timeout is 90s: https://go.dev/src/net/http/transport.go
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-03 14:01:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/466" class=".btn">#466</a>
            </td>
            <td>
                <b>
                    [v0.12.0-manifests] manifests for v0.12.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Echelberger <david.echelberger@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-02 21:49:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/465" class=".btn">#465</a>
            </td>
            <td>
                <b>
                    Allow passing a tokenIndex to "mint"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some connectors may support (or require) this.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-02 20:24:37 +0000 UTC
    </div>
</div>

