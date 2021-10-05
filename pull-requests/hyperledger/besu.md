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
                PR <a href="https://github.com/hyperledger/besu/pull/2854" class=".btn">#2854</a>
            </td>
            <td>
                <b>
                    [#538] Add a bash/zsh autocomplete script to distributions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR adds bash/zsh autocomplete support using [PicoCLI Command Line Completion](https://picocli.info/autocomplete.html).

## Fixed Issue(s)
Fixes  #538

## Running
The simpler way to see how it works is within a Docker container:
```shell
$ ./gradlew clean build
$ tar -zxvf build/distributions/besu-21.10.0-RC1-SNAPSHOT.tar.gz -C build/distributions
$ docker run -v `pwd`/build/distributions/besu-21.10.0-RC1-SNAPSHOT:/besu -it --rm openjdk:11 /bin/bash

# source /besu/besu.autocomplete.sh
# /besu/bin/besu -<TAB><TAB>
```

## Changelog

- [ ] Added CLI autocomplete scripts
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-05 17:19:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2853" class=".btn">#2853</a>
            </td>
            <td>
                <b>
                    customized test results location
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin.florentine@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Adds the sonarqube plugin and an initial configuration for it. To use:

`./gradlew jacocoRootReport sonarqube -Dsonar.login=$SONAR_TOKEN`

With a valid SONAR_TOKEN defined in your environment. This will push analysis reports to Hyperledgers account on Sonar Cloud.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #2811

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-05 11:23:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2851" class=".btn">#2851</a>
            </td>
            <td>
                <b>
                    Listener fix
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
        Created At 2021-10-05 09:01:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2850" class=".btn">#2850</a>
            </td>
            <td>
                <b>
                    fix equality for finalized head check in forkChoiceUpdated
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
fix forkchoiceupdate finalized root check

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-05 07:34:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2849" class=".btn">#2849</a>
            </td>
            <td>
                <b>
                    errata discovered during m2/m3 testing
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
fix various issues found during m2/m3 testing:
* fix baseFeePerGas serialization in EngineBlockResult
* fix terminal total difficulty determination for non-PoW consensus
* fix for protocolSchedule on transition (m3)
* persist chaindata on consensusValidated


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-04 20:25:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2848" class=".btn">#2848</a>
            </td>
            <td>
                <b>
                    changelog for 21.10.0-RC2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update changelog for 21.10.0-RC2

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-04 18:44:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2847" class=".btn">#2847</a>
            </td>
            <td>
                <b>
                    r 21.10.0 RC2 SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                21.10.0-RC2-SNAPSHOT

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-04 18:08:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2846" class=".btn">#2846</a>
            </td>
            <td>
                <b>
                    Release 21.10.0-RC1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-04 17:25:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2845" class=".btn">#2845</a>
            </td>
            <td>
                <b>
                    null on consensus validated
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
        Created At 2021-10-04 09:31:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2844" class=".btn">#2844</a>
            </td>
            <td>
                <b>
                    Bugfix/unblock pow mining
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

unblock PoW mining

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-04 08:02:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2843" class=".btn">#2843</a>
            </td>
            <td>
                <b>
                    Bugfix/inverted finalize check
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
fix an inverted finalize check


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-03 14:03:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2842" class=".btn">#2842</a>
            </td>
            <td>
                <b>
                    Feature/any consensus premerge
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
changes necessary to transition from any consensus engine to merge consensus:
* create TransitionContext
* create sparse ConsensusContext interface and implement it for all consensus context objects
* make MergeContext an interface and move implementation to PostMergeContext class


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-03 04:51:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2841" class=".btn">#2841</a>
            </td>
            <td>
                <b>
                    Feature/add random to header
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
* add random to BlockHeader
* honor feeRecipient in blocks created by engine_preparePayload

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-03 02:15:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2840" class=".btn">#2840</a>
            </td>
            <td>
                <b>
                    Feature/mining till fork
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
* addition of TransitionCoordinator, TransitionProtocolSchedule
* fix difficulty calculation for proposed blocks
* add MergeMiningCoordinator interface
* start/stop mining on the basis of terminalTotalDifficulty

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-02 14:11:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2839" class=".btn">#2839</a>
            </td>
            <td>
                <b>
                    Feature/local mergenet errata
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

fix parameter type issues for engine_preparePayload and engine_getPayload
## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-02 06:07:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2838" class=".btn">#2838</a>
            </td>
            <td>
                <b>
                    #1851 FastSyncDownloader should stop processing after receiving shutdown
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …own signal

Signed-off-by: Liu-yuan Lai <lailiuyuan@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
CancelationException is thrown if runner has been stopped. In this case, should not be treated as unexpected error and re-schedule, but bubble up the exception to the caller to be handled.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #1851 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-02 00:04:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2837" class=".btn">#2837</a>
            </td>
            <td>
                <b>
                    Added subcommand for validate-config
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
        Created At 2021-10-01 23:25:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2836" class=".btn">#2836</a>
            </td>
            <td>
                <b>
                    2742: Fix flaky timestamp unit test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">flake</span>
            </td>
            <td>
                Signed-off-by: Caitlin Harding <chardingcs@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
The unit test `PeerDiscoveryTimestampsTest.lastContactedTimestampUpdatedOnOutboundMessage()` fails intermittently due to a timestamp precision issue. In the unit tests, we are comparing the before and after state of a timestamp to ensure it was updated. When the test runs too quickly, the before and after states appear equal due to a loss of precision.

I tried the following solutions:
1. Fixing the precision issue by using the `org.hyperledger.besu.testutil.TestClock` test fixture.
- This did not solve the problem because the underlying class used in the SUT (`DiscoveryPeer`) stores the timestamps as longs, so we are constrained by the precision of longs.
2. Using Mockito to spy on the peer and assert that the `setLastSeen` and `setLastContacted` setters are called.
- This did not solve the problem because the SUT creates the peer object under the hood, and there is no easy way to inject my spy version in there.

So I landed on a simple, albeit not fancy or elegant, solution of adding a 1 ms `sleep` in the test between the two send message calls to ensure the timestamps will be at least 1 ms different.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes https://github.com/hyperledger/besu/issues/2742

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog). - Since this is "Internal technical improvements with no user impact", I think no changelog update is required.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-01 20:14:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2835" class=".btn">#2835</a>
            </td>
            <td>
                <b>
                    Feature/terminal total difficulty
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
merge-488 (protocol-misc)
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-01 14:39:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2834" class=".btn">#2834</a>
            </td>
            <td>
                <b>
                    Feature/milestone1 testing
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
* passes [geth test vectors](https://notes.ethereum.org/@9AeMAlpyQYaAAyuj47BzRw/rkwW3ceVY)
* add json-rpc object parameters to reflect current spec
* block proposal flow follows block processing candidate block flow


## Fixed Issue(s)
fixes #2381

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-01 11:06:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2833" class=".btn">#2833</a>
            </td>
            <td>
                <b>
                    Feature/prepare and get
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
implement preparePayload / getPayload according to latest interop spec


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes merge-479
fixes #2831 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-01 06:24:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2832" class=".btn">#2832</a>
            </td>
            <td>
                <b>
                    [MINOR] Rename whitelist -> allowlist
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Renamed some variables still using whitelist

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-01 05:23:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2829" class=".btn">#2829</a>
            </td>
            <td>
                <b>
                    [MINOR] typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Fixed some typos

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-30 21:07:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2828" class=".btn">#2828</a>
            </td>
            <td>
                <b>
                    Step2 snapsync as server integration
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
        Created At 2021-09-30 15:07:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2827" class=".btn">#2827</a>
            </td>
            <td>
                <b>
                    Remove benchmark from workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Remove benchmark from workflow

Signed-off-by: Antony Denyer <git@antonydenyer.co.uk>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-30 14:53:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2825" class=".btn">#2825</a>
            </td>
            <td>
                <b>
                    Add manual approval to benchmark until fixed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add manual approval to benchmark until fixed

Alternatively we could revert https://github.com/hyperledger/besu/commit/ce28aae8b1c789298097deba0b4acc188e5088cb


Signed-off-by: Antony Denyer <git@antonydenyer.co.uk>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-30 13:08:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2823" class=".btn">#2823</a>
            </td>
            <td>
                <b>
                    Fix changelog to have bug fix under correct version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix changelog to have bug fix under correct version

Signed-off-by: Antony Denyer <git@antonydenyer.co.uk>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-30 11:11:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2822" class=".btn">#2822</a>
            </td>
            <td>
                <b>
                    Feature/merge get payload
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
in support of test mergenet:
 * add MergeBlockCreator
 * remove some of the rayonism hacks

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
addresses merge-488

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 23:15:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2821" class=".btn">#2821</a>
            </td>
            <td>
                <b>
                    Jumpdest constructor inj
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
Alternate implementation of [this PR](https://github.com/hyperledger/besu/pull/2809), which does not require a singleton for the jumpdest cache.
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #2607 

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 15:19:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2820" class=".btn">#2820</a>
            </td>
            <td>
                <b>
                    test benchmark CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Taccat Isid <taccatisid@protonmail.com>

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
        Created At 2021-09-29 01:47:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2819" class=".btn">#2819</a>
            </td>
            <td>
                <b>
                    added trace logging for ip -> dns when checking smart contract permissioning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>
Added some logging so users can see more details on what is being resolved and what is being rejected/permitted with regard to IP and DNS versions of enode. This will help when troubleshooting DNS + permissioning.

```
2021-09-29 11:08:50.183+10:00 | vert.x-eventloop-thread-2 | TRACE | NodePermissioningController | Node permissioning: Checking enode://3548c87b9920ff16aa4bdcf01c85f25117a29ae1574d759bad48cc9463d8e9f7c3c1d1e9fb0d28e73898951f90e02714abb770fd6d22e90371882a45658800e9@127.0.0.1:40404 -> enode://fcbe9f83218487b3c0b50878193880e6c25cfd86708c0a0bf0ca91f0ce633746a892fe240afa5b9a880b8bca48e8a22704ef937fdda2d7cc63e4d41ed1b417ae@127.0.0.1:30303
2021-09-29 11:08:50.186+10:00 | vert.x-eventloop-thread-2 | INFO  | NodeSmartContractV2PermissioningController | Permitted? false for IP enode://3548c87b9920ff16aa4bdcf01c85f25117a29ae1574d759bad48cc9463d8e9f7c3c1d1e9fb0d28e73898951f90e02714abb770fd6d22e90371882a45658800e9@127.0.0.1:40404
2021-09-29 11:08:50.189+10:00 | vert.x-eventloop-thread-2 | INFO  | NodeSmartContractV2PermissioningController | Permitted? false for DNS enode://3548c87b9920ff16aa4bdcf01c85f25117a29ae1574d759bad48cc9463d8e9f7c3c1d1e9fb0d28e73898951f90e02714abb770fd6d22e90371882a45658800e9@localhost:40404
2021-09-29 11:08:50.190+10:00 | vert.x-eventloop-thread-2 | TRACE | NodePermissioningController | Node permissioning - NodeSmartContractV2PermissioningController: Rejected enode://3548c87b9920ff16aa4bdcf01c85f25117a29ae1574d759bad48cc9463d8e9f7c3c1d1e9fb0d28e73898951f90e02714abb770fd6d22e90371882a45658800e9@127.0.0.1:40404 -> enode://fcbe9f83218487b3c0b50878193880e6c25cfd86708c0a0bf0ca91f0ce633746a892fe240afa5b9a880b8bca48e8a22704ef937fdda2d7cc63e4d41ed1b417ae@127.0.0.1:30303
```

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 01:13:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2818" class=".btn">#2818</a>
            </td>
            <td>
                <b>
                    Rename: OffChain -> offchain
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

We are treating "offchain" as a single word.
Rename refactor. See #2750 for "onchain" change

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 00:15:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2817" class=".btn">#2817</a>
            </td>
            <td>
                <b>
                    Qbft RPCs should be disabled after starting with or switching to use validator contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Qbft RPCs should be disabled after starting with or switching to use validator contract
Signer metrics and getValidatorsByBlock... should remain enabled.

## Fixed Issue(s)
Related to https://github.com/hyperledger/besu/issues/2795

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 19:45:53 +0000 UTC
    </div>
</div>

