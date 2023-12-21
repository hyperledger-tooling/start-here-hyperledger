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
                PR <a href="https://github.com/hyperledger/besu/pull/6316" class=".btn">#6316</a>
            </td>
            <td>
                <b>
                    add missing check for static peers to allow them to exceed the connection limit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
In one place there was a check missing to allow static peers to exceed the connection limit.
Another improvement is that streamBestPeers() does only return fully validated peers.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-20 02:13:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6315" class=".btn">#6315</a>
            </td>
            <td>
                <b>
                    Log/Address Trielog rolling failure
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
        Created At 2023-12-19 23:41:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6313" class=".btn">#6313</a>
            </td>
            <td>
                <b>
                    fix: call OperationTracer.traceEndTx for failing transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Call `OperationTracer.traceEndTx` even when a transaction failed.

## Fixed Issue(s)
fixes #6312 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-19 13:06:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6310" class=".btn">#6310</a>
            </td>
            <td>
                <b>
                    Release 23.10.3-RC4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                RC3 failed on one specific canary; it ran into an edge case during a backwards sync on a single testing canary for lodestar on mainnet doing a checkpoint sync (see attached logfile, timestamp 2023-12-15T21:36:50,193 ). This did not happen for any other clients, including teku and sepolia variants.

There is a known issue in Besu where during a sync, a very tight loop will max out the CPU. We would like to add the fix for this issue to RC4.

