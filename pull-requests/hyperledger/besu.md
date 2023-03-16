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
                PR <a href="https://github.com/hyperledger/besu/pull/5228" class=".btn">#5228</a>
            </td>
            <td>
                <b>
                    Reference Test v12
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Upgrade reference tests to v12.
* Extend the UncleFromSideChain exception to all future forks
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-16 14:08:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5226" class=".btn">#5226</a>
            </td>
            <td>
                <b>
                    junit 5 for util tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use Junit 5 for besu/util tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-16 06:47:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5225" class=".btn">#5225</a>
            </td>
            <td>
                <b>
                    [GHA] Checklist action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This GHA will add the checklist that's currently in the PR template, as a comment, on newly opened PRs. 

Because it needs write access (to add the comment), it needs to run on the `pull_request_target` action, which means you won't see the outcome on _this_ PR, but only once it's merged in, you'll see it on subsequent PRs - example - https://github.com/daisy-row/vigilant-octo-umbrella/pull/51
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-16 02:17:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5224" class=".btn">#5224</a>
            </td>
            <td>
                <b>
                    Add getForNextBlockHeader to protocol schedule
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
Add getForNextBlockHeader to protocol schedule

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
        Created At 2023-03-16 00:48:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5221" class=".btn">#5221</a>
            </td>
            <td>
                <b>
                    Remove getbyblocknumber from flexibleprivacyprecompiledcontract
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
This PR aims to remove the usage of getByBlockNumber from the FlexiblePrivacyPrecompiledContract. As far as analysis shows the only requirement is to get a protocolSpec (it doesn't matter which one) currently it always fetches the protocolSpec for block number 1 which can vary according to the network config. We're changing that get the protocolSpec for block 0 which is the only block we always have the header.

AT nonmainnet on circle CI
Pipeline - 21048

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #5160 

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
        Created At 2023-03-15 12:26:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5220" class=".btn">#5220</a>
            </td>
            <td>
                <b>
                    add register useless response to multiple tasks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">peering</span>
            </td>
            <td>
                ## PR description
Some of the tasks in Besu, especially the Snapsync ones, did not register a useless response when necessary. When a specific number of useless reponses have been registered against an EthPeer within a certain time, the EthPeer is disconnected.
Without this mechanism it is possible that Besu is looping through useless peers for a long time.
With the change, useless peers will be disconnected, which makes room for Besu to find new, hopefully useful, peers.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-15 07:29:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5219" class=".btn">#5219</a>
            </td>
            <td>
                <b>
                    Add links to PRs in changelog
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

Reviewing the changelog I think it's nice to have clickable links to faster get to the PRs I might wanna review more in detail
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-15 07:27:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5217" class=".btn">#5217</a>
            </td>
            <td>
                <b>
                    openj9 docker build
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
Docker image which uses semeru openjdk-17 jammy container base for besu

Quoting https://www.infoq.com/news/2021/10/ibm-introduces-semeru-openj9/ :

IBM has [introduced](https://developer.ibm.com/blogs/introducing-the-ibm-semeru-runtimes/) no-cost [Semeru Runtimes](https://developer.ibm.com/languages/java/semeru-runtimes/) that use class libraries from OpenJDK together with the Eclipse [OpenJ9](https://www.eclipse.org/openj9/) Java Virtual Machine (JVM). The runtimes, based on OpenJ9, may be used as an alternative for runtimes based on [HotSpot](https://openjdk.java.net/groups/hotspot/). Previously, [AdoptOpenJDK](https://adoptopenjdk.net/) produced binaries with OpenJ9, however that’s no longer legally allowed since their [move to the Eclipse Foundation](https://www.infoq.com/news/2020/06/adoptopenjdk-eclipse-adoptium/) under the new name, [Adoptium](https://adoptium.net/).


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#5181

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
        Created At 2023-03-15 02:09:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5214" class=".btn">#5214</a>
            </td>
            <td>
                <b>
                    [MINOR] junit5 for eth/sync tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                migrate some more tests to junit5
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 05:45:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5209" class=".btn">#5209</a>
            </td>
            <td>
                <b>
                    increased default to 5000
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                Increase max log range to 5000 - was reduced to 1000 in #4597 

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
        Created At 2023-03-13 07:18:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5208" class=".btn">#5208</a>
            </td>
            <td>
                <b>
                    [MINOR] junit5 for RPC ATs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updated to junit 5 for non-parameterized tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-13 07:13:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5207" class=".btn">#5207</a>
            </td>
            <td>
                <b>
                    [GHA] add separate dco yml for merge_group event
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a separate yml file with the merge_group event trigger that doesn't invoke the PR based dco

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
        Created At 2023-03-13 06:56:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5206" class=".btn">#5206</a>
            </td>
            <td>
                <b>
                    Fix console logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Based on https://github.com/hyperledger/besu/pull/5202

Getting a fix onto main while we work on a valid acceptance test.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-13 05:34:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5205" class=".btn">#5205</a>
            </td>
            <td>
                <b>
                    [MINOR] use junit 5 for plugin and some other ATs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use junit 5 for plugins ATs 

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
        Created At 2023-03-13 04:36:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5204" class=".btn">#5204</a>
            </td>
            <td>
                <b>
                    [GHA] no DCO on merge_group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                argh dco does not support merge_group event - it's the same problem we had with merge to main https://github.com/hyperledger/besu/actions/runs/4400701640 


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
        Created At 2023-03-13 02:22:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5203" class=".btn">#5203</a>
            </td>
            <td>
                <b>
                    [MINOR] use constants for strings in test plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use constants for strings in test plugin

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
        Created At 2023-03-13 01:54:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5202" class=".btn">#5202</a>
            </td>
            <td>
                <b>
                    Verify default logging is INFO
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Add an acceptance test to verify that default logging is at least INFO.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-12 04:37:16 +0000 UTC
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
These usages were also using getBlockByNumber which is ultimately what we're trying to remove.
I ideally want to remove this method completely and may follow up with another PR, but the method is currently quite useful for some unit tests. I am considering making streamMilestoneBlocks test-only scope but will do in another PR.

# Testing

- [x] Added/modified unit tests to ensure these changes were covered
- [x] 2x sepolia syncs
- [x] RunnerBuilder: run a network through a block number and also timestamp fork to ensure the node record is updated correctly - e.g. forkId should change in peering logs.
- [x] TransitionPoolFactory: Ensure that the BaseFee vs GasPrice sorting order is respected pre/post London and also post-Shanghai. (This is working the same as it was before my change, have asked if it's a bug or not below)
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
cherry-pick and rebase on main of #5183 

The existing implementation of BlockchainQueries gets a worldstate from the worldstatearchive only during the query.  But in case of tracing, several endpoints reference the worldstate indirectly via the updater to generate the response.  This is not a problem for forest mode storage, but bonsai and specifically bonsai snapshot worldstates "close" after use in BlockchainQueries.  

Closing the worldstate after the trace, but before the response has been formed creates a race which can lead to a segfault.  If there is an attempt to access the snapshot worldstate after it has been released (like while generating the trace response) a segfault will occur.  

This PR changes all of the tracing endpoints to keep open a worldstate for the duration of tracing and response generation.  

All of the tracing endpoints are modified:
* trace_get
* trace_transaction
* debug_accountAt
* debug_standardTraceBlockToFile  
* debug_traceTransaction
* trace_block
* trace_callMany
* trace_replayBlockTransactions

* debug_accountRange (not implemented for bonsai)
* debug_storageRangeAt (not implemented for bonsai)
* eth_getProof (not implemented for bonsai)

* debug_traceBlock (times out on mainnet, see #5131)
* debug_traceBlockByHash (times out on mainnet, see #5131)
* debug_traceBlockByNumber (times out on mainnet, see #5131)


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

