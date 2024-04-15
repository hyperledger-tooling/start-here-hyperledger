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
                PR <a href="https://github.com/hyperledger/besu/pull/6953" class=".btn">#6953</a>
            </td>
            <td>
                <b>
                    Split acceptance tests by time
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Was looking at why our ATs are not correctly split by time, and found that the action that we are using is based on a tool, [that requires a special XML report with additional attributes](https://github.com/mtsmfm/split-test?tab=readme-ov-file#note), so as fallback the split is just done by name, this PR implements the split by time using a custom shell script

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-15 14:31:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6952" class=".btn">#6952</a>
            </td>
            <td>
                <b>
                    optimize node startup speed and memory allocation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

In summary, if a user employs a large genesis file and activates the `--genesis-state-hash-cache-enabled` parameter, their node can start in under **10 seconds**, requiring less than **2GB of memory**. This is the essence of what this PR accomplishes.

1. Regarding the process of serializing the string into a GenesisConfigFile, many parts of the code follow a similar logic pattern: `GenesisConfigFile.fromConfig(genesisContent).getConfigOptions()`, which means obtaining config options from the GenesisConfigFile. In fact, it does not care about the rest of the content, especially the accounts information, while large genesis files often have accounts occupying a large portion.

    Therefore, this PR introduces a new method, `fromConfigWithoutAccounts`, for all places where accounts are not needed. During the serialization of the string into a GenesisConfigFile, it ignores the accounts information. This change is should be safe because the only time accounts information is needed is during the calculation of the genesis state hash.

2. Based on the `-genesis-state-hash-cache-enabled` parameter added in https://github.com/hyperledger/besu/pull/6758, this PR further enhances the performance improvements that the parameter can offer.

    Originally, the parameter's purpose was to cache and skip the calculation of the genesis state hash value. Building upon the previous improvements, this PR determines that if this parameter is enabled and there is a cached genesis state hash in the database, then it will directly ignore the accounts content when reading the genesis file.

The table below outlines the comparison of node startup time and total memory reclaimed before and after the optimizations made in this PR. All tests utilized a genesis file of 1.1GB in size.

|  | Time Consuming - Before optimization | Memory Allocated - Before optimization | Time Consuming - Optimized (this PR) | Memory Allocated - Optimized (this PR) |
| --- | --- | --- | --- | --- |
| --genesis-state-hash-cache-enabled=false && block number=0 | 7min37s | 184.95GB | 7min24s | 158.83GB |
| --genesis-state-hash-cache-enabled=false && block number=1 | 2min53s | 125.47GB | 2min36s | 96.53GB |
| --genesis-state-hash-cache-enabled=true && block number=0 | 7min35s | 183.33GB | 7min34s | 154.68GB |
| --genesis-state-hash-cache-enabled=true && block number=1 | 0min50s | 66.75GB | 0min9s | 1.31GB |

Without the `--genesis-state-hash-cache-enabled` parameter enabled, the startup time reduced from **2 minutes and 53 seconds** to **2 minutes and 36 seconds**, and the total memory reclaimed decreased from **125.47GB** to **96.53GB**. The optimization effect here is modest.

With the `--genesis-state-hash-cache-enabled` parameter enabled, the startup time can be reduced from **50 seconds** to **9 seconds**, and the total memory reclaimed from **66.75GB** to **1.31GB**, marking a significant optimization effect.

This is the unit test coverage report for the PR: [Unit Test Coverage Report](https://lyfsn.github.io/besu-starter/pr2/).

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [x] unit tests: `./gradlew build`
- [x] acceptance tests: `./gradlew acceptanceTest`
- [x] integration tests: `./gradlew integrationTest`
- [x] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-15 12:38:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6951" class=".btn">#6951</a>
            </td>
            <td>
                <b>
                    chore: fix some typos in comments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

 fix some typos in comments


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-15 11:43:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6950" class=".btn">#6950</a>
            </td>
            <td>
                <b>
                    Sync worldstate MerkleTrieException
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Handle MerkleTrieException that can thrown during snapsync worldstate sync in the heal pipeline by triggering the trie heal process to start again. Not handling the exception causes the worldstate download to halt.

Stacktrace from custom build with try/catch around the steps in `SnapWorldStateDownloadProcess` 
```
{"@timestamp":"2024-04-11T00:54:12,336","level":"INFO","thread":"nioEventLoopGroup-3-8","class":"SnapWorldDownloadState","message":"Running world state heal process from peers with pivot block 19628877","throwable":""}
{"@timestamp":"2024-04-11T00:54:15,862","level":"INFO","thread":"EthScheduler-Services-22 (requestLoadLocalTrieNodeData)","class":"SnapWorldStateDownloadProcess","message":"Sync exception detected org.hyperledger.besu.ethereum.trie.MerkleTrieException: Unable to load trie node value for hash 0x2950ee2415e7eb2d2e4e68da92c26f0bdbd4b4b6f5479674ffe90217f70df113 location 0x000700060003","throwable":""}
{"@timestamp":"2024-04-11T00:54:15,863","level":"INFO","thread":"EthScheduler-Services-23 (requestLoadLocalTrieNodeData)","class":"SnapWorldStateDownloadProcess","message":"Sync exception detected org.hyperledger.besu.ethereum.trie.MerkleTrieException: Unable to load trie node value for hash 0x9a508f8523133ecd0b74e76ac41f9da3c095622a2f06b9a767affd460f9553ba location 0x000700050806","throwable":""}
org.hyperledger.besu.ethereum.trie.MerkleTrieException: Unable to load trie node value for hash 0x2950ee2415e7eb2d2e4e68da92c26f0bdbd4b4b6f5479674ffe90217f70df113 location 0x000700060003
        at org.hyperledger.besu.ethereum.trie.StoredNode.lambda$load$0(StoredNode.java:135)
        at java.base/java.util.Optional.orElseThrow(Optional.java:403)
        at org.hyperledger.besu.ethereum.trie.StoredNode.load(StoredNode.java:133)
        at org.hyperledger.besu.ethereum.trie.StoredNode.accept(StoredNode.java:65)
        at org.hyperledger.besu.ethereum.trie.patricia.GetVisitor.visit(GetVisitor.java:51)
        at org.hyperledger.besu.ethereum.trie.patricia.BranchNode.accept(BranchNode.java:85)
        at org.hyperledger.besu.ethereum.trie.StoredNode.accept(StoredNode.java:66)
        at org.hyperledger.besu.ethereum.trie.patricia.GetVisitor.visit(GetVisitor.java:51)
        at org.hyperledger.besu.ethereum.trie.patricia.BranchNode.accept(BranchNode.java:85)
        at org.hyperledger.besu.ethereum.trie.StoredNode.accept(StoredNode.java:66)
        at org.hyperledger.besu.ethereum.trie.StoredMerkleTrie.getPath(StoredMerkleTrie.java:97)
        at org.hyperledger.besu.ethereum.eth.sync.snapsync.request.heal.AccountTrieNodeHealingRequest.getRootStorageRequests(AccountTrieNodeHealingRequest.java:117)
        at org.hyperledger.besu.ethereum.eth.sync.snapsync.LoadLocalDataStep.loadLocalDataTrieNode(LoadLocalDataStep.java:86)
        at org.hyperledger.besu.ethereum.eth.sync.snapsync.SnapWorldStateDownloadProcess$Builder.lambda$build$23(SnapWorldStateDownloadProcess.java:560)
        at org.hyperledger.besu.services.pipeline.FlatMapProcessor.processNextInput(FlatMapProcessor.java:32)
        at org.hyperledger.besu.services.pipeline.ProcessingStage.run(ProcessingStage.java:38)
        at org.hyperledger.besu.services.pipeline.Pipeline.lambda$runWithErrorHandling$3(Pipeline.java:170)
        at java.base/java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:572)
        at java.base/java.util.concurrent.FutureTask.run(FutureTask.java:317)
        at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1144)
        at java.base
````

I haven't been able to reproduce the issue on another node to test that the trie heal works as intended. But we use this elsewhere in the SnapWorldStateDownloadProcess.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-15 08:58:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6948" class=".btn">#6948</a>
            </td>
            <td>
                <b>
                    Attempt to speed up ATs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Attempt to revert long running AT times from 7e46889


Signed-off-by: Simon Dudley <simon.dudley@consensys.net>

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-15 05:34:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6947" class=".btn">#6947</a>
            </td>
            <td>
                <b>
                    Peer disconnect message - add client info
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">logging</span><span class="chip">peering</span>
            </td>
            <td>
                ## PR description
Add client name to summary disconnect message - makes cross-referencing disconnects much easier.
Also whether the connection was active.

## Fixed Issue(s)
Refs #6945


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-15 05:19:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6944" class=".btn">#6944</a>
            </td>
            <td>
                <b>
                    Implementation of Issue #3810 QBFT no empty block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Implementing `emptyblockperiodseconds` for producing empty blocks at a specific interval independently of the value of the existing  `blockperiodseconds` setting

## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/3810

### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [x] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-14 13:27:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6943" class=".btn">#6943</a>
            </td>
            <td>
                <b>
                    Fix named network default disabled for downgrade protection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Address downgrade default for named networks.  Previously the check for named network was only considering command line params, and not toml config files.

Also implemented Comparable on VersionMetadata, and added explicit version test cases for a variety of build versions.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-12 19:08:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6942" class=".btn">#6942</a>
            </td>
            <td>
                <b>
                    Update execution-spec-tests support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update t8n, b11r, and friends to support current execution spec
* bonsai migration introduced issues with deleted storage/accounts
* status on pre-constantinople json was invalid
* track refund across tx, not call frame
* allow tests to be executed by name

Signed-off-by: Danno Ferrin <danno@numisight.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-12 16:20:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6941" class=".btn">#6941</a>
            </td>
            <td>
                <b>
                    Consistent nonce handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Make handling of absurdly large nonces
more consistent across txpool and EVM.

Signed-off-by: Danno Ferrin <danno@numisight.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-12 15:26:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6940" class=".btn">#6940</a>
            </td>
            <td>
                <b>
                    Layered txpool tuning for blob transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                ## PR description

Introduce a new configuration option, `tx-pool-max-prioritized-by-type`, to tune the max number of transaction of a specified type that are kept in the prioritized layer at any time.
This new option is mostly useful to tune the amount of blob txs to keep in the prioritized layer, that is the layer with the transactions that are candidate for inclusion in a potential next block. Keeping this layer sorted is costly so it makes sense to only keep there the max amount of txs that could fit in a block, plus a small buffer, there is already an option to limit the max number of txs in this layer, but since very few blob txs can be included in a block (max 6 at this time), having the possibility to tune the max number of txs by type help with keeping the prioritized layer performant.

By default `tx-pool-max-prioritized-by-type=["BLOB=6"]`

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-12 14:25:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6939" class=".btn">#6939</a>
            </td>
            <td>
                <b>
                    Change Blockminer log
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Change block miner log to include all the performance number on one line with Info level.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [x] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-12 13:15:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6938" class=".btn">#6938</a>
            </td>
            <td>
                <b>
                    check for empty in disconnect reason bytes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Fix bug introduced in #6925
UNKNOWN disconnect reason has null code

## Fixed Issue(s)
Fixes #6937


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-12 07:08:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6936" class=".btn">#6936</a>
            </td>
            <td>
                <b>
                    Fix Flaky test permv2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span><span class="chip">flake</span>
            </td>
            <td>
                ## PR description
Do the extra verify step before sending transactions, in a different test

## Fixed Issue(s)
follow up to initial fix for #6914 


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-12 05:41:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6934" class=".btn">#6934</a>
            </td>
            <td>
                <b>
                    fix npe on trace msg
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Currently seeing NPE on trace level due to the possibility of the ethPeer variable be null at that point of the code.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-11 23:28:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6933" class=".btn">#6933</a>
            </td>
            <td>
                <b>
                    Add Paris Support to tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Execution-spec-tests and reference tests have migrated Merge to Paris.
Support both.

Signed-off-by: Danno Ferrin <danno@numisight.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-11 21:40:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6931" class=".btn">#6931</a>
            </td>
            <td>
                <b>
                    [MINOR] logging for fork ID check failed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">logging</span><span class="chip">peering</span>
            </td>
            <td>
                ## PR description
Logging was confusing - we were getting a "fork id check failed" for a peer that had already responded and given us a good block. I suspect they were in the process of disconnecting us. 
This PR adds some extra (trace) logging for why the EthProtocolManager does not want to connect, and ensures we only log "fork ID check failed" if in fact that is the problem.

## Fixed Issue(s)



### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-11 06:49:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6930" class=".btn">#6930</a>
            </td>
            <td>
                <b>
                    Fix permissions for publish and gradle issue for publishArtifactory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The changes in https://github.com/hyperledger/besu/pull/6705 broke the release process
and https://github.com/hyperledger/besu/pull/6856 maybe never worked
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-11 06:30:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6925" class=".btn">#6925</a>
            </td>
            <td>
                <b>
                    richness for breach of protocol reasons
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-10 04:41:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6924" class=".btn">#6924</a>
            </td>
            <td>
                <b>
                    Snap pipeline errors logged
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
This is to log any possible throwables we're getting up on snap requests

### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-10 04:29:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6922" class=".btn">#6922</a>
            </td>
            <td>
                <b>
                    follow up improvement in ordering to fix flakiness
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span><span class="chip">flake</span>
            </td>
            <td>
                ## PR description
Follow up to #6917 - need to check nodes are synced before permissions are modified since that's on chain

## Fixed Issue(s)
Fixes #6921


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-10 02:54:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6920" class=".btn">#6920</a>
            </td>
            <td>
                <b>
                    Fork/verkle final
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-09 15:06:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6919" class=".btn">#6919</a>
            </td>
            <td>
                <b>
                    Add RPC errors metric
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add RPC errors metric to Besu. The metric should be labeled with the method RPC name and the error type.
I simulated two errors on eth_call and we can see below the metrics retrieved by prometheus

![image](https://github.com/hyperledger/besu/assets/5099602/457dd22c-47a3-425c-b394-57fbbf50f622)


## Fixed Issue(s)
https://github.com/Consensys/protocol-misc/issues/925
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [x] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-09 13:22:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6917" class=".btn">#6917</a>
            </td>
            <td>
                <b>
                    Fix flaky test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Use block chain height not syncing status
Fixes the flaky test disabled in #6915 

## Fixed Issue(s)
Fixes #6914 


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-09 10:54:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6916" class=".btn">#6916</a>
            </td>
            <td>
                <b>
                    Fix and reformat produced block timing log
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-09 10:15:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6912" class=".btn">#6912</a>
            </td>
            <td>
                <b>
                    BadCLIPlugin test - disable on mac
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
These 2 tests always fail on mac so disable them by OS

## Fixed Issue(s)
Fixes #5599 
Fixes #6815 

### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [x] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`
- [x] confirm that these 2 tests ran on GHA before merging


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-09 05:21:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6911" class=".btn">#6911</a>
            </td>
            <td>
                <b>
                    Block import progress logging: add peer count
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add peer count to info level log

## Fixed Issue(s)
Fixes #6910 


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-09 02:26:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6907" class=".btn">#6907</a>
            </td>
            <td>
                <b>
                    Added waitTime option on engine ATs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Added an option for waiting for some time before sending an engine API request during ATs. Mostly to help when building blocks, to be able to give the node some time to actually include transactions etc.

## Fixed Issue(s)
N/A

### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-08 22:00:36 +0000 UTC
    </div>
</div>

