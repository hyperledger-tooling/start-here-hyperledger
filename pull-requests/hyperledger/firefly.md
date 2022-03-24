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
    * `blockchain_pin_batch` - previously `blockchain_batch_pin`
    * `dataexchange_send_batch` - previously `dataexchange_batch_send`
    * `dataexchange_send_blob` - previously `dataexchange_blob_send`
    * `sharedstorage_upload_batch` - previously `sharedstorage_batch_broadcast`
    * `sharedstorage_upload_blob` - new
    * `sharedstorage_download_batch` - new
    * `sharedstorage_download_blob` - new

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

