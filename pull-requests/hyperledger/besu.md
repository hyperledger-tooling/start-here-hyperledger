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
                PR <a href="https://github.com/hyperledger/besu/pull/3340" class=".btn">#3340</a>
            </td>
            <td>
                <b>
                    Merge slf4j stragglers
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

remove log4j dependency in merge project, switch to slf4j on a few classes that didn't pop up during the merge of slf4j changes from main


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 23:19:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3339" class=".btn">#3339</a>
            </td>
            <td>
                <b>
                    Merge main into merge branch
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

Merge `main` into `merge`
* merge main
* convert merge-specific classes using log4j to slf4j
* add slf4j labmda shim to util project, for parameters that are expensive to evaluate

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 20:02:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3333" class=".btn">#3333</a>
            </td>
            <td>
                <b>
                    Add ec-curve parameter public key export/export-address subcommands
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
- Add ec-curve parameter public key export/export-address subcommands
- Defaults to secp256k1
- Support secp256k1 and secp256r1
- Added a log message when creating a key with the selected ec curve name 

## Fixed Issue(s)
fixes #3206 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 09:46:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3331" class=".btn">#3331</a>
            </td>
            <td>
                <b>
                    Update besu-native to 0.4.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                https://github.com/hyperledger/besu-native/releases/tag/0.4.3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 05:21:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3330" class=".btn">#3330</a>
            </td>
            <td>
                <b>
                    21.10.9 update hashes to match regenerated artefacts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Besu CI pipeline was re-run on the same commit, generating the same artefact with a different hash

Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

See https://app.circleci.com/pipelines/github/hyperledger/besu?branch=release-21.10.x&filter=all 
^ looking at this - pipeline for commit 8f465c0 was run twice. 7 days ago and 2 days ago.
Since the commit is the same https://github.com/hyperledger/besu/commit/8f465c0faf568b395c8e271c6caff6f79d77a7a7
I'm updating the hashes.
Also ref https://github.com/hyperledger/homebrew-besu/pull/70

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 04:29:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3328" class=".btn">#3328</a>
            </td>
            <td>
                <b>
                    Prepare for version 22.1.0-RC4-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prepare for version 22.1.0-RC4-SNAPSHOT
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-26 00:07:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3327" class=".btn">#3327</a>
            </td>
            <td>
                <b>
                    Release 22.1.0-RC3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 22.1.0-RC3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-25 23:32:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3326" class=".btn">#3326</a>
            </td>
            <td>
                <b>
                    Refactor to async retrieve blocks, and change peer when retrying to get a block
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

`GetBlockFromPeersTask` is replaced with `RetryingGetBlockFromPeersTask` everywhere, since it is more effective in refreshing the peers while retrying.
`RetryingGetBlockFromPeersTask` has been changed to first try the peer that announce the block if known, and the try a different peer on every retry, and exit if the block has been downloaded by someone else in the meantime.
The task to get block from peers in `BlockPropagationManager` was blocking, and this had effect on the propagation of the `onBlockAdded` event, actually pausing it until the task was done, now the get block from peers task is async, and we keep track of the requests for non announced block, to avoid doing redoundant work.

A lot of debug/trace logs has been added to help the investigation on sync issues.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3304

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-25 14:38:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3325" class=".btn">#3325</a>
            </td>
            <td>
                <b>
                    (fix) Failing test in java 17 - jackson optional parsing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                Signed-off-by: Frank Li <b439988l@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Related to https://github.com/hyperledger/besu/pull/3082
Use jdk8module for jackson so optionals in class types are parsed correctly during json deserialisation

## Fixed Issue(s)
fixes https://github.com/hyperledger/besu/issues/3318
helps https://github.com/hyperledger/besu/issues/3320
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-25 07:41:34 +0000 UTC
    </div>
</div>

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

To correctly shutdown the ChainDownloader, the method `cancel()` must be used, and it aborts the underlying pipeline, that  triggers a `CancellationException`, but the downloader exits anyway since the `cancelled.get()` now returns `true`

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
#3300
## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
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

