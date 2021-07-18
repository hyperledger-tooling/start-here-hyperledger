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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/126" class=".btn">#126</a>
            </td>
            <td>
                <b>
                    Database events across all objects
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #109 

- Doesn't include docs - need to do reference docs for WebSockets to cover the new `&changeevents=.*` option
- Updates e2e test with change events - turned on for all tests, so they're chatty, but hopefully that makes it easier to debug if they fail too
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-12 04:53:14 +0000 UTC
    </div>
</div>

