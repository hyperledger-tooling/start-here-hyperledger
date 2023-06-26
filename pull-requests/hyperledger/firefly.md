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
                PR <a href="https://github.com/hyperledger/firefly/pull/1354" class=".btn">#1354</a>
            </td>
            <td>
                <b>
                    Further optimize blockchain transaction inserts to DB
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In PR chain with #1343 

- Creates a new `txwriter` package that depends on both `operations` and `txcommon` to do batched inserts
   - Dispatches to a pool of background workers
   - Assigns a new ID to each transaction in the batch
   - Splits to transactions with/without `idempotencyKey` set
   - Attempts to insert all with new `InsertTransactions` multi-insert function in DB layer
   - Handles partial results on the `idempotencyKey` set TX, by querying those idempotency keys
   - Compares ID of the transactions in the DB, with the inserts, to find the duplicates
   - Inserts the `operations` with a new multi-insert function in the DB layer (these always have new IDs)
- Updates `contracts` package to use ^^^ instead of one-by-one insertion of tx+ops
   - The inbound thread for invoke/deploy requests doesn't even have a DB transaction now (`RunAsGroup` call removed)
   - Creation of the `core.Operation` moved up the function, as need to be passed in
   - Idempotency handling to resubmit operations in the case of a clash, unchanged
- Updates blockchain connector interface to split parsing with execution
   - We were compiling the FFI schema twice per transaction in the blockchain connector
- Adds caching to `contracts` package
   - For requests referencing an FFI: FFI ID + `methodPath` -> `FFIMethod` + `[]*FFIError`
   - For all requests: Hash of compiled JSON Schema, to the JSON Schema object
   - Also builds a hash-of-hashes across the combination of method+errors, which is used to cache the result from the blockchain connector validation

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-24 03:32:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1353" class=".btn">#1353</a>
            </td>
            <td>
                <b>
                    feat: expose retry and HTTP options for webhooks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A few considerations when reviewing:
- I modified the interface for the events plugin to pass the context through as we were using the global plugin context for events which I believe was incorrect.
- Instead of copying the client for each request in the webhook, we store the client in the subscription object. We populate it when reading a subscription from the DB or creating a new one through the API. I thought here about exposing a new function at the interface level such as `ParseSubscriptionOptions` where each plugin could parse the options and modify it but seem redundant do `ValidateOptions` so did it there instead
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-23 16:09:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1352" class=".btn">#1352</a>
            </td>
            <td>
                <b>
                    Add E2E test for indexing an existing ERC1155
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Requires https://github.com/hyperledger/firefly-tokens-erc1155/pull/129
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-22 15:58:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1351" class=".btn">#1351</a>
            </td>
            <td>
                <b>
                    Use NetworkName instead of Name for definition topics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1349

Related fix that will also need to be integrated: https://github.com/hyperledger/firefly-common/pull/76
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-22 15:55:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1348" class=".btn">#1348</a>
            </td>
            <td>
                <b>
                    Docs improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding two improvements in docs:

- adding a note for macOS users (port 5000 already in use)
- updating the command to be consistent with previous page (created `dev` stack but next page started `demo`)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-21 17:27:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1346" class=".btn">#1346</a>
            </td>
            <td>
                <b>
                    Fix uniqueness check in InsertOrGetFFI to match indexes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When guessing the reason for an insert conflict, the query needs to exactly match the configured database indexes. That means that the "name" and "networkName" queries need to both include "version" as well, otherwise we risk grabbing a row that isn't actually a conflict.

Fixes #1347 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-19 15:58:28 +0000 UTC
    </div>
</div>

