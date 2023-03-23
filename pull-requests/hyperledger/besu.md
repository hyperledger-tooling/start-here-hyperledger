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
                PR <a href="https://github.com/hyperledger/besu/pull/5259" class=".btn">#5259</a>
            </td>
            <td>
                <b>
                    getByBlockNumber replaced by getByBlockHeader on tests
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
This PR removes the getByBlockNumber from tests and replace it's usage by getByBlockHeader.

## Fixed Issue(s)
Fixes #5165 
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-23 04:36:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5258" class=".btn">#5258</a>
            </td>
            <td>
                <b>
                    update snakeyaml to 2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Update snakeyaml dependency
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-23 04:24:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5257" class=".btn">#5257</a>
            </td>
            <td>
                <b>
                    additional merkle trie refactoring
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
additional refactoring missed by #5251 
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-22 23:37:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5256" class=".btn">#5256</a>
            </td>
            <td>
                <b>
                    fence repolinter docker action
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
restrict docker based github actions to specific self-hosted runners to prevent docker user from poisoning the filesystem permissions

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-22 18:04:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5255" class=".btn">#5255</a>
            </td>
            <td>
                <b>
                    Plugin API - Add Trace Service to the Plugin API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span><span class="chip">plugins</span>
            </td>
            <td>
                ## PR description
Plugin API - Add Trace Service to the Plugin API

- Allow users to trace a block using a custom operation tracer instance.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-22 03:20:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5254" class=".btn">#5254</a>
            </td>
            <td>
                <b>
                    Isolate bft getByBlockNumber
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                Fixes #5162 and #5164 

Introduce BftProtocolSchedule with a copy of MutableProtocolSchedule.getByBlockNumber
This method will be deleted from the ProtocolSchedule interfaces and so will only exist in BftProtocolSchedule (although it may be renamed in a subsequent commit).

Rename existing *BftProtocolSchedule classes to append Builder for clarity (and inline with other ProtocolScheduleBuilder classes)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-22 01:42:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5253" class=".btn">#5253</a>
            </td>
            <td>
                <b>
                    Cleanup after GHA docker user
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
Docker actions that write to files during actions leave files in the repository owned by the docker user rather than the runner user.  This leaves the runner filesystem in a state that makes non-docker actions fail.  

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-22 00:37:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5252" class=".btn">#5252</a>
            </td>
            <td>
                <b>
                    [MINOR] Add unstable annotation to the BlockchainService
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">plugins</span>
            </td>
            <td>
                ## PR description
Add unstable annotation to the BlockchainService
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-21 23:56:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5251" class=".btn">#5251</a>
            </td>
            <td>
                <b>
                    Merkle trie radix abstraction
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

Abstract the MerklePatriciaTrie to support tries with a different radix


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-21 23:19:10 +0000 UTC
    </div>
</div>

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
                <span class="chip">mainnet</span><span class="chip">peering</span>
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

