---
layout: default
title: besu
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    GHA.TESTRUN.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    GHA.TESTRUN.1
                </span>
            </td>
            <td>
                ## What's Changed
* prep for release 24.1.1 by @macfarla in https://github.com/hyperledger/besu/pull/6432
* Use `From` field in a `PING` packet when creating a peer table entry by @matthew1001 in https://github.com/hyperledger/besu/pull/6225
* Only accept an address from a peer if it is a valid IP address by @matthew1001 in https://github.com/hyperledger/besu/pull/6439
* Fix changelog after incorrect merge of 6225 by @matthew1001 in https://github.com/hyperledger/besu/pull/6438
* Import export trie log by @gfukushima in https://github.com/hyperledger/besu/pull/6363
* Make fork id the default and try to recover the DiscoveryPeer for incoming connections from the PeerTable by @pinges in https://github.com/hyperledger/besu/pull/5628
* Addition of Profile Configuration CLI Option by @Gabriel-Trintinalia in https://github.com/hyperledger/besu/pull/6418
* Trie log prune using TrieLogEvent by @gfukushima in https://github.com/hyperledger/besu/pull/6394
* Reuse --bonsai-historical-block-limit for limit trie logs feature by @siladu in https://github.com/hyperledger/besu/pull/6445
* feat: add `OperationTracer.tracePrepareTransaction` by @delehef in https://github.com/hyperledger/besu/pull/6453
* use reference tests to verify trielog generation by @matkt in https://github.com/hyperledger/besu/pull/6415
* Add broadcast address to PingPacketData from filter by @garyschulte in https://github.com/hyperledger/besu/pull/6456
* silence dns query error warning by @garyschulte in https://github.com/hyperledger/besu/pull/6458
* ignore bws sync requests until initial sync is complete by @garyschulte in https://github.com/hyperledger/besu/pull/6455
* Enable limit on range Of JSON-RPC API trace_filter method (#5971) by @alyokaz in https://github.com/hyperledger/besu/pull/6446
* Snap sync downloader logging by @macfarla in https://github.com/hyperledger/besu/pull/6403
* [Refactor] - Extract websocket options to a new class by @Gabriel-Trintinalia in https://github.com/hyperledger/besu/pull/6461
* Skip pruning if trie log count is less than retention limit by @siladu in https://github.com/hyperledger/besu/pull/6463
* Fix `poa-block-txs-selection-max-time` option that was inadvertently reset to its default after being configured by @fab-10 in https://github.com/hyperledger/besu/pull/6444
* Log blob count when importing a block via Engine API by @fab-10 in https://github.com/hyperledger/besu/pull/6466
* Fix 24.1.1 changelog by @garyschulte in https://github.com/hyperledger/besu/pull/6468
* [CHANGELOG] updated download links and added contributor thanks by @macfarla in https://github.com/hyperledger/besu/pull/6477
* remove repeated part of toString() by @pinges in https://github.com/hyperledger/besu/pull/6480
* [Refactor] - Extract JsonRpcHttpOptions to a new class  by @Gabriel-Trintinalia in https://github.com/hyperledger/besu/pull/6478
* Write a DEBUG log entry to make it clear of a BFT node is a validator… by @matthew1001 in https://github.com/hyperledger/besu/pull/6470
* Fix typos by @Thabokani in https://github.com/hyperledger/besu/pull/6481
* filter empty ipv4 and ipv6 ping packet source addresses by @garyschulte in https://github.com/hyperledger/besu/pull/6474
* [Refactor ] Move permission options to its own class by @Gabriel-Trintinalia in https://github.com/hyperledger/besu/pull/6490
* Remove `--engine-jwt-enabled` deprecated option by @Gabriel-Trintinalia in https://github.com/hyperledger/besu/pull/6491
* Backward Sync, reduce retries from 20 to 2 by @pinges in https://github.com/hyperledger/besu/pull/6482
* Upgrade Prometheus and Opentelemetry dependencies by @fab-10 in https://github.com/hyperledger/besu/pull/6422
* Implement "pending" for qbft_getValidatorsByBlockNumber by @matthew1001 in https://github.com/hyperledger/besu/pull/6436
* Delete development artifacts by @shemnon in https://github.com/hyperledger/besu/pull/6487
* Add pragueTime configuration by @shemnon in https://github.com/hyperledger/besu/pull/6473
* Optimized Keccak Hashing for Account Storage Slots by @matkt in https://github.com/hyperledger/besu/pull/6452
* info level log for pipeline abort by @garyschulte in https://github.com/hyperledger/besu/pull/6459
* [Refactor] Move graphqloptions to its own class by @Gabriel-Trintinalia in https://github.com/hyperledger/besu/pull/6496
* Code storage by hash by @jframe in https://github.com/hyperledger/besu/pull/5889
* [MINOR] remove duplicate setting of default values for CLI options by @macfarla in https://github.com/hyperledger/besu/pull/6500
* standardize on length of truncated peer ID logging by @macfarla in https://github.com/hyperledger/besu/pull/6485
* Filter Discovered peers for ipv6 support by @garyschulte in https://github.com/hyperledger/besu/pull/6498
* Disconnect worst peer by @pinges in https://github.com/hyperledger/besu/pull/6443
* add sync condition for privacy tests by @macfarla in https://github.com/hyperledger/besu/pull/6479
* Revert "Bonsai code storage by hash (#5889)" by @jframe in https://github.com/hyperledger/besu/pull/6504
* Store trielog as blobdb by @usmansaleem in https://github.com/hyperledger/besu/pull/6289
* GitHub Actions CI/CD by @jflo in https://github.com/hyperledger/besu/pull/6427
* Test that peers are not disconnected in `RetryingSwitchingPeerMessageTaskTest::failsWhenAllPeersFail by @fab-10 in https://github.com/hyperledger/besu/pull/6508
* Flat db heal - deprecate CLI option and set to always true by @macfarla in https://github.com/hyperledger/besu/pull/6499
* Report estimated disk space freed up by x-trie-log prune subcommand by @siladu in https://github.com/hyperledger/besu/pull/6483
* [Refactor] Move api options to its own class by @Gabriel-Trintinalia in https://github.com/hyperledger/besu/pull/6512
* Add minimalist staker profile by @Gabriel-Trintinalia in https://github.com/hyperledger/besu/pull/6449

## New Contributors
* @alyokaz made their first contribution in https://github.com/hyperledger/besu/pull/6446

**Full Changelog**: https://github.com/hyperledger/besu/compare/24.1.1...GHA.TESTRUN.1
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/GHA.TESTRUN.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-02-01 08:36:11 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Release 24.1.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    24.1.1
                </span>
            </td>
            <td>
                ## 24.1.1

### Breaking Changes
- New `EXECUTION_HALTED` error returned if there is an error executing or simulating a transaction, with the reason for execution being halted. Replaces the generic `INTERNAL_ERROR` return code in certain cases which some applications may be checking for [#6343](https://github.com/hyperledger/besu/pull/6343)
- The Besu Docker images with `openjdk-latest` tags since 23.10.3 were incorrectly using UID 1001 instead of 1000 for the container's `besu` user. The user now uses 1000 again. Containers created from or migrated to images using UID 1001 will need to chown their persistent database files to UID 1000 [#6360](https://github.com/hyperledger/besu/pull/6360) - thanks @h4l 
- The deprecated `--privacy-onchain-groups-enabled` option has now been removed. Use the `--privacy-flexible-groups-enabled` option instead. [#6411](https://github.com/hyperledger/besu/pull/6411)
- The time that can be spent selecting transactions during block creation is not capped at 5 seconds for PoS and PoW networks, and for PoA networks, at 75% of the block period specified in the genesis, this to prevent possible DoS in case a single transaction is taking too long to execute, and to have a stable block production rate, but it could be a breaking change if an existing network used to have transactions that takes more time to executed that the newly introduced limit, if it is mandatory for these network to keep processing these long processing transaction, then the default value of `block-txs-selection-max-time` or `poa-block-txs-selection-max-time` needs to be tuned accordingly. [#6423](https://github.com/hyperledger/besu/pull/6423)

### Deprecations

### Additions and Improvements
- Optimize RocksDB WAL files, allows for faster restart and a more linear disk space utilization [#6328](https://github.com/hyperledger/besu/pull/6328)
- Disable transaction handling when the node is not in sync, to avoid unnecessary transaction validation work [#6302](https://github.com/hyperledger/besu/pull/6302)
- Introduce TransactionEvaluationContext to pass data between transaction selectors and plugin, during block creation [#6381](https://github.com/hyperledger/besu/pull/6381)
- Upgrade dependencies [#6377](https://github.com/hyperledger/besu/pull/6377)
- Upgrade `com.fasterxml.jackson` dependencies [#6378](https://github.com/hyperledger/besu/pull/6378)
- Upgrade Guava dependency [#6396](https://github.com/hyperledger/besu/pull/6396)
- Upgrade Mockito [#6397](https://github.com/hyperledger/besu/pull/6397)
- Upgrade `tech.pegasys.discovery:discovery` [#6414](https://github.com/hyperledger/besu/pull/6414)
- Options to tune the max allowed time that can be spent selecting transactions during block creation are now stable [#6423](https://github.com/hyperledger/besu/pull/6423)

### Bug fixes
- INTERNAL_ERROR from `eth_estimateGas` JSON/RPC calls [#6344](https://github.com/hyperledger/besu/issues/6344)
- Fix Besu Docker images with `openjdk-latest` tags since 23.10.3 using UID 1001 instead of 1000 for the `besu` user [#6360](https://github.com/hyperledger/besu/pull/6360) - thanks @h4l 
- Fluent EVM API definition for Tangerine Whistle had incorrect code size validation configured [#6382](https://github.com/hyperledger/besu/pull/6382)
- Correct mining beneficiary for Clique networks in TraceServiceImpl [#6390](https://github.com/hyperledger/besu/pull/6390)
- Fix to gas limit delta calculations used in block production. Besu should now increment or decrement the block gas limit towards its target correctly (thanks @arbora) #6425
- Ensure Backward Sync waits for initial sync before starting a session [#6455](https://github.com/hyperledger/besu/issues/6455)
- Silence the noisy DNS query errors [#6458](https://github.com/hyperledger/besu/issues/6458)

### Download Links
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/24.1.1/besu-24.1.1.zip / sha256 e23c5b790180756964a70dcdd575ee2ed2c2efa79af00bce956d23bd2f7dc67c
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/24.1.1/besu-24.1.1.tar.gz / sha256 4b0ddd5a25be2df5d2324bff935785eb63e4e3a5f421614ea690bacb5b9cb344

### Errata
Note, due to a CI race with the release job, the initial published version of 24.1.1 were overwritten by artifacts generated from the same sources, but differ in their embedded timestamps.  The initial SHAs are noted here but are deprecated:
~~https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/24.1.1/besu-24.1.1.zip / sha256 b6b64f939e0bb4937ce90fc647e0a7073ce3e359c10352b502059955070a60c6~~
~~https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/24.1.1/besu-24.1.1.tar.gz / sha256 cfcae04c30769bf338b0740ac65870f9346d3469931bb46cdba3b2f65d311e7a~~

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/24.1.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-01-26 01:04:20 +0000 UTC
    </span>
</div>

