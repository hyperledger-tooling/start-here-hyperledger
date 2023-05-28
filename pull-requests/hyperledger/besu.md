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
                PR <a href="https://github.com/hyperledger/besu/pull/5505" class=".btn">#5505</a>
            </td>
            <td>
                <b>
                    GraphQL: Migrate Long types to strings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Migrate from EIP specified numeric values to execution-spec specified
string values.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 19:32:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5504" class=".btn">#5504</a>
            </td>
            <td>
                <b>
                    Prepare for next version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 04:38:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5503" class=".btn">#5503</a>
            </td>
            <td>
                <b>
                    Change disconnect peer message to debug level.
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
Change the peer disconnect message to debug level. Since that's not useful to end users.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 01:28:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5502" class=".btn">#5502</a>
            </td>
            <td>
                <b>
                    run non-mainnet ATs on PRs, split into sub groups
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Run all ATs on PRs, but split into 
* mainnet
* Clique + BFT
* Privacy + Permissioning
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 00:50:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5501" class=".btn">#5501</a>
            </td>
            <td>
                <b>
                    Release 23.4.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 23.4.1
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 00:49:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5500" class=".btn">#5500</a>
            </td>
            <td>
                <b>
                    Specify optional scheme (ws or wss) in Ethstats url option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
- Allow scheme (ws:// or wss://) optionally to be specified in ethstats url. If user specify the scheme, the connection logic doesn't need to switch from ssl to non-ssl on each retry logic.
- Change order of ethstats service start after main ethereum loop is up because ethstats service needs local node address.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #5494 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-25 23:36:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5499" class=".btn">#5499</a>
            </td>
            <td>
                <b>
                    Revert "Add plugin API to select Transactions (#5396)"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit 65bcc557e41cca2568588a21441aa5d8658a5e79.

Due to breaking Clique (in the ATs at least)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-25 22:33:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5498" class=".btn">#5498</a>
            </td>
            <td>
                <b>
                    Stop evaluating txs for sender after the first skipped one
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

This PR is built on top of  #5492 and #5491 so check them first.

This PR introduce a simple optimization to avoid to waste time validating transactions that will not be selected during the current block creation process. 
Basically if a sender have more than one prioritized candidate transactions, and for some reason any of them is not selected during the block creation process, it make no sense to keep evaluating any more transaction after the skipped one, since it will not be selected due to the nonce gap.

Enabling the selection stats implemented in #5492 is it possible to see the difference before and after this PR, the wasted validation work that we are removing is represented by the `INVALID_TRANSIENT(NONCE_TOO_HIGH)` label.

Before
```
Selection stats: Totals[Evaluated=2000, Selected=109, Skipped=1891, Dropped=0]; Detailed[INVALID_TRANSIENT(GAS_PRICE_BELOW_CURRENT_BASE_FEE)=1712, INVALID_TRANSIENT(NONCE_TOO_HIGH)=158, INVALID_TRANSIENT(TX_TOO_LARGE_FOR_REMAINING_GAS)=21, SELECTED=109]
```

After
```
Selection stats: Totals[Evaluated=1743, Selected=126, Skipped=1617, Dropped=0]; Detailed[INVALID_TRANSIENT(GAS_PRICE_BELOW_CURRENT_BASE_FEE)=1600, INVALID_TRANSIENT(TX_TOO_LARGE_FOR_REMAINING_GAS)=17, SELECTED=126]
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-25 09:26:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5497" class=".btn">#5497</a>
            </td>
            <td>
                <b>
                    Remove maybeHead from BackwardSyncContext
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Built on top of https://github.com/hyperledger/besu/pull/5470
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-25 07:31:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5496" class=".btn">#5496</a>
            </td>
            <td>
                <b>
                    GraphQL Support for withdrawals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add support for withdrawals in GraphQL, including needed changes to testing infrastructure for shanghai-era blocks.
Also align existing adapters with graphql schema optionality.

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
        Created At 2023-05-25 01:04:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5495" class=".btn">#5495</a>
            </td>
            <td>
                <b>
                    NPE in peer discovery disconnect
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

encountered during testing.  Quick fix.

```
...
rocketpool_eth1  | 2023-05-24 23:45:06.677+00:00 | Timer-0 | INFO  | DNSResolver | Resolved 2409 nodes
rocketpool_eth1  | 2023-05-24 23:45:34.417+00:00 | vert.x-eventloop-thread-3 | ERROR | ContextBase | Unhandled exception
rocketpool_eth1  | java.lang.NullPointerException: Cannot invoke "java.util.Map.remove(java.lang.Object)" because "peerInteractionStateMap" is null
rocketpool_eth1  |      at org.hyperledger.besu.ethereum.p2p.discovery.internal.PeerDiscoveryController$PeerInteractionState.execute(PeerDiscoveryController.java:802)
rocketpool_eth1  |      at org.hyperledger.besu.ethereum.p2p.discovery.internal.PeerDiscoveryController$PeerInteractionState.lambda$execute$0(PeerDiscoveryController.java:797)
rocketpool_eth1  |      at org.hyperledger.besu.ethereum.p2p.discovery.internal.VertxTimerUtil.lambda$setTimer$1(VertxTimerUtil.java:34)
rocketpool_eth1  |      at io.vertx.core.impl.VertxImpl$InternalTimerHandler.handle(VertxImpl.java:932)
rocketpool_eth1  |      at io.vertx.core.impl.VertxImpl$InternalTimerHandler.handle(VertxImpl.java:903)
rocketpool_eth1  |      at io.vertx.core.impl.EventLoopContext.emit(EventLoopContext.java:55)
rocketpool_eth1  |      at io.vertx.core.impl.ContextBase.emit(ContextBase.java:239)
rocketpool_eth1  |      at io.vertx.core.impl.ContextInternal.emit(ContextInternal.java:194)
rocketpool_eth1  |      at io.vertx.core.impl.VertxImpl$InternalTimerHandler.run(VertxImpl.java:921)
rocketpool_eth1  |      at io.netty.util.concurrent.PromiseTask.runTask(PromiseTask.java:98)
rocketpool_eth1  |      at io.netty.util.concurrent.ScheduledFutureTask.run(ScheduledFutureTask.java:153)
rocketpool_eth1  |      at io.netty.util.concurrent.AbstractEventExecutor.runTask(AbstractEventExecutor.java:174)
rocketpool_eth1  |      at io.netty.util.concurrent.AbstractEventExecutor.safeExecute(AbstractEventExecutor.java:167)
rocketpool_eth1  |      at io.netty.util.concurrent.SingleThreadEventExecutor.runAllTasks(SingleThreadEventExecutor.java:470)
rocketpool_eth1  |      at io.netty.channel.epoll.EpollEventLoop.run(EpollEventLoop.java:406)
rocketpool_eth1  |      at io.netty.util.concurrent.SingleThreadEventExecutor$4.run(SingleThreadEventExecutor.java:997)
rocketpool_eth1  |      at io.netty.util.internal.ThreadExecutorMap$2.run(ThreadExecutorMap.java:74)
rocketpool_eth1  |      at io.netty.util.concurrent.FastThreadLocalRunnable.run(FastThreadLocalRunnable.java:30)
rocketpool_eth1  |      at java.base/java.lang.Thread.run(Thread.java:857)
```
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-24 23:55:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5493" class=".btn">#5493</a>
            </td>
            <td>
                <b>
                    Add MCOPY Operation (EIP-5656)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add the MCOPY operation targeting cancun.
Testing required adding memory to the text fixture.

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
        Created At 2023-05-24 20:28:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5492" class=".btn">#5492</a>
            </td>
            <td>
                <b>
                    Detailed transaction selection stats for layered txpool
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

Expand the transaction selection result adding more fine grained info specifically about the reason a transaction is skipped or tagged as invalid, and also specify if the selection ended due to block full or block over min occupancy ratio.
These results are also collected so at the end of the selection we can log detailed stats, that are useful to understand which are the main reasons for a transaction not to be selected, and so improve the way transactions are prioritized, to avoid proposing these transactions in the first place.

Stats are logged at debug level, and here it is a sample:
```
Selection stats: Totals[Evaluated=2693, Selected=353, Skipped=2340, Dropped=0]; Detailed[INVALID_TRANSIENT(GAS_PRICE_BELOW_CURRENT_BASE_FEE)=2321, INVALID_TRANSIENT(TX_TOO_LARGE_FOR_REMAINING_GAS)=19, SELECTED=353]
```

This helped spotting some optimizations and understand [the effect of `min-block-occupancy-ratio` on PoS networks](https://github.com/hyperledger/besu/pull/5492)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-24 12:27:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5491" class=".btn">#5491</a>
            </td>
            <td>
                <b>
                    Ignore min-block-occupancy-ratio option when on PoS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

[`min-block-occupancy-ratio` option ](https://besu.hyperledger.org/en/stable/public-networks/reference/cli/options/#min-block-occupancy-ratio) make sense on PoW networks where you need to be faster that other nodes in finding a block, so you can set be satisfied when the block produced is enough filled, but on PoS you do not need to compete with other nodes, since you have an allocated slot to produce the block, so in this case make sense to always try to fill the block, until the remaining gas is less than the minimum needed for the smaller transaction.
So for PoS the `min-block-occupancy-ratio` option is ignored since we always try to fill 100% of the block.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-24 08:37:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5483" class=".btn">#5483</a>
            </td>
            <td>
                <b>
                    Remove TOML table headings before checking for valid config parameters
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR modifies the TOML parsing function `checkUnknownOptions()` to remove TOML headings before checking if all of the attributes are valid. E.g. for the following file:

```
[TxPool]
tx-pool-max-size = 1024
```

the `TxPool` TOML parameter will be removed and ignored as per the discussion in the related issue.

## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/5482

Remaining tasks before PR review:

- [ ] Add unit test
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-23 14:52:29 +0000 UTC
    </div>
</div>

