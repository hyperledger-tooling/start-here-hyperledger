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
                PR <a href="https://github.com/hyperledger/besu/pull/4246" class=".btn">#4246</a>
            </td>
            <td>
                <b>
                    try to remove arm runner, instead build with architecture env only
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Antoine Toulme <antoine@lunar-ocean.com>

## PR description
Trying to see if it's possible to build an arm docker image on a x86 runner.

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 06:05:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4241" class=".btn">#4241</a>
            </td>
            <td>
                <b>
                    quieten DynamicPivotBlockManager
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
* Only change pivot block if it is different than the existing syncTarget pivotBlock
* move logging level to debug

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #4211
## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-09 23:36:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4240" class=".btn">#4240</a>
            </td>
            <td>
                <b>
                    remove MergeUnfinalizedValidationRule
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
The CL is allowed to reorg around finalized via social consensus.  Remove this validation rule and rely solely on the CL for that social coordination.

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
        Created At 2022-08-09 18:38:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4237" class=".btn">#4237</a>
            </td>
            <td>
                <b>
                    Better management of jemalloc presence/absence
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">logging</span>
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

If jemalloc is not present, an error message is printed, but the absence of jemalloc is not a real error, so in this PR we try to understand if jemalloc is available and print messages that are easier for the user to understand, and invite him to install jemalloc to get better memory usage

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
        Created At 2022-08-09 13:59:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4236" class=".btn">#4236</a>
            </td>
            <td>
                <b>
                    Always switch full sync target when local chain is close to chain head
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Full sync has a sync target stability feature that works well when syncing from genesis, but is not optimal when the initial sync is done and local chian head is equal or very close to the target head, when the stability feature could prevent switching to the best peer.

By default the stability feature prevent to switch to the best peer, if its height is not 200 block greather, or the difficulty is not 1_000_000_000_000_000_000L greather than the current sync target. 

These value are too large when we are already in sync and just need to follow the best peer, so this PR, changes only enable the stability feature when the current chain head is far from the target head, that occurs when doing a full sync from genesis or when you restart Besu after some hours or days.

This can help Besu to stay in sync, because if the block propagation manager is missing some blocks, then it stops caching incoming blocks when the distance with the local chain head is > 30, but since the chain state of a peer is only updated when a new block is seen from that peer, there could not be enough information for the current sync target switching strategy to switch to the best peer.

On an already synced node, there are 2 hidden configuration flags to always for the switch to the best peer, without this patch:
`--Xsynchronizer-downloader-change-target-threshold-by-td=0`
`--Xsynchronizer-downloader-change-target-threshold-by-height=0`


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

potential fix for #3955

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-09 12:20:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4234" class=".btn">#4234</a>
            </td>
            <td>
                <b>
                    peer count - just count the live ones
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">peering</span>
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

This does not address the root cause, but will address the problem of users complaining that the logs report too many peers.

This should mean that the number of peers reported in the logs will be the correct number ie the number of connected peers

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-09 10:18:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4230" class=".btn">#4230</a>
            </td>
            <td>
                <b>
                    Introduce a cap to reputation score increase
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">peering</span>
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

#4130 introduced an way to increase reputation in case the peer is doing good, but there is no cap to the reputation score the peer can have.

The log shows peers with very high reputation, for example:
```
FullSyncTargetManager","message":"Caught up to best peer: PeerId 0xb3e02a84270c590f562e2c8b8274930c54b0a00ae001d44bd790b55c3bbc578c70738e6d4a2d32df78b6cf27a071fe54a068f3192c42ac29bd81a6663fe4fa0f, reputation PeerReputation 561, validated? true, disconnected? false, client: Geth/v1.10.21-stable-67109427/linux-amd64/go1.18.5, connection 1312721736, enode enode://b3e02a84270c590f562e2c8b8274930c54b0a00ae001d44bd790b55c3bbc578c70738e6d4a2d32df78b6cf27a071fe54a068f3192c42ac29bd81a6663fe4fa0f@34.92.61.128:29888, chain state: ChainState{estimatedHeight=7369229, bestBlock=BestBlock{totalDifficulty=0x0000000000000000000000000000000000000000000000000000000000a45b44, blockHash=0xb7c2ba396d3f4561fe619796e7ef399080823161f4b831c5b3f48445e7bf13a1, number=7369228}}. Current peers: 3","throwable":""}
```
since there is no cap to how much the reputation can increase.

