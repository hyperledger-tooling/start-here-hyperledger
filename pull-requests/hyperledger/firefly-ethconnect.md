---
layout: default
title: firefly-ethconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-ethconnect
---

# firefly-ethconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-ethconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/161" class=".btn">#161</a>
            </td>
            <td>
                <b>
                    Make requestABIId omitempty
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Two small observations in e2e testing of #159 fix:
- `requestABIId` does not have `omitempty`
  - Change made here
-  Would be helpful to fill this in, for the case we generated the ABI ID from the request ID, to make it clear we did that
  - This is actually really hard, due to where it's assigned. So suggesting we do not action this.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 22:41:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/160" class=".btn">#160</a>
            </td>
            <td>
                <b>
                    Assign message ID before dispatching message to Kafka in all cases
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently an ID is only assigned to the message in these cases:
- When using the Webhooks route to input a raw JSON message (`/` or `/hooks`) - before dispatching (to Kafka/sync)
- When explicitly passing a `fly-id`/`kaleido-id` param to the REST API Gateway - before dispatching (to Kafka/sync)
  - Added in #139 
- When the message is received at the Kafka side, and we find no ID inside there

This means in the Kakfa case there is always a message ID assigned at the point of processing.
But in the Sync dispatcher, as used by the FireFly CLI environment, there was no ID being assigned.

We hit an issue with #139 where we found it was leaking through an ID in the REST API Gateway case, that actually came from the gateway ID - that was just fixed in #158.

That fix then in turn exposed the problem of messages ended up with _no ID at all_ and cause the break in the e2e builds for FireFly seen in #159
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 13:17:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/158" class=".btn">#158</a>
            </td>
            <td>
                <b>
                    Honor fly-id for contract deployments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This also prevents bugs where the loaded deployMsg already had an ID and
the ID is reused.

Signed-off-by: Andrew Richardson <andrew.richardson@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 17:47:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/157" class=".btn">#157</a>
            </td>
            <td>
                <b>
                    ES Subscriptions: Store checkpoint after a stale subscription is processed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * We update the checkpoint block for a subscription when it's stale. However, we also need to store the checkpoint after since any restart must pick up from that point on.
* Set initial block height for stream when non-zero. Noticed we were not storing the "starting" block height when a custom value is configured when creating a stream
* Update deps

Fixes: https://github.com/hyperledger/firefly-ethconnect/issues/156
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-06 17:57:36 +0000 UTC
    </div>
</div>

