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
                PR <a href="https://github.com/hyperledger/besu/pull/4304" class=".btn">#4304</a>
            </td>
            <td>
                <b>
                    Log the number of connected peers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The number of connected peers is what matters. 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-24 01:29:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4303" class=".btn">#4303</a>
            </td>
            <td>
                <b>
                    Reinstate Tessera tests with a fixed version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Use a fixed version of Tessera docker image. 
* Enable the ignored privacy tests that use Tessera 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-23 20:46:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4300" class=".btn">#4300</a>
            </td>
            <td>
                <b>
                    add logs for bonsai investigation
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
        Created At 2022-08-23 12:44:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4299" class=".btn">#4299</a>
            </td>
            <td>
                <b>
                    [MINOR] turn down logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

turn down logging on the "comparing timestamps" message

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-23 09:50:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4298" class=".btn">#4298</a>
            </td>
            <td>
                <b>
                    Reduce fast-sync-min-peers for post merge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Post merge we no longer need to wait to have 5 peers to validate a pivot block knowing that the pivot block comes from the  consensus client. This PR proposes to reduce the min peers to 1 for post merge network. It will always be possible to change it via the flag if necessary

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
        Created At 2022-08-23 09:49:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4297" class=".btn">#4297</a>
            </td>
            <td>
                <b>
                    ignore the tests that use tessera enclave via docker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

