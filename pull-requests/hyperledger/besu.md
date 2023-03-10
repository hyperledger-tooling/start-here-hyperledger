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
                PR <a href="https://github.com/hyperledger/besu/pull/5199" class=".btn">#5199</a>
            </td>
            <td>
                <b>
                    Replace streamMilestoneBlocks with getScheduledProtocolSpecs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                WIP
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-10 00:40:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5198" class=".btn">#5198</a>
            </td>
            <td>
                <b>
                    Replace ProtocolSchedule.streamMilestoneBlocks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #5163 

Replace usages of streamMilestoneBlocks on production code paths: RunnerBuilder and TransactionPoolFactory.
I ideally want to remove this method completely and may follow up with another PR, but the method is currently quite useful for some unit tests.

# Testing

- [x] Added/modified unit tests to ensure these changes were covered
- [ ] 2x sepolia syncs
- [ ] RunnerBuilder: run a network through a block number and also timestamp fork to ensure the node record is updated correctly - forkId should change in peering logs.
- [ ] TransitionPoolFactory: Create some txs with a known sort order and ensure that the BaseFee vs GasPrice sorting order is respected pre/post London and also post-Shanghai.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-09 22:47:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5197" class=".btn">#5197</a>
            </td>
            <td>
                <b>
                    Feature/minimal safe tracing
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

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [ ] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-09 21:18:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5196" class=".btn">#5196</a>
            </td>
            <td>
                <b>
                    (WIP) EIP-6110: Add deposit validation and apis
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

Add deposit validation and related apis. This PR depends on PR #5055. Work is still in progress please do not review.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

#5044 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [ ] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-09 15:55:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5195" class=".btn">#5195</a>
            </td>
            <td>
                <b>
                    Remove getByBlockNumber from dao classic specs
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
This PR removes getByBlockNumber from the ProtocolScheduleBuilder using the existing builders to fetch the original Spec for the blocks where the Dao/Classic fork will be inserted.

This PR has successfully generated the same ProtocolSchedules for Sepolia/Goerli and Mainnet. 
Samples:
- Sepolia
`2023-03-10 16:42:13.691+11:00 | main | INFO  | AbstractProtocolScheduleBuilder | Protocol schedule created with milestones: [London: 0, ParisFork: 1735371]
2023-03-10 16:42:13.695+11:00 | main | INFO  | AbstractProtocolScheduleBuilder | Protocol schedule created with milestones: [Shanghai: 1677557088]`
- Goerli
`2023-03-10 16:47:02.803+11:00 | main | INFO  | AbstractProtocolScheduleBuilder | Protocol schedule created with milestones: [Petersburg: 0, Istanbul: 1561651, Berlin: 4460644, London: 5062605]
2023-03-10 16:47:02.807+11:00 | main | INFO  | AbstractProtocolScheduleBuilder | Protocol schedule created with milestones: [Shanghai: 1678832736]
`
- Mainnet
`2023-03-10 16:41:05.327+11:00 | main | INFO  | AbstractProtocolScheduleBuilder | Protocol schedule created with milestones: [Frontier: 0, Homestead: 1150000, DaoRecoveryInit: 1920000, DaoRecoveryTransition: 1920001, Homestead: 1920010, TangerineWhistle: 2463000, SpuriousDragon: 2675000, Byzantium: 4370000, Petersburg: 7280000, Istanbul: 9069000, MuirGlacier: 9200000, Berlin: 12244000, London: 12965000, ArrowGlacier: 13773000, GrayGlacier: 15050000]
`
- Classic
`2023-03-10 16:39:19.567+11:00 | main | INFO  | AbstractProtocolScheduleBuilder | Protocol schedule created with milestones: [Frontier: 0, Homestead: 1150000, ClassicRecoveryInit: 1920000, Homestead: 1920001, TangerineWhistle: 2500000, DieHard: 3000000, Gotham: 5000000, DefuseDifficultyBomb: 5900000, Atlantis: 8772000, Agharta: 9573000, Phoenix: 10500839, Thanos: 11700000, Magneto: 13189133, Mystique: 14525000]
`

Pr has also successfully synced:
- [x] Sepolia
- [x] Goerli
- [ ] Mainnet

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #5161

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [x] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-09 12:54:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5194" class=".btn">#5194</a>
            </td>
            <td>
                <b>
                    Remove deprecated EF bootnodes
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

Removed some deprecated EF bootnodes. The same nodes have been removed on geth: https://github.com/ethereum/go-ethereum/pull/26828 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [ ] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-09 08:40:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5193" class=".btn">#5193</a>
            </td>
            <td>
                <b>
                    Parse t8n command txs properly
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

When receiving transactions from a file parse them as an RLP list.

## Fixed Issue(s)
fixes #5190 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [ ] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-09 01:49:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5192" class=".btn">#5192</a>
            </td>
            <td>
                <b>
                    Evmtool graalvm support
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

Changes and config to support using GraalVM AOT to compile and
execute evmTool.  While not as long-term performant the startup time
makes filling reference tests with Besu reasonable.

Builds off of #5189 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [ ] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-08 23:18:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5189" class=".btn">#5189</a>
            </td>
            <td>
                <b>
                    Isolate log4j
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

Remove some of the tendrils of Log4J that have snuck into various code locations. Isolate them into a single class.

