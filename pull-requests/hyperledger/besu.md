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
                PR <a href="https://github.com/hyperledger/besu/pull/3319" class=".btn">#3319</a>
            </td>
            <td>
                <b>
                    Do not exit ChainDownloader in case of a generic CancellationException
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There right way of halting a ChainDownloader is only via the cancel method,
no special action should be taken on a generic CancellationException, that
could be triggered by peer tasks that run in the pipeline, since in that
case the error is transient and the download should restart.

Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

For example this exception that is triggered by a timeout talking with a peer, causes the ChainDownloader to completely exit, while it should restart after the configured timeout.

To correctly shutdown the ChainDownloader, the method `cancel()` must be used, and it aborts the underlying pipeline, that  triggers a `CompletionException`, but the downloader exits anyway since the `cancelled.get()` now returns `true`

```
{
	"timestamp": "2022-01-23T01:04:14,278",
	"level": "DEBUG",
	"thread": "EthScheduler-Services-1410 (downloadHeaders)",
	"class": "Pipeline",
	"message": "Unhandled exception in pipeline. Aborting.",
	"throwable": "java.lang.RuntimeException: Async operation failed. java.util.concurrent.CancellationException
	at org.hyperledger.besu.services.pipeline.AsyncOperationProcessor.outputNextCompletedTask(AsyncOperationProcessor.java:86)
	at org.hyperledger.besu.services.pipeline.AsyncOperationProcessor.attemptFinalization(AsyncOperationProcessor.java:70)
	at org.hyperledger.besu.services.pipeline.ProcessingStage.run(ProcessingStage.java:43)
	at org.hyperledger.besu.services.pipeline.Pipeline.lambda$runWithErrorHandling$3(Pipeline.java:152)
	at java.base/java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:515)
	at java.base/java.util.concurrent.FutureTask.run(FutureTask.java:264)
	at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1128)
	at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:628)
	at java.base/java.lang.Thread.run(Thread.java:829)
Caused by: java.util.concurrent.ExecutionException: java.util.concurrent.CancellationException
	at java.base/java.util.concurrent.CompletableFuture.reportGet(CompletableFuture.java:395)
	at java.base/java.util.concurrent.CompletableFuture.get(CompletableFuture.java:2022)
	at org.hyperledger.besu.services.pipeline.AsyncOperationProcessor.waitForAnyFutureToComplete(AsyncOperationProcessor.java:94)
	at org.hyperledger.besu.services.pipeline.AsyncOperationProcessor.outputNextCompletedTask(AsyncOperationProcessor.java:81)
	... 8 more
Caused by: java.util.concurrent.CancellationException
	at java.base/java.util.concurrent.CompletableFuture.cancel(CompletableFuture.java:2396)
	at org.hyperledger.besu.ethereum.eth.manager.PendingPeerRequest.abort(PendingPeerRequest.java:116)
	at org.hyperledger.besu.ethereum.eth.manager.EthPeers.abortPendingRequestsAssignedToDisconnectedPeers(EthPeers.java:108)
	at org.hyperledger.besu.ethereum.eth.manager.EthPeers.registerDisconnect(EthPeers.java:97)
	at org.hyperledger.besu.ethereum.eth.manager.EthProtocolManager.handleDisconnect(EthProtocolManager.java:343)
	at org.hyperledger.besu.ethereum.p2p.network.NetworkRunner.lambda$setupHandlers$2(NetworkRunner.java:157)
	at org.hyperledger.besu.ethereum.p2p.rlpx.connections.PeerConnectionEvents.lambda$dispatchDisconnect$0(PeerConnectionEvents.java:55)
	at org.hyperledger.besu.util.Subscribers.lambda$forEach$0(Subscribers.java:112)
	at java.base/java.lang.Iterable.forEach(Iterable.java:75)
	at org.hyperledger.besu.util.Subscribers.forEach(Subscribers.java:109)
	at org.hyperledger.besu.ethereum.p2p.rlpx.connections.PeerConnectionEvents.dispatchDisconnect(PeerConnectionEvents.java:55)
	at org.hyperledger.besu.ethereum.p2p.rlpx.connections.AbstractPeerConnection.disconnect(AbstractPeerConnection.java:159)
	at org.hyperledger.besu.ethereum.eth.manager.EthPeer.disconnect(EthPeer.java:158)
	at java.base/java.util.Optional.ifPresent(Optional.java:183)
	at org.hyperledger.besu.ethereum.eth.manager.EthPeer.recordRequestTimeout(EthPeer.java:149)
	at org.hyperledger.besu.ethereum.eth.manager.task.AbstractPeerRequestTask.lambda$executeTask$2(AbstractPeerRequestTask.java:78)
	at java.base/java.util.concurrent.CompletableFuture.uniWhenComplete(CompletableFuture.java:859)
	at java.base/java.util.concurrent.CompletableFuture$UniWhenComplete.tryFire(CompletableFuture.java:837)
	at java.base/java.util.concurrent.CompletableFuture.postComplete(CompletableFuture.java:506)
	at java.base/java.util.concurrent.CompletableFuture.completeExceptionally(CompletableFuture.java:2088)
	at org.hyperledger.besu.ethereum.eth.manager.EthScheduler.lambda$failAfterTimeout$11(EthScheduler.java:278)
	at java.base/java.util.concurrent.FutureTask.run(FutureTask.java:264)
	at java.base/java.util.concurrent.ScheduledThreadPoolExecutor$ScheduledFutureTask.run(ScheduledThreadPoolExecutor.java:304)
	... 3 more
"
}
```


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 09:54:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3317" class=".btn">#3317</a>
            </td>
            <td>
                <b>
                    add trivy workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

