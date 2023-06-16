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
                PR <a href="https://github.com/hyperledger/besu/pull/5611" class=".btn">#5611</a>
            </td>
            <td>
                <b>
                    Ensure that blobs, proofs and  commitments have the same number of elements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Ensure blobs proofs commitments have the same size

## Fixed Issue(s)
fixes #5488 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-16 05:51:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5610" class=".btn">#5610</a>
            </td>
            <td>
                <b>
                    [4844] Add toString to VersionedHash
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add toString to VersionedHash and set it to be the JsonValue of the VersionedHash object

Actual: 
```
{
...
  blobVersionedHashes: [{
      versionId: 1
  }, {
      versionId: 1
  }, {
      versionId: 1
  }, {
      versionId: 1
  }, {
      versionId: 1
  }, {
      versionId: 1
  }],
 ...
}
```
Expected:

```
{
...
  blobVersionedHashes: ["0x01a8a4a49dcd1b91c376c87d7d6a6e73ee3792205864bf61781e8e3ad19d0092", 
"0x01069693395fb9a698b257e6c25380f32393bc0cf17a290f9e7fcea3c4ae7b8b", 
"0x01111dafbfcc0caa0803fc22f697fd3b9171252504e14ec0443f04a2b3288715", 
"0x01d1dfff9c15b3201980d8f9b958a8ade73e3e1e0ca76c54785a33e09519be7a", 
"0x01a7b4b55dd68d59685abcd629708c5de44c8e9edf3671602538eba23375893c", 
"0x013586020d67ab6808e681c2e6a2d1e854c84e5bc49df2ed34e218eace844f8b"],
...
}
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-16 03:58:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5609" class=".btn">#5609</a>
            </td>
            <td>
                <b>
                    Prepare for version 23.4.3-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prepare for version 23.4.3-SNAPSHOT
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-16 01:31:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5608" class=".btn">#5608</a>
            </td>
            <td>
                <b>
                    Release 23.4.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 23.4.2
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-16 01:00:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5607" class=".btn">#5607</a>
            </td>
            <td>
                <b>
                    Removed GoQuorum permissioning interop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Removed GoQuorum permissioning from Besu

## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/5459
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-15 16:55:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5606" class=".btn">#5606</a>
            </td>
            <td>
                <b>
                    Option to disable txpool
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
        Created At 2023-06-15 15:25:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5603" class=".btn">#5603</a>
            </td>
            <td>
                <b>
                    [4844] Increase blob sidecar size
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Increase blob sidecar size
## PR description

## Fixed Issue(s)
fixes #5590 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-15 05:02:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5601" class=".btn">#5601</a>
            </td>
            <td>
                <b>
                    [MINOR] Move noisy Pipeline log to debug
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
        Created At 2023-06-14 22:30:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5600" class=".btn">#5600</a>
            </td>
            <td>
                <b>
                    metrics - migrate tests from Junit4 to Junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
metrics Tests
Added dependency for junit.jupiter (junit5) and Removed dependency on junit 4
Migrated test from junit4 to junit5

## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/5562
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-14 17:26:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5598" class=".btn">#5598</a>
            </td>
            <td>
                <b>
                    EnclaveFactoryTest - migrate tests from Junit4 to Junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
EnclaveFactoryTest

Added dependency for junit.jupiter (junit5)
Removed dependency on junit 4
Migrated test from junit4 to junit5

## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/5566
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-14 12:27:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5594" class=".btn">#5594</a>
            </td>
            <td>
                <b>
                    Fix verification metadata for spotless task
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
        Created At 2023-06-13 10:49:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5593" class=".btn">#5593</a>
            </td>
            <td>
                <b>
                    Revert Console appender changes since it is managed programmatically
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

Since the Console appender is managed programmatically, adding it in the default log4j2 configuration caused that every line is logged twice, reverting the configuration and thinking of a better way to manage updates to the Console configuration

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-13 10:20:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5592" class=".btn">#5592</a>
            </td>
            <td>
                <b>
                    update pipeline
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
        Created At 2023-06-13 10:07:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5591" class=".btn">#5591</a>
            </td>
            <td>
                <b>
                    [4844] Increase blob throughput
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">4844</span>
            </td>
            <td>
                ## PR description
Increase blob throughput according to spec

## Fixed Issue(s)
#5590 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-13 07:44:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5588" class=".btn">#5588</a>
            </td>
            <td>
                <b>
                    [CHANGELOG] moved 5131 to the right version section
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixing an issue reported here https://discord.com/channels/905194001349627914/938504958909747250/1117975723366436924
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-13 05:54:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5586" class=".btn">#5586</a>
            </td>
            <td>
                <b>
                    [4844] Add dataGasUsed and excessDataGas to  Blockresult
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR adds dataGasUsed and excessDataGas to the BlockResult
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-13 03:52:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5585" class=".btn">#5585</a>
            </td>
            <td>
                <b>
                    Revert "Update Tuweni to 2.4.1 (#5513)"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Besu nightly nodes showed threads blocked exceptions with DNS stack trace.

Reverting this library upgrade so that we can investigate further.

`
"@timestamp":"2023-06-13T01:06:02,046","level":"WARN","thread":"vertx-blocked-thread-checker","class":"BlockedThreadChecker","message":"Thread Thread[vert.x-eventloop-thread-1,5,main] has been blocked for 15888080 ms, time limit is 2000 ms","throwable":" io.vertx.core.VertxException: Thread blocked\n\tat java.base@17.0.7/jdk.internal.misc.Unsafe.park(Native Method)\n\tat java.base@17.0.7/java.util.concurrent.locks.LockSupport.parkNanos(LockSupport.java:252)\n\tat app//kotlinx.coroutines.BlockingCoroutine.joinBlocking(Builders.kt:88)\n\tat app//kotlinx.coroutines.BuildersKt__BuildersKt.runBlocking(Builders.kt:59)\n\tat app//kotlinx.coroutines.BuildersKt.runBlocking(Unknown Source)\n\tat app//kotlinx.coroutines.BuildersKt__BuildersKt.runBlocking$default(Builders.kt:38)\n\tat app//kotlinx.coroutines.BuildersKt.runBlocking$default(Unknown Source)\n\tat app//org.apache.tuweni.discovery.DNSTimerTask.run(DNSDaemon.kt:89)\n\tat app//org.apache.tuweni.discovery.DNSDaemon$$Lambda$1330/0x0000000801603c80.handle(Unknown Source)\n\tat app//io.vertx.core.impl.VertxImpl$InternalTimerHandler.handle(VertxImpl.java:927)\n\tat app//io.vertx.core.impl.VertxImpl$InternalTimerHandler.handle(VertxImpl.java:903)\n\tat app//io.vertx.core.impl.EventLoopContext.emit(EventLoopContext.java:55)\n\tat app//io.vertx.core.impl.ContextBase.emit(ContextBase.java:239)\n\tat app//io.vertx.core.impl.ContextInternal.emit(ContextInternal.java:194)\n\tat app//io.vertx.core.impl.VertxImpl$InternalTimerHandler.run(VertxImpl.java:921)\n\tat app//io.netty.util.concurrent.PromiseTask.runTask(PromiseTask.java:98)\n\tat app//io.netty.util.concurrent.ScheduledFutureTask.run(ScheduledFutureTask.java:159)\n\tat app//io.netty.util.concurrent.AbstractEventExecutor.runTask(AbstractEventExecutor.java:174)\n\tat app//io.netty.util.concurrent.AbstractEventExecutor.safeExecute(AbstractEventExecutor.java:167)\n\tat app//io.netty.util.concurrent.SingleThreadEventExecutor.runAllTasks(SingleThreadEventExecutor.java:470)\n\tat app//io.netty.channel.epoll.EpollEventLoop.run(EpollEventLoop.java:406)\n\tat app//io.netty.util.concurrent.SingleThreadEventExecutor$4.run(SingleThreadEventExecutor.java:997)\n\tat app//io.netty.util.internal.ThreadExecutorMap$2.run(ThreadExecutorMap.java:74)\n\tat app//io.netty.util.concurrent.FastThreadLocalRunnable.run(FastThreadLocalRunnable.java:30)\n\tat java.base@17.0.7/java.lang.Thread.run(Thread.java:833)\n"}
`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-13 02:56:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5584" class=".btn">#5584</a>
            </td>
            <td>
                <b>
                    Use the node's configuration to decide if adding a peer with DNS in the enode is allowed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Uses the node configuration to decide if `admin_addPeer()` should allow enodes with DNS in them. Previously this was hard coded to DNS-disabled.

I had to flow the enode DNS configuration through from `RunnerBuilder` to the JSON RPC method factory so that AdminAddPeer` has access to it. It may be that this isn't necessary, but I couldn't see another way to do it.

## Fixed Issue(s)
Fixes https://github.com/hyperledger/besu/issues/5583
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-12 11:04:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5582" class=".btn">#5582</a>
            </td>
            <td>
                <b>
                    Migrate plugins module to Junit 5.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Migrate the plugins module from JUnit 4.0 to JUnit 5.0\
#5559 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-11 13:59:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5581" class=".btn">#5581</a>
            </td>
            <td>
                <b>
                    Migrate util module to JUnit 5.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Migrate the util module from Junit 4.0 to Junit 5.0 
#5556 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-11 13:18:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5575" class=".btn">#5575</a>
            </td>
            <td>
                <b>
                    Migrate EVM module to JUnit 5
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

Migrate EVM module tests to JUnit 5.
Mostly parameterized test and mockito support changes.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-09 17:28:56 +0000 UTC
    </div>
</div>