[besu.log.zip](https://github.com/hyperledger/besu/files/13707409/besu.log.zip)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-18 19:19:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6309" class=".btn">#6309</a>
            </td>
            <td>
                <b>
                    Quick fix to avoid a tight loop when processing added blocks in txpool
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

When a node is full syncing or backward syncing, it is possible the processing of block added in the txpool, causes a tight loop, with the result of high cpu consumption, that causes the node to basically halt doing other tasks.
This is a quick workaround, while a proper solution, that also avoids to process added blocks during full sync is in progress, and will be ready.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-18 19:12:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6307" class=".btn">#6307</a>
            </td>
            <td>
                <b>
                    Restrict downgrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">doc-change-required</span>
            </td>
            <td>
                ## PR description
This PR aims to prevent accidental downgrade of Besu, which can potentially cause the DB to be irrevocably corrupted.

The approach I've used is as follows:

 - Add a new file `VERSION_METADATA.json` in the configured data path
   - Contains a single `besuVersion` field, e.g. `{"besuVersion":"23.10.3"}` 
 - Add a new `--allow-downgrade` configuration option
 - Update the gradle prereqs to pull in `org.apache.maven:maven-artifact` to provide access to the maven `ComparableVersion` class
 - Add a function `performDowngradeCheck()` to `BesuCommand` as the first function to call after configuration options have been validated.
   - `performDowngradeCheck()` throws an exception if the version in `VERSION_METADATA.json` is higher (when compared using the maven `ComparableVersion` class) than the version in as recorded in the `BesuCommand` class implementation version

Any value after the first `-` character in the version number is ignored. This limits version comparison to the 3 calver digits, which is all that can be logically compared as higher or lower. An example of a version number that has trailing characters is `23.10.4-dev-c9338660` where the latest commit has been appended to the version. The `-dev-c9338660` is ignored in the version comparison.

The validation logic is as follows:
- If the `VERSION_METADATA.json` file doesn't exist, no further checks are made and the node starts. The `VERSION_METADATA.json` file is written to allow version checks from this point onwards.
- If the file and `besuVersion` field are present and the version is lower than the installed/runtime version, Besu updates it to have the latest version in it and continues to start up
- If the file and `besuVersion` field are present and the version is greater than the installed/runtime version, Besu fails to start unless `--allow-downgrade` is set, because a lower version of Besu is being started than the version that most recently updated the file.

## Remaining TODOs

- [x] Update/add tests
- [x] Add CLI arg such as `--allow-downgrade` to allow a downgrade if specified

## Fixed Issue(s)
Fixes https://github.com/hyperledger/besu/issues/6266
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-18 12:25:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6306" class=".btn">#6306</a>
            </td>
            <td>
                <b>
                    Generate genesis root hash with the used data storage format
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

Before, we always generated the root hash of the genesis with forest, even if we activated bonsai. I am modifying the logic to use the correct storage format that we activated. This will facilitate a potential removal of forest and also be able to generate the genesis root hash using verkle when it is integrate

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-18 09:34:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6305" class=".btn">#6305</a>
            </td>
            <td>
                <b>
                    mark deleted slot during clear storage step
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
        Created At 2023-12-15 18:27:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6303" class=".btn">#6303</a>
            </td>
            <td>
                <b>
                    Add --X-trie-log subcommand
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
This is a more direct approach to the previous attempt in #6188.
Tests showed that the previous approach was taking too long (3 hours) to prune a 3.5 months old (keeping the lastest 512 only).
The approach this PR takes is faster since it resets the column family and only retain the necessary trie logs (saved in files in batches of 20_000 trie logs).
Drawback of this approach is that we do store the trie logs in disk (in files) before dropping the column. Realistic speaking there's little to no reason to actually keep many more trie logs than the default(512).
In any case, I've made some adjustments to the code to allow this to go as far as a user might like.
 
Ran tests on nodes retaining 512 / 20_000 / 250_000 trie logs.

Below some of the logs condensed

```dev-elc-besu-teku-mainnet-trielog-prune-test-08:~/besu-23.10.4-SNAPSHOT/bin$ sudo ./besu --config-file=/etc/besu/config.toml storage x-trie-log prune
2023-12-20 05:52:28.506+00:00 | main | INFO  | Besu | 0 Bootnodes configured
2023-12-20 05:52:28.721+00:00 | main | INFO  | KeyPairUtil | Attempting to load public key from /data/besu/key
2023-12-20 05:52:28.756+00:00 | main | INFO  | KeyPairUtil | Loaded public key 0x1cfe10534f14fc067be9fc88bcde02ab4970a36b907bbd38918236ec8767142c07316ab4c5de5c6f893442cf8f2deb422d2917f5a9d443cd81d04e055e65741d from /data/besu/key
2023-12-20 05:52:29.160+00:00 | main | INFO  | ProtocolScheduleBuilder | Protocol schedule created with milestones: [Frontier:0, Homestead:1150000, DaoRecoveryInit:1920000, DaoRecoveryTransition:1920001, Homestead:1920010, TangerineWhistle:2463000, SpuriousDragon:2675000, Byzantium:4370000, Petersburg:7280000, Istanbul:9069000, MuirGlacier:9200000, Berlin:12244000, London:12965000, ArrowGlacier:13773000, GrayGlacier:15050000, Shanghai:1681338455]
2023-12-20 05:52:29.313+00:00 | main | INFO  | ProtocolScheduleBuilder | Protocol schedule created with milestones: [Paris:0, Paris:1150000, Paris:1920000, Paris:1920001, Paris:1920010, Paris:2463000, Paris:2675000, Paris:4370000, Paris:7280000, Paris:9069000, Paris:9200000, Paris:12244000, Paris:12965000, Paris:13773000, Paris:15050000, Shanghai:1681338455]
2023-12-20 05:52:29.736+00:00 | main | INFO  | DatabaseMetadata | Lookup database metadata file in data directory: /data/besu
2023-12-20 05:52:29.790+00:00 | main | INFO  | RocksDBKeyValueStorageFactory | Existing database detected at /data/besu. Version 2. Compacting database...
2023-12-20 05:52:36.209+00:00 | main | INFO  | BonsaiWorldStateKeyValueStorage | Bonsai flat db mode found PARTIAL
2023-12-20 05:52:37.270+00:00 | main | INFO  | TransactionPoolFactory | Transaction pool disabled while initial sync in progress
2023-12-20 05:52:37.273+00:00 | main | INFO  | EthPeers | Updating the default best peer comparator
2023-12-20 05:52:37.290+00:00 | main | INFO  | BesuControllerBuilder | TTD difficulty is present, creating initial sync for PoS
2023-12-20 05:52:37.302+00:00 | main | INFO  | CheckpointDownloaderFactory | Checkpoint sync was requested, but cannot be enabled because the local blockchain is not empty.
2023-12-20 05:52:37.304+00:00 | main | INFO  | TransitionBesuControllerBuilder | TTD present, creating DefaultSynchronizer that stops propagating after finalization
2023-12-20 05:52:37.320+00:00 | main | INFO  | BonsaiWorldStateKeyValueStorage | Bonsai flat db mode found PARTIAL
2023-12-20 05:52:38.399+00:00 | main | INFO  | TrieLogHelper | Saving trie logs to retain in file (batch 1)...
2023-12-20 05:52:38.423+00:00 | main | INFO  | TrieLogHelper | Obtaining trielogs from db, this may take a few minutes...
2023-12-20 05:52:59.221+00:00 | main | INFO  | TrieLogHelper | Saving trie logs to retain in file (batch 2)...
2023-12-20 05:52:59.221+00:00 | main | INFO  | TrieLogHelper | Obtaining trielogs from db, this may take a few minutes...
2023-12-20 05:53:36.325+00:00 | main | INFO  | TrieLogHelper | Saving trie logs to retain in file (batch 3)...
2023-12-20 05:53:36.325+00:00 | main | INFO  | TrieLogHelper | Obtaining trielogs from db, this may take a few minutes...
2023-12-20 05:54:31.376+00:00 | main | INFO  | TrieLogHelper | Saving trie logs to retain in file (batch 4)...
2023-12-20 05:54:31.376+00:00 | main | INFO  | TrieLogHelper | Obtaining trielogs from db, this may take a few minutes...
2023-12-20 05:55:43.574+00:00 | main | INFO  | TrieLogHelper | Saving trie logs to retain in file (batch 5)...
2023-12-20 05:55:43.575+00:00 | main | INFO  | TrieLogHelper | Obtaining trielogs from db, this may take a few minutes...
2023-12-20 05:57:03.626+00:00 | main | INFO  | TrieLogHelper | Saving trie logs to retain in file (batch 6)...
2023-12-20 05:57:03.627+00:00 | main | INFO  | TrieLogHelper | Obtaining trielogs from db, this may take a few minutes...
2023-12-20 05:58:25.553+00:00 | main | INFO  | TrieLogHelper | Saving trie logs to retain in file (batch 7)...
2023-12-20 05:58:25.553+00:00 | main | INFO  | TrieLogHelper | Obtaining trielogs from db, this may take a few minutes...
2023-12-20 05:59:52.073+00:00 | main | INFO  | TrieLogHelper | Saving trie logs to retain in file (batch 8)...
2023-12-20 05:59:52.073+00:00 | main | INFO  | TrieLogHelper | Obtaining trielogs from db, this may take a few minutes...
2023-12-20 06:01:19.833+00:00 | main | INFO  | TrieLogHelper | Saving trie logs to retain in file (batch 9)...
2023-12-20 06:01:19.834+00:00 | main | INFO  | TrieLogHelper | Obtaining trielogs from db, this may take a few minutes...
2023-12-20 06:02:50.251+00:00 | main | INFO  | TrieLogHelper | Saving trie logs to retain in file (batch 10)...
2023-12-20 06:02:50.252+00:00 | main | INFO  | TrieLogHelper | Obtaining trielogs from db, this may take a few minutes...
2023-12-20 06:04:21.662+00:00 | main | INFO  | TrieLogHelper | Saving trie logs to retain in file (batch 11)...
2023-12-20 06:04:21.662+00:00 | main | INFO  | TrieLogHelper | Obtaining trielogs from db, this may take a few minutes...
2023-12-20 06:05:53.057+00:00 | main | INFO  | TrieLogHelper | Saving trie logs to retain in file (batch 12)...
2023-12-20 06:05:53.058+00:00 | main | INFO  | TrieLogHelper | Obtaining trielogs from db, this may take a few minutes...
2023-12-20 06:07:20.839+00:00 | main | INFO  | TrieLogHelper | Saving trie logs to retain in file (batch 13)...
2023-12-20 06:07:20.840+00:00 | main | INFO  | TrieLogHelper | Obtaining trielogs from db, this may take a few minutes...
2023-12-20 06:08:02.864+00:00 | main | INFO  | TrieLogHelper | Clear trie logs...
2023-12-20 06:08:06.872+00:00 | main | INFO  | TrieLogHelper | Restoring trie logs retained from batch 1...
…
2023-12-20 06:18:32.525+00:00 | main | INFO  | TrieLogHelper | Deleting files...
2023-12-20 06:18:32.629+00:00 | main | INFO  | TrieLogHelper | Prune ran successfully. Enjoy some disk space back! 🚀
```
 


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Part of #5390 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-15 04:10:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6302" class=".btn">#6302</a>
            </td>
            <td>
                <b>
                    Disable txpool during fullsync
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
        Created At 2023-12-14 15:52:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6300" class=".btn">#6300</a>
            </td>
            <td>
                <b>
                    create trie package for bonsai and forest
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

A PR to place Bonsai and Forest in the same trie package. This PR is a preparation for the introduction of Verkle. This trie package will have Verkle in a next PR and we will add a common package so that the different trie substructures can share classes if needed. 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-14 10:58:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6299" class=".btn">#6299</a>
            </td>
            <td>
                <b>
                    [MINOR] Trailing peer limit log
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span><span class="chip">logging</span>
            </td>
            <td>
                fixes #6269 

```
sallymacfarlane@dev-elc-besu-teku-mainnet-dev-sally-trailing-peer-log-3:/var/log/besu$ grep Trailing besu.log
{"@timestamp":"2023-12-14T12:50:11,138","level":"DEBUG","thread":"nioEventLoopGroup-3-5","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0xadb935a416b0c19aaf... with height 18783177","throwable":""}
{"@timestamp":"2023-12-14T12:51:47,696","level":"DEBUG","thread":"nioEventLoopGroup-3-9","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0xc8a80e895f6b85f8ff... with height 18299999","throwable":""}
{"@timestamp":"2023-12-14T12:51:49,471","level":"DEBUG","thread":"nioEventLoopGroup-3-1","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0x48f462dab313723e05... with height 18001000","throwable":""}
{"@timestamp":"2023-12-14T12:52:19,523","level":"DEBUG","thread":"nioEventLoopGroup-3-5","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0xd9c1f1b8c84f4dcd96... with height 13883323","throwable":""}
{"@timestamp":"2023-12-14T12:52:40,702","level":"DEBUG","thread":"nioEventLoopGroup-3-4","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0xd9c1f1b8c84f4dcd96... with height 13885662","throwable":""}
{"@timestamp":"2023-12-14T12:52:49,897","level":"DEBUG","thread":"nioEventLoopGroup-3-2","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0xd9c1f1b8c84f4dcd96... with height 13886842","throwable":""}
{"@timestamp":"2023-12-14T12:53:19,501","level":"DEBUG","thread":"nioEventLoopGroup-3-9","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0xd9c1f1b8c84f4dcd96... with height 13889692","throwable":""}
{"@timestamp":"2023-12-14T12:53:49,340","level":"DEBUG","thread":"nioEventLoopGroup-3-3","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0xd9c1f1b8c84f4dcd96... with height 13891310","throwable":""}
{"@timestamp":"2023-12-14T12:54:19,841","level":"DEBUG","thread":"nioEventLoopGroup-3-10","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0xd9c1f1b8c84f4dcd96... with height 13893155","throwable":""}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-14 09:20:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6297" class=".btn">#6297</a>
            </td>
            <td>
                <b>
                    [MINOR] add genesis file name to config overview
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">logging</span><span class="chip">ux</span><span class="chip">non mainnet (private networks)</span>
            </td>
            <td>
                ```
# Configuration:                                                                                   #
# Network: Custom genesis file                                                                     #
# /Users/sm/workspace/besu/config/besu/genesis-linea.json                                          #
# Network Id: 59140                                                                                #
# Data storage: Forest                                                                             #
# Sync mode: Snap                                                                                  #
# RPC HTTP APIs: ADMIN,ETH,NET,WEB3,PERM,DEBUG,MINER,EEA,PRIV,TXPOOL                               #
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-14 06:32:29 +0000 UTC
    </div>
</div>

