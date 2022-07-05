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
                PR <a href="https://github.com/hyperledger/besu/pull/4049" class=".btn">#4049</a>
            </td>
            <td>
                <b>
                    log for bonsai
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-04 09:25:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4045" class=".btn">#4045</a>
            </td>
            <td>
                <b>
                    Fix for TransitionProtocolSchedule by header when terminal block exactly at TTD
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
hive engine test "Sync Client Post Merge" highlighted a corner case with a method in TransitionProtocolSchedule which supported backward sync below/around TTD block.  

`getByBlockHeader` defers to the block header to find the appropriate pre or post merge protocol schedule, but in the case where we do not have a finalized block, and the terminal block difficulty was *exactly* the TTD value, we would erroneously return a pre-merge protocol schedule for blocks which were children of the terminal block.

PR fixes this behavior, adds some additional logging, and fixes the hive engine test.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
relates to #3841

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-02 15:10:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4044" class=".btn">#4044</a>
            </td>
            <td>
                <b>
                    add additional engine info logging 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
add info logging on engine api endpoints to increase the visibility of the EL/CL interactions

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-02 14:08:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4042" class=".btn">#4042</a>
            </td>
            <td>
                <b>
                    Hive engine suite conformance: Invalid Timestamp, Invalid Transition Payload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Addresses failures of hive engine test suite "Invalid Timestamp" and "Invalid Transition Payload" tests.  

* on invalid timestamp, return a success response with an INVALID status and validation error message rather than error response
* for latest valid ancestor blocks which are PoW, return Hash.ZERO rather than the PoW hash 
* check tracked bad blocks for forkchoiceUpdated head blockhash, return INVALID rather than SYNCING


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 23:27:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4041" class=".btn">#4041</a>
            </td>
            <td>
                <b>
                    fix for bonsai state root mismatch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

The problem comes from concurrent access to Bonsai's storageToUpdate map. These concurrent accesses can lead to the overwriting of certain data or just missing in this map and impact the behavior when importing a block

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 16:49:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4040" class=".btn">#4040</a>
            </td>
            <td>
                <b>
                    checkpoint sync retry download block when we did not get receipts
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

Fixes a mostly benign error during checkpoint sync which causes the pipeline to pause and restart upon failure to import blocks.  If during the CheckpointDownloadBlockStep we fail to get receipts for the block we are importing, CheckpointBlockImportStep will throw an NPE when attempting to save receipts.

```
2022-07-01 15:14:59.361+00:00 | EthScheduler-Services-29 (importBlock) | ERROR | PipelineChainDownloader | Chain download failed. Restarting after short delay.
java.util.concurrent.CompletionException: java.lang.NullPointerException
...
Caused by: java.lang.NullPointerException
        at org.hyperledger.besu.ethereum.rlp.RLPOutput.writeList(RLPOutput.java:245)
        at org.hyperledger.besu.ethereum.storage.keyvalue.KeyValueStoragePrefixedKeyBlockchainStorage$Updater.lambda$rlpEncode$2(KeyValueStoragePrefixedKeyBlockchainStorage.java:230)
        at org.hyperledger.besu.ethereum.rlp.RLP.encode(RLP.java:85)
        at org.hyperledger.besu.ethereum.storage.keyvalue.KeyValueStoragePrefixedKeyBlockchainStorage$Updater.rlpEncode(KeyValueStoragePrefixedKeyBlockchainStorage.java:230)
        at org.hyperledger.besu.ethereum.storage.keyvalue.KeyValueStoragePrefixedKeyBlockchainStorage$Updater.putTransactionReceipts(KeyValueStoragePrefixedKeyBlockchainStorage.java:166)
        at org.hyperledger.besu.ethereum.chain.DefaultBlockchain.unsafeImportBlock(DefaultBlockchain.java:355)
        at org.hyperledger.besu.ethereum.eth.sync.checkpointsync.CheckpointBlockImportStep.lambda$accept$0(CheckpointBlockImportStep.java:43)
        at java.base/java.util.Optional.ifPresent(Optional.java:183)
        at org.hyperledger.besu.ethereum.eth.sync.checkpointsync.CheckpointBlockImportStep.accept(CheckpointBlockImportStep.java:41)
        at org.hyperledger.besu.ethereum.eth.sync.checkpointsync.CheckpointBlockImportStep.accept(CheckpointBlockImportStep.java:24)
        at org.hyperledger.besu.services.pipeline.CompleterStage.run(CompleterStage.java:37)
        at org.hyperledger.besu.services.pipeline.Pipeline.lambda$runWithErrorHandling$3(Pipeline.java:152)
        ... 5 more

```

