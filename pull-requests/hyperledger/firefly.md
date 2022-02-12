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

