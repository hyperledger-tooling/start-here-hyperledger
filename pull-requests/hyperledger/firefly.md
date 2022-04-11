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
                PR <a href="https://github.com/hyperledger/firefly/pull/669" class=".btn">#669</a>
            </td>
            <td>
                <b>
                    [charts-isCapped] adding isCapped key to charts response
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                New Response:
```json
[
    {
        "count": "0",
        "isCapped": false,
        "timestamp": "2022-04-06T23:21:00Z",
        "types": []
    },
    {
        "count": "100",
        "isCapped": true,
        "timestamp": "2022-04-07T00:57:00Z",
        "types": [
            {
                "count": "1",
                "type": "token_pool_confirmed"
            },
            {
                "count": "37",
                "type": "message_confirmed"
            },
            {
                "count": "12",
                "type": "token_transfer_confirmed"
            },
            {
                "count": "25",
                "type": "transaction_submitted"
            },
            {
                "count": "25",
                "type": "blockchain_event_received"
            }
        ]
    }
]
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 02:33:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/668" class=".btn">#668</a>
            </td>
            <td>
                <b>
                    New operations admin APIs and revamped change-event listener on admin WebSocket
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The policy engine described in https://github.com/hyperledger/firefly-ethconnect/issues/149#issuecomment-920866244 is starting to come together, with some evolved architecture.

The intention is for this to be a separate microservice, so it can be pluggable with different implementations easily, have a separate scaling model, and be closer to EthConnect in where it sits in the architecture than to the core.

However, the source of truth for the completion of operations is still FireFly. So this is more like an augmented _component_ of FireFly, than it is a plugin/connector that performs a particular task on behalf of FireFly. So as such I believe it should connect _in_ to FireFly to perform actions.

Currently (before this PR) we have some of things it would need - with gaps:
- Operations API - query only, and limited to one namespace.
- Operation change events - oddly side-car attached to the main application events, without sophisticated filtering

So this PR proposes we create a proper separation of concerns between the components that have super-access to update FireFly state, because they are part of it (the `admin` API already exists for this), and the external API that applications use.

- Adding `GET` `/admin/api/v1/operations` routes - including a `PUT` to update operation status (per same rules that apply to internal plugins like Data Exchange today)
- **Moving** the database change events firehose WebSocket to `/admin/ws` with extra options, and a simplified no-confirm model. It's best effort up to a buffer size, and then operation of the core is prioritized over avoiding any event loss, and always ephemeral. No guarantees.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 00:15:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/667" class=".btn">#667</a>
            </td>
            <td>
                <b>
                    Latest UI v0.6.9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Thanks @eberger727 !
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-06 22:12:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/666" class=".btn">#666</a>
            </td>
            <td>
                <b>
                    Remove misleading payload_ref DB field and fix Group JSON tag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In diagnosing a recent issue, I noticed that the `payloadRef` of a batch is a Database stored field, but is never set when you query in the database.

This is because we were writing it when we sealed the batch for delivery, but then overwriting it when we confirmed the batch.

It also had `VARCHAR(64)` in PSQL and `VARCHAR(256)` in SQLite.

The code actually only _needed_ it to pass the `payloadRef` from the batch upload operation, to the batch pin operation. Instead of relying on that, I've added it explicitly to the inputs of the Batch Pin operation - which overall feels much more consistent.

Then I've removed the DB field (for newly created envs - it nullable so no need for a migration to remove it).

I had to update the operations interface to return the outputs though, as it wasn't currently.

Unrelated fix - the `json:` tag on `Group` was wrong on `BatchPersisted` so we were returning `Group` rather than `group` on the JSON.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-06 17:50:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/665" class=".btn">#665</a>
            </td>
            <td>
                <b>
                    Add rewinder to handle enrichment off event poller critical path
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Issue #663 demonstrated that the event loops of the various plugins cannot safely ask the DB for information the event aggregator loop is updating, concurrently to the event poller writing it.

However, we don't want to slow the event poller down by making it do complex enrichment tasks to work out how to rewind. These tasks are as follows:
- For blobs: Query all `data` IDs associated with a `blob` hash, then find all `message` IDs that are associated with that data
- For token transfers: Query the `batch` ID associated with the message, which is associated with the on-chain transfer

So this PR introduces the architecture summarized in the diagram below. This ensures we do **not** start the enrichment DB activities (in loop 2) until the event poller has completed the cycle that might have been active while the plugin event that generated the rewind was active

![pr_665_diagram_1](https://user-images.githubusercontent.com/6660217/161826863-3c4dc41b-03a0-444a-a851-cf476e6f22d5.jpg)



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-05 18:37:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/662" class=".btn">#662</a>
            </td>
            <td>
                <b>
                    Proper handling of token approval events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Ensure existing approvals are not being overwritten
- Remove localID from async/sync POST response
- Commented out approvals from synchronous tokens e2e test due to https://github.com/hyperledger/firefly/issues/661
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-04 20:08:52 +0000 UTC
    </div>
</div>

