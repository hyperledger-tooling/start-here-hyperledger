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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5479" class=".btn">#5479</a>
            </td>
            <td>
                <b>
                    Remove bonsai accumulator trielogfactory
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
Fixes a refactor omission.  TrieLogFactory was still statically constructed and used in accumulator.  This would lead to besu writing trie logs to its database with the default TrieLog serializer rather than one (potentially) configured via plugin.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-19 19:18:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5476" class=".btn">#5476</a>
            </td>
            <td>
                <b>
                    Implement debug_getRawReceipts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                ## PR description
Implements the `debug_getRawReceipts` RPC method. This allows retrieving all receipts in a block in one call without the overhead of computing derived values. Return value is a plain array of RLP encoded receipts from the block.  e.g:

```shell
cast rpc debug_getRawReceipts latest
["0x7ef9010c0182fa0db9010000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000c08353766d"]
```

Method is included in https://ethereum.github.io/execution-apis/api-documentation/ though not with a lot of detail.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-19 10:35:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5475" class=".btn">#5475</a>
            </td>
            <td>
                <b>
                    Blobdb for static data
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

This PR is built on top of https://github.com/hyperledger/besu/pull/5471, so check it first.

This PR introduces optimizations for RocksDB column families that contain static data, i.e. key value entries that are never changed, but only added, like an append log storage, the best example is the blockchain storage, that benefit if [BlobDB ](https://github.com/facebook/rocksdb/wiki/BlobDB) is used for them, since the write amplification is highly reduced, with the result of faster initial sync and less wear out of SSD.

Preliminary test shows that checkpoint sync is faster with BlobDB enabled, more tests are ongoing, and will share the results later.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #4607 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-19 09:29:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5474" class=".btn">#5474</a>
            </td>
            <td>
                <b>
                    remove old EF bootnodes
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
This PR removes old EF bootnodes .Would like someone from the EF team validate this before we move forward with that.
@skylenet @parithosh Could please confirm these bootnodes don't exist anymore?


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-19 05:20:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5473" class=".btn">#5473</a>
            </td>
            <td>
                <b>
                    Invalid transaction type - report to user
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">RPC</span><span class="chip">ux</span>
            </td>
            <td>
                If transaction validation fails because of "Invalid transaction type", report that error back to the user (previously was "invalid params")
This will make situations like this easier to troubleshoot -
https://discord.com/channels/905194001349627914/938504958909747250/1108931495797727354
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-19 03:50:49 +0000 UTC
    </div>
</div>

