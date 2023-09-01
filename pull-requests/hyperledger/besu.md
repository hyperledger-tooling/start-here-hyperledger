---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5836" class=".btn">#5836</a>
            </td>
            <td>
                <b>
                    Add world context to transaction tracing API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Add world context to the start/end transaction hooks in the tracing API.

## Fixed Issue(s)

fixes: #5835 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-01 08:00:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5833" class=".btn">#5833</a>
            </td>
            <td>
                <b>
                    ]POC] modify blockchain sync
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-31 09:45:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5832" class=".btn">#5832</a>
            </td>
            <td>
                <b>
                    Update RocksDB version from 8.0.0 to 8.3.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Update RocksDB version from 8.0.0 to [8.3.2](https://github.com/facebook/rocksdb/releases/tag/v8.3.2).


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-31 09:37:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5831" class=".btn">#5831</a>
            </td>
            <td>
                <b>
                    add versioned hashes and number of blobs to toString()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Adding missing information to the toString() method of Transaction
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-31 06:45:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5830" class=".btn">#5830</a>
            </td>
            <td>
                <b>
                    Do not create ignorable segments on `revert storage-variables`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
The `revert storage-variables` subcommand correctly reverts the storage-variable column family move, but inadvertently creates ignorable column family segments.  This behavior breaks backward compatibility prior to 23.1.0.  

This PR exposes `setIgnorableStorageSegments()` from BesuCommand and calls it from the revert storage-variables subcommand.

Additionally, this PR adds much needed visibility into the column family errors that RocksDB reports by parsing the RocksDBException and translating them into printable strings for more useful/actionable error messages.

example output for unidentified column family:
```
RocksDBException: Unhandled column families: ['Donny'(0x446f6e6e79), 'Walter'(0x57616c746572), 'Maude'(0x4d61756465), 'Dude'(0x44756465)]
```

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #5808 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-30 23:45:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5826" class=".btn">#5826</a>
            </td>
            <td>
                <b>
                    enforce that BlobTransactions have at least one blob
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
make sure that a blob transaction has at least one blob. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-30 05:40:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5823" class=".btn">#5823</a>
            </td>
            <td>
                <b>
                    [4844] EngineNewPayloadV3 - Validate non null required paremeters
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">4844</span>
            </td>
            <td>
                ## Description
This PR enhances the validation of null for the `EngineNewPayloadV3` parameters. Previously, these parameters were extracted using the `getOptionalParameter` method, which returns an `Optional.empty `if the parameters are null. This approach was insufficient as the engine can accept empty lists of versionedHashes, but cannot accept a null parameter.

The main changes introduced by this PR include:

- Modification of the parameter extraction method to allow for more robust null validation.
- Adjustment of the validation logic to correctly handle empty lists of versionedHashes and reject null parameters.
- Will now return "Invalid Parameters" if any required parameters are null.
- Renames `EnginePayloadParameter` to `EngineExecutionPayloadParameter` to match spec naming
- validateParams becomes `getAndCheckEngineNewPayloadRequestParams`

Fixes the following Hive tests:

- NewPayloadV3 Versioned Hashes, Nil Hashes
- NewPayloadV3 Versioned Hashes, Nil Hashes (Syncing) 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-29 08:29:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5820" class=".btn">#5820</a>
            </td>
            <td>
                <b>
                    WIP [4844] BlobTransactions - Add decodeType to TransactionDecoder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">4844</span>
            </td>
            <td>
                ## PR description
Incorporated a new parameter into the transaction decoding function to support decoding blob transactions from two different flows. This enhancement allows for the appropriate decoding method to be selected and invoked depending on the specific flow of the transaction processing.

## Fixed Issue(s)
fixes #5818

Fixes hive tests:

- blob_txs_full/reject_valid_full_blob_in_block_rlp/000-fork=Cancun-one_full_blob_one_tx
- blob_txs_full/reject_valid_full_blob_in_block_rlp/001-fork=Cancun-one_full_blob_max_txs
- blob_txs_full/reject_valid_full_blob_in_block_rlp/002-fork=Cancun-one_full_blob_at_the_end_max_txs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-29 06:38:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5819" class=".btn">#5819</a>
            </td>
            <td>
                <b>
                    fix ForkId if there are no Forks and the starting timestamp is not 0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Make sure that we are passing the fork id check if there are no forks and the genesis timestamp is not 0

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-29 03:30:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5817" class=".btn">#5817</a>
            </td>
            <td>
                <b>
                    Burn in release of 23.7.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-28 18:02:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5816" class=".btn">#5816</a>
            </td>
            <td>
                <b>
                    Remove Kotti network support (ETC)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Following core-geth's [decision](https://github.com/etclabscore/core-geth/pull/552), this PR removes the Kotti network as one of the preconfigured ones. If needed, this network can be still synced using the genesis definition explicitly from the CLI.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-28 15:43:28 +0000 UTC
    </div>
</div>

