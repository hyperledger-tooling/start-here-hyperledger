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
                PR <a href="https://github.com/hyperledger/besu/pull/5326" class=".btn">#5326</a>
            </td>
            <td>
                <b>
                    Add withdrawals to PayloadIdentifier to avoid collisions (#5321)
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
Cherry-pick https://github.com/hyperledger/besu/pull/5321 into the 23.1.3 release.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-11 00:50:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5325" class=".btn">#5325</a>
            </td>
            <td>
                <b>
                    Revert "add register useless response to multiple tasks (#5220)"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit 64efb668c7a4ebf721f7fedd196f98bd0ec0df7a.

## PR description
This reverts a change that can cause us to loose peers. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-11 00:16:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5324" class=".btn">#5324</a>
            </td>
            <td>
                <b>
                    23.1.3 bump
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
bump version and changelog

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-10 23:58:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5323" class=".btn">#5323</a>
            </td>
            <td>
                <b>
                    Prep 23.1.3
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
merge 23.1.2 into release-23.1.x in preparation for 23.1.3 

commits squashed to avoid DCO issues.

`git diff 23.1.2` returns empty.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-10 23:18:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5321" class=".btn">#5321</a>
            </td>
            <td>
                <b>
                    Add withdrawals to PayloadIdentifier to avoid collisions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We have come across a case where certain network conditions cause nimbus to replay an engine_forkchoiceUpdatedV2 (FCU) request with payloadParameters, except with a small change to the Withdrawal amounts (since the validator balances have changed between requests).

This ultimately results in a missed proposal.

No error log present on besu side. Here is the error you would see on nimbus:
```
WRN 2023-04-09 00:59:12.717+00:00 Execution client did not return correct withdrawals topics="beacval" withdrawals_from_cl_len=16 withdrawals_from_el_len=16 

withdrawals_from_cl="@[
(index: 2265686, validator_index: 351739, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1814587), 
(index: 2265687, validator_index: 351740, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1767132), 
(index: 2265688, validator_index: 351741, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1778701), 
(index: 2265689, validator_index: 351742, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1806524), 
(index: 2265690, validator_index: 351743, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1730569), 
(index: 2265691, validator_index: 351744, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1809174), 
(index: 2265692, validator_index: 351745, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1820438), 
(index: 2265693, validator_index: 351746, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1804021), 
(index: 2265694, validator_index: 351747, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1802687), 
(index: 2265695, validator_index: 351748, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1786983), 
(index: 2265696, validator_index: 351749, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1793804), 
(index: 2265697, validator_index: 351750, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1764766), 
(index: 2265698, validator_index: 351751, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1847616), 
(index: 2265699, validator_index: 351752, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1797693), 
(index: 2265700, validator_index: 351753, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1746126), 
(index: 2265701, validator_index: 351754, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1804971)]" 

withdrawals_from_el="@[
(index: 2265686, validator_index: 351739, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1803288), 
(index: 2265687, validator_index: 351740, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1755833), 
(index: 2265688, validator_index: 351741, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1767402), 
(index: 2265689, validator_index: 351742, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1795225), 
(index: 2265690, validator_index: 351743, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1719270), 
(index: 2265691, validator_index: 351744, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1797875), 
(index: 2265692, validator_index: 351745, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1811708), 
(index: 2265693, validator_index: 351746, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1792722), 
(index: 2265694, validator_index: 351747, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1791388), 
(index: 2265695, validator_index: 351748, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1775684), 
(index: 2265696, validator_index: 351749, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1782505), 
(index: 2265697, validator_index: 351750, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1753467), 
(index: 2265698, validator_index: 351751, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1838886), 
(index: 2265699, validator_index: 351752, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1786394), 
(index: 2265700, validator_index: 351753, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1734827), 
(index: 2265701, validator_index: 351754, address: (data: [65, 191, 37, 252, 140, 82, 210, 146, 189, 102, 211, 188, 236, 216, 169, 25, 236, 185, 239, 136]), amount: 1793672)]"

ERR 2023-04-09 00:59:12.727+00:00 Cannot create block for proposal 
```

Here's how besu behaviour leads to this mismatch:
1. Receive FCU(1) with payloadParameter instruction to build a block including withdrawals
2. Generate payloadId from the payloadParameters, caches it and responds with the payloadId to the CL.
3. Receive FCU(2) identical to FCU(1) other than Withdrawal amounts
4. Generate colliding payloadId
5. Find payloadId in the cache so would hit the "Block proposal for the same payload id {} already present, nothing to do" log 6. Respond with the same payloadId to CL.
7. Receive getPayload request relating to FCU(2) and respond with block cached against FCU(1).

Eth R&D Discord thread with more details here: https://discord.com/channels/595666850260713488/892088344438255616/1093963476948496455

Note, I have not noticed any other CL behaving like this, all FCU replays I've seen have the same Withdrawal amounts.

Note geth added withdrawals to payloadId
https://github.com/ethereum/go-ethereum/pull/26554

It appears nethermind may have behave the same as besu and therefore also have this bug (in combination with nimbus):  
https://github.com/NethermindEth/nethermind/blob/4407c97970e4e392d014f5fdfb5f7773244530d4/src/Nethermind/Nethermind.Merge.Plugin/BlockProduction/PayloadPreparationService.cs#L77-L89
https://github.com/NethermindEth/nethermind/blob/e4a91624f63ad9f97cc93762da0969f250ab62fc/src/Nethermind/Nethermind.Merge.Plugin/BlockProduction/PayloadPreparationService.cs#L226-L235

It's not clear from the spec whether FCU(2) should be different to FCU(1) but it seems reasonable for besu to include withdrawals in the payloadId anyway.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-10 10:09:12 +0000 UTC
    </div>
</div>

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
- [x] Snap Sync non-validating node with all public networks
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
add jackson version metadata necessary for some gradle tasks

It isn't clear why circle-ci and docker based builds require these older jackson dependencies.  I tried a few different ways to intercept and remap, but in the end just added the sha256 sums of these older packages into the verification-metadata.  I did confirm they are not leaking into the build artifact, since there are a handful of CVEs for prior jackson versions, e.g.:
https://mvnrepository.com/artifact/com.fasterxml.jackson.core/jackson-databind

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

- [x] next release is 23.4
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