I think make sense to have an upper bound, a peer can increase its repution until it reaches the default max again, otherwise a peer that is good for a long time, and start to be useless, will take a long time before its reputation goes below other more recent good peers


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
        Created At 2022-08-08 17:41:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4228" class=".btn">#4228</a>
            </td>
            <td>
                <b>
                    Change default size for header and chain segment size
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span><span class="chip">mainnet</span><span class="chip">peering</span>
            </td>
            <td>
                Signed-off-by: Stefan <stefan.pingel@consensys.net>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-08 06:23:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4227" class=".btn">#4227</a>
            </td>
            <td>
                <b>
                    Improve pending blocks retrieval mechanism
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span><span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Gabriel Trintinalia <gabriel.trintinalia@consensys.net>

## PR description
When a block is saved for future import, requesting the lowest announced block parent does not seem to be always the best option. It can be that we cannot retrieve this block and then we keep selecting the lowest block over and over and eventually it does not fix the gap. A better approach for trying to unstick could be to request the parent of the lowest pending ancestor

Changes:
- When saving a block for future import, try to retrieve the parent of the lowest pending block connected to this block.
- When saving a block for future import, do not try to retrieve the parent the lowest announced block.
- Avoid requesting the same parent block several times when saving pending blocks
- Improve logs when saving/importing a block

## Fixed Issue(s)
potential aid for #3955
#4197

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-08 03:21:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4224" class=".btn">#4224</a>
            </td>
            <td>
                <b>
                    fix for fast sync regression on post-merge networks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamChupa</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
* re-enable PoW, Timestamp, and Difficulty block header validation rules regardless of merge configuration.  
* if merge is enabled, use an AttachedBlockHeaderValidationRule version of ProofOfWorkValidationRule

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
        Created At 2022-08-05 19:07:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4223" class=".btn">#4223</a>
            </td>
            <td>
                <b>
                    correct fallback ttd to correct value
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

The fallback TTD for mainnet had off-by-one error. We need to set it to `2^256 - 2^10`, but our code was 
```
Difficulty.MAX_VALUE.subtract(UInt256.valueOf(1024L)
````

The problem is that `MAX_VALUE` is `2^256 - 1`, not `2^256`. So we were calculating in the end `2^256 - 1 - 2^10`.

This PR replaces the calculation with the hard coded value as hex in the config and as decimal in the test.

I confirmed the value with the mainnet genesis file for the consensus clients: https://github.com/ethereum/consensus-specs/blob/981b05afb01d5b19be3a5a60ccb12c3582e4c0cf/configs/mainnet.yaml#L16

## Fixed Issue(s)
fixes #4220

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-05 10:37:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4222" class=".btn">#4222</a>
            </td>
            <td>
                <b>
                    Log unexpected exceptions in execution engine rpc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Teku is reporting theses errors https://github.com/ConsenSys/teku/issues/6027

which are preceded by "Execution Client is offline":
```
java.io.IOException: -32603: Internal error
	at tech.pegasys.teku.ethereum.executionclient.web3j.Web3JClient.lambda$doRequest$0(Web3JClient.java:69)
	at java.base/java.util.concurrent.CompletableFuture.uniHandle(CompletableFuture.java:934)
	at java.base/java.util.concurrent.CompletableFuture$UniHandle.tryFire(CompletableFuture.java:911)
	at java.base/java.util.concurrent.CompletableFuture.postComplete(CompletableFuture.java:510)
	at java.base/java.util.concurrent.CompletableFuture.complete(CompletableFuture.java:2147)
	at tech.pegasys.teku.infrastructure.async.SafeFuture.lambda$propagateResult$3(SafeFuture.java:147)
	at java.base/java.util.concurrent.CompletableFuture.uniWhenComplete(CompletableFuture.java:863)
	at java.base/java.util.concurrent.CompletableFuture$UniWhenComplete.tryFire(CompletableFuture.java:841)
	at java.base/java.util.concurrent.CompletableFuture.postComplete(CompletableFuture.java:510)
	at java.base/java.util.concurrent.CompletableFuture.complete(CompletableFuture.java:2147)
	at org.web3j.utils.Async.lambda$run$1(Async.java:38)
	at java.base/java.util.concurrent.CompletableFuture$AsyncRun.run(CompletableFuture.java:1804)
	at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1136)
	at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:635)
	at java.base/java.lang.Thread.run(Thread.java:833)
```

but these internal errors are not reported in besu
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-05 10:30:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4217" class=".btn">#4217</a>
            </td>
            <td>
                <b>
                    [MINOR] typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-04 03:13:53 +0000 UTC
    </div>
</div>