This pr will cause the pipeline to retry the block download step if we were unable to get the receipts for the block.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 16:15:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4039" class=".btn">#4039</a>
            </td>
            <td>
                <b>
                    jwt auth on websockets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #3990 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 13:51:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4038" class=".btn">#4038</a>
            </td>
            <td>
                <b>
                    Enable rocksDb metrics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Enable RocksDB metrics to evaluate the overhead. 

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#3369
## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 13:48:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4037" class=".btn">#4037</a>
            </td>
            <td>
                <b>
                    Enforce RocksDB to respect block cache size
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Enforce RocksDB to respect Block cache size, knowing that we can modify this block cache size with --Xplugin-rocksdb-cache-capacity.

We can read from [RocksDB Documentation](https://github.com/facebook/rocksdb/wiki/Block-Cache) that :
> strict_capacity_limit: In rare case, block cache size can go larger than its capacity. This is when ongoing reads or iterations over DB pin blocks in block cache, and the total size of pinned blocks exceeds the capacity. If there are further reads which try to insert blocks into block cache, if strict_capacity_limit=false(default), the cache will fail to respect its capacity limit and allow the insertion. This can create undesired OOM error that crashes the DB if the host don't have enough memory. Setting the option to true will reject further insertion to the cache and fail the read or iteration. The option works on per-shard basis, means it is possible one shard is rejecting insert when it is full, while another shard still have extra unpinned 



Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 09:23:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4035" class=".btn">#4035</a>
            </td>
            <td>
                <b>
                    re-add a sync check before accepting/processing remote transactions
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
Re-adds a check to ensure the node is ready to accept and process remote transactions

* uses SyncState::isInitialSyncPhaseDone 
* adds safe handling of chain head parameters when processing transactions

relates to #3937

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #4030 


## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-30 20:42:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4034" class=".btn">#4034</a>
            </td>
            <td>
                <b>
                    [Issue-3867] Limit outbound eth message sizes
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
Builds on #4002.

Add logic to limit the size of outbound `eth` subprotocol messages:
* Explicitly limit the size of messages constructed in response to queries from other nodes (requests for headers, bodies, etc).
* Add logging to surface issues with any other types of messages that are generated by the node internally. 

This should prevent nodes from being disconnected from their peers for sending messages that exceed the 10MB limit.  

## Fixed Issue(s)
Fixes #3867

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-30 20:40:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4033" class=".btn">#4033</a>
            </td>
            <td>
                <b>
                    Move Taccat to Emeritus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I propose moving Taccat from Active Maintainer to Emeritus Maintainer status, pursuant to the inactivity clause. Taccat has had no activity in the past 6 months, as identified by an automated report run by the Hyperledger Foundation:

@taccatisid  - [last github action](https://github.com/ryjones/gal-besu/blob/main/reports/GAL-taccatisid.md) (a PR create) was 17 Dec 2021

We very much appreciate their contributions but changing status to emeritus (and thus revoking PR approval privileges) is in the interest of an orderly project. If Taccat expresses in this PR that they intend to make contributions in the next quarter, then they will not be moved to emeritus status.

I propose this vote be open until either an absolute majority of active maintainers (13) votes for the same outcome, or until two weeks has passed (14 July 2022), after which a voting majority will determine the outcome (with a tie resulting in no change).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-30 16:50:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4032" class=".btn">#4032</a>
            </td>
            <td>
                <b>
                    turns down logging output to debug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-30 14:22:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4031" class=".btn">#4031</a>
            </td>
            <td>
                <b>
                    Revert "Upgrade OpenTelemetry (#3675)"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit 78717ade1d45902c13e77e84bc201338e159c3c4.

Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Issues with "Failed to connect" errors 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-29 23:50:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4027" class=".btn">#4027</a>
            </td>
            <td>
                <b>
                    Return transaction type for legacy transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## PR description

Instead of omitting the transaction type when serializing a legacy transaction, we return the spec conform value of `0x0`.

## Fixed Issue(s)

fixes #4025 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 13:38:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4026" class=".btn">#4026</a>
            </td>
            <td>
                <b>
                    Add terminal block hash and number to Ropsten genesis file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Add terminal block hash and number to Ropsten genesis file, and also require that peers on Ropsten must have that block

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 13:09:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4024" class=".btn">#4024</a>
            </td>
            <td>
                <b>
                    Add Sepolia TTD and DNS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                ## PR description

Adds the correct TTD and DNS config to the Sepolia config file

## Fixed Issue(s)
fixes #4021 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 09:06:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4023" class=".btn">#4023</a>
            </td>
            <td>
                <b>
                    Print full exception when NatService fails to configure automaticially
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                https://github.com/hyperledger/besu/issues/3787

Signed-off-by: Antony Denyer <git@antonydenyer.co.uk>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 08:56:09 +0000 UTC
    </div>
</div>