trivy workflow

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 05:07:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3316" class=".btn">#3316</a>
            </td>
            <td>
                <b>
                    [MINOR] Typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                typo in constant name

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 04:26:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3314" class=".btn">#3314</a>
            </td>
            <td>
                <b>
                    DO NOT MERGE - Sonar tour much better
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

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-23 18:17:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3313" class=".btn">#3313</a>
            </td>
            <td>
                <b>
                    DO NOT MERGE - sonar tour
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

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-23 17:15:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3312" class=".btn">#3312</a>
            </td>
            <td>
                <b>
                    DO NOT MERGE - sonar demo
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

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-23 17:08:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3311" class=".btn">#3311</a>
            </td>
            <td>
                <b>
                    [MINOR] testing: changed more classes to MockitoJunitRunner 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

* Changed runner where minimal changes required
* removed unnecessary stubbings

See #2951

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 07:57:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3309" class=".btn">#3309</a>
            </td>
            <td>
                <b>
                    Remove unnecessary log when block timer expiry happens after the proposal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Removes an unnecessary warning from the QBFT logs. Due to precision of the Java timer sometimes the proposal message can be received before our block timer expiry event.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-20 00:12:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3307" class=".btn">#3307</a>
            </td>
            <td>
                <b>
                    added 21.10.9 to main changelog
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>


## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 22:49:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3306" class=".btn">#3306</a>
            </td>
            <td>
                <b>
                    new snapshot for 21.10.10
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
        Created At 2022-01-19 19:44:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3305" class=".btn">#3305</a>
            </td>
            <td>
                <b>
                    21.10.9 release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes CORS regression caused by Vert.x upgrade.

Signed-off-by: Justin Florentine <justin+github@florentine.us>


- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 16:07:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3303" class=".btn">#3303</a>
            </td>
            <td>
                <b>
                    Test for TLS channel pipeline handlers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Added a test to ensure all required handlers are correctly added to the channel pipeline when using TLS.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 04:14:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3302" class=".btn">#3302</a>
            </td>
            <td>
                <b>
                    make ethFeeHistory accept hex values for blockCount
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
Correctly parse hex parameters for ethFeeHistory blockCount

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #3301

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 00:51:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3298" class=".btn">#3298</a>
            </td>
            <td>
                <b>
                    handle NPE caused by empty json
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

First commit adds a failing test.
Second commit handles the NPE

Fixes #3294 

See it work:
Now if I uncheck content-length header in postman, I get this response
`{"jsonrpc":"2.0","id":null,"error":{"code":-32700,"message":"Parse error"}}`

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-18 06:14:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3297" class=".btn">#3297</a>
            </td>
            <td>
                <b>
                    vertx 4.2.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Update to vert.x 4.2.3

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-18 05:29:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3296" class=".btn">#3296</a>
            </td>
            <td>
                <b>
                    [regression] Reenable cors-origin to support any protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Diego López León <dieguitoll@gmail.com>

## PR description
Before the vert.x upgrade (#3135), the usage of `*` in the Cors-Origin [allowed any string](https://github.com/vert-x3/vertx-web/blob/3.9.8/vertx-web/src/main/java/io/vertx/ext/web/handler/impl/CorsHandlerImpl.java#L169) to pass. Meanwhile the [current version](https://github.com/vert-x3/vertx-web/blob/4.2.1/vertx-web/src/main/java/io/vertx/ext/web/handler/impl/CorsHandlerImpl.java#L231) performs a series of validations for the same wildcard, which allows only a fixed set of protocols (i.e. ftp, http, https). To return the original semantics of `*` according the documentation, an actual regex must be used.

This causes problems when a browser extension, like [Metamask](https://metamask.io/), tries to connect to a Besu client because they tend to use custom protocols. E.g. Chrome uses `chrome-extension` and Firefox `moz-extension`

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-18 03:22:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3295" class=".btn">#3295</a>
            </td>
            <td>
                <b>
                    add trivy dockerScan
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Add CI step for scanning develop docker images with trivy

See #3293 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-18 02:19:46 +0000 UTC
    </div>
</div>

