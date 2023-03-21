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
                PR <a href="https://github.com/hyperledger/besu/pull/5250" class=".btn">#5250</a>
            </td>
            <td>
                <b>
                    Fix Blockchain Plugin service javadoc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Fix missing comments for javadoc

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-21 08:12:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5248" class=".btn">#5248</a>
            </td>
            <td>
                <b>
                    Add plugin RPC exception type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">plugins</span><span class="chip">RPC</span>
            </td>
            <td>
                ## PR description
Add Plugin RPC Exception type

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-21 05:01:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5247" class=".btn">#5247</a>
            </td>
            <td>
                <b>
                    Plugin API -  Blockchain Service 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">plugins</span>
            </td>
            <td>
                ## PR description
Introduces a new feature to the plugin API, enabling third-party plugins to access the blockchain service and retrieve information about a specific block based on its number.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-21 02:10:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5245" class=".btn">#5245</a>
            </td>
            <td>
                <b>
                    use tags compatible with github runners
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
revert GHA tags to ones that will trigger with github runners, also tag jobs which require x86 architecture with 'x64'

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-20 21:47:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5244" class=".btn">#5244</a>
            </td>
            <td>
                <b>
                    Metrics via dagger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Introduces Dagger to provide dependencies.  

- Migrates an existing MetricsSystem module up into the metrics gradle module.
- Makes BesuCommand accessible from Dagger components, to enable configuration reuse.
- Uses CachedMerkleTrieLoader as an example of how to get and use a MetricSystem.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-20 21:35:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5242" class=".btn">#5242</a>
            </td>
            <td>
                <b>
                    change the way to count peers to make it the same as in 4759
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
        Created At 2023-03-20 09:57:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5241" class=".btn">#5241</a>
            </td>
            <td>
                <b>
                    Invalid params data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added `data` to error in case of INVALID_PARAMS to give users more info as to what's gone wrong

See #4212 - possible solution to #5098

Not sure if this will break some hive tests?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-20 03:08:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5240" class=".btn">#5240</a>
            </td>
            <td>
                <b>
                    Move protocol schedule streamMilestoneBlocks into test scope
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span>
            </td>
            <td>
                It's now only used by the tests following removal of production code paths in https://github.com/hyperledger/besu/commit/08b822a860cd12133fcfa53d6ff0057bc03d56f8 A simple decorater would have been a nicer implementation but I didn't want to expose the protocolSpecs from within the schedule hence why I've used inheritance.

ForksIdsNetworkConfigTest has a particularly hairy construction since it relies on TransitionProtocolSchedule but I've isolated this as an inner class. I am hopeful that we can refactor ForksIdsNetworkConfigTest out of existance eventually and avoid using streamMilestoneBlocks at the same time.

Furthermore, the end goal is have a unified schedule that can handle milestone as blockNumber or timestamp, so we won't need two versions of things such as TimestampStreamingProtocolSchedule
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-20 01:56:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5239" class=".btn">#5239</a>
            </td>
            <td>
                <b>
                    Extract tests for Schedule out of the ScheduleBuilder tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-19 21:21:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5238" class=".btn">#5238</a>
            </td>
            <td>
                <b>
                    Minor improvements to logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span><span class="chip">logging</span>
            </td>
            <td>
                * During startup print "Besu version ..." instead of just "Besu ..." to make searching for the version in the logs easier.

* eth_getLogs now prints request along with exception:
```
2023-03-20 12:42:17.918+10:00 | Test worker | DEBUG  | EthGetLogs | eth_getLogs request JsonRpcRequest{id=null, method='eth_getLogs', params=[FilterParameter{fromBlock=BlockParameter{type=NUMERIC, number=Optional[0]}, toBlock=BlockParameter{type=NUMERIC, number=Optional[50]}, fromAddress=[], toAddress=[], addresses=[], topics=[], maybeBlockHash=Optional.empty, logsQuery=LogsQuery{addresses=[], topics=[], after=Optional.empty, count=Optional.empty, isValid=true}], version='2.0', isNotification=true} failed
java.lang.IllegalArgumentException: Requested range exceeds maximum range limit
	at org.hyperledger.besu.ethereum.api.jsonrpc.internal.methods.EthGetLogs.lambda$response$3(EthGetLogs.java:90) ~[main/:?]
	at java.util.Optional.orElseGet(Optional.java:364) ~[?:?]
	at org.hyperledger.besu.ethereum.api.jsonrpc.internal.methods.EthGetLogs.response(EthGetLogs.java:70) ~[main/:?]
	...
```

* Better formatting of the fast sync retry interval: Instead of printing
```
ERROR | FastSyncDownloader | Encountered an unexpected error during fast sync. Restarting sync in PT5S seconds.
```
we now print:
```
ERROR | FastSyncDownloader | Encountered an unexpected error during fast sync. Restarting sync in 5 seconds.
```


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-19 20:40:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5237" class=".btn">#5237</a>
            </td>
            <td>
                <b>
                    Prepare for version 23.1.3-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prepare for version 23.1.3-SNAPSHOT
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-18 03:56:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5236" class=".btn">#5236</a>
            </td>
            <td>
                <b>
                    Release 23.1.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 23.1.2
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-18 03:08:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5235" class=".btn">#5235</a>
            </td>
            <td>
                <b>
                    use x86 for codeQL github action
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
A few  github actions explicitly uses amd64 binary version of java.  needs to specify they can only run on X64:
- codeql
- spotless
- javadoc_17

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-18 01:14:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5234" class=".btn">#5234</a>
            </td>
            <td>
                <b>
                    Mainnet AT reduce parallelism and self-hosted runners
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
same as #5232 but with additional self-hosted runner config 


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-17 23:11:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5233" class=".btn">#5233</a>
            </td>
            <td>
                <b>
                    [GHA] actions not required on merge group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Don't run not-required actions on merge_group
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-17 08:57:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5230" class=".btn">#5230</a>
            </td>
            <td>
                <b>
                    Schedule shanghaiTime for Mainnet and configure forkId for tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                🦉 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-16 19:27:58 +0000 UTC
    </div>
</div>

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
Replace usages of ProtocolSchedule.getForBlockNumber that are being used for the next block by adding a getForNextBlockHeader method.

* Adds a getForNextBlockHeader method to the HeaderBasedProtocolSchedule
* Fixes a bug using the UnsignedIntParameter in RPC methods, this was causing the eth_feeHistory RPC to fail 

### Testing
- [x] Sync on Goerli
- [ ] Sync on mainnet
- [x] Besu and Teku on a local interop network using Shanghai
- [x] QBFT single validator node
- [x] EthHash single node
- [x] Manual testing of the eth_feeHistory

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #5159 

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

