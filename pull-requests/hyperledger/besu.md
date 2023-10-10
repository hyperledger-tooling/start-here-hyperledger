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
                PR <a href="https://github.com/hyperledger/besu/pull/6010" class=".btn">#6010</a>
            </td>
            <td>
                <b>
                    [Plugin API] - TransactionSelector - Send TransactionSelectionResult to the plugin when not transaction is not selected
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Adds the `TransactionSelectionResult` to `TransactionSelector.onTransactionNotSelected` so that plugins have more context.

Addresses the comment in this PR https://github.com/hyperledger/besu/pull/6005#r1351753669

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-10 10:48:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6009" class=".btn">#6009</a>
            </td>
            <td>
                <b>
                    Cache last blocks data (block headers, block bodies, transactions' receipts and total difficulty)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cache last blocks data (block headers, block bodies, transactions' receipts and total difficulty).
The default number of blocks to keep in the cache is 0.

This PR will mainly improve the performances of some RPC calls :
- Eth_getBlockByNumber
- Eth_getBlockByHash
- Eth_feeHistory
- Eth_getTransactionReceipt
- ...

The biggest improvement is on Eth_feeHistory.

The new cache in DefaultBlockchain uses **1.35 GiB** on Mainnet **for 2048 last blocks** :
- Transactions receipts : 676 MiB
- Blocks' bodies : 555 MiB
- Blocks' headers : 2 MiB
- Total difficulty : less than 1 MiB
 

![image](https://github.com/hyperledger/besu/assets/5099602/6f8a9b9e-0d73-414b-899c-03351f9db302)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-10 10:41:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6007" class=".btn">#6007</a>
            </td>
            <td>
                <b>
                    docs: fix typo
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
        Created At 2023-10-10 09:30:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6006" class=".btn">#6006</a>
            </td>
            <td>
                <b>
                    Describe the migration to and how to configure the layered txpool
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

Read the rendered version [here](https://github.com/fab-10/besu/blob/release-23.10.x/CHANGELOG.md#layered-transaction-pool-the-new-default-transaction-pool-implementation)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-10 09:07:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6005" class=".btn">#6005</a>
            </td>
            <td>
                <b>
                    [Plugin API] - TransactionSelector - Notify plugins when transaction is selected/rejected
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Notify plugins when a transaction is selected/rejected

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-09 23:44:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6004" class=".btn">#6004</a>
            </td>
            <td>
                <b>
                    add retry logic on sync pipeline for rocksdb issue
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
        Created At 2023-10-09 15:36:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6003" class=".btn">#6003</a>
            </td>
            <td>
                <b>
                    Fleet mode
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
        Created At 2023-10-09 13:31:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6002" class=".btn">#6002</a>
            </td>
            <td>
                <b>
                    Release 23.10.0-RC2 burn in
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
        Created At 2023-10-09 09:54:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6000" class=".btn">#6000</a>
            </td>
            <td>
                <b>
                    [WIP] Trie log pruning 
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
        Created At 2023-10-09 07:33:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5998" class=".btn">#5998</a>
            </td>
            <td>
                <b>
                    Change Array Copying
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

Change array copying by re-using arrays when safe.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-08 16:58:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5997" class=".btn">#5997</a>
            </td>
            <td>
                <b>
                    Use existing Bytes48 for KZGCommitment and KZGProof
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

Since we have a native `Bytes48` datatype in Tuweni, we can use it for `KZGCommitment` and `KZGProof` to also have better checks and sematic
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-06 16:04:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5995" class=".btn">#5995</a>
            </td>
            <td>
                <b>
                    [Plugin API] - Simplify plugin transaction selector interface to return object instead of list
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">plugins</span>
            </td>
            <td>
                ## PR description
Revert plugin interface to return an object instead of a list
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-06 06:11:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5994" class=".btn">#5994</a>
            </td>
            <td>
                <b>
                    [skip ci] Add trace functionality for transaction selection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This change in the API allows the plugin to provide a tracer that will be used while executing transaction that could be selected for the block
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-06 05:38:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5993" class=".btn">#5993</a>
            </td>
            <td>
                <b>
                    hive tests explicitly attempt zero
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                more hive tests for engine api
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-05 21:06:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5991" class=".btn">#5991</a>
            </td>
            <td>
                <b>
                    Set version to 23.10.0-RC
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
        Created At 2023-10-05 13:52:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5990" class=".btn">#5990</a>
            </td>
            <td>
                <b>
                    Bump version to 23.10.1-SNAPSHOT
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
        Created At 2023-10-05 13:33:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5989" class=".btn">#5989</a>
            </td>
            <td>
                <b>
                    Release 23.10.0-RC burn in
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
        Created At 2023-10-05 12:39:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5988" class=".btn">#5988</a>
            </td>
            <td>
                <b>
                    Plugin Api - Add evaluateTransactionPostProcessing to TransactionSelector interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add evaluateTransactionPostProcessing to TransactionSelector interface
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-05 01:53:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5986" class=".btn">#5986</a>
            </td>
            <td>
                <b>
                    Validation ordering
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - corrects a number of validation errors by adjusting priority of evaluations
- covers and corrects a subtle issue where besu would propose bad blocks in the event of a re-org prior to a proposal which restored blob transactions to mempool.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-04 22:03:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5985" class=".btn">#5985</a>
            </td>
            <td>
                <b>
                    Transaction detachedCopy to optimize txpool memory usage
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

When a tx is decoded from RLP, some of its fields are reference to slices of the encoded RLP byte array, the latter could be shared by many transactions at the same time, for example when decoding the block body, every tx object keep a reference to the large RLP byte array, that could be hundred of KB long, the same happens when we receive a bunch on txs via p2p in the same message.
This approach works fine if the tx objects are short lived, since it means allocating and copying less data around, but does not fit well for pending txs, since they could live much longer in the txpool and a single tx could keep a reference to a large byte array, while actually only it only needs a small portion of it.

This PR solve this memory inefficiency, by creating a _detachedCopy_ of the tx when this is added to the txpool. A _detachedCopy_ is a copy that does not share any byte array with others. This also changes previous assumptions on the estimation of the amount of memory used by a pending tx, so the calculation have been updated and extended to cover also the Blob tx estimation.

relates #5977 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-04 12:57:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5983" class=".btn">#5983</a>
            </td>
            <td>
                <b>
                    [MINOR] Expose getSize to transaction interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Exposes getSize to transaction interface so it can be used by plugins
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-04 05:48:13 +0000 UTC
    </div>
</div>

