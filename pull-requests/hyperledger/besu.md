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
                PR <a href="https://github.com/hyperledger/besu/pull/2909" class=".btn">#2909</a>
            </td>
            <td>
                <b>
                    Added log for validator selection mode transition
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
- Add a log message when validator selection mode changes between blocks
- Notification logic implemented on `QbftTransitionNotifier`
- Check happens upon creation of a new `QbftBlockHeighManager` in the corresponding factory. That means that we notify before the transition actually happens, to help diagnose any issues with the transition that is about to happen (e.g. wrong address for the validator contract).

Example messages:
```
Transitioning validator selection mode from BLOCKHEADER to ADDRESS(0x0000000000000000000000000000000000008888)

Transitioning validator selection mode from ADDRESS(0x0000000000000000000000000000000000008888) to BLOCKHEADER

Transitioning validator selection mode from ADDRESS(0x0000000000000000000000000000000000008888) to ADDRESS(0x0000000000000000000000000000000000007777)
```

## Fixed Issue(s)
fixes #2784

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-15 01:53:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2908" class=".btn">#2908</a>
            </td>
            <td>
                <b>
                    Always copy create code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Always copy the create code. Since it is memory bytes it is subject to
re-writing by the caller and all data would otherwise have to be treated
 as mutable.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>


## Fixed Issue(s)
#2899

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-14 17:04:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2904" class=".btn">#2904</a>
            </td>
            <td>
                <b>
                    Add trace_filter API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">doc-change-required</span>
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

This PR adds the trace_filter API. This API returns traces matching given filter

    fromBlock:  trace will start at this block (optional) .
    toBlock:race will stop at this block (optional) .
    fromAddress: only traces with this senders  (optional) .
    toAddress: only traces with this destination addresses  (optional) .
    after: the offset 
    count:  maximum number of traces to return

#### Request
```json
{
    "jsonrpc": "2.0",
    "method": "trace_filter",
    "params": [
      {
        "fromBlock": "0x1",
        "toBlock": "0x21",
        "after": 2,
        "count": 2,
        "fromAddress": [
          "0xfe3b557e8fb62b89f4916b721be55ceb828dbd73"
        ]
      }
    ],
    "id": 415
  }
```


