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
                PR <a href="https://github.com/hyperledger/firefly/pull/652" class=".btn">#652</a>
            </td>
            <td>
                <b>
                    Cannot assume zero as reason to insert vs. update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Tweak to the logic from #650 - the assumption made in the code was invalid on assuming a value of `0` was enough to determine if we needed to use `INSERT` (vs. `UPDATE`) for the `nonces` collection. 

Because if multiple private messages go into a batch, this value will be incremented.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 20:41:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/651" class=".btn">#651</a>
            </td>
            <td>
                <b>
                    [charts-config] chart buckets are now capped at a configurable max
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously, histogram buckets were created with a `CASE` query. This lead to performance issues when a large amount of data was queried from the database. 

This new method sets a max amount of rows to be queried in each bucket, with a default of 100 rows. 

The data structure and expected response is unchanged.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 19:38:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/650" class=".btn">#650</a>
            </td>
            <td>
                <b>
                    Assign nonces more efficiently, with minimal DB ops
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR addresses two problems:

1) Currently when we are flushing a batch, we perform a DB read+update individually. This is very inefficient when you have a large number of messages for the same topic+group combination in the same batch. Instead we can keep a track in memory of the nonce increments, and flush them one time at the end of the dispatch.

2) I found while investigating (1) that we were not including the `author` of the message in the calculation of which Nonce we assigned from the DB. This is a bug. e.g. if you sent a message on `topicA` in a group with both `bob` and `sally` using author `bob`, then sent another message _from the same node_ as `sally` on the same `topicA` - then `sally` would get the wrong nonce.

As per the comments, some consideration has been made to ensure we take allocation of nonces seriously. Two key scenarios:

- Double assigning a nonce to a message: If we crashed after allocating a nonce in sending a batch, then after restart included the same messages back into a _new_ batch then we need to **re-use the same nonce** rather than allocating a new one.
- Failing to assign a nonce due to DB retry: If we span round the `sealBatch` logic once, then got a DB error and retried, the nonces we notionally assigned to the messages would not have been flushed to disk (we flush the nonces to the DB right at the end of this logic, and all DB plugins today have atomic TXs). This means when we retry we need to do the allocation again.

The above scenarios is why we check that the `msg.Pins` array hasn't been assigned, and only assign it after we've exited the retry loop.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 17:23:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/649" class=".btn">#649</a>
            </td>
            <td>
                <b>
                    Call out memory needed in docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This docs update should fix issue #648. I already chatted with @nguyer briefly on Discord about it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 14:31:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/647" class=".btn">#647</a>
            </td>
            <td>
                <b>
                    Use a single commit to generate all batch ops, before initiating the HTTP calls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Use a single database transaction to write all the `pending` `operations` needed to dispatch a private messaging batch
- Then initiate all the HTTP calls to DX separately - noting these should be *pending* until the asynchronous callback comes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 13:30:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/646" class=".btn">#646</a>
            </td>
            <td>
                <b>
                    Add background workers to flush updates to operations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updating an operation is quite an expensive set of DB calls when taken in isolation, and currently happens on the critical path of a number of event processing threads:

- Blockchain events - this is critical as it affects batch pin and custom contract event dispatch latency
- Token events - similar to blockchain events, with some extra complexity for event emission of operation events
- DX Transfer results - affects the notification of arrival of incoming events

So this PR proposes a dedicated set of workers (similar to we now have for message writing), that asynchronously flush operation updates to the DB in efficient batch transactions.

Some additional notes:
- Unlike message workers, we use a hash-bucket allocation of operation UUIDs to workers, so if there are retries etc. going on for a single operation we don't risk having two workers processing updates in parallel so the wrong one "wins" (a retry failure overtakes eventual success).
- After a recent change that means we're passing the ID into DX when we perform a send, this PR removes the logic that performed multiple retries to find an operation ID and was specific to DX (where originally DX generated the ID and passed it back to FF core to do the insert). Now DX is not "special", so if we find we need such logic in the future, we can put it into this logic by re-scheduling the update back to the worker as a retry (rather than discarding it with a warning as we do currently).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 00:55:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/645" class=".btn">#645</a>
            </td>
            <td>
                <b>
                    Fix IF EXISTS check on transactions_id INDEX migration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Fixes migration
