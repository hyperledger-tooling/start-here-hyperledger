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
                Created a partial copy of the ForkingValidatorProvider in order to use a read-only version of the BlockValidatorProvider (which contains its own voteTallyCache).

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
                    Qbft validation selection was incorrectly being applied for non validator selection mode transitions
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
Qbft validation selection was incorrectly being applied for non validator selection mode transitions. This was cause by the QbftProtocolSchedule not considering the current validator selection mode. The BftForksSchedule has been added to the QbftProtocolSchedule so that current mode is used even when the transition is not for changing the validation selection mode.

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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2866" class=".btn">#2866</a>
            </td>
            <td>
                <b>
                    Leave block p2p messages enabled
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
To support following the chain prior to TTD being reached, the NEW_BLOCK_HASHES and NEW_BLOCK messages must remain enabled.  

Potentially validation could/should be added to reject an new blocks if their parent already meets the total difficulty requirement for transition but that likely should live in the block import code rather than the networking code. That hasn't been done in this PR.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 04:29:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2865" class=".btn">#2865</a>
            </td>
            <td>
                <b>
                    Added support for PKCS11 keystore on PKI Block Creation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
- Extracted nested `KeyStoreWrapperProvider` interface into its own file
- Created a default implementation of this interface that takes care of instantiating the correct `KeyStoreWrapper` based on the type configuration.

## Fixed Issue(s)
fixes #2764 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 02:15:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2864" class=".btn">#2864</a>
            </td>
            <td>
                <b>
                    Fixed build badge: image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

master.svg -> main.svg

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 02:06:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2863" class=".btn">#2863</a>
            </td>
            <td>
                <b>
                    Fixed build badge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixed links for build and license badges: changed master to main.
Fixed some typos.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 00:45:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2862" class=".btn">#2862</a>
            </td>
            <td>
                <b>
                    Common Bft forks schedule
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
Create a common bft forks schedule that can be used between both ibft and qbft. This is necessary to add a bft transition for block period.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 23:46:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2861" class=".btn">#2861</a>
            </td>
            <td>
                <b>
                    Feature/no op candidate
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

no-op executePayload  for existing blocks

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 16:39:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2860" class=".btn">#2860</a>
            </td>
            <td>
                <b>
                    remove random from blockhash calc and blockheader in executePayload
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
* remove random from blockhash calc and blockheader in executePayload
* re-add stop at TTD to PostMergeContext
* remove old spec KNOWN status
* disable short-circuiting for known blocks

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 11:01:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2858" class=".btn">#2858</a>
            </td>
            <td>
                <b>
                    [MINOR] change DNS permissioning logging to TRACE
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changed recently added extra logging to TRACE level (same as other permissioning logging)

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 02:31:35 +0000 UTC
    </div>
</div>

