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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2857" class=".btn">#2857</a>
            </td>
            <td>
                <b>
                    stop syncing at terminal total difficulty, add MergeBlockImporter whi…
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

* add MergeBlockImporter
* add TTD to syncState to prevent re-syncing when we have already sync'd up-to/past TTD

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-06 18:23:44 +0000 UTC
    </div>
</div>

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

