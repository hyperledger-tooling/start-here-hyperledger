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
1c888a1b30bc205272a80cc074b185813e625e470a1f74003ac25165f89ed4d6  besu-GHA.TESTRUN.1.tar.gz
72af7ba6ed20635229bb3fe43db6d14e17238127df9110608b7a0ef12a571529  besu-GHA.TESTRUN.1.zip

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

