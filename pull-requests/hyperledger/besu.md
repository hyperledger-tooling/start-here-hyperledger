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
                PR <a href="https://github.com/hyperledger/besu/pull/3351" class=".btn">#3351</a>
            </td>
            <td>
                <b>
                    Release 22.1.0 rc4
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
Update the next rc to RC5-SNAPSHOT

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-31 03:35:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3350" class=".btn">#3350</a>
            </td>
            <td>
                <b>
                    2914 execution specific endpoint
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
Adds dedicated http service for just the engine apis.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2914

## Changelog
- Adds ability to specify Engine API endpoint on its own port, using --engine-rpc-http-port

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-31 02:14:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3349" class=".btn">#3349</a>
            </td>
            <td>
                <b>
                    Release 22.1.0 rc4
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
Release candidate

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-31 02:04:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3347" class=".btn">#3347</a>
            </td>
            <td>
                <b>
                    Bugfix/merge mining fix
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

* add kintsugi-v1 network parameter
* separate block producer CLI params from mining-only params
* ensure execution engine can operate with or without coinbase
* TransitionCoordinator correctly starts/restarts mining operations on the basis of mining parameters 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#3321 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-29 00:50:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3346" class=".btn">#3346</a>
            </td>
            <td>
                <b>
                    change dependencies for trivy scan step
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

small executor does not have sudo
but we don't need libSodium install in order to scan the docker image

See #3293 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-28 20:12:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3344" class=".btn">#3344</a>
            </td>
            <td>
                <b>
                    Changed almost all test classes to MockitoJunitRunner
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->
Signed-off-by: Swarnim Pratap Singh swarnimpratap132@gmail.com

## PR description
Changes remaining classes to MockitoJunitRunner test classes as much as possible in the main directory in besu/src/test/java/org/hyperledger/besu
 Only class files of ForkIdsTest(running with Parameterized.class) and PrivacyReordTest(Test failed with MockitoJunitRunner) were not converted

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2951

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-28 16:15:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3342" class=".btn">#3342</a>
            </td>
            <td>
                <b>
                    Eliminate connect to self
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prevent connecting to self enode.

See #2689 and #3322

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-28 05:10:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3341" class=".btn">#3341</a>
            </td>
            <td>
                <b>
                    backport merge updates to main
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

update main with merge specific changes:
* slf4j lambda shim
* execute payload bugfix from kintsugi consensus issue

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-28 01:06:22 +0000 UTC
    </div>
</div>

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

