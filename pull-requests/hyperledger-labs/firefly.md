---
layout: default
title: firefly
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/141" class=".btn">#141</a>
            </td>
            <td>
                <b>
                    Set max connections to 1 for SQLite and allow config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Per https://github.com/hyperledger-labs/firefly-cli/pull/64 we've seen issues with SQLite returning:
```
FF10116: Database insert failed: database is locked
```

We're setting a default `_busy_timeout` in the CLI now, but it still seems the concurrency inherent in FireFly means it's easy to drive SQLite to a point it returns errors.
So the other approach is to limit the concurrent connections - and with 1 as the default that should not stress SQLite. Clearly that has a performance impact, but SQLite is primarily for lighter weight Dev scenarios where reliability matters more than performance.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-21 14:35:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/140" class=".btn">#140</a>
            </td>
            <td>
                <b>
                    Fix dispatcher deadlock when using custom readahead
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Encountered the below deadlock with a zero readahead connection, where we can see:
- The `eventLoop` routine is waiting in `bufferedDelivery` to push message 2 of 3 into `eventDelivery` channel
- The `deliverEvents` routine is stuck in `deliveryResponse` trying to notify the the `eventLoop`

The architecture is intended to avoid this deadlock, by having a channel big enough that the `eventLoop` can always get all `dispatchable` events into it.

In the logs before the hang, I can see `matched=3` `dispatchable=3`.
This _should_ indicate that the readahead is at least 2, which means the channel should have 3 slots in it.

```
[2021-07-19T18:29:04.086Z] DEBUG Dispatcher event state: candidates=3 matched=3 inflight=0 queued=0 dispatched=0 dispatchable=3 lastAck=0 nacks=0 highest=25 pid=1 role=ed[pTv5Nky2] sub=ac36320d-55d9-479e-abb1-82c7d04cf720/default:ac36320d-55d9-47...
```

The problem is this line that tweaks the readAhead is after we created the channel:
```
	if sub.definition.Options.ReadAhead != nil {
		ed.readAhead = int(*sub.definition.Options.ReadAhead)
	}
```

This is true for the system events subscription (used for request/reply correlation) which defaults to 50:
https://github.com/hyperledger-labs/firefly/blob/526b45577f2eb6a501edec3ed833029df457109e/internal/events/system/events.go#L54

### Deadlock threads

```
goroutine 639 [select, 39 minutes]:
github.com/hyperledger-labs/firefly/internal/events.(*eventDispatcher).deliveryResponse(0xc0000a3520, 0xc000513770)
	/firefly/internal/events/event_dispatcher.go:425 +0x45a
github.com/hyperledger-labs/firefly/internal/events.(*subscriptionManager).deliveryResponse(0xc0000b7ea0, 0xe8c3b8, 0x12cdfc0, 0xc000337888, 0x8, 0xc000513770)
	/firefly/internal/events/subscription_manager.go:471 +0x125
github.com/hyperledger-labs/firefly/internal/events.(*boundCallbacks).DeliveryResponse(0xc00038c7b0, 0xc000337888, 0x8, 0xc000513770)
	/firefly/internal/events/bound_events_callbacks.go:38 +0x5e
github.com/hyperledger-labs/firefly/internal/events/system.(*Events).DeliveryRequest(0x12cdfc0, 0xc000337888, 0x8, 0xc0000a2f70, 0xc0001f63f0, 0x0, 0x0, 0x0, 0x0, 0x0)
	/firefly/internal/events/system/events.go:104 +0x25f
github.com/hyperledger-labs/firefly/internal/events.(*eventDispatcher).deliverEvents(0xc0000a3520)
	/firefly/internal/events/event_dispatcher.go:380 +0x4de
created by github.com/hyperledger-labs/firefly/internal/events.(*eventDispatcher).electAndStart
	/firefly/internal/events/event_dispatcher.go:139 +0x273
```