These tests are uniformly failing since about 6 hours ago. Docker container startup error. eg
```
org.testcontainers.containers.ContainerLaunchException: Container startup failed
	at app//org.testcontainers.containers.GenericContainer.doStart(GenericContainer.java:345)
	at app//org.testcontainers.containers.GenericContainer.start(GenericContainer.java:326)
	at app//org.hyperledger.enclave.testutil.TesseraTestHarness.start(TesseraTestHarness.java:83)
	at app//org.hyperledger.besu.tests.acceptance.dsl.privacy.PrivacyNode.start(PrivacyNode.java:194)
	at app//org.hyperledger.besu.tests.acceptance.dsl.privacy.PrivacyCluster.startNode(PrivacyCluster.java:182)
	at app//org.hyperledger.besu.tests.acceptance.dsl.privacy.PrivacyCluster.lambda$selectAndStartBootnode$6(PrivacyCluster.java:136)
...
            org.testcontainers.containers.ContainerLaunchException: Could not create/start container
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
        Created At 2022-08-23 09:07:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4291" class=".btn">#4291</a>
            </td>
            <td>
                <b>
                    upreved to new snapshot
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-22 17:27:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4290" class=".btn">#4290</a>
            </td>
            <td>
                <b>
                    snapshot version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-22 16:03:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4289" class=".btn">#4289</a>
            </td>
            <td>
                <b>
                    Synchronous Vertx as dependency for engine api
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
Make synchronous vertex EngineJsonRpcMethods a dependency instead of creating a new one. Key reasons for this change:
- allow other methods that require synchronization with `engine_` to share same vertx instance. (e.g `rollup_` extension method in #4146)
- improve testability, before some tests failed with too many files open because vext inside EngineJsonRpcMethods was not being closed on test's `afterEach` hook;

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
        Created At 2022-08-22 14:58:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4288" class=".btn">#4288</a>
            </td>
            <td>
                <b>
                    Reduce megamorphic call sites in AbstractCallOperation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

The four instances of gas in the CALL operations are all implemented
identically.  Refactor the method into the abstract parent.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-22 14:30:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4287" class=".btn">#4287</a>
            </td>
            <td>
                <b>
                    Changes MergeCoordinator fields to protected to allow extension
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Pedro Novais <jpvnovais@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Changes some fields modifiers to protected to allow class extension

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
        Created At 2022-08-22 14:17:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4286" class=".btn">#4286</a>
            </td>
            <td>
                <b>
                    create AbstractJsonRpcTest for better code reuse in other similar tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Pedro Novais <jpvnovais@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Abstracts some logic to be reused in similar tests, as suggested in PR #4146. (Helpful in downstream [fork](https://github.com/hyperledger/besu/pull/4146/files#diff-d27d85eaed527f7ef2ead8611cf0a17b4e33ed7c11dd341385eb9e9acfd30b70R11))

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
        Created At 2022-08-22 13:14:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4285" class=".btn">#4285</a>
            </td>
            <td>
                <b>
                    Reduced fast-sync-min-peers default value to 2.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span><span class="chip">mainnet</span><span class="chip">peering</span>
            </td>
            <td>
                Signed-off-by: mark-terry <mark.terry@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Reduces the default fast-sync minimum peers from 5 to 2 to improve syncing performance in low participation networks

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Partially addresses #4202 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-22 10:53:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4283" class=".btn">#4283</a>
            </td>
            <td>
                <b>
                    interpret an empty string (0x80) as an unsigned byte of 0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Stefan <stefan.pingel@consensys.net>

## PR description
This PR addresses Besu failure to decode a devp2p Hello message that contains the witness protocol capability version 0. In that Hello message the version of the witness protocol is encoded as 0x80 (zero length string), which is a valid way of encoding the version number 0.  

## Fixed Issue(s)
fixes #4279

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-22 05:55:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4282" class=".btn">#4282</a>
            </td>
            <td>
                <b>
                    Flexible Privacy Groups feature - Support to Tessera's EC encryptor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Flexible privacy contracts are modified so they allow the use of enclave public keys longer than 32 bytes. This way the feature will now support the EC encryptor mode of Tessera. Java classes adapted as well so they could encode/decode Solidity `bytes` properly.

Since there were `bytes32` parameters in the method signatures of the proxy contract, I could not just upgrade the implementation. This means that the changelog should warn about this change. I guess it is ok since [in the actual documentation, this feature is referred to as an experimental one](https://besu.hyperledger.org/en/stable/HowTo/Use-Privacy/Use-FlexiblePrivacy/) and changes like this might be expected.

## Fixed Issue(s)

fixes https://github.com/hyperledger/besu/issues/4262


## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-19 15:21:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4280" class=".btn">#4280</a>
            </td>
            <td>
                <b>
                    working on snapshot impl for bonsai
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
        Created At 2022-08-19 12:37:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4278" class=".btn">#4278</a>
            </td>
            <td>
                <b>
                    Trace block timeout
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
Added some thread management around `trace_block` to prevent large traces from blocking the node.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Addresses #4050 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-18 23:30:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4277" class=".btn">#4277</a>
            </td>
            <td>
                <b>
                    Update Paris Block Definition
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description

Paris block definition was set up prior to gray glacier.  Update the
base to be gray glacier.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-18 06:02:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4276" class=".btn">#4276</a>
            </td>
            <td>
                <b>
                    Bugfix/clique post merge fast sync
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">P3</span><span class="chip">mainnet</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
similar to #4224 for PoW, there are three clique block header validation rules that need to be evaluated at block import time rather than during fast sync header validation if merge is enabled (like on goerli):
* MixHash ConstantFieldValidationRule
* VoteValidationRule
* clique-specific TimestampMoreRecentThanParent

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #4272 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-17 23:32:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4273" class=".btn">#4273</a>
            </td>
            <td>
                <b>
                    Gradle repository maintenance
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

Cleanup repository references and limit scope of non-mavenCentral
repositories.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-17 20:41:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4271" class=".btn">#4271</a>
            </td>
            <td>
                <b>
                    Retry mechanism when getting a broadcasted block fail on all peers
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

Currently even if we use the RetryingGetBlockFromPeers, that tries to download the block, checking every peer in turn, if all peers fail, the retrieval is not repeated, unless the block is announced again.
This PR improve the block propagation manager, to repeat the download of a block, until some conditions apply: it is still not imported and the distance from the local head is within configured range.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

relates to #3955 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-17 13:22:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4269" class=".btn">#4269</a>
            </td>
            <td>
                <b>
                    Filter out disconnected peers when fetching available peers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">peering</span>
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Currently a peer that is marked as disconnected can be returned when asking `EthPeers` for available peers, but returning a disconnected peer is not useful and potentially a cause of problems since all tasks will fail on it.
Not sure how much this affect peer selection in the real world, but in unit tests it happens to choose a disconnected peer for request.
In any case it seems reasonable to add this check, and we can evaluate if we also need to require that a peer is fully validated, before returning it as available

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
        Created At 2022-08-17 11:55:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4268" class=".btn">#4268</a>
            </td>
            <td>
                <b>
                    Improve logging for BREACH_OF_PROTOCOL
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                added the peer that caused the breach in some places and added "BREACH_OF_PROTOCOL" to the debug logging

Signed-off-by: Stefan <stefan.pingel@consensys.net>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-17 05:29:14 +0000 UTC
    </div>
</div>

