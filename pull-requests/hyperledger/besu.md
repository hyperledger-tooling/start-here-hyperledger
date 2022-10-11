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
                PR <a href="https://github.com/hyperledger/besu/pull/4513" class=".btn">#4513</a>
            </td>
            <td>
                <b>
                    Corrected eth_getLogs default fromBlock value.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span><span class="chip">RPC</span>
            </td>
            <td>
                Signed-off-by: mark-terry <mark.terry@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Changes the default ```fromBlock``` value in ```eth_getLogs``` from ```earliest``` to ```latest``` per the spec.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #4123 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-10 15:12:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4510" class=".btn">#4510</a>
            </td>
            <td>
                <b>
                    RPC parameter error improvements. Test updates.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span><span class="chip">logging</span><span class="chip">RPC</span>
            </td>
            <td>
                Signed-off-by: mark-terry <mark.terry@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Increase level of detail in RPC parameter error logging to improve usability.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #4326 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-10 12:40:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4508" class=".btn">#4508</a>
            </td>
            <td>
                <b>
                    Reduce the number of runtime exceptions (SecurityModuleException)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
During handshake, flip the encrypted message decryption by starting with the new format (EIP-8), and if there is an exception, try the old format. This will reduce the number of exceptions and unnecessary executions.

I noticed by adding some debug logs that on 4400 calls to ECIESHandshaker.handleMessage, there're only 7 cases where the encrypted message has the old format.
<img width="1263" alt="image" src="https://user-images.githubusercontent.com/5099602/194858040-c017f3ab-da50-4c5b-9f54-674d9e7b0c32.png">

By changing the order of execution, starting by decoding the new format (eip8) and without resetting the logs, we can notice  there're no more exceptions

<img width="1263" alt="image" src="https://user-images.githubusercontent.com/5099602/194858841-a730ae13-d550-40b5-b38e-5ad446cd77dd.png">

There is one case I'm not sure about it : if (buf.writerIndex() < size), do we need to try to decode with the old format or we should just throw HandshakeException. With the current PR, HandshakeException will be caught and the old format decryption will be executed.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-10 11:50:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4501" class=".btn">#4501</a>
            </td>
            <td>
                <b>
                    hide deprecated option tx-pool-max-hashes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <macfarla.github@gmail.com>

Deprecated since 22.1.3 https://github.com/hyperledger/besu/blob/main/CHANGELOG.md#2213

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-10 00:30:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4499" class=".btn">#4499</a>
            </td>
            <td>
                <b>
                    update changelog for 22.7.6
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
update changelog for 22.7.6

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-07 23:50:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4498" class=".btn">#4498</a>
            </td>
            <td>
                <b>
                    Update cherry-pick version for 22.7.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
update cherry-pick version to 22.7.6

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-07 22:54:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4497" class=".btn">#4497</a>
            </td>
            <td>
                <b>
                    Log receipts reorg
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                ## PR description

re-emits correct blockadded event on chain rewind during reorgs.

## Fixed Issue(s)
 
fixes #4495


## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-07 20:35:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4494" class=".btn">#4494</a>
            </td>
            <td>
                <b>
                    update changelog for 22.10.0-RC2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
prep 22.10.0-RC2
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-07 00:34:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4493" class=".btn">#4493</a>
            </td>
            <td>
                <b>
                    Prepare for version 22.10.0-RC2-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prepare for version 22.10.0-RC2-SNAPSHOT
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-06 23:54:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4492" class=".btn">#4492</a>
            </td>
            <td>
                <b>
                    Release 22.10.0-RC1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 22.10.0-RC1
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-06 23:08:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4489" class=".btn">#4489</a>
            </td>
            <td>
                <b>
                    The block variable was keeping too much memory while waiting for future to finish
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                
The `exceptionally` was holding a pointer to a block and was not released for potentially long time. 

Signed-off-by: Jiri Peinlich <jiri.peinlich@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-06 16:27:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4488" class=".btn">#4488</a>
            </td>
            <td>
                <b>
                    Optimize pivot block selector on PoS networks 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span><span class="chip">mainnet</span><span class="chip">syncing</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

This PR is built on top of #4487 so check it first

This is the 3rd PR of a series to optimize the initial sync on PoS networks, that is ongoing here https://github.com/hyperledger/besu/pull/4462, but since it is quite big, I am splitting it in smaller PRs to simplify the code review.


