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
                PR <a href="https://github.com/hyperledger/firefly/pull/591" class=".btn">#591</a>
            </td>
            <td>
                <b>
                    Scope subscription check to the appropriate stream ID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: jebonfig <joe.bonfiglio@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-08 21:00:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/590" class=".btn">#590</a>
            </td>
            <td>
                <b>
                    Switch from https to ffdx
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
        Created At 2022-03-08 20:30:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/589" class=".btn">#589</a>
            </td>
            <td>
                <b>
                    Use CLI to deploy test contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR changes the E2E tests to use the new FireFly CLI feature to deploy contracts, rather than having deployment code baked in to the E2E tests directly.

Depends on https://github.com/hyperledger/firefly-cli/issues/151
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-08 18:40:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/587" class=".btn">#587</a>
            </td>
            <td>
                <b>
                    add `fetchreferences` param to events api
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `fetchreferences` will add the referred object to the GET /events response

in a chain with #579 

closes #580 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-06 19:32:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/586" class=".btn">#586</a>
            </td>
            <td>
                <b>
                    Added version command to Core Binary
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Swarnim Pratap Singh <swarnimpratap132@gmail.com>
Fixes #132
It provides a command for listing the firefly build version and creating an internal package for the version so that it was accessible to the versionCmd in the cmd package.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-05 08:10:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/584" class=".btn">#584</a>
            </td>
            <td>
                <b>
                    Blockchain metrics for Ethereum
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR introduces blockchain metrics for:

- FireFly performing a blockchain transaction with a smart contract method
- FireFly querying the blockchain with a smart contract method
- Events emitted by a smart contract that FireFly is listening for

Each of these has two labels `location` and `methodName` for transactions/queries or `signature` (for events). The `location` is a blockchain specific appropriate string for describing where the event came from. The value of this label is 
 in the format of `"<key1>=<value1>,<key2>=<value2>"`. For Ethereum, it is just `address=<contract_address>`.

Fabric metrics will also be added in a subsequent PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 17:23:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/582" class=".btn">#582</a>
            </td>
            <td>
                <b>
                    Update batch logic to only store+hash the manifest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #506 

A few notes on the implementation.

Improvements related to performance:
- The hash on a batch is now just a hash of the manifest, rather than the full payload
  - `tx` was added to the manifest to include in the hash
- The database object for a batch is now the manifest
- The manifest has been updated to include everything the batch aggregator needs to find pins
  - A count of the `topics` were needed for this
- We now have a cache for messages + all data associated with a message

Improvements related to debug:
- Added to-string helpers to definition batch actions, and log the results
- Added a `GET` `/status/pins` collection to peekinside the pins status

Migration:
- The code copes with a persisted batch of the old type stored in the DB
  - `Version` in manifest used to distinguish this, and provide future extensibility
- The code copes with processing a batch that has a payload hash, rather than a manifest hash
  - To handle late-join/re-sync to a network processing old broadcasts

Potential follow-on work:
- Update the code in #587 to use the message cache
- Add a `batch` cache - to help the aggregator logic when managing pins
- Add a `transaction` cache - to help #587 event enrichment
- Trawl for any remaining `GetMessageByID` calls

## Message/data cache implementation notes

Messages have fields that are mutable, in two categories

  1. Can change multiple times like `state` - you *cannot* rely on the cache for these
  2. Can go from being un-set, to being set, and once set are immutable.

For (2) the cache provides a set of `CacheReadOption` modifiers that makes it safe to query the cache, even if the cache we slow to update asynchronously (active/active cluster being the ultimate example here, but from code inspection this is possible in the current cache).

If you use `CRORequestBatchID` then the cache will return a miss, if there is no `BatchID` set.

If you use `CRORequirePins` then the cache will return a miss, if the number of pins does not match the number of topics in the message.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 12:58:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/579" class=".btn">#579</a>
            </td>
            <td>
                <b>
                    Enhance subscription filters & event enrichment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 - Support for `Transaction` and `BlockchainEvent` subscription filtering
 - Added ws event enrichment for transactions and blockchain events

Subscription filter payload now look like:
```
  "filter": {
    "blockchainevent": {
      "listener": "string",
      "name": "string"
    },
    "events": "string",
    "message": {
      "author": "string",
      "group": "string",
      "tag": "string",
      "topics": "string"
    },
    "transaction": {
      "type": "string"
    }
  },
```

closes #545 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-03 21:24:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/578" class=".btn">#578</a>
            </td>
            <td>
                <b>
                    Handle operations with retries in transaction status
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
        Created At 2022-03-03 20:07:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/577" class=".btn">#577</a>
            </td>
            <td>
                <b>
                    Add missing itype column in SQLite migration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The testing for #549 focussed on PostgreSQL and one of the updates to the migration got missed in the SQLite one.

Raising and will do a test before looking for a review.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-03 14:23:56 +0000 UTC
    </div>
</div>

