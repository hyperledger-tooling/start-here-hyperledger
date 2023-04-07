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
                PR <a href="https://github.com/hyperledger/besu/pull/5319" class=".btn">#5319</a>
            </td>
            <td>
                <b>
                    init flat db filling
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
        Created At 2023-04-07 09:22:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5317" class=".btn">#5317</a>
            </td>
            <td>
                <b>
                    TrieLog shipping prep
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
prep bonsai for trielog shipping
add zero reads of slot storage and accounts to bonsai accumulator storageToUpdate and accountsToUpdate

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
protocols-misc 707
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-06 00:51:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5315" class=".btn">#5315</a>
            </td>
            <td>
                <b>
                    Add metrics for accounts and storage reads (Flat databasae vs MPT)
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
The objective of this PR is to introduce 8 new metrics (counters) that will track important aspects of account and storage reads. These metrics will include:

- Total number of calls (for both accounts and storage)
- Number of account or storage entries found in the flat database
- Number of storage slots located in the merkle trie but not found in the flat database
- Number of account or storage entries not found in either the flat database or the merkle trie

The insights provided by these new metrics will be visualized through Grafana graphs, which will enable us to better monitor and analyze the performance of accounts and storage reads. By leveraging these graphs, we can gain a deeper understanding of the state of the flat database, the number of missing entries in Merkle Patricia Trie database and take steps to optimize performance.

It is important to keep in mind that we're not counting here all the calls to the Patricia Merkle Trie for accounts and storage, but we're are counting only 1 for getting the leaf from the trie, which in practice corresponds to several calls.

