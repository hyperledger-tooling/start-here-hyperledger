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
                PR <a href="https://github.com/hyperledger/firefly/pull/617" class=".btn">#617</a>
            </td>
            <td>
                <b>
                    Add route to lookup identity by DID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See #583

This is more of a starting point - the functionality works, but I'm pretty certain the API spelling is not what we want.

I was struggling with the best way to provide this functionality - it seems like it must be a query param, because `/` is a valid char for query params but not for path params. Assuming we do use a query param, it would also be nice to flag it as "required" from the Swagger perspective.

Side note: you can already query the `/namespaces/{ns}/identities` endpoint with a query param for `did`, but you have to know the namespace you're looking for in that case.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 21:30:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/616" class=".btn">#616</a>
            </td>
            <td>
                <b>
                    Change node/org lookups to support name or ID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See #583
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 21:20:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/615" class=".btn">#615</a>
            </td>
            <td>
                <b>
                    Update microservices versions for v0.14.0
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
        Created At 2022-03-18 20:06:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/613" class=".btn">#613</a>
            </td>
            <td>
                <b>
                    Dependency updates for v0.14 testing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Broadhurst <peter.broadhurst@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 16:32:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/612" class=".btn">#612</a>
            </td>
            <td>
                <b>
                    [blockchainevents-charts] support for blockchain event charting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding support for blockchain event charting, so that the new UI can include blockchain event histograms.
This was a bigger change than expected since blockchain events have no `type` field, and are also timestamped by a `timestamp` field rather than a `created` field. This resulted in a `getHistogramNoTypes()` method and a `getHistogramWithTypes()` method.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 12:25:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/611" class=".btn">#611</a>
            </td>
            <td>
                <b>
                    Add E2E test support for ERC20/ERC721
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Depends on https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/33
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 03:37:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/608" class=".btn">#608</a>
            </td>
            <td>
                <b>
                    Restart stack and re-run E2E tests in daily integration job
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This does not affect the PR test runs - only the daily integration test job - or if a `RESTART` environment variable is set to `true`.

Resolves https://github.com/hyperledger/firefly/issues/566
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 15:58:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/607" class=".btn">#607</a>
            </td>
            <td>
                <b>
                    Add Shared Storage Download Manager
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #601
Resolves #568 

Summary of the changes in this PR:

1. Add workers that download from IPFS asynchronously, then notify with callbacks when they are ready

3. Add `batch_hash` column to `pins`
    - So we can compare the hash of the persisted batch, against the pin - common to private and broadcast

4. Add option to set `outputs` to the operation manager
    - Useful to have the outputs persisted from download, so you can see the public refs

5. Add operations for downloading shared storage (IPFS) batches and blobs

