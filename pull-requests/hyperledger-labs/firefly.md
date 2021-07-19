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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/131" class=".btn">#131</a>
            </td>
            <td>
                <b>
                    Create CODEOWNERS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-15 14:10:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/130" class=".btn">#130</a>
            </td>
            <td>
                <b>
                    Rename topic field to topics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In a message header, previously there was a field named `topic` but it was of type `[]string`. It makes more sense to call this field `topics` because it is a list of several topic names. This PR changes this, but it is important to note that this is an API breaking change (though small in size).

Example message:

```json
{
  "header": {
    "tag": "new_widget_created",
    "topics": ["widget_id_12345"]
  },
  "data": [
    {
      "value": {
        "id": "widget_id_12345",
        "name": "superwidget"
      }
    }
  ]
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 19:36:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/128" class=".btn">#128</a>
            </td>
            <td>
                <b>
                    Update addressable in Gemfile.lock for vulnerability
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See https://github.com/hyperledger-labs/firefly/security/dependabot/docs/Gemfile.lock/addressable/open
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 03:47:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/127" class=".btn">#127</a>
            </td>
            <td>
                <b>
                    Latency optimize event delivery by default
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Early adopter feedback suggests that latency of event delivery is more important than throughput optimization, in the most common scenarios. Particularly in non-blockchain backed event scenarios, and even more in request/reply scenarios.

Currently we use a 250ms default latency on event delivery, to reduce pressure on the DB in high throughput scenarios by giving time for messages to arrive between queries.

This PR proposes making the default 0, optimizing for latency by default (before we cut the first release).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 03:16:19 +0000 UTC
    </div>
</div>