- Fixes a log entry that was at the wrong level
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-29 17:40:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/643" class=".btn">#643</a>
            </td>
            <td>
                <b>
                    Fix `transactions_id` index
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Discovered we're doing full table scans for transactions when looking by ID, which is a performance critical query for the blockchain event processing routine (to update operations when we receive receipt notifications from EthConnect/FabConnect).

The reason was a simple typo in a migration.

```
postgres=# explain ANALYZE select * from transactions where id = '159b0bab-1a3f-406f-8862-bf8e05248789';
                                                  QUERY PLAN
---------------------------------------------------------------------------------------------------------------
 Seq Scan on transactions  (cost=0.00..4253.98 rows=1 width=116) (actual time=170.148..201.237 rows=1 loops=1)
   Filter: (id = '159b0bab-1a3f-406f-8862-bf8e05248789'::uuid)
   Rows Removed by Filter: 130390
 Planning Time: 0.126 ms
 Execution Time: 201.268 ms
(5 rows)
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-29 16:21:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/642" class=".btn">#642</a>
            </td>
            <td>
                <b>
                    Update our cache for event enrichment on message confirm
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Noticed in the UI that confirmed messages on the Timeline view are showing as `Pending` - which is because they are using the cache rather than an explicit query against the DB. This PR updates the cache when messages are batched, or confirmed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-29 03:41:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/641" class=".btn">#641</a>
            </td>
            <td>
                <b>
                    Add extra convenience functions for identities
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #625 

Adds a number of convenience functions:

- `GET` `/api/v1/network/identities` - global (cross namespace) collection of identities
- `GET` `/api/v1/network/identities?fetchverifiers` - same with verifiers embedded
- `GET` `/api/v1/network/identities/did:firefly:org/1?fetchverifiers` - get by DID with verifiers
- `GET` `/api/v1/network/diddocs/did:firefly:org/1` - get DID Document by DID
- `GET` `/api/v1/namespaces/{ns}/identities?fetchverifiers` - get with namespace with verifiers
- `GET` `/api/v1/namespaces/{ns}/identities/{id}?fetchverifiers` - get by ID in namespace with verifiers
- `GET` `/api/v1/status` - adds an `org.verifiers` array

All of the convenience `verifiers` arrays above just have the `type` + `value` (not the `hash` or `identity` fields which are irrelevant when embedded).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 22:01:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/639" class=".btn">#639</a>
            </td>
            <td>
                <b>
                    Add index on message_id for token transfers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Found a very expensive DB query for this message - which is a transfer broadcast:
```
{"log":"[2022-03-28T18:28:15.165Z] DEBUG node_0: Aggregating pin 0000628232 batch=30699806-5fc3-441e-b05f-8d2c9d28fc5e msg=7e41907b-5d34-41c0-87a5-61ccafaf9885 pinIndex=1 msgBaseIndex=1 hash=37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f masked=false dbtx=Z5gQrpfP role=aggregator\n","stream":"stderr","time":"2022-03-28T18:28:15.16525934Z"}
{"log":"[2022-03-28T18:28:15.165Z] DEBUG node_0: Cache hit for message 7e41907b-5d34-41c0-87a5-61ccafaf9885 dbtx=Z5gQrpfP role=aggregator\n","stream":"stderr","time":"2022-03-28T18:28:15.16527267Z"}
{"log":"[2022-03-28T18:28:15.165Z] DEBUG node_0: Attempt dispatch msg=7e41907b-5d34-41c0-87a5-61ccafaf9885 broadcastContexts=[37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f] privatePins= dbtx=Z5gQrpfP role=aggregator\n","stream":"stderr","time":"2022-03-28T18:28:15.16527981Z"}
{"log":"[2022-03-28T18:28:15.165Z] DEBUG node_0: SQL-\u003e query: SELECT type, local_id, dbtx=Z5gQrpfP role=aggregator\n","stream":"stderr","time":"2022-03-28T18:28:15.165441134Z"}
{"log":"[2022-03-28T18:28:15.839Z] DEBUG node_0: SQL\u003c- query dbtx=Z5gQrpfP role=aggregator\n","stream":"stderr","time":"2022-03-28T18:28:15.839742326Z"}
```

`18:28:15.165Z` -> `18:28:15.839Z` - so 700ms ish

This query looks to be the culprit, as we do not have an index:
https://github.com/hyperledger/firefly/blob/282d6237e1c6840c2f27fb87ec8ddd95e32a9536/internal/events/aggregator.go#L492-L498
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 19:46:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/638" class=".btn">#638</a>
            </td>
            <td>
                <b>
                    Cache blockchain events for event enrichment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Based on this flame graph analysis:
![image](https://user-images.githubusercontent.com/6660217/160471295-c2095fcd-fb65-4db0-9008-01bd5432108a.png)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 19:21:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/637" class=".btn">#637</a>
            </td>
            <td>
                <b>
                    Update txType in private message schema
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
        Created At 2022-03-28 19:11:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/636" class=".btn">#636</a>
            </td>
            <td>
                <b>
                    [ui-v0.6.7] ui manifest
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
        Created At 2022-03-28 18:25:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/635" class=".btn">#635</a>
            </td>
            <td>
                <b>
                    [ui-v0.6.6] manifest release
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
        Created At 2022-03-27 23:08:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/634" class=".btn">#634</a>
            </td>
            <td>
                <b>
                    Created timestamp index on events shouldn't be unique
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Saw the below error in a long-run test, where an attempt to insert an event resulted in no rows being added in PSQL with `ON CONFLICT DO NOTHING RETURNING seq`. I found there's an index that is set to `UNIQUE` on the `created` timestamp, and while a clash there is unlikely it's definitely possible.

```
{"log":"[2022-03-27T20:45:44.100Z]  WARN node_0: SQL! transaction rollback dbtx=WLXd2cMS httpreq=GJpFajph req=w6nJtbSg\n","stream":"stderr","time":"2022-03-27T20:45:44.102693254Z"}
{"log":"[2022-03-27T20:45:44.102Z]  INFO node_0: \u003c-- POST /api/v1/namespaces/default/contracts/invoke [500] (19.62ms): FF10116: Database insert failed: FF10375: Failed to retrieve sequence for insert row 1 (could mean duplicate insert) httpreq=GJpFajph req=w6nJtbSg\n","stream":"stderr","time":"2022-03-27T20:45:44.10280407Z"}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-27 22:50:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/633" class=".btn">#633</a>
            </td>
            <td>
                <b>
                    Update batch manager dispatch to track inflight and fix private blobs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Batch manager updates

