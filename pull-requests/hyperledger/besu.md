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
                PR <a href="https://github.com/hyperledger/besu/pull/3308" class=".btn">#3308</a>
            </td>
            <td>
                <b>
                    trivy scan on main | release branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Trivy scan of docker develop images on main | release branch

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 23:57:20 +0000 UTC
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3288" class=".btn">#3288</a>
            </td>
            <td>
                <b>
                    dependency check - added gradle plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Add plugin for gradle dependency check

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-17 07:52:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3287" class=".btn">#3287</a>
            </td>
            <td>
                <b>
                    Release 21.10.8
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changelog entry and download links for 21.10.8

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-17 04:41:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3286" class=".btn">#3286</a>
            </td>
            <td>
                <b>
                    Release 21.10.9 SNAPSHOT version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                SNAPSHOT version

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-17 03:57:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3285" class=".btn">#3285</a>
            </td>
            <td>
                <b>
                    Introduce SLF4J for logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Given the latest events regarding Log4J2 security issues and the advent of Besu modularization, it would be interesting to introduce an abstraction layer for logging so we don't force any implementation for future adopters.

This PR replaces every `org.apache.logging.log4j.Logger` instance with its analog `org.slf4j.Logger` but still respects every hard dependency on Log4J2 (now more easily identifiable). Also, a new helper was introduced to deal with situations where a `org.apache.logging.log4j.core.LoggerContext` was created outside the scope of SLF4J.

This is quite large to review so I kept different commits for the different decisions being made
 - [8863bc5](https://github.com/hyperledger/besu/commit/8863bc5e899b6e9705165b6636b9ad6bc116d111): just adds the slf4j API
 - [4c2545b](https://github.com/hyperledger/besu/commit/4c2545bda533d160f25e189c228b1ce4e66379d2): this is the biggest one. 90% of it is just replacing the `Logger` instances, but there are also some other minor changes for respecting the same behavior of Log4J2 in SLF4j, e.g. wrap in an `if (LOG.isXxxxEnabled)` values that would have been resolved through lambdas in Log4J2.
 - [a1b98a9](https://github.com/hyperledger/besu/commit/a1b98a95248a74041f7e2265db043a3a645d755a): changes an specific Logger from Log4J2 for a regular one. If this a really wanted feature, we can add it into the logging definition and attach that appender to the enclosing class.
 - [0cbc0c3](https://github.com/diega/besu/commit/0cbc0c31c2b629a83d563b5865ecc6b88261f23e): changes the default value of a CLI option
 - [cd9b7e0](https://github.com/hyperledger/besu/commit/cd9b7e06c0a81c2e4d97ccf325f1818cc81c4b9a): Emulates [Log4J2 Configurator](https://github.com/apache/logging-log4j2/blob/rel%2F2.17.1/log4j-core/src/main/java/org/apache/logging/log4j/core/config/Configurator.java) behavior but resolving the logging context through SLF4j

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-16 23:07:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3284" class=".btn">#3284</a>
            </td>
            <td>
                <b>
                    revert to using bundled solc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Remove install of solc on CI executor and revert to using solc that is bundled with the gradle plugin

Fixes #3277 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-16 22:27:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3283" class=".btn">#3283</a>
            </td>
            <td>
                <b>
                    Include ETC Mystique specification in 21.10.8
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR is for adding ETC specs according with [ECIP-1104](https://ecips.ethereumclassic.org/ECIPs/ecip-1104)

### Note
This was cherry-picked from [b964e90](https://github.com/hyperledger/besu/commit/b964e9098f2c95faca7a65f0a3447d7cd2825f73) but the `discovery` section of the _genesis_ files was removed because this release doesn't include #2944 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-16 22:06:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3282" class=".btn">#3282</a>
            </td>
            <td>
                <b>
                    besu-3259 Add Compression to TLS P2P
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Enabling Snappy compression for DevP2P-over-TLS. I'll follow up with a PR adding some testing around the Netty pipeline, however, this code is already being tested as part of our TLS acceptance tests so it is safe to merge.

## Fixed Issue(s)
see #3259
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-14 06:28:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3281" class=".btn">#3281</a>
            </td>
            <td>
                <b>
                    try tuweni upgrade
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
Test upgrade to Tuweni 2.1.0. This is just a draft PR to make sure no regressions are introduced.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-14 05:44:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3280" class=".btn">#3280</a>
            </td>
            <td>
                <b>
                    added changelog and links for 21.10.7 release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Download links for 21.10.7

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-14 03:19:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3279" class=".btn">#3279</a>
            </td>
            <td>
                <b>
                    21.10.8-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

21.10.8-SNAPSHOT version in case we need it

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-14 02:14:23 +0000 UTC
    </div>
</div>

