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
                PR <a href="https://github.com/hyperledger/besu/pull/2771" class=".btn">#2771</a>
            </td>
            <td>
                <b>
                    CHANGELOG: moved experimental features
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Moved QBFT experimental features to the "Early access features" section

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 23:58:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2770" class=".btn">#2770</a>
            </td>
            <td>
                <b>
                    Changelog for 21.7.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Move entires that were mistakenly added to 21.7.3 lists to 21.7.4.
Add entry for ETC gas calculator bug.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 21:30:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2769" class=".btn">#2769</a>
            </td>
            <td>
                <b>
                    Add additional minimum merge spec stubs  #474
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
* Stub out additional [minimum merge spec](https://gist.github.com/mkalinin/e26f1fe70df83a25834cc6a62b6afdac)  endpoints 



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 19:51:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2768" class=".btn">#2768</a>
            </td>
            <td>
                <b>
                    Refactor Pico CLI options to make usage consistent
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
        Created At 2021-09-15 14:39:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2767" class=".btn">#2767</a>
            </td>
            <td>
                <b>
                    Exclude qbft reference-test resources from spotless check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                ## PR description

Exclude qbft reference-test resources from spotless check as it was causing an error on a fresh build

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 09:59:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2763" class=".btn">#2763</a>
            </td>
            <td>
                <b>
                    Stub out new execution endpoint api, #474
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update json-rpc consensus API (474)
* change rpc endpoint to engine_* rather than consensus_*
* split consensus_assembleBlock into engine_preparePayload and engine_getPayload
* engine_preparePayload should be stubbed to return a success response
* engine_getPayload should repurpose consensus_assembleBlock

stub out:
* engine_executePayload
* engine_consensusValidated
* engine_forkChoiceUpdated

remove/repurpose:
* consensus_finalizeBlock
* consensus_newBlock
* consensus_setHead
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 00:01:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2761" class=".btn">#2761</a>
            </td>
            <td>
                <b>
                    Gradle 7.2 upgrade / Java 17 Build Support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Upgrade to Gradle 7.2, which supports Java 17
* Regenerate gradlew script and wrapper (as recommended)
* Suppress the removal warning for `AccessController` for now
* Update the JMH version to get rid of Gradle deprecation warning
* Add spotless `targetExcludes` so it won't re-format submodules

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 17:54:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2758" class=".btn">#2758</a>
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

Fixed a typo

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 04:04:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2754" class=".btn">#2754</a>
            </td>
            <td>
                <b>
                    Initial PoC for RPC end points via the plugin mechanism.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                ## PR description
re-implementation of https://github.com/PegaSysEng/pantheon/pull/1909/


Implements https://github.com/hyperledger/besu/issues/1317
## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 14:56:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2752" class=".btn">#2752</a>
            </td>
            <td>
                <b>
                    Metrics idle timeout is now configurable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
#2748 introduced a timeout for metrics TCP connections. With this PR user can set a value in seconds for that timeout.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-10 18:03:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2751" class=".btn">#2751</a>
            </td>
            <td>
                <b>
                    Remove duplication between Qbft protocol schedule and Ibft protocol schedule
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
Remove duplication between Qbft protocol schedule and Ibft protocol schedule

Note: This build on top of the qbft contract vote migration PR, once that is in this will be significantly smaller in changes.
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-10 05:58:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2748" class=".btn">#2748</a>
            </td>
            <td>
                <b>
                    Cleanup metrics connections after idle timeout
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When metrics are in use in teku (which uses besu metrics), and the prometheus service restarts, connections can be left open and never closed.

These connections should close after an idle timeout to avoid causing issues with running out of ports.

Reported in teku issue https://github.com/ConsenSys/teku/issues/4327 .

Signed-off-by: Paul Harris <paul.harris@consensys.net>

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-10 00:51:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2747" class=".btn">#2747</a>
            </td>
            <td>
                <b>
                    merge main into Rayonism
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                dust off the rayonism branch
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 23:01:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2746" class=".btn">#2746</a>
            </td>
            <td>
                <b>
                    Set TransactionGasCalculator in ETC specs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
On #2659 the gas calculator was split but the ETC specification wasn't properly updated, letting 21.7.3 nodes out of consensus.

## Fixed Issue(s)
Fixes #2715

## Changelog

- [ ] Update Ethereum Classic Phoenix and Magneto specs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 20:09:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2745" class=".btn">#2745</a>
            </td>
            <td>
                <b>
                    Add snap protocol message compatibility
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

Added the first part that allows to manage the reception and the response of snap messages as well as an experimental flag. Subsequently this flag will be deleted and SNAP will be put directly in the flag (sync-mode)

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 15:29:40 +0000 UTC
    </div>
</div>

