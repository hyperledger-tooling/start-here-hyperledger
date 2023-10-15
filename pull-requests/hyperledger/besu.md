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
                PR <a href="https://github.com/hyperledger/besu/pull/6029" class=".btn">#6029</a>
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
                thx to @vuittont60
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-13 04:33:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6028" class=".btn">#6028</a>
            </td>
            <td>
                <b>
                    remove code duplication
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Noticed that these lines of code were duplicated.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-13 00:18:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6027" class=".btn">#6027</a>
            </td>
            <td>
                <b>
                    Mining options refactor
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
        Created At 2023-10-12 16:21:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6026" class=".btn">#6026</a>
            </td>
            <td>
                <b>
                    Add trie log pruning triggered after trie log persist
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger/besu/issues/5390

TrieLogPruner loads all trie logs on startup.
Each time a trie log is persisted it is added to the "prune queue" and also the pruner is run.
Pruner executes over a pruning window (currently hardcoded to 1000) to chip away at an initially large backlog of trie logs. 
Once backlog is cleared, each prune run should just be a single trie log.

TODO:
- [x] Test with local node using smaller defaults for retain/prune window
- [ ] Add feature toggle
- [ ] Feasibility of streaming all trie logs on startup?
- [ ] Test on real nodes using current defaults: retain latest 512 blocks; backlog prune window of 1000 blocks;
- [ ] Consider an option to only prune forks
- [ ] Consider using safeBlock instead of 512 layers to retain
  - would be a nice strategy to prune only blocks older than RETAINED_LAYERS that have a subsequent finalized blockhash
- [ ] Consider belts and braces protection during rollback/forward in case pruned trielog may be in use
- [ ] Deal with "orphaned" trie logs (related to building: ones that aren't referenced in the `blockchain`; neither canonical nor a fork)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-12 07:42:15 +0000 UTC
    </div>
</div>

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

The tests below are done on a Standard_D4s_v5 Azure VM (4 vCPU, 16 GiB RAM)

### Before this PR :
Besu wasn't able to handle 5 TPS for eth_feeHistory (with 1024 blocks) for near head calls

flood eth_feeHistory localhost:8545 -d 300 -r 5 --metrics p50 p90 p99
<img width="343" alt="image" src="https://github.com/hyperledger/besu/assets/5099602/3e3e3791-6e23-42b7-adf9-9515a31a1358">

**CPU profiling**
![image](https://github.com/hyperledger/besu/assets/5099602/4a02b7b2-55ac-4cd8-85a5-f93c213e6400)


### After this PR
Besu is able to handle 50 TPS with 99th percentile in 139 ms. Combining this PR with PR https://github.com/hyperledger/besu/pull/6009, Besu was able to handle 500 TPS on near head calls with 1024 blocks.

flood eth_feeHistory localhost:8545 -d 300 -r 50 --metrics p50 p90 p99

<img width="330" alt="image" src="https://github.com/hyperledger/besu/assets/5099602/688d751b-8629-4d19-b42c-44b5c4a05d3b">

**CPU profiling**
![image](https://github.com/hyperledger/besu/assets/5099602/44fa849c-f562-438f-84e2-98e7258a4582)


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
                This PR introduces a new flag **_--cache-last-blocks=n_** to cache last n blocks data (block headers, block bodies, transactions' receipts and total difficulty).

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