On PoS network we use as pivot block, the last finalized block sent by the Consensus Layer, so we do
not need peers, and so all the logic for selecting the pivot block from peers
has been moved from `FastSyncActions` to `PivotSelectorFromPeers`.
We do not need anymore the `TransictionPeerSelector`, and the `--fast-sync-min-peers`
applies only to PoW networks.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-06 13:08:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4487" class=".btn">#4487</a>
            </td>
            <td>
                <b>
                    Refactor unverified forkchoice event
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Renaming to make clear everywhere that the forkchoice is not verified, so it will be clear in case there will be a future event for a verified forkchoice. Finalized block hash no more optional.

Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
This is the 2nd PR of a series to optimize the initial sync on PoS networks, that is ongoing here https://github.com/hyperledger/besu/pull/4462, but since it is quite big, I am splitting it in smaller PRs to simplify the code review.

This is mostly a refactoring to make clear everywhere that the forkchoice is not verified, so
in case there will be a future event for a verified forkchoice it will be simpler.
Then the finalized block hash is no more optional, making the code more simple.
The order of hashes is always heah, safe, finalized.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-06 11:12:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4486" class=".btn">#4486</a>
            </td>
            <td>
                <b>
                    Improve UX of initial sync logs, pushing not relevant logs to debug l…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">logging</span>
            </td>
            <td>
                …evel

Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

This is the first PR of a series to optimize the initial sync on PoS networks, that is ongoing here https://github.com/hyperledger/besu/pull/4462, but since it is quite big, I am splitting it in smaller PRs to simplify the code review.

Initial sync logs are not always easy to read, because instead of having only the sync updates, there are also other logs that are not relevant during the initial sync, and looking at user reports, they can be confused and do not get if the sync is progressing or not

This PR only keeps the logs relevant to the initial sync progress at info and push at debug all the others.

Below logs before and after the PR

