---
layout: default
title: firefly-transaction-manager
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-transaction-manager
---

# firefly-transaction-manager <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-transaction-manager){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/85" class=".btn">#85</a>
            </td>
            <td>
                <b>
                    Persistence enhancements - including adding PostgreSQL support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Work in progress - release should be marked v1.3 when complete/merged.

Making as pragmatic as possible change to the persistence mechanism, to support PostgreSQL as an alternative to LevelDB when persisting transactions, checkpoints, subscriptions, and listeners.

Aiming to make the impact on policy engine extensions as minimal as possible, but there are some changes shaping up:
- `TXHistory` moving into persistence, as implementation will be fundamentally different for PSQL to LevelDB
     - Updates to substatus history & actions are discrete operations
     - Can now return `error` and only take the `ID` of the `ManagedTX` object (not the full object)
     - History limits only likely to apply to LevelDB (as expensive to implement in SQL)
- Reconciling the `ManagedTX` object into core object fields, and related objects that can be merged in during a `GET` operation for backwards compatibility
     - `History` / `HistorySummary` were the big things
     - `TransactionHeaders` ended up a bit confused, so I've attempted to reconcile it (more info owed by me here)
     - `Receipt` - TBD if this stays separate
      - LevelDB continues to be a single fat JSON payload
- Rather than a single `WriteTransaction` function  with a `new` boolean, moved to `InsertTransaction` and `UpdateTransaction` - with clearer update semantics
      - This avoid re-writing huge JSON blobs to SQL DBs when simply tweaking a status field

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-06 03:11:17 +0000 UTC
    </div>
</div>