![image](https://user-images.githubusercontent.com/5099602/230375723-45db64d3-fb57-4059-a55a-89a35c58bbd6.png)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-05 14:47:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5314" class=".btn">#5314</a>
            </td>
            <td>
                <b>
                    Exclude sources and javadoc from dependencies verification to avoid IntelliJ failures
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

Suggested by Gradle project https://docs.gradle.org/6.8.3/userguide/dependency_verification.html#sec:skipping-javadocs 
See also: https://youtrack.jetbrains.com/issue/IDEA-258328

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-05 14:23:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5313" class=".btn">#5313</a>
            </td>
            <td>
                <b>
                    Attempt to fix flaky getBlockByNumberForLatest test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span>
            </td>
            <td>
                Lock down timestamp

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#5296
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-05 04:36:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5312" class=".btn">#5312</a>
            </td>
            <td>
                <b>
                    Configure gradle AT tasks to run junit5 tests
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
Gradle tasks for the acceptance tests were not running any Junit5 tests.

current mainnet tests: 61
with this change mainnet tests: 137

current non-mainnet tests: 271
with this change non-mainnet tests: 279

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #5299 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-05 04:17:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5311" class=".btn">#5311</a>
            </td>
            <td>
                <b>
                    Handle busy exception on fast/snap WS Download process
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
This PR is an attempt to stop the worldstate download pipeline from breaking when RocksDB returns a Status.Busy Exception.
We currently don't handle that scenario and forest does seem to trigger that often.
I suspect Bonsai rarely hits this scenario but it could also leverage from the exception handler.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #5300 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 23:30:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5310" class=".btn">#5310</a>
            </td>
            <td>
                <b>
                    Unified protocol schedule - combine TimestampSchedule and MutableProtocolSchedule
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a necessarily large PR, but it's mostly type removal/renaming/unification changes.
I have added comments to highlight the interesting parts that require closer review.

Currently, one reference test file breaking due to invalid test inputs see https://github.com/hyperledger/besu/pull/5310#issuecomment-1497012579

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

- Combine MutableProtocolSchedule and DefaultTimestampSchedule into `UnifiedProtocolSchedule`. 
- Implement getByBlockHeader taking into account both timestamp-based and blockNumber-based forks
- Unstitch timestampSchedule from TransitionProtocolSchedule
- BftProtocolSchedule extends UnifiedProtocolSchedule (instead of MutableProtocolSchedule)
- [DONE] ~Optimise getByBlockHeader algorithm (once all tests are passing)~
- [TODO next PR] Unify StreamingProtocolSchedules and extend UnifiedProtocolSchedule
- [TODO next PR] Fold AbstractProtocolScheduleBuilder into ProtocolScheduleBuilder
- [TODO next PR] Rename UnifiedProtocolSchedule -> DefaultProtocolSchedule
- [TODO next PR] Tidy up WithdrawalsValidatorProvider


Should end up with this hierarchy:

```
                            ----> PrivacySupportingProtocolSchedule 
                           |
                           | 
                   ProtocolSchedule
                    - public getByBlockHeader
                           ^ 
                           |
         ----->    UnifiedProtocolSchedule  <------ ---------------------------------
        |           - public getByBlockHeader      |                                 |
        |           - private getByTimestamp       |                                 |
        |           - private getByBlockNumber     |                                 |
        |                                          |                                 |
        |                                          |                                 |
BftProtocolSchedule                MilestoneStreamingProtocolSchedule    TransitionProtocolSchedule
 - public getByBlockNumber          - public streamMilestones             - public getByBlockNumber
```

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

#5260

## Testing

- [x] Automated coverage
- [x] Local PoS block production with shanghai-at-genesis using https://github.com/siladu/beku-timestamp
- [x] Local PoS block production with transition from paris -> shanghai  using https://github.com/rolfyone/playground/tree/main/capella/beku
- [x] Local ethash block production
- [x] Local QBFT single-node network byzantium -> berlin -> london -> validator contract mode
- [x] Local IBFT2 single-node network berlin -> london
- [ ] Snap Sync non-validating node with all public networks
- [ ] Full sync goerli?
- [ ] Deploy to validator on testnet (e.g. clc-sepolia)
- [ ] Ensure EVM tool works
- [ ] Performance test? Since getByBlockHeader algorithm has significantly changed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 22:34:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5308" class=".btn">#5308</a>
            </td>
            <td>
                <b>
                    rebase cred trunc behavior
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
trunc sensitive data in trace logging, leaving enough for comparison 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
addresses static analysis alerts 597 and 810

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 19:45:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5305" class=".btn">#5305</a>
            </td>
            <td>
                <b>
                    Env var to debug child processes.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                export BESU_DEBUG_CHILD_PROCESS_PORT=5005 and when running ProcessBesuNodeRunner (i.e. acceptance tests) the child process will suspend and wait for a debugger to attach.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 15:33:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5303" class=".btn">#5303</a>
            </td>
            <td>
                <b>
                    [23.4] Remove GoQuorum privacy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Do not merge until the next release is 23.4
Fixes #4886

- [ ] next release is 23.4
- [x] acceptanceTestsNonMainnet passed in CI
- [ ] Besu with other types of privacy still works as expected

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 08:23:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5302" class=".btn">#5302</a>
            </td>
            <td>
                <b>
                    [23.4] Remove IBFT1 consensus mechanism
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This feature has been deprecated and is being removed in 23.4 (that is - do not merge until all other releases have been completed and 23.4 is the next release)

Fixes #4922 

- [ ] next release is 23.4
- [x] acceptanceTestsNonMainnet passed in CI
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 02:33:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5301" class=".btn">#5301</a>
            </td>
            <td>
                <b>
                    Ethstat retry fix
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
Fix ethstats retry logic. Attempt to connect with and without ssl. If `--ethstats` is specified without a port, use port 443 (for wss://) and port 80 (for ws://) as defaults instead of 3000. This will help in k8 or similar environment where ethstats is running behind a reverse proxy.

Introduced optional `--ethstats-cacert-file`. This option specifies the path to the root CA (Certificate Authority) certificate file that has signed ethstats server certificate (or reverse proxy certificate). This option is optional. Useful in non-production setup.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#4696 
Potentially #3792 

## Local Testing
https://github.com/usmansaleem/ethstats-proxy
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 01:07:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5295" class=".btn">#5295</a>
            </td>
            <td>
                <b>
                     EIP-6110: Add deposit validation and apis
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span><span class="chip">EIP</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Add deposit validation and related apis.
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#5004 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 04:47:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5294" class=".btn">#5294</a>
            </td>
            <td>
                <b>
                    BFT acceptance tests for Berlin and London
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
Add acceptance tests for IBFT2 and QBFT for the Berlin and London forks.

* Update the ibft and qbft genesis configs to use berlin as the default instead byzantium
* Add tests for Berlin fork with gas and without gas
* Add tests for London fork with gas and without gas including using Frontier and EIP-1559 transactions
* Changed the DSL to make it clearer when we are using EIP-1559 transactions
* Added support in DSL to do transfers with a gas price

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #5282 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 03:51:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5292" class=".btn">#5292</a>
            </td>
            <td>
                <b>
                    Use cached header for latest eth_getBlockByNumber
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span>
            </td>
            <td>
                While syncing, it is possible that we access the cached header's number before the block itself has had chance to be imported. In other words there is a mismatch between cached blockNumber and non-cached blockHeader that is being retrieved for the RPC.

Discovered after adding debug in https://github.com/hyperledger/besu/pull/5288

## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/5281

## Testing

Tested X_SNAP with each CL on sepolia as well as nimbus on goerli.
Without the fix: prysm, lighthouse and nimbus received the error (see https://github.com/hyperledger/besu/issues/5281#issuecomment-1491753557).
With the fix: no errors
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-02 01:45:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5291" class=".btn">#5291</a>
            </td>
            <td>
                <b>
                    For PoS, use extraData that was configured in the miner-extra-data cli option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span>
            </td>
            <td>
                This was hardcoded to "0x" as part of The Merge implementation. 

Fixes https://github.com/hyperledger/besu/issues/4471

Tested locally with https://github.com/siladu/beku-timestamp
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-01 05:22:45 +0000 UTC
    </div>
</div>

