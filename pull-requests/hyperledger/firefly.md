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
                PR <a href="https://github.com/hyperledger/firefly/pull/691" class=".btn">#691</a>
            </td>
            <td>
                <b>
                    Rename "contract" field to "interface" on FFIMethod/FFIEvent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">migration_consideration</span>
            </td>
            <td>
                This is consistent with the underlying database field name and with the
naming of the field on other related objects (like contract APIs and
listeners).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-11 01:01:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/690" class=".btn">#690</a>
            </td>
            <td>
                <b>
                    Fix postgres migrations and add to PR checks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes a regression that was introduced recently into PostgreSQL migrations. The issue first occurred when the `payload_ref` column was removed in this commit: https://github.com/hyperledger/firefly/commit/7b02d90d85c1632b65c11f73667a1f35f9f5ac20#diff-aace6955c9ca1493ae6a4a7f8bb03aa93f8d12ea4ca6f4b7ee74321bc875d379L12. 

A later postgres migration (number `21`) referenced this column but it was no longer, so it failed to migrate the database with the following message:

```
Error: FF10163: Database migration failed: FF10163: Database migration failed: 2 errors occurred:
	* migration failed: column "payload_ref" does not exist (column 70) in line 8: BEGIN;

ALTER TABLE data DROP COLUMN blobstore;
ALTER TABLE data ADD blob_hash CHAR(64);
ALTER TABLE data ADD blob_public VARCHAR(1024);

-- Make payload_ref larger and a varchar, to accomodate more flexible IDs for non-IPFS shared storage plugins
ALTER TABLE batches ALTER COLUMN payload_ref TYPE VARCHAR(256) USING payload_ref;

CREATE INDEX data_blobs ON data(blob_hash);

COMMIT;
 (details: pq: column "payload_ref" does not exist)
	* pq: current transaction is aborted, commands ignored until end of transaction block in line 0: SELECT pg_advisory_unlock($1)
```

A misguided attempt to fix this issue was merged in https://github.com/hyperledger/firefly/pull/683. That PR removed postgres migrations `20` and `21` in an attempt to match the sqlite migrations. However, that "fix" did not work.

This PR undoes https://github.com/hyperledger/firefly/pull/683 by adding `20` and `21` back again. It also fixes the original problem, by not attempting to alter the column in `21` that no longer exists.

