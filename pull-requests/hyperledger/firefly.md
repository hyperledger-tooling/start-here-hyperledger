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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/464" class=".btn">#464</a>
            </td>
            <td>
                <b>
                    ui version 0.5.0
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
        Created At 2022-02-02 04:29:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/462" class=".btn">#462</a>
            </td>
            <td>
                <b>
                    Add DefinitionBatchActions to execute after a batch of system definitions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #463

Work still pending:
1. ~~Remaining test coverage~~
2. Adjusting other definition handlers (besides token pools) to use the new `Finalize` pattern

If the foundation looks good, I'll add on these remaining pieces.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-01 18:50:28 +0000 UTC
    </div>
</div>