#### Response
```json
{
    "jsonrpc": "2.0",
    "result": [
      {
        "action": {
          "callType": "call",
          "from": "0xfe3b557e8fb62b89f4916b721be55ceb828dbd73",
          "gas": "0xffad82",
          "input": "0x0000000000000000000000000000000000000999",
          "to": "0x0020000000000000000000000000000000000000",
          "value": "0x0"
        },
        "blockHash": "0xcd5d9c7acdcbd3fb4b24a39e05a38e32235751bb0c9e4f1aa16dc598a2c2a9e4",
        "blockNumber": 6,
        "result": {
          "gasUsed": "0x7536",
          "output": "0x"
        },
        "subtraces": 1,
        "traceAddress": [],
        "transactionHash": "0x91eeabc671e2dd2b1c8ddebb46ba59e8cb3e7d189f80bcc868a9787728c6e59e",
        "transactionPosition": 0,
        "type": "call"
      },
      {
        "action": {
          "callType": "call",
          "from": "0xfe3b557e8fb62b89f4916b721be55ceb828dbd73",
          "gas": "0xffad52",
          "input": "0xf000000000000000000000000000000000000000000000000000000000000001",
          "to": "0x0030000000000000000000000000000000000000",
          "value": "0x0"
        },
        "blockHash": "0xeed85fe57db751442c826cfe4fdf43b10a5c2bc8b6fd3a8ccced48eb3fb35885",
        "blockNumber": 7,
        "result": {
          "gasUsed": "0x1b",
          "output": "0xf000000000000000000000000000000000000000000000000000000000000002"
        },
        "subtraces": 0,
        "traceAddress": [],
        "transactionHash": "0x47f4d445ea1812cb1ddd3464ab23d2bfc6ed408a8a9db1c497f94e8e06e85286",
        "transactionPosition": 0,
        "type": "call"
      }
    ],
    "id": 415
  }
```

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-14 09:11:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2903" class=".btn">#2903</a>
            </td>
            <td>
                <b>
                    fix some flakey onchain privacy tests (ConsenSys/protocol-misc#419)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ConsenSys/protocol-misc#419 lists a number of onchain privacy acceptance tests that are flakey. 

All these tests fail because of a timeout while checking that a privacy group has been created on all the member nodes.

This PR changes the timeout from the default 10s to 20s

Signed-off-by: Stefan Pingel <stefan.pingel@consensys.net>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-14 05:09:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2902" class=".btn">#2902</a>
            </td>
            <td>
                <b>
                    Bft block period transition
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">consensus</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Allow the Bft block period to be changed using a transition. This allows the block period to be changed in either IBFT2 or QBFT.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-14 04:06:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2896" class=".btn">#2896</a>
            </td>
            <td>
                <b>
                    Fix concurrency issue on Ethpeers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

We just detected a concurrency exception on one of our canary nodes. Synchronizing the block does not seem to be enough to prevent concurrent modifications during foreach. I propose to use an iterator for this part in order to resolve this issue

```
{“timestamp”:“2021-10-12T21:08:32,573",“level”:“ERROR”,“thread”:“nioEventLoopGroup-3-7",“class”:“Subscribers”,“message”:“Error in callback: “,”throwable”:” java.util.ConcurrentModificationException
	 java.base/java.util.ArrayList$ArrayListSpliterator.forEachRemainin
g(ArrayList.java:1661)
	 java.base/java.util.stream.AbstractPipeline.copyInto(AbstractPipeline.java:484)
	 java.base/java.util.stream.AbstractPipeline.wrapAndCopyInto(AbstractPipeline.java:474)
	 java.base/java.util.stream.ForEachOps$ForEachOp.evaluateSequen
tial(ForEachOps.java:150)
	 java.base/java.util.stream.ForEachOps$ForEachOp$OfRef.evaluateSequential(ForEachOps.java:173)
	 java.base/java.util.stream.AbstractPipeline.evaluate(AbstractPipeline.java:234)
	 java.base/java.util.stream.ReferencePipeline.forEach
(ReferencePipeline.java:497)
	 org.hyperledger.besu.ethereum.eth.manager.EthPeers.abortPendingRequestsAssignedToDisconnectedPeers(EthPeers.java:107)
	 org.hyperledger.besu.ethereum.eth.manager.EthPeers.registerDisconnect(EthPeers.java:96)
	 org.hyperledger.b
esu.ethereum.eth.manager.EthProtocolManager.handleDisconnect(EthProtocolManager.java:343)
	 org.hyperledger.besu.ethereum.p2p.network.NetworkRunner.lambda$setupHandlers$2(NetworkRunner.java:157)
	 org.hyperledger.besu.ethereum.p2p.rlpx.connections.PeerConnection
Events.lambda$dispatchDisconnect$0(PeerConnectionEvents.java:55)
	 org.hyperledger.besu.util.Subscribers.lambda$forEach$0(Subscribers.java:112)
	 java.base/java.lang.Iterable.forEach(Iterable.java:75)
	 org.hyperledger.besu.util.Subscribers.forEach(Subscribe
rs.java:109)
	 org.hyperledger.besu.ethereum.p2p.rlpx.connections.PeerConnectionEvents.dispatchDisconnect(PeerConnectionEvents.java:55)
	 org.hyperledger.besu.ethereum.p2p.rlpx.connections.AbstractPeerConnection.terminateConnection(AbstractPeerConnection.java:14
5)
	 org.hyperledger.besu.ethereum.p2p.rlpx.connections.netty.NettyPeerConnection.lambda$new$0(NettyPeerConnection.java:62)
	 io.netty.util.concurrent.DefaultPromise.notifyListener0(DefaultPromise.java:578)
	 io.netty.util.concurrent.DefaultPromise.notifyLis
tenersNow(DefaultPromise.java:552)
	 io.netty.util.concurrent.DefaultPromise.notifyListeners(DefaultPromise.java:491)
	 io.netty.util.concurrent.DefaultPromise.setValue0(DefaultPromise.java:616)
	 io.netty.util.concurrent.DefaultPromise.setSuccess0(DefaultPr
omise.java:605)
	 io.netty.util.concurrent.DefaultPromise.trySuccess(DefaultPromise.java:104)
	 io.netty.channel.DefaultChannelPromise.trySuccess(DefaultChannelPromise.java:84)
	 io.netty.channel.AbstractChannel$CloseFuture.setClosed(AbstractChannel.java:118
2)
	 io.netty.channel.AbstractChannel$AbstractUnsafe.doClose0(AbstractChannel.java:773)
	 io.netty.channel.AbstractChannel$AbstractUnsafe.close(AbstractChannel.java:749)
	 io.netty.channel.AbstractChannel$AbstractUnsafe.close(AbstractChannel.java:620)
	
io.netty.channel.nio.AbstractNioByteChannel$NioByteUnsafe.closeOnRead(AbstractNioByteChannel.java:105)
	 io.netty.channel.nio.AbstractNioByteChannel$NioByteUnsafe.read(AbstractNioByteChannel.java:174)
	 io.netty.channel.nio.NioEventLoop.processSelectedKey(NioEve
ntLoop.java:719)
	 io.netty.channel.nio.NioEventLoop.processSelectedKeysOptimized(NioEventLoop.java:655)
	 io.netty.channel.nio.NioEventLoop.processSelectedKeys(NioEventLoop.java:581)
	 io.netty.channel.nio.NioEventLoop.run(NioEventLoop.java:493)
	 io.ne
tty.util.concurrent.SingleThreadEventExecutor$4.run(SingleThreadEventExecutor.java:986)
	 io.netty.util.internal.ThreadExecutorMap$2.run(ThreadExecutorMap.java:74)
	 io.netty.util.concurrent.FastThreadLocalRunnable.run(FastThreadLocalRunnable.java:30)
	 java
.base/java.lang.Thread.run(Thread.java:829)
”}
```

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-13 08:56:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2895" class=".btn">#2895</a>
            </td>
            <td>
                <b>
                    Add tracing of the EVM with OpenTelemetry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Antoine Toulme <antoine@lunar-ocean.com>

## PR description
Add OpenTelemetry tracing for the EVM as an experiment.


## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-13 05:57:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2893" class=".btn">#2893</a>
            </td>
            <td>
                <b>
                    Amphora merge again
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
merge latest main 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-13 01:34:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2892" class=".btn">#2892</a>
            </td>
            <td>
                <b>
                    Amphora merge main
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

Merge main into `merge` branch

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-12 23:21:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2891" class=".btn">#2891</a>
            </td>
            <td>
                <b>
                    Fix #2890: Allow eth_call and eth_estimateGas to accept contract address as sender
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Fixed Issue(s)
Closes #2890 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-12 23:16:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2881" class=".btn">#2881</a>
            </td>
            <td>
                <b>
                    Qbft RPCs should read validators from the contract when in contract mode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ~Created a partial copy of the ForkingValidatorProvider in order to use a read-only version of the BlockValidatorProvider (which contains its own voteTallyCache).~

Create readOnlyValidatorProvider in QbftBesuControllerBuilder and pass into QbftJsonRpcMethods constructor (better than using protocolContext as is only used once when creating the RPCs

This requires storing transactionValidatorProvider in a field and relying on its earlier creation during createConsensusContext()

Fixes https://github.com/hyperledger/besu/issues/2795
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-12 09:50:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2880" class=".btn">#2880</a>
            </td>
            <td>
                <b>
                    change version 21.10.0-RC3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

change version 21.10.0-RC3

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-12 08:17:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2878" class=".btn">#2878</a>
            </td>
            <td>
                <b>
                    Release 21.10.0-RC2
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
        Created At 2021-10-12 06:38:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2876" class=".btn">#2876</a>
            </td>
            <td>
                <b>
                    Release 21.10.0-RC2
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
        Created At 2021-10-12 06:25:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2874" class=".btn">#2874</a>
            </td>
            <td>
                <b>
                    Qbft validator selection was incorrectly being applied to non validator selection mode transitions
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
Qbft validation selection was incorrectly being applied for non validator selection mode transitions. This was caused by the QbftProtocolSchedule not considering the current validator selection mode. The BftForksSchedule has been added to the QbftProtocolSchedule so that current mode is used even when the transition is not for changing the validation selection mode.

fixes #2894

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-12 03:23:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2872" class=".btn">#2872</a>
            </td>
            <td>
                <b>
                    Use web3j gradle plugin for acceptance tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Generate wrappers using web3j for all contracts in `./acceptance-tests/tests/contracts`

Signed-off-by: Antony Denyer <git@antonydenyer.co.uk>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 14:50:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2871" class=".btn">#2871</a>
            </td>
            <td>
                <b>
                    add jacoco store artifacts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 12:48:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2870" class=".btn">#2870</a>
            </td>
            <td>
                <b>
                    Clarify text in javadocs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Antony Denyer <git@antonydenyer.co.uk>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 12:12:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2869" class=".btn">#2869</a>
            </td>
            <td>
                <b>
                    Fix for Select correct ValidatorProvider when transitioning from validator contract to block header mode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

During the transition from contract mode to block header mode, when creating the extra data for a new block, we need to look ahead to the next block's voteProvider to obtain the nonEmpty one associated with the BlockValidatorProvider.

This only applies to ForkingValidatorProvider which is currently only used for QBFT. However, we don't want QBFT to know it's using a ForkingValidatorProvider. Therefore we need to implement getVoteProviderAfterBlock on the ValidatorProvider interface even though it's implementation is equivalent to getVoteProvider.

Update qbft integration tests to expose this bug.

## Fixed Issue(s)
Fixes https://github.com/hyperledger/besu/issues/2868

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 07:43:06 +0000 UTC
    </div>
</div>