```
goroutine 638 [chan send, 39 minutes]:
github.com/hyperledger-labs/firefly/internal/events.(*eventDispatcher).bufferedDelivery(0xc0000a3520, 0xc000447170, 0x3, 0x3, 0x0, 0x16, 0xe8d8d0)
	/firefly/internal/events/event_dispatcher.go:286 +0x17a
github.com/hyperledger-labs/firefly/internal/events.(*eventPoller).dispatchEventsRetry.func1(0x1, 0x0, 0xc0001d5938, 0x0)
	/firefly/internal/events/event_poller.go:224 +0x54
github.com/hyperledger-labs/firefly/internal/retry.(*Retry).Do(0xc000620348, 0xe87d60, 0xc000319f50, 0xd7d599, 0xe, 0xc000635f08, 0x0, 0xc000447170)
	/firefly/internal/retry/retry.go:55 +0xad
github.com/hyperledger-labs/firefly/internal/events.(*eventPoller).dispatchEventsRetry(0xc0003a7d40, 0xc000447170, 0x3, 0x3, 0x0, 0x0, 0x0)
	/firefly/internal/events/event_poller.go:223 +0xce
github.com/hyperledger-labs/firefly/internal/events.(*eventPoller).eventLoop(0xc0003a7d40)
	/firefly/internal/events/event_poller.go:206 +0x15b
created by github.com/hyperledger-labs/firefly/internal/events.(*eventPoller).start
	/firefly/internal/events/event_poller.go:123 +0x1a5
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-19 19:21:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/139" class=".btn">#139</a>
            </td>
            <td>
                <b>
                    Fix sequencing of submgr/webhooks and fix loop detection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Fixes #115 - webhook subscriptions not working after restart
  - The problem here was that the submanager was initializing after Webhooks had registered the global connection, and the code was assuming no connections existed at the time submanager was starting. So it wasn't starting the dispatchers.
- Fixes an error where webhook message delivery stop functioning after the following error is logged:
  ```
  DEBUG Webhook subscription with reply enabled called with reply event '1cb8bc49-40e6-4496-bb96-620527d5eca9' pid=1
  ```
  - Here the problem was the loop detection code missing an ack on the event, so no further events were being delivered.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-19 18:16:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/138" class=".btn">#138</a>
            </td>
            <td>
                <b>
                    Emit events for locally produced unpinned private messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently we have a difference between unpinned and pinned private messaging:
- Pinned private messages emit a `message_confirmed` on _all_ members when the blockchain TX completes
- Unpinned messages emit a `message_confirmed` on all members _except_ the sender when they arrive
  - Originally it was thought this might be less confusing than emitting a message locally in the unpinned case.
  - We've found that it's actually more confusing. Particularly as it means that if you have a request/response messaging scenario via FireFly it changes the behavior of whether the locally connected apps get triggered or not.

With this PR in place, we become consistent.
- Pinned private messages emit a `message_confirmed` on _all_ members when the blockchain TX completes
- Unpinned messages emit a `message_confirmed` on _all_ members
  - Sender gets their event immediately
  - Other nodes get their events when the off-chain message arrives via DX

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-19 15:53:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/137" class=".btn">#137</a>
            </td>
            <td>
                <b>
                    Add PUT for subscriptions and fix delete to clean up offset
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Working on an app, I found a few things that are annoying when setting up subscriptions addressed in this PR:
- Deleting and recreating a subscription does not give you the events again
  - Because we weren't deleting the offset associated with the subscription, so when you recreated it you got the same offset
  - This is just a bug
- It's hard to create logic in your app to create/update subs
  - You have to query, then compare, then delete and recreate
  - Made harder when the above bug is fixed, as you'd have to work out the offset to recreate at

So this PR:
1. Fixes the bug - deleting a subscription, cleans up the offset
2. Introduces a `PUT` for `/api/v1/namespaces/:ns/subscriptions` where the `namespace` + `name` determine uniqueness
    - Adds an `updated` field on subscriptions for when they are changed
    - Adds handling to ignore no-op updates
    - Updates all connected apps, but does *not* reset the subscription offset
3. Changes `offset` to be referenced by the `RowID` and to be deleted by subscription ID (no more `ID` or `Namespace`)
   - This was necessary as otherwise I couldn't delete the offset
   - Also means there's no chance of an old subscription re-using an offset

In a PR chain with #136 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-18 03:20:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/136" class=".btn">#136</a>
            </td>
            <td>
                <b>
                    Allow multiple durable subscriptions to be started on a single websocket
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This made encountering #134 really likely for the app under test, as it was subscribing to one durable subscription, then immediately subscribing to another.
However, because the `webSocketsConnection` only allowed a single subscription in the matcher, that second subscribe was actually causing subscription manager to close the first subscription (as it no longer matched the connection).

Note in a PR chain with #135 (which is the fix for the deadlock in #134)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-18 00:31:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/135" class=".btn">#135</a>
            </td>
            <td>
                <b>
                    Retry for errors on event poller startup, and only wait for ep close in one place
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix for https://github.com/hyperledger-labs/firefly/issues/134

Fixes two problems:
1. If we break out of the loop for leadership election before we start the event poller, then `close` will hang as it was waiting on `eventPoller.closed`.
  - No need for `ed.close` to wait on that, it can just wait on `ed.closed`
2. We were not handling errors from `eventPoller.start()`
  - Added retry for restoring the offset, and stopped it from returning an error in the case that the context is closed before it starts - it simply marks itself closed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-17 23:59:07 +0000 UTC
    </div>
</div>