6. Add operation for uploading blobs (per #568)

7. More consistently name all operation types, with `type_verb_noun`
    - 'blockchain_pin_batch' (was 'blockchain_batch_pin')
    - 'blockchain_invoke'
    - 'dataexchange_send_batch' (was 'dataexchange_batch_send')
    - 'dataexchange_send_blob' (was 'dataexchange_blob_send')
    - 'sharedstorage_upload_batch' (was 'sharedstorage_batch_broadcast')
    - 'sharedstorage_upload_blob'
    - 'sharedstorage_download_batch'
    - 'sharedstorage_download_blob'

9. Fixes a bug where we might miss rewinds to process pins after batch arrival
    - Fix: `rewindPollingOffset` needed to return the decision it made on whether to rewind in `event_poller.go`
    - Cause: The `rewindPollingOffset` code in the event poller checks for queued rewinds each time round the polling loop, and contained a check to make sure it only went backwards. However, it didn't return the outcome of that check to the calling function, which then always assumed the rewind had been applied. Meaning if there was a "rewind forwards" scenario, it could do it and mean it missed pins. This left those messages stalled.

11. Fixes a bug where a node receiving messages, but not sending any, could delay for a long time before confirming messages.
    - Fix: Add a new goroutine to the batch manager, to continually process new-message events
    - Cause: There was a situation on the recently updated batching logic, where it wasn't consuming new-message events while waiting in a polling cycle. As on the 2nd node there are no events arriving, that was meaning Database commits were blocked waiting to emit these new-message events.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 03:28:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/606" class=".btn">#606</a>
            </td>
            <td>
                <b>
                    Add "info" field to token pools, consume "symbol" from connectors
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
        Created At 2022-03-16 17:54:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/605" class=".btn">#605</a>
            </td>
            <td>
                <b>
                    Upgrade dependencies
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
        Created At 2022-03-16 15:31:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/604" class=".btn">#604</a>
            </td>
            <td>
                <b>
                    Custom contracts docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves https://github.com/hyperledger/firefly/issues/398
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-15 18:46:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/603" class=".btn">#603</a>
            </td>
            <td>
                <b>
                    Add firstEvent field to contract listeners
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves https://github.com/hyperledger/firefly/issues/585
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-15 17:03:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/602" class=".btn">#602</a>
            </td>
            <td>
                <b>
                    Remove route /messages/{msgid}/operations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Operations are strongly tied to transactions, but they really are not
tied to messages directly. This helper for retrieving a "third level"
object association probably creates more confusion than it's worth.

It seems cleaner to retrieve the message transaction, then retrieve
the transaction operations as separate queries.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-15 16:19:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/600" class=".btn">#600</a>
            </td>
            <td>
                <b>
                    Batch confirm messages, and update events to contain topic+tag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently there is no clean way to query messages on a given `topic` in the same order that they were dispatched to your application.

More worryingly, we imply that the that you might be able to use the `confirmed` timestamp of the message as a substitute, as currently it's unique for each message. The problem with this is that timestamps are not guaranteed to only move forwards.

The only object in FireFly that is guaranteed to have a sequence you can rely upon is `events`, and these are delivered to your application with the `message` in-line in the case of a `message_confirmed` event. We just added `?fetchreferences` (thanks @shorsher) on the `/events` resource collection, so that's an important piece of the puzzle. So with the extra change in this PR, if you want to query messages on a topic in the order they happened you just do:

- `/api/v1/namespaces/{NS}/events?type=message_confirmed&fetchreferences&topic=MYTOPIC`
  - Reverse `sequence` is the default sort - so you can add `&sort=sequence` for ascending

> Note that this does not return you the data (there is no 2nd tier `?fetchdata` option). Adding this needs extra discussion as we'd drawn a line in the sand of only doing one level of auto-fetching for you. However, the convenience of `fetchdata` _might_ be the exception that proves the rule 🤔 

In a PR chain with #599

- Adds `topic` as am indexed field on events (64 chars)
- If there are multiple `topics` in a message to generates multiple `message_confirmed` events.
- Batch confirms messages, so multiple messages have the same `confirmed` timestamp
- Updates E2E test to apply the best practice described above
- Topics are assigned to all events, including non-message events (table below)

This has two benefits:
1) Performance increase due to being able to do a blanket set of confirmed to a single timestamp in the aggregator.
2) The ability to query all history for a topic cleanly in applications, without implicitly relying on positively increasing timestamps, and being confident its the same order that the confirmations happened in and your application was delivered the events. 

### Topic events

| Event | Topic | Comment |
|------|-------|-----------|
| `message_confirmed` | Message Topic | The key use case of filtering on topic |
| `message_rejected` | Message Topic | " |
| `blockchain_event_received` | `ff_batch_pin` for the built-in batch pin listener.<br/>Topic from the listener if specified.<br/>Listener ID as string otherwise | Setting a topic on the blockchain listener allows grouping of multiple events into a common stream |
| `token_pool_confirmed` | Token pool ID as string | Allows querying of all events on a token pool |
| `token_transfer_confirmed` | Token pool ID as string | " |
| `token_transfer_op_failed` | Token pool ID as string | " |
| `token_approval_confirmed` | Token pool ID as string | " |
| `namespace_confirmed` | `ff_definitions` | Catch all topic for FireFly system definitions |
| `datatype_confirmed` | `ff_definitions` | " |
| `identity_confirmed` | `ff_definitions` | " |
| `identity_updated` | `ff_definitions` | " |
| `contract_interface_confirmed` | `ff_definitions` | " |
| `contract_api_confirmed` | `ff_definitions` | " |

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-14 17:48:00 +0000 UTC
    </div>
</div>