Before
```
{"@timestamp":"2022-10-06T09:25:49,947","level":"INFO","thread":"ForkJoinPool.commonPool-worker-5","class":"BackwardsSyncAlgorithm","message":"Waiting for preconditions...","throwable":""}
{"@timestamp":"2022-10-06T09:26:12,086","level":"INFO","thread":"EthScheduler-Services-90 (importBlock)","class":"FastImportBlocksStep","message":"Completed importing chain segment 11279689 to 11280888 (1200 blocks in 11920ms), Peers: 25","throwable":""}
{"@timestamp":"2022-10-06T09:26:35,707","level":"INFO","thread":"vert.x-worker-thread-0","class":"EngineForkchoiceUpdated","message":"SYNCING for fork-choice-update: head: 0x9e8bcadc5bf45225603a0a499179053c0686c1e8428fa04738a5645abe2b10d2, finalized: 0x892379f25213ade77ec1964a45940c5019d36556713b86f9454b3ace8fbdb1a1, safeBlockHash: 0x0d6dc3205963d193b2e18699e46e3ff0879f5a9f1800b1ba7eb7e731702ccb8e","throwable":""}
{"@timestamp":"2022-10-06T09:27:36,261","level":"INFO","thread":"vert.x-worker-thread-0","class":"EngineForkchoiceUpdated","message":"SYNCING for fork-choice-update: head: 0xd7757feee22c7fc9ebdce097a2b51f304c16727b9d4ae3053e6da5a664c465ac, finalized: 0x0d6dc3205963d193b2e18699e46e3ff0879f5a9f1800b1ba7eb7e731702ccb8e, safeBlockHash: 0x618656c42fa3136023ca782cde049c77ba1971eb5b3a56a84177d4f7401d939f","throwable":""}
{"@timestamp":"2022-10-06T09:27:49,947","level":"INFO","thread":"ForkJoinPool.commonPool-worker-5","class":"BackwardsSyncAlgorithm","message":"Waiting for preconditions...","throwable":""}
{"@timestamp":"2022-10-06T09:28:36,398","level":"INFO","thread":"vert.x-worker-thread-0","class":"EngineForkchoiceUpdated","message":"SYNCING for fork-choice-update: head: 0x3ad9b6189f29cf62e97106bbf4c678c76507e806744afdb5282fa35896dd8654, finalized: 0x0d6dc3205963d193b2e18699e46e3ff0879f5a9f1800b1ba7eb7e731702ccb8e, safeBlockHash: 0x618656c42fa3136023ca782cde049c77ba1971eb5b3a56a84177d4f7401d939f","throwable":""}
{"@timestamp":"2022-10-06T09:28:50,005","level":"INFO","thread":"EthScheduler-Services-3 (batchPersistAccountData)","class":"SnapsyncMetricsManager","message":"Worldstate download in progress synced=17.98%, accounts=32928267, slots=217186625, codes=4379638, nodes=239266039","throwable":""}
{"@timestamp":"2022-10-06T09:29:05,775","level":"INFO","thread":"EthScheduler-Services-90 (importBlock)","class":"FastImportBlocksStep","message":"Completed importing chain segment 11282089 to 11282888 (800 blocks in 11643ms), Peers: 25","throwable":""}
{"@timestamp":"2022-10-06T09:29:21,798","level":"INFO","thread":"EthScheduler-Services-90 (importBlock)","class":"FastImportBlocksStep","message":"Completed importing chain segment 11282889 to 11284088 (1200 blocks in 11213ms), Peers: 25","throwable":""}
{"@timestamp":"2022-10-06T09:29:36,466","level":"INFO","thread":"vert.x-worker-thread-0","class":"EngineForkchoiceUpdated","message":"SYNCING for fork-choice-update: head: 0x0198ba0940d1ef58602e8f22a349f2f522042b2625c60c7dd11e8be96bee6a35, finalized: 0x0d6dc3205963d193b2e18699e46e3ff0879f5a9f1800b1ba7eb7e731702ccb8e, safeBlockHash: 0x618656c42fa3136023ca782cde049c77ba1971eb5b3a56a84177d4f7401d939f","throwable":""}
{"@timestamp":"2022-10-06T09:29:44,753","level":"INFO","thread":"EthScheduler-Services-90 (importBlock)","class":"FastImportBlocksStep","message":"Completed importing chain segment 11284089 to 11285088 (1000 blocks in 11715ms), Peers: 25","throwable":""}
{"@timestamp":"2022-10-06T09:29:49,948","level":"INFO","thread":"ForkJoinPool.commonPool-worker-5","class":"BackwardsSyncAlgorithm","message":"Waiting for preconditions...","throwable":""}
{"@timestamp":"2022-10-06T09:29:56,197","level":"INFO","thread":"EthScheduler-Services-90 (importBlock)","class":"FastImportBlocksStep","message":"Completed importing chain segment 11285089 to 11286288 (1200 blocks in 11441ms), Peers: 25","throwable":""}
{"@timestamp":"2022-10-06T09:30:06,166","level":"INFO","thread":"EthScheduler-Services-3 (batchPersistAccountData)","class":"SnapsyncMetricsManager","message":"Worldstate download in progress synced=18.06%, accounts=33082540, slots=217671580, codes=4403571, nodes=239998416","throwable":""}
{"@timestamp":"2022-10-06T09:30:15,109","level":"INFO","thread":"EthScheduler-Services-90 (importBlock)","class":"FastImportBlocksStep","message":"Completed importing chain segment 11286289 to 11286888 (600 blocks in 11245ms), Peers: 25","throwable":""}
{"@timestamp":"2022-10-06T09:30:47,571","level":"INFO","thread":"vert.x-worker-thread-0","class":"EngineForkchoiceUpdated","message":"SYNCING for fork-choice-update: head: 0x95a791258cf96def7e8e19f432645c645bcf8091c9b1f2cc0ab3abc98da69bc7, finalized: 0x0d6dc3205963d193b2e18699e46e3ff0879f5a9f1800b1ba7eb7e731702ccb8e, safeBlockHash: 0x618656c42fa3136023ca782cde049c77ba1971eb5b3a56a84177d4f7401d939f","throwable":""}
{"@timestamp":"2022-10-06T09:31:15,092","level":"INFO","thread":"EthScheduler-Services-3 (batchPersistAccountData)","class":"SnapsyncMetricsManager","message":"Worldstate download in progress synced=18.33%, accounts=33576771, slots=220443622, codes=4469443, nodes=242939929","throwable":""}
{"@timestamp":"2022-10-06T09:31:47,894","level":"INFO","thread":"vert.x-worker-thread-0","class":"EngineForkchoiceUpdated","message":"SYNCING for fork-choice-update: head: 0x53fd3276724e230f9c6a9a38b65e65baa5013addbeea0653ef606b40fd996cf6, finalized: 0x0d6dc3205963d193b2e18699e46e3ff0879f5a9f1800b1ba7eb7e731702ccb8e, safeBlockHash: 0x618656c42fa3136023ca782cde049c77ba1971eb5b3a56a84177d4f7401d939f","throwable":""}
{"@timestamp":"2022-10-06T09:31:49,948","level":"INFO","thread":"ForkJoinPool.commonPool-worker-5","class":"BackwardsSyncAlgorithm","message":"Waiting for preconditions...","throwable":""}
{"@timestamp":"2022-10-06T09:32:07,387","level":"INFO","thread":"EthScheduler-Services-91 (importBlock)","class":"FastImportBlocksStep","message":"Completed importing chain segment 11287689 to 11288288 (600 blocks in 12429ms), Peers: 25","throwable":""}
{"@timestamp":"2022-10-06T09:32:18,464","level":"INFO","thread":"EthScheduler-Services-3 (batchPersistAccountData)","class":"SnapsyncMetricsManager","message":"Worldstate download in progress synced=18.75%, accounts=34347841, slots=223981505, codes=4572077, nodes=246865094","throwable":""}
```

