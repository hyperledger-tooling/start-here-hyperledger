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
                PR <a href="https://github.com/hyperledger/besu/pull/6023" class=".btn">#6023</a>
            </td>
            <td>
                <b>
                    Journaled world state
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

Introduce a new Journaled World State Updater, that within a transaction keeps one copy of account and storage state, restoring previous revisions on reverts and exceptional halts.  This updater only supports post-merge semantics with regard to empty accounts, namely that they do not exist in world state.

Adds an EvmConfiguration option for stacked vs journaled updater, and
wire it in where needed.  This is high touch as it's dependency
injection, but fairly simple code.

Staked and Journaled updaters both continue to exist in the codebase, with Stacked updaters being the default

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-11 21:47:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6022" class=".btn">#6022</a>
            </td>
            <td>
                <b>
                    Add bool TX pool flag to allow TX selection to avoid prioritizing TXs from the same sender
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
WIP

## Fixed Issue(s)
Fixes https://github.com/hyperledger/besu/issues/6021
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-11 21:19:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6020" class=".btn">#6020</a>
            </td>
            <td>
                <b>
                    Transaction Validation and Selection Plugin API update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR makes some changes to the Transaction Validation and Selection Plugin API to make them more useful.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-11 06:03:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6019" class=".btn">#6019</a>
            </td>
            <td>
                <b>
                    Codehash compare
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
A hacked build of #5889 to compare the code storage before and after changes to check for inconsistencies.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-11 06:00:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6017" class=".btn">#6017</a>
            </td>
            <td>
                <b>
                    Update 23.10.0 changelog
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
        Created At 2023-10-10 19:24:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6015" class=".btn">#6015</a>
            </td>
            <td>
                <b>
                    Set version to 23.10.0
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
        Created At 2023-10-10 16:48:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6013" class=".btn">#6013</a>
            </td>
            <td>
                <b>
                    add method to disable root verification for T8n and not Reference tests
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

add method to disable root verification for T8n and not Reference tests

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#5979 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-10 14:00:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6012" class=".btn">#6012</a>
            </td>
            <td>
                <b>
                    Standardize pubkey and public key naming in deposit
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
Currently there are various naming for public key (`publicKey`, `pubkey`, `pubKey`) in Deposit/DepositReceipt. This PR is to standardize them to `pubkey` such that they are consistent with the naming convention in [execution-api](https://github.com/ethereum/execution-apis/blob/584905270d8ad665718058060267061ecfd79ca5/src/engine/experimental/eip6110.md?plain=1#L31)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-10 13:14:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6011" class=".btn">#6011</a>
            </td>
            <td>
                <b>
                    Optimize Eth_feeHistory RPC method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR enhances the Eth_feeHistory method through the implementation of a new cache for storing computed rewards. 
Furthermore, it introduces enhancements in the process of calculating rewards.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-10 12:57:55 +0000 UTC
    </div>
</div>

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

