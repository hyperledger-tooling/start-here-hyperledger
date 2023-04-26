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
                PR <a href="https://github.com/hyperledger/firefly/pull/1291" class=".btn">#1291</a>
            </td>
            <td>
                <b>
                    Use a more optimistic approach when inserting token transfer events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR aims to improve the performance of handling token transfer event batches from the token connector.

It stems from some performance testing of FireFly's ability to process contract invocations & their respective token transfer events. Analysis of FireFly logs show that for a single token transfer event we go through the following DB calls:

1. Begin TX
2. Query token pool **<<-- could be cached**
3. Query token transfer  **<<-- no entry found in most cases**
4. Insert into blockchain events
5. Query token transfer again.  **<<-- In many cases this 2nd call can take 0.025 seconds on its own**
6. Insert token transfer
7. Query token balance
8. Insert token balance
9. Lock namespace
10. Insert events
11. Commit

There is a precedent in other areas of the codebase for using more "optimistic" approach for DB inserts that are likely to succeed first time without a clash. This follows an approach of "insert and handle conflicts" rather than "check for existing entry, then insert if not found".

This PR aims to improve `2` and `5/6`. In the case of `2` caching will be used to prevent having to call out to the DB for every event. For `5/6` we insert first and check for conflict errors. In the majority of cases this is expected to eliminate `5` entirely.

Notes on code changes:

1. In other places in the codebase where we do an optimistic `insert`, we don't support `update` - only `insert` and `get`. However in the case of token transfers we do allow a token transfer to be updated. This leaves us with the slightly oddly named `InsertUpdateOrGetTokenTransfer()` function which will:
   -  Insert a token transfer if none exists already
   -  Update a token transfer if it does already exist
   -  Return the existing token transfer if present
2. I've removed the previous `UpsertTokenTransfer()` since it is no longer needed
3. There is still a call to `GetTokenTransferByProtocolID()` (step `3` above). I feel like this could be removed entirely but I haven't done that yet. @awrichar could maybe do with some guidance on this part of the code: https://github.com/hyperledger/firefly/blob/5a78f152021e5cb0d32d8ce35cf28aeb03a17534/internal/events/tokens_transferred.go#L77 Removing that Get call seems obvious, but that affects the order of other calls (e.g. `maybePersistBlockchainEvent`, `emitBlockchainEventMetric`...). We could move `em.database.InsertUpdateOrGetTokenTransfer(ctx, &transfer.TokenTransfer)` to before https://github.com/hyperledger/firefly/blob/5a78f152021e5cb0d32d8ce35cf28aeb03a17534/internal/events/tokens_transferred.go#L84 but I didn't want to start reordering those calls without more input from someone like yourself.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-24 15:43:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1290" class=".btn">#1290</a>
            </td>
            <td>
                <b>
                    feat: Upgrade to latest ffresty with mTLS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Depends on:
- https://github.com/hyperledger/firefly-common/pull/65
- https://github.com/hyperledger/firefly/pull/1289

Once those are in I'll update this one
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-24 15:18:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1289" class=".btn">#1289</a>
            </td>
            <td>
                <b>
                    chore: remove deprecated config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">migration_consideration</span>
            </td>
            <td>
                - Remove deprecated config for blockchain, tokens, factory, database, dex and shared storaged config
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-24 09:28:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1288" class=".btn">#1288</a>
            </td>
            <td>
                <b>
                    Fix 1287
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1287 

In PR chain with #1280 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-20 18:50:57 +0000 UTC
    </div>
</div>

