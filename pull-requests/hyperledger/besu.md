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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4214" class=".btn">#4214</a>
            </td>
            <td>
                <b>
                    Update for next release
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

Set versions for next release - 22.7.1-SNAPSHOT

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ X I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-03 16:08:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4213" class=".btn">#4213</a>
            </td>
            <td>
                <b>
                    Release 22.7.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Release Besu 22.7.0

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-03 16:07:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4210" class=".btn">#4210</a>
            </td>
            <td>
                <b>
                    Revert: mainnet blockheder validation merge check
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
This is a stopgap revert to address a post-merge sync regression caused by #4190.  The correct fix for this will need to wait until after the 22.7.0 release

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
workaround for #4209 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-03 07:34:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4209" class=".btn">#4209</a>
            </td>
            <td>
                <b>
                    Fix post-merge fast sync regression
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



## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #4208

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 21:23:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4207" class=".btn">#4207</a>
            </td>
            <td>
                <b>
                    Increase Gradle max heap size
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Diego López León <dieguitoll@gmail.com>

## PR description
This PR increases the maximum heap size for the Gradle build. [By default](https://docs.gradle.org/current/userguide/build_environment.html#sec:configuring_jvm_memory) it's set to 512 megabytes but it doesn't seem enough to run the build process from IntelliJ.
Without this proposed property I could see this message in the Build console:
```
Expiring Daemon because JVM heap space is exhausted
Daemon will be stopped at the end of the build after running out of JVM memory
Expiring Daemon because JVM heap space is exhausted
Expiring Daemon because JVM heap space is exhausted
Expiring Daemon because JVM heap space is exhausted
Daemon is stopping immediately JVM garbage collector thrashing and after running out of JVM memory
```

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 17:58:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4206" class=".btn">#4206</a>
            </td>
            <td>
                <b>
                    Fix ConcurrentModificationException on ReattemptPendingPeerRequests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Gabriel Trintinalia <gabriel.trintinalia@consensys.net>

## PR description
A ConcurrentModificationExpetion happens when EthPeers reattempts to execute its Pending Requests and one  request causes a peer to disconnect. This happens because RemoveIf on CopyOnWriteArrayList will test the filter for each item first and mark those who need to be removed and then throw the exception if the list was modified by any filter. 

Replacing removeIf with iterator seems to solve the issue.

## Fixed Issue(s)
#3491

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 13:43:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4205" class=".btn">#4205</a>
            </td>
            <td>
                <b>
                    Fix Optional handling when TTD is absent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
fix an oversight in the Optional<MergeContext> handling when TTD is absent.  Also ensure the unit test mocks the absence of MergeContext not just the absence of TTD.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
bugfix for #4172 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 02:48:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4204" class=".btn">#4204</a>
            </td>
            <td>
                <b>
                    Set snap sync as default for named ethereum networks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Set snap sync as default for named ethereum networks.  No rush to merge this one ahead of the 22.7.0 release

* changes NetworkName to specify the default SyncMode, rather than just a boolean for support FAST sync or not
* sets snap sync as the default for:
  - kiln
  - goerli
  - sepolia 
  - ropsten
  - rinkeby
  - mainnet
  
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #4203 


## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 02:41:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4200" class=".btn">#4200</a>
            </td>
            <td>
                <b>
                    lower bound peer limit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span><span class="chip">TeamRevenant</span><span class="chip">mainnet</span><span class="chip">peering</span>
            </td>
            <td>
                Added (experimental) CLI option for a lower bound for p2p peers. Similar to Teku's https://docs.teku.consensys.net/en/latest/Reference/CLI/CLI-Syntax/#p2p-peer-lower-bound

So we actively try to find more peers up to --Xp2p-peer-lower-bound, but still allow incoming connections until we hit --p2p-peer-upper-bound AKA --max-peers, only then we refuse incoming connections.

* Note currently this PR changes the default for max-peers - happy to change this back once the plumbing for deploying canary nodes supports the "lower-bound" param
* Timer refresh for the peer table `tableRefreshIntervalMs` is 30 minutes

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-01 02:25:10 +0000 UTC
    </div>
</div>