I believe I've found an issue in the way the batch manager and the batch processors interact
Because the messages stay in ready state while they are being dispatched, the `readPage` loop will still see all messages that are dispatched

Currently it attempts to re-dispatch them when it's told to rewinds, and relies on the processor to de-dup those messages
It all works from a consistency perspective, but with the pattern of workload from the long-run it's a little inefficient in terms of how many rewinds and re-processing we do. It seems this can reach the point the batch manager can get jammed up trying to do those re-dispatches to the processor, while the processor is busy flushing what it's got

This PR simplifies the logic significantly, by preventing duplicate dispatches in the batch manager.

The manager keeps a map of all in-flight dispatched sequences to processors, and the processors call back to the manager when they have flushed a batch (so the messages will no longer turn up in `readPage` queries).

### Fix to private blobs

The private message batch dispatcher, was only sending the first blob in a batch. Meaning other messages with blobs in the batch would never be confirmed, because the blobs never arrived.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-27 18:43:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/630" class=".btn">#630</a>
            </td>
            <td>
                <b>
                    Do not return an error from status if node lookup fails
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In `v0.14.0` if you register your org (only), and then call `/api/v1/status` you receive:

```js
{"error":"FF10277: Identity could not be resolved via DID 'did:firefly:node/zzhc7hdmc0'"}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 20:15:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/629" class=".btn">#629</a>
            </td>
            <td>
                <b>
                    [ui-v0.6.3] v0.6.3 release of ui in manifest
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
        Created At 2022-03-25 19:23:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/627" class=".btn">#627</a>
            </td>
            <td>
                <b>
                    Simplfy solc compilation of BatchPin contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a slight simplification to the way the BatchPin contract is compiled at build time. This allows us to remove some deprecated code in the FireFly CLI and goes along with the changes in https://github.com/hyperledger/firefly-cli/pull/165
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 19:41:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/626" class=".btn">#626</a>
            </td>
            <td>
                <b>
                    Add pool config to activate call
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Enables https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/36
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 18:40:07 +0000 UTC
    </div>
</div>