This is preparatory for GraalVM compilation of EVMTool as it doesn't play well with log4j and Besu needs to be able to operate with log4j removed from the classpath.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [X] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-08 21:50:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5188" class=".btn">#5188</a>
            </td>
            <td>
                <b>
                    Post 23.1.1 update changelog
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
update changelog with download links and new block for 23.1.2-SNAPSHOT

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [ ] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 23:59:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5187" class=".btn">#5187</a>
            </td>
            <td>
                <b>
                    Fix flaky engine api acceptance test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">EIP</span>
            </td>
            <td>
                Assert on objects but use prettyString for failure message

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 23:38:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5186" class=".btn">#5186</a>
            </td>
            <td>
                <b>
                    Prepare for version 23.1.2-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prepare for version 23.1.2-SNAPSHOT
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 23:10:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5185" class=".btn">#5185</a>
            </td>
            <td>
                <b>
                    Release 23.1.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 23.1.1
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 21:49:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5183" class=".btn">#5183</a>
            </td>
            <td>
                <b>
                    Bonsai cleaning and robustness part 2 : tracing 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">TeamChupa</span><span class="chip">bonsai</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [ ] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 14:04:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5182" class=".btn">#5182</a>
            </td>
            <td>
                <b>
                    Fix for backward sync wrongly thinking it is done after a restart
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">syncing</span><span class="chip">TeamChupa</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

There is an issue when restarting Besu when a backward sync session is running, since after the restart it is possible that the Consensus client sends a FcU or a NewPayload for a block that is present in the backward sync storage, but not yet imported, so not on the main chain, but still the backward sync thinks it should not do anything with that block, so it returns like it has completed the sync, but since the sync is not done actually then the internal error that the finalize block is not present.

The solution is to persist the backward sync status, so in case of a restart, it can resume from where it was interrupted.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #5053 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [x] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 11:02:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5180" class=".btn">#5180</a>
            </td>
            <td>
                <b>
                    Fix Issues decoding the ephemeral public key (#5177)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Fix an issue where Besu fails to decode an ephemeral public key when dealing with an inbound handshake (Rlpx)

## Fixed Issue(s)

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [ ] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 02:31:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5179" class=".btn">#5179</a>
            </td>
            <td>
                <b>
                    copy layered worldstate fix for eth_call
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
This is mitigation fix for eth_call concurrency failures, similar to #5076. 

This mitigation will be obseleted by #5123.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#5175 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [ ] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 00:50:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5174" class=".btn">#5174</a>
            </td>
            <td>
                <b>
                    Fix empty body concept after shanghai
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">TeamGroot</span><span class="chip">mainnet</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
This PR adds withdrawals to the method that checks for empty block bodies in CompleteBlocksTask.java
Adding withdrawals allows Besu to be able to distinguish empty blocks after shanghai skiping the block body download when body is empty.
Prior to this PR Besu would understand blocks like (0txs, 0 ommers, x ws) as an empty block, during the sync process. (x > 0)

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #4976 

This PR has performed the following tests:
- [x] Recreated and tested fix on zhejiang-testnet using FAST sync
- [x] Successfully synced Sepolia (starting from checkpoint and transitioning to Shanghai)
- [x] Successfully synced Goerli 
- [ ] Successfully synced Mainnet
 
## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [x] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-06 10:16:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5173" class=".btn">#5173</a>
            </td>
            <td>
                <b>
                    Remove getByBlockNumber for CheckpointSync
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                Pull up and simplify data passed to CheckpointSource, which then allows checkpointBlockHeader to be used by protocolSchedule.getByBlockHeader.

Fixes #5167 

Alternative approach explored: https://github.com/siladu/besu/commit/bbaa80dcd88c517fb0d7a07a6fcd9f8a027bf5a5
but I didn't like the way ScheduleBasedHeaderBlockHeaderFunctions requires an explicit delegation override (otherwise it implicitly gets the wrong value).

CheckpointSync testing:
- [x] Sepolia (prysm)
- [x] Sepolia (lighthouse)
- [x] Goerli (lighthouse)
  - got in sync but required a restarted to transition from initial sync to backwards sync 
  - resync completed without intervention 
- [x] Mainnet (teku)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-06 06:53:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5171" class=".btn">#5171</a>
            </td>
            <td>
                <b>
                    Replace getByBlockNumber by getByBlockHeader in getBlockHeaderFunctions
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
This PR is a simple replace of the method getByBlockNumber by the wider getByBlockHeader for the ScheduleBasedBlockHeaderFunctions.getBlockHeaderFunctions method.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #5166

Successfully synced networks:
- [x] Sepolia
- [x] Goerli
- [x] Mainnet

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [x] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-06 03:44:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5170" class=".btn">#5170</a>
            </td>
            <td>
                <b>
                    Change transaction simulator to use ProtocolSchedule.getByBlockHeader
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
Change transaction simulator to use ProtocolSchedule.getByBlockHeader

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
related to #5158 

Manually tested the eth_call, trace_replayBlockTransaction, trace_block, and trace_transaction RPCs on Goerli.

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [x] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-06 03:24:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5169" class=".btn">#5169</a>
            </td>
            <td>
                <b>
                    Ask for Consensus Client and version on issue template
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Remove what appear to be unused templates
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-06 01:04:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5157" class=".btn">#5157</a>
            </td>
            <td>
                <b>
                    Burn-in candidate #1 of 23.1.1 
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
Candidate 1 for 23.1.1 burn-in.  This candidate is without the bonsai refactor from #5123 


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [ ] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 20:28:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5156" class=".btn">#5156</a>
            </td>
            <td>
                <b>
                    update changelog in main to reflect current releases
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
Update changelog in main to reflect releases for 23.1.0 and 23.1.1-RC1

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [ ] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 20:14:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5155" class=".btn">#5155</a>
            </td>
            <td>
                <b>
                    Merge main into 23.1.x release branch to prep for 23.1.1 release
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
prep 23.1.x release branch for alternate burn-in candidate by merging main into release-23.1.x

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [ ] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 19:55:21 +0000 UTC
    </div>
</div>

