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
                    Handle ConcurrentModificationException on ReattemptPendingPeerRequests
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
A ConcurrentModificationExpetion happens when EthPeers reattempts to execute its Pending Requests and one  request causes a peer to disconnect.

This PR logs the exception gracefully instead of letting the callback to handle the exception because:
- If the peer is disconnected, the request  aborts.
- The disconnection event will reattempts to execute any other Pending Requests that does not belong to the disconnected peer.

Two test cases were created to test these assumption.

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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4198" class=".btn">#4198</a>
            </td>
            <td>
                <b>
                    poc add to blacklist invalid nodes
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

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-29 10:01:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4196" class=".btn">#4196</a>
            </td>
            <td>
                <b>
                    Upgrade gradle to 7.5, silence the welcome message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Antoine Toulme <antoine@lunar-ocean.com>

## PR description
Upgrade Gradle to 7.5. Silence the Gradle welcome message.

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-29 03:03:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4195" class=".btn">#4195</a>
            </td>
            <td>
                <b>
                    upgrade spotless to 6.8.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Antoine Toulme <antoine@lunar-ocean.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Upgrade spotless to 6.8.0, removing workaround for JDK 17 support.

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-29 01:13:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4194" class=".btn">#4194</a>
            </td>
            <td>
                <b>
                    Panda print only when crossing TTD the first time
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
ensure Pandas only print when we merge, not just when we initially set a new merge state (like on startup)

* make panda printer static
* add prior merge state to MergeStateHandler
* move pandas into TransitionControllerBuilder's transition watcher
*  before we print, ensure we are PoS AND the prior merge state was pre-merge



## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#3954 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 23:47:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4190" class=".btn">#4190</a>
            </td>
            <td>
                <b>
                    Feature/engine api override
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
Allow besu to have the engine api enabled, when there are not merge configs.  includes:
* un-hiding/un-deprecating `--engine-rpc-enabled`
* remove old isMergeEnabled checks in a few block header validators
* use merge-specific block header validator, rather than appending to MainnetBlockHeaderValidator
* disable all engine api methods except engine_exchangeTransitionConfigurationV1 in the absence of an engine-api-compatible coordinator
* add "placeholder" TTD in the absence of a TTD configuration

Tested with Hive and Kurtosis since this affects block validation.  Both are 🟢 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #4172 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 04:48:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4189" class=".btn">#4189</a>
            </td>
            <td>
                <b>
                    Accept empty header set in range headers validation
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

If a response to the get header P2P request only returns the header that
is the start of the range we may need to trim it to an empty response,
this is breaking the validation response. One client has started
returning only the range header start in some circumstances (which is a
valid response per spec). Because we sometimes request an overlapping
header this results in an empty stream once we cut the duplicates.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 04:33:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4186" class=".btn">#4186</a>
            </td>
            <td>
                <b>
                    Only stop block propagation, not tx handling.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                
## PR description

Since there is a Subscribers for each type of message handler in EthMessages, and only on handler, they all get a subscriber id of 1.  This changes the unsubscribe logic to require the caller to specify the message code handler being unsubscribed from, and removes it from the map of handlers.

## Fixed Issue(s)
fixes #3890 

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-27 22:48:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4185" class=".btn">#4185</a>
            </td>
            <td>
                <b>
                    Switching info to trace on several noisey logs during sync.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">logging</span>
            </td>
            <td>
                Signed-off-by: matt-nelson-csi <matt.nelson@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
Fixes #4182 - switches info to trace on the three noisy Sync commands 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-27 21:55:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4181" class=".btn">#4181</a>
            </td>
            <td>
                <b>
                    Prepare for version 22.7.0-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prepare for version 22.7.0-SNAPSHOT
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-27 17:57:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4180" class=".btn">#4180</a>
            </td>
            <td>
                <b>
                    Release 22.7.0-RC3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 22.7.0-RC3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-27 17:14:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4179" class=".btn">#4179</a>
            </td>
            <td>
                <b>
                    fix enr request order
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">peering</span><span class="chip">TeamChupa</span>
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

After a Geth<>Besu peerring test we found that sometimes we had "ENR request failed                       id=68f8eb309602c1a6 addr=3.16.90.60:30303      err=“RPC timeout”

Besu does not respond to the ENR request. By investigating we found that sometimes ENR_REQUEST comes before the PONG and so Besu ignores the request.

This PR allows to cache the request if it arrives before the PONG to answer once the bond is done


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
        Created At 2022-07-27 13:22:54 +0000 UTC
    </div>
</div>