This PR also adds postgres to the test matrix for PR approval which should prevent us from winding up in this situation again.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-10 23:06:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/689" class=".btn">#689</a>
            </td>
            <td>
                <b>
                    Status plugins
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `GET /api/v1/status` now returns a `plugin` key:
```json
{
  "node": {...},
  "org": {...},
  "defaults": {...},
  "plugins": {
    "blockchain": [
      {
        "pluginType": "ethereum"
      }
    ],
    "database": [
      {
        "pluginType": "sqlite3"
      }
    ],
    "dataExchange": [
      {
        "pluginType": "ffdx"
      }
    ],
    "events": [
      {
        "pluginType": "system"
      },
      {
        "pluginType": "websockets"
      },
      {
        "pluginType": "webhooks"
      }
    ],
    "identity": [
      {
        "pluginType": "onchain"
      }
    ],
    "sharedStorage": [
      {
        "pluginType": "ipfs"
      }
    ],
    "tokens": [
      {
        "name": "erc1155",
        "pluginType": "fftokens"
      }
    ]
  }
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-10 22:27:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/688" class=".btn">#688</a>
            </td>
            <td>
                <b>
                    Move ffresty to pkg for use by other microservices
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The logging, retry and other configuration features we have in the FireFly wrapper on resty, should be available to other microservices. That way we can have consistency in how you configure it and the features you get.

In PR chain with #668 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-10 21:39:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/687" class=".btn">#687</a>
            </td>
            <td>
                <b>
                    Include interface metadata routes in FFI-generated Swagger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allows fetching info about the associated FFI, including the details of all
methods and events.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-10 16:53:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/686" class=".btn">#686</a>
            </td>
            <td>
                <b>
                    Add helper at /apis/{apiName}/listen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This existed in the past and was removed due to perceived redundancy. However, it _would_ allow creating contract listeners with a single step if you know only the API name and not the underlying FFI ID (currently creating a listener in that case is a 2-step process, to go from API to FFI and then create the listener).

Note that this exists in parallel to the other RPC-style endpoints at `/apis/{apiName}/query` and `/apis/{apiName}/invoke`. It's worth discussing if a similar API should be added next to `/contracts/interfaces/{interfaceId}/query` and `/contracts/interfaces/{interfaceId}/invoke` (or possibly discussing the opposite, ie if _those_ should be pruned as redundant).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-10 12:50:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/685" class=".btn">#685</a>
            </td>
            <td>
                <b>
                    Add contract listeners only by event definition or event pathname
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">migration_consideration</span>
            </td>
            <td>
                Previously, contract listeners could be added in 3 ways:
1. By passing a full event definition inline
2. By passing a partial event definition (containing just an event name) along with an interface reference
3. By passing an event ID

Number (2) is slightly confusing in how it is expressed and differentiated from (1), and also has been slightly broken since we don't actually support event lookup by "name" (rather it's by "pathname", and "pathname" isn't a field available on the FFIEventDefinition type).

To clean all this up, I'm proposing here that we drop the existing (2) and (3) and instead end up with only these two ways to add a listener:
1. By passing a full event definition inline
2. By passing an interface reference and event pathname

Technically there's no reason to drop the lookup by event ID, so if there is a strong argument to keep it, we can. But I like the simplicity of these two codepaths that I anticipate will be the most common.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-10 12:16:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/683" class=".btn">#683</a>
            </td>
            <td>
                <b>
                    Remove extra postgres migrations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It looks like at some point we removed sqlite migrations 20 and 21, but did not remove the corresponding postgres migrations. This was causing FireFly to fail to start when attempting to apply postgres migrations. This PR aligns the postgres migrations with the working sqlite migrations.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-09 12:33:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/682" class=".btn">#682</a>
            </td>
            <td>
                <b>
                    Fix make docker command in release build GitHub Action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-09 02:10:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/681" class=".btn">#681</a>
            </td>
            <td>
                <b>
                    Enforce config descriptions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 20:55:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/680" class=".btn">#680</a>
            </td>
            <td>
                <b>
                    Add /api/v1/status/websockets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #679
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 19:57:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/678" class=".btn">#678</a>
            </td>
            <td>
                <b>
                    Configuration docs, and packaging config/i18n for re-use by microservices
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A bunch of changes to improve our config docs (thanks @nguyer for your work there), and some structural changes to the `config` and `i18n` packages to allow them to be used by other microservices building in Go within the FireFly project.

- `pkg/config` - moved out the package for configuration, including the facility for Markdown generation
  - Split out the configuration that is base (just `log` and `lang`) from the Core configuration
  - `internal/coreconfig` contains the core configuration
  - Note that `coreconfig.Reset()` initializes all the defaults in a lock (needed to avoid concurrent map errors)
- `pkg/i18n` - moved out the translation framework
  - All the framework for translation moved
  - Tweak to how the default `en` translations are initialized, to allow sub-modules to keep adding keys
  - Split out `ErrorMessageKey` from `MessageKey` - with the distinction that errors have to have a registered prefix, that means microservices will not re-use message codes from other microservices
  - `FF10` errors are the FireFly Core errors
  - `FF00` errors are raised from the common utilities in `pkg` - note this mean renames of some codes
  - `FF201` errors are for the new Transaction Manager microservice being split out of EthConnect (the reason for doing this work now)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 18:10:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/677" class=".btn">#677</a>
            </td>
            <td>
                <b>
                    Update manifest for v1.0.0-rc.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 17:52:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/676" class=".btn">#676</a>
            </td>
            <td>
                <b>
                    [ui-v0.6.10] manifest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Echelberger <eberger727@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 17:29:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/674" class=".btn">#674</a>
            </td>
            <td>
                <b>
                    Check up-front for duplicate token pool name
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
        Created At 2022-04-07 18:57:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/673" class=".btn">#673</a>
            </td>
            <td>
                <b>
                    Clean up blockchain parameters returned by token connectors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Requires matching changes in all token connectors as well.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 17:48:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/671" class=".btn">#671</a>
            </td>
            <td>
                <b>
                    Remove references to old firefly-e2e stack name
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
        Created At 2022-04-07 16:08:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/670" class=".btn">#670</a>
            </td>
            <td>
                <b>
                    Do not update cache until messages/data assured to be in DB
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I was diagnosing a message stuck in `Pending` state on the latest mainline code, even though the logs and state all showed it had been confirmed. It was an identity claim broadcast.

I found this log entry, which was from the batch persist logic running _concurrently_ with the aggregator:

```
[2022-04-07T02:34:35.666Z] DEBUG ...firefly: Batch data insert optimization failed for batch '21319666-b115-491c-af29-48da417904db': FF10116: Database insert failed: FF10375: Failed to retrieve sequence for insert row 1 (could mean duplicate insert) dbtx=3pRrPKf3 role=event-manager
```

I believe the problem is we're updating the cache before the DB commit at the moment when persisting the batch, so what was happening was the aggregator was confirming it with an `UPDATE messages SET ...` statement, but that was happening _before_ the messages were being upserted.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 04:39:24 +0000 UTC
    </div>
</div>

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

