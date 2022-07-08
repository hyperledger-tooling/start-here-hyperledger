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
                PR <a href="https://github.com/hyperledger/besu/pull/4072" class=".btn">#4072</a>
            </td>
            <td>
                <b>
                    Loads uncached logs on cache miss.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description

On a miss of the on-disk logs bloom cache, we check the uncached storage, and return that if available.

## Fixed Issue(s)
fixes #3921 

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 00:13:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4069" class=".btn">#4069</a>
            </td>
            <td>
                <b>
                    fix issue because parent world state is not available
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

We have this issue because we are replacing valid trielog by invalid trielog during a reorg. 

Can explain this strange trie log layer

>  : 0xd77f7f8868f20835fdfc8c7e851f6f23ce9f651d
   - StateTrieAccountValue{nonce=859, balance=0x00000000000000000000000000000000000000000000000006d141b0befb39fe, storageRoot=0x56e81f171bcc55a6ff8345e692c0f86e5b48e01b996cadc001622fb5e363b421, codeHash=0xc5d2460186f7233c927e7db2dcc703c0e500b653ca82273b7bfad8045d85a470}
   + StateTrieAccountValue{nonce=858, balance=0x00000000000000000000000000000000000000000000000006e96a274881e7b6, storageRoot=0x56e81f171bcc55a6ff8345e692c0f86e5b48e01b996cadc001622fb5e363b421, codeHash=0xc5d2460186f7233c927e7db2dcc703c0e500b653ca82273b7bfad8045d85a470}

The nonce comes from 859 to 858 and it’s not possible in a normal use case. 


### How to reproduce it (it's an example)

- We import block 5. we create a trie log for this block (4->5). A trie log it’s a diff between the previous block and the last one
- We import block 6 bis. we create a trie log for this block (5->6bis)
- We import block 7 bis. we create a trie log for this block (6bis->7bis)
- We detect a reorg with 6third with a common ancestor == 4. Rollback to 4 and we persist block 4. But in this issue we replace the valid trie log layer (3-4) with an invalid trie log (7bis->4)
- We import block 5 third. we create a trie log for this block (5 third ->6 third)
- We import block 6 third. we create a trie log for this block (6 third ->7 third)
- We detect a reorg with 6 with a common ancestor == 3. Rollback to 3 is failing because of the trie log == (7bis->4). 


In the code the problem is here

We persist after a rollback/rollfoward https://github.com/hyperledger/besu/blob/main/ethereum/core/src/main/java/org/hyperledger/besu/ethereum/bonsai/BonsaiWorldStateArchive.java#L247

We replace the trie log 
https://github.com/hyperledger/besu/blob/e79cf0e50724d7b5203708bf6b7abc24524f3dcb/ethereum/core/src/main/java/org/hyperledger/besu/ethereum/bonsai/BonsaiPersistedWorldState.java#L257


⚠️ if we have this issue we need to resync besu . there is not way to recover

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #4068 
fixes #4052

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 09:14:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4066" class=".btn">#4066</a>
            </td>
            <td>
                <b>
                    After merge add a rule to check that the current block is more recent than its parent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

In PoS current block timestamp must be greather than its parent block timestamp, so adding a new header validation rule to check that.
There is also a fix in the `shouldUsePostMergeRules` that was not correctly checking for TD >= TTD.

With this the Hive test *Invalid Ancestor Chain Re-Org, Invalid Timestamp, Invalid P9', Reveal using sync* passes.

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
        Created At 2022-07-06 18:31:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4065" class=".btn">#4065</a>
            </td>
            <td>
                <b>
                    Update dev genesis for anvil
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds anvil test accounts and milestone blocks to dev genesis. Builds on (fixing tests for) https://github.com/hyperledger/besu/pull/3872

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 11:22:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4064" class=".btn">#4064</a>
            </td>
            <td>
                <b>
                    CHANGELOG added 22.7.0-RC1 download links
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Added download links for 22.7.0-RC1

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 05:21:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4063" class=".btn">#4063</a>
            </td>
            <td>
                <b>
                    22.7.0-RC2-snapshot
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

22.7.0-RC2

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 04:17:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4062" class=".btn">#4062</a>
            </td>
            <td>
                <b>
                    22.7.0-RC1 non-snapshot version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

new RC1

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 03:51:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4059" class=".btn">#4059</a>
            </td>
            <td>
                <b>
                    Log message when path unavailable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Replaces https://github.com/hyperledger/besu/pull/3989

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 22:13:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4058" class=".btn">#4058</a>
            </td>
            <td>
                <b>
                    3943 stop blocks on finalized
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixed #3943 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 17:32:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4056" class=".btn">#4056</a>
            </td>
            <td>
                <b>
                    Return the correct latest valid hash in case of bad block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

In case a bad block is passed to `newPayload` or `forkchoiceUpdate` then response must contain the hash of the lastest valid block on the chain of the bad block, while now we just return the zero hash.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #3893 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 12:22:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4055" class=".btn">#4055</a>
            </td>
            <td>
                <b>
                    fcU: Ignore newHead if it is an ancestor of chain head
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                ## PR description
A forkchoice update will be ignored if `newHead` is an ancestor of chain head.

## Fixed Issue(s)
fixes #4051

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 09:39:53 +0000 UTC
    </div>
</div>

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