After
```
{"@timestamp":"2022-10-06T09:34:09,784","level":"INFO","thread":"EthScheduler-Services-32 (importBlock)","class":"FastImportBlocksStep","message":"Completed importing chain segment 4045158 to 4046557 (1400 blocks in 10259ms), Peers: 25","throwable":""}
{"@timestamp":"2022-10-06T09:34:10,455","level":"INFO","thread":"EthScheduler-Services-3 (batchPersistAccountData)","class":"SnapsyncMetricsManager","message":"Worldstate download in progress synced=54.42%, accounts=99670425, slots=604502342, codes=13261095, nodes=691089522","throwable":""}
{"@timestamp":"2022-10-06T09:34:30,802","level":"INFO","thread":"EthScheduler-Services-32 (importBlock)","class":"FastImportBlocksStep","message":"Completed importing chain segment 4046558 to 4048157 (1600 blocks in 21015ms), Peers: 25","throwable":""}
{"@timestamp":"2022-10-06T09:34:40,975","level":"INFO","thread":"EthScheduler-Services-32 (importBlock)","class":"FastImportBlocksStep","message":"Completed importing chain segment 4048158 to 4050357 (2200 blocks in 10167ms), Peers: 25","throwable":""}
{"@timestamp":"2022-10-06T09:34:51,104","level":"INFO","thread":"EthScheduler-Services-32 (importBlock)","class":"FastImportBlocksStep","message":"Completed importing chain segment 4050358 to 4052357 (2000 blocks in 10124ms), Peers: 25","throwable":""}
{"@timestamp":"2022-10-06T09:35:02,098","level":"INFO","thread":"EthScheduler-Services-32 (importBlock)","class":"FastImportBlocksStep","message":"Completed importing chain segment 4052358 to 4054957 (2600 blocks in 10826ms), Peers: 25","throwable":""}
{"@timestamp":"2022-10-06T09:35:12,201","level":"INFO","thread":"EthScheduler-Services-32 (importBlock)","class":"FastImportBlocksStep","message":"Completed importing chain segment 4054958 to 4056957 (2000 blocks in 10096ms), Peers: 25","throwable":""}
{"@timestamp":"2022-10-06T09:35:16,980","level":"INFO","thread":"EthScheduler-Services-3 (batchPersistAccountData)","class":"SnapsyncMetricsManager","message":"Worldstate download in progress synced=54.71%, accounts=100196801, slots=606855952, codes=13330951, nodes=694009270","throwable":""}
```

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-06 09:40:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4485" class=".btn">#4485</a>
            </td>
            <td>
                <b>
                    Reduced logging level on Subscriber error callback.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span><span class="chip">mainnet</span><span class="chip">logging</span>
            </td>
            <td>
                Signed-off-by: mark-terry <mark.terry@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Reduces the logging level of Subscriber callback exceptions from Error to Info

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
Addresses #4454 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-06 06:00:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4483" class=".btn">#4483</a>
            </td>
            <td>
                <b>
                    uprev version to 22.10.RC1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-05 17:39:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4482" class=".btn">#4482</a>
            </td>
            <td>
                <b>
                    Prepping 22.7.5
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

Cherry picked issues for 22.7.5 release.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-05 16:33:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4481" class=".btn">#4481</a>
            </td>
            <td>
                <b>
                    Better handler for --fast-sync-min-peers flag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dev experience</span><span class="chip">mainnet</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Changes the misleading warn of --fast-sync-min-peers to a more accurate handler which throws a ParameteresException only if this flag is used combined with sync-mode=FULL

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #4315
## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-05 11:29:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4480" class=".btn">#4480</a>
            </td>
            <td>
                <b>
                    Move Frank to emeritus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I propose moving the following maintainers to Emeritus status, pursuant to the inactivity clause. These maintainers have had no activity since May 2022:

@frankisawesome 

We very much appreciate their contributions but moving their status to emeritus (and thus revoking PR approval privileges) is in the interest of an orderly project. If any of these maintainers express in this PR that they intend to make contributions in the next quarter, then they will not be moved to emeritus status.
I propose this vote is open until either an absolute majority of active maintainers votes for the same outcome, or until two weeks has passed, after which a voting majority will determine the outcome (with a tie resulting in no change).

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-04 23:17:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4479" class=".btn">#4479</a>
            </td>
            <td>
                <b>
                    add Gabriel Trintinalia as a maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <macfarla.github@gmail.com>

Proposing @Gabriel-Trintinalia as a new Besu maintainer - has made over 5 significant [commits](https://github.com/hyperledger/besu/pulls?q=is%3Apr+author%3AGabriel-Trintinalia+is%3Aclosed) that improved the quality of Besu and/or added new features.

Voting ends 2 weeks from the publication of this PR or once more than 50% of the current maintainers approve.

For more information on this process see the Becoming a Maintainer section in the MAINTAINERS.md file.


## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-04 23:13:28 +0000 UTC
    </div>
</div>

