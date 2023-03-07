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
                PR <a href="https://github.com/hyperledger/besu/pull/5184" class=".btn">#5184</a>
            </td>
            <td>
                <b>
                    Remove the fourth response element in eth_getWork
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                ## PR description
The [spec](https://ethereum.org/en/developers/docs/apis/json-rpc/#eth_getwork)  for `eth_getWork` only defines three return values and certain parsers rejects a longer response array.

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
        Created At 2023-03-07 15:15:38 +0000 UTC
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
- [ ] Successfully synced Goerli 
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
- [ ] Sepolia (prysm)
- [ ] Sepolia (lighthouse)
- [x] Goerli (lighthouse)
  - got in sync but required a restarted to transition from initial sync to backwards sync 
  - resync completed without intervention 
- [ ] Mainnet (teku)
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5151" class=".btn">#5151</a>
            </td>
            <td>
                <b>
                    Schedule Goerli shanghaiTime and configure forkId for tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span><span class="chip">EIP</span>
            </td>
            <td>
                Announced here: https://github.com/ethereum/execution-specs/pull/724

~Still waiting for confirmation of the forkId hash.~

Marius confirmed:
> I can confirm 0xf9843abf with 1678832736

Sepolia change for comparison: https://github.com/hyperledger/besu/commit/54521591f4dc2b9f142172d60c7a362b83ba3d32

I _could_ update `ForkIdsNetworkConfigTest` but Goerli hasn't been kept up to date for that test since Istanbul. I checked code coverage and I don't believe that test is providing any extra value beyond what `ForkIdTest` is already doing. I would suggest we remove `ForkIdsNetworkConfigTest` and the unnecessary parts of `ForkIdTestUtil`. Would like some feedback from @jframe about that first though.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 20:29:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5146" class=".btn">#5146</a>
            </td>
            <td>
                <b>
                    Add an acceptance test to ensure eth_getBlockByNumber and eth_getBlockByHash return withdrawals correctly for shanghai
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span><span class="chip">EIP</span>
            </td>
            <td>
                Fixes https://github.com/hyperledger/besu/issues/4808

I spent a good amount of time trying to add a test similar to https://github.com/hyperledger/besu/blob/main/ethereum/api/src/integration-test/java/org/hyperledger/besu/ethereum/api/jsonrpc/methods/fork/frontier/EthGetBlockByNumberIntegrationTest.java

...but was ultimately thwarted by some post-merge genesis protocol schedule issues. 

I think this AT-style is actually easier to understand and work with, and also tests the JSON serialization as a bonus.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 05:16:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5145" class=".btn">#5145</a>
            </td>
            <td>
                <b>
                    [MINOR] Add slf4j api so that acceptance tests work with using acctests.runBesuAsProcess = false
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 04:12:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5144" class=".btn">#5144</a>
            </td>
            <td>
                <b>
                    Upgrade Gradle to 8.0.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dev experience</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Upgrade Gradle to 8.0.1

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

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
        Created At 2023-03-01 05:47:02 +0000 UTC
    </div>
</div>

