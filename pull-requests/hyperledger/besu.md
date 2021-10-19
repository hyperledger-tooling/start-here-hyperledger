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
                PR <a href="https://github.com/hyperledger/besu/pull/2924" class=".btn">#2924</a>
            </td>
            <td>
                <b>
                    Simplify clock in ValidatorContractTest
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
        Created At 2021-10-19 05:56:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2923" class=".btn">#2923</a>
            </td>
            <td>
                <b>
                    QBFT Contract based validators Acceptance test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">consensus</span>
            </td>
            <td>
                ## PR description
Add Acceptance test for QBFT contract based validators [#2620]

Signed-off-by: Usman Saleem <usman@usmans.info>

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 03:12:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2922" class=".btn">#2922</a>
            </td>
            <td>
                <b>
                    [MINOR] Typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixed some typos

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 01:11:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2919" class=".btn">#2919</a>
            </td>
            <td>
                <b>
                    propagate the changelog and next version from RC3 release to main
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

propagate changelog and version from RC3 branch to main

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-18 16:29:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2918" class=".btn">#2918</a>
            </td>
            <td>
                <b>
                    [#2454] Set gas fees to zero when simulating a transaction without enforcing balance checks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">documentation</span><span class="chip">doc-change-required</span>
            </td>
            <td>
                Before we set the sender balance to the maximum allowed, but this has
side effects in smart contracts that use `msg.sender.balance`.

Setting `strict` field to `false` in the `eth_call` call, forces gas fees to be set to zero,
so the execution of the transaction is not constrained to the balance of the sender.


Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#2454 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-18 13:57:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2917" class=".btn">#2917</a>
            </td>
            <td>
                <b>
                    EVM Speed Improvements for MSTORE
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR Description

More EVM Speed Improvements aimed at improving MSTORE times.
* Move Memory from raw bytes to byte array
* Add calls for 32 byte MSB aligned writes
* Remove `incrementProgramCounter` and move data into OperationResult

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-18 00:19:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2916" class=".btn">#2916</a>
            </td>
            <td>
                <b>
                    2705 - logging unused request fields during serialization for JsonCallParameter class
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

- used the @JsonAnySetter marker annotation to catch unused request fields and log their values and class type for JsonCallParameter.java domain class.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fix for #2705 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-17 17:45:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2911" class=".btn">#2911</a>
            </td>
            <td>
                <b>
                    Prepare for version 21.10.0-RC4-SNAPSHOT
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
        Created At 2021-10-15 17:44:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2910" class=".btn">#2910</a>
            </td>
            <td>
                <b>
                    Release 21.10.0-RC3
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
        Created At 2021-10-15 17:13:58 +0000 UTC
    </div>
</div>

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
Transitioning validator selection mode from blockheader to contract (address: 0x0000000000000000000000000000000000008888)

Transitioning validator selection mode from contract (address: 0x0000000000000000000000000000000000008888) to blockheader

Transitioning validator selection mode from contract (address: 0x0000000000000000000000000000000000008888) to contract (address: 0x0000000000000000000000000000000000007777)
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

Example configuration for ibft2 to change the block period to 4 seconds at block 1240 would be:
```
"transitions": {
	"ibft2": [
		{
			"block": 1240,
			"blockperiodseconds": 4
		}
	]
}
```		

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

