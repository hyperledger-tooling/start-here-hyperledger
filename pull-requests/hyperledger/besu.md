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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5806" class=".btn">#5806</a>
            </td>
            <td>
                <b>
                    evmtool: update readme for execution-spec-tests python 3.11 support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update [execution-spec-tests](https://github.com/ethereum/execution-spec-tests) installation in the evmtool's README

execution-spec-tests now additionally supports Python 3.11 ([ethereum/execution-spec-tests#193](https://github.com/ethereum/execution-spec-tests/pull/193), but requires additional packages on macOS (https://github.com/ethereum/execution-spec-tests/issues/274).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-25 12:05:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5805" class=".btn">#5805</a>
            </td>
            <td>
                <b>
                    mark account when proof is invalid during snapsync
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
        Created At 2023-08-25 10:00:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5804" class=".btn">#5804</a>
            </td>
            <td>
                <b>
                    don't check block timestamp drift for PoS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Geth has removed this check (block too far in the future) since the merge. Fixes #5800 - and 9 related hive tests that start with `cancun/eip4788_beacon_root/beacon_root_contract/`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-25 05:47:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5803" class=".btn">#5803</a>
            </td>
            <td>
                <b>
                    EngineNewPayload -  Fix Invalid Block Hash return
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                EngineNewPayload should not return the  latestValidHash when blockHash validation fails:

Current:
{status: INVALID_BLOCK_HASH, latestValidHash: `latestValidHash`, validationError: errorMessage | null} if the blockHash validation has failed

Expected:
{status: INVALID_BLOCK_HASH, latestValidHash: `null`, validationError: errorMessage | null} if the blockHash validation has failed


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-25 05:02:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5802" class=".btn">#5802</a>
            </td>
            <td>
                <b>
                    EngineNewPayloadV2  -  Reject non-null Blob fields 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">4844</span>
            </td>
            <td>
                ## PR description
Validate blobGasUsed and excessblobGas pre-Cancun. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-25 04:38:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5801" class=".btn">#5801</a>
            </td>
            <td>
                <b>
                    Improve Reference Test Performance
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description

Improve reference test performance by caching protocol specs and stacked world state values.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-25 03:01:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5797" class=".btn">#5797</a>
            </td>
            <td>
                <b>
                    Add Holešky as predefined network name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
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
        Created At 2023-08-24 15:01:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5795" class=".btn">#5795</a>
            </td>
            <td>
                <b>
                    add log for unexpected pipeline error
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

This PR allows displaying unexpected errors during the sync. Indeed, until now, it was necessary to go into debug mode to see them and therefore we could have stuck pipelines without knowing what the error is.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-24 13:51:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5794" class=".btn">#5794</a>
            </td>
            <td>
                <b>
                    Make checkSpdxHeader task cross platform
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

Another small PR to allow running checkSpdxHeader task on Windows

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-24 08:55:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5793" class=".btn">#5793</a>
            </td>
            <td>
                <b>
                    Remove versionedHashes from EngineNewPayload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">4844</span>
            </td>
            <td>
                Remove versionedHashes from EngineNewPayload. 

It does not belong to the payload parameter:
https://github.com/ethereum/execution-apis/blob/main/src/engine/cancun.md#executionpayloadv3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-24 05:41:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5792" class=".btn">#5792</a>
            </td>
            <td>
                <b>
                    EngineNewPayload - Validate parameters before fork validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">4844</span>
            </td>
            <td>
                Parameters validation should occur before fork validation

> Specification
> This method follows the same specification as [engine_newPayloadV2](https://github.com/ethereum/execution-apis/blob/main/src/engine/shanghai.md#engine_newpayloadv2) with the addition of the following:
> 
> 1. Client software MUST check that provided set of parameters and their fields strictly matches the expected one and return -32602: Invalid params error if this check fails. Any field having null value MUST be considered as not provided.
> 
> 2. Client software MUST return -38005: Unsupported fork error if the timestamp of the payload does not fall within the time frame of the Cancun fork.
> ...
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-24 05:38:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5790" class=".btn">#5790</a>
            </td>
            <td>
                <b>
                    Example
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
        Created At 2023-08-23 14:44:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5789" class=".btn">#5789</a>
            </td>
            <td>
                <b>
                    Make referencetests build script Windows friendly
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

#5774 broken builds on Windows due to the different separation char, this PR just replace the '/' with the system separator char as provided by the jvm

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-23 10:05:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5787" class=".btn">#5787</a>
            </td>
            <td>
                <b>
                    fix #5744: Incorrect ForkId when first fork timestamp matches genesis timestamp
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
If the genesis timestamp equaled the first timestamp fork an additional ForkId was added, which was incorrect.

## Fixed Issue(s)
fixes #5744
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-23 06:43:12 +0000 UTC
    </div>
</div>

