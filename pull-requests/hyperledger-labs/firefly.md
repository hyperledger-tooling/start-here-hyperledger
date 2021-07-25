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
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/144" class=".btn">#144</a>
            </td>
            <td>
                <b>
                    Add MAINTAINERS.md, CONTRIBUTING.md and other required files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a proposed process for adding new maintainers, as well as a short guide on making contributions. I've also included several other required files to get us up to spec with: https://github.com/hyperledger-labs/hyperledger-community-management-tools/tree/main/repo_structure

Still missing is a CHANGELOG.md. I'm looking into ways to automate this. This PR will remain in draft state until existing maintainers have had time to discuss and agree on the process for adding new maintainers.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 19:25:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/143" class=".btn">#143</a>
            </td>
            <td>
                <b>
                    Repeated groupinit messages: Make sure we sort the group members, before existence check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes a case where we saw repeated `groupinit` messages being sent every time an unpinned message exchange was being performed in a request/reply scenario between two parties in the network.

The problem was the "_does the group already exist?_" check was being done using DB query with a hash calculated on an _unsorted_ list of members. Whereas the creation was correctly using `group.Seal()` which sorts the list of members before hashing. So we would repeat the creation over and over.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 14:39:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/142" class=".btn">#142</a>
            </td>
            <td>
                <b>
                    Avoid writing pins that can never be resolved
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We saw a situation where broadcasts were not being processed by a network, and the reason logged was:
```
[2021-07-21T13:29:22.474Z] DEBUG Message 29ef8ae6-06a0-461c-b9d1-fa754e6f3315 pinned at sequence 11775 blocked by earlier context f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d at sequence 10667 dbtx=oWj1wBCU pid=1 role=aggregator
```

This was in a FireFly environment where it had been rebuilt, with fresh FireFly databases, but using the same on-chain contract. The context of the batches that could not be processed were organizataion definitions.

Inspecting the `pins` database table, we could see a list of un-dispatched pins for the same context (e.g. the same on-chain organization ID):
```
  seq  | masked |                               hash                               |               batch_id               | idx | dispatched |       created       
-------+--------+------------------------------------------------------------------+--------------------------------------+-----+------------+---------------------
     7 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | 43b86d42-63de-40af-aa5b-389577cbff0a |   0 | f          | 1626873947548837682
    10 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | 9f4f148d-0e9b-4cc9-80f1-1eb2dd7d7549 |   0 | f          | 1626873947701026182
    11 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | 16c95a7b-5459-4d33-93b5-4e9ffb7a037f |   0 | f          | 1626873947813108703
    17 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | 041ef318-713d-49f1-9837-6a0c8f7a7d03 |   0 | f          | 1626873948148579427
    18 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | adb54417-ab2f-4545-88d4-3bdaa85902a8 |   0 | f          | 1626873979795296873
    30 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | d8fec3c5-98d3-4fb6-96b8-5008471b5a06 |   0 | f          | 1626873980089044029
    31 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | d8fec3c5-98d3-4fb6-96b8-5008471b5a06 |   1 | f          | 1626873980092709323
  1275 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | b2e5cf70-748c-43db-bf53-8ffd2617be6c |   0 | f          | 1626873997040283520
  1276 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | d29e6e92-1897-4c98-af44-3a93143e754a |   0 | f          | 1626873997091277560
 10666 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | 4de72a48-abff-46e7-bf6c-86b4bcbe45f0 |   0 | f          | 1626874141923359231
 10667 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | 7a442e04-5c81-4d7f-a562-4b76c81ff106 |   0 | f          | 1626874141990760266
 11775 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | 8fc90cde-1a2d-4d11-895f-cae1ee828a12 |   0 | f          | 1626874162367960540
 11776 | f      | f80c0fb74bf21261afe26836caeb7fa4569580b5ba07f2cf35f4a645d000769d | ef5a83f8-b99a-4ee3-a98d-4390a8dd4db4 |   0 | f          | 1626874162428103422
```

The batch was **not** stored in the `batches` table, but looking in the `transactions` table where `ref` is the batch, we could see that the blockchain transaction had a `payloadRef` to IPFS that could be resolved.

From this we could work out that the problem is the batches were rejected **without being stored** ~surmising this is because the authors were not known, because they were from a previous chain where the organizations got defined in a different order to the current FireFly environment.~ - after further code inspection we do not verify the organization exists at this point. Rather just that the author identity can be resolved. However, the fact the batch is missing, but the pin is there was conclusive in the investigation.

The problem here is that we knew at the point we inserted the pin, it could never be resolved!!! ... so we shouldn't have inserted the pin at all. We should only have un-dispatched pins for cases where we are _waiting_ for data.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 22:18:18 +0000 UTC
    </div>
</div>

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

