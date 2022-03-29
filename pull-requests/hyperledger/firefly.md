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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/624" class=".btn">#624</a>
            </td>
            <td>
                <b>
                    Re-read configuration on restart of orchestrator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Now that we are using more standard deployment of Ethereum contracts in the FireFly CLI, where a unique Eth address is generated each time, we need to set that configuration.

Rather than having configuration like this that's only in the DB, this PR proposes we re-read the configuration after the reset to pick up patched YAML configuration containing the instance address.

We still need to use the `preInit` trick in the CLI to let it start in a zombie mode so Docker compose is happy, while we're using EthConnect to deploy the contract, but the only thing we use the DB config patch for is to unset this flag (which is true already today).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 03:09:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/623" class=".btn">#623</a>
            </td>
            <td>
                <b>
                    [fetchreferences2] Adding event enrichment for all event types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `GET /events?fetchreferences` now returns enriched events for all event types:

```go
type EnrichedEvent struct {
	Event
	BlockchainEvent   *BlockchainEvent `json:"blockchainevent,omitempty"`
	ContractAPI       *ContractAPI     `json:"contractAPI,omitempty"`
	ContractInterface *FFI             `json:"contractInterface,omitempty"`
	Datatype          *Datatype        `json:"datatype,omitempty"`
	Identity          *Identity        `json:"identity,omitempty"`
	Message           *Message         `json:"message,omitempty"`
	NamespaceDetails  *Namespace       `json:"namespaceDetails,omitempty"`
	TokenApproval     *TokenApproval   `json:"tokenApproval,omitempty"`
	TokenPool         *TokenPool       `json:"tokenPool,omitempty"`
	Transaction       *Transaction     `json:"transaction,omitempty"`
	TokenTransfer     *TokenTransfer   `json:"tokenTransfer,omitempty"`
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 19:12:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/620" class=".btn">#620</a>
            </td>
            <td>
                <b>
                    [ui-v0.6.0-release] new ui release
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
        Created At 2022-03-22 17:24:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/619" class=".btn">#619</a>
            </td>
            <td>
                <b>
                    [ui-v0.6.0] PR for new UI release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Will get exact release hash once it's released
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-22 14:05:53 +0000 UTC
    </div>
</div>

