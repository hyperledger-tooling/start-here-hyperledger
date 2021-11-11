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
                PR <a href="https://github.com/hyperledger/besu/pull/3042" class=".btn">#3042</a>
            </td>
            <td>
                <b>
                    deprecation: replace calls to isEqualToComparingFieldByField 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                with usingRecursiveComparison().isEqualTo

Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Simple find and replace. 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-11 06:57:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3041" class=".btn">#3041</a>
            </td>
            <td>
                <b>
                    Updating the jacoco toolVersion
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Jacoco failed to instrument some tests using the old version of the tool
when build under jdk17

Signed-off-by: Jiri Peinlich <jiri.peinlich@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

Fixes #3040

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-11 06:26:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3039" class=".btn">#3039</a>
            </td>
            <td>
                <b>
                    Shift Optimization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Reduce shift calculations to shifts that may have an actual result.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>


## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-11 05:50:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3037" class=".btn">#3037</a>
            </td>
            <td>
                <b>
                    Maintainers: move to emeritus x 3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

I propose moving the following maintainers to Emeritus status, pursuant to the inactivity clause. These maintainers have had no activity during Q3 2021 (since July 2021):
* @edwardmac - last commit was in Nov 2020
* @rain-on - last commit was in Mar 2021
* @davemec - last commit was in May 2021

We very much appreciate their contributions but moving their status to emeritus (and thus revoking PR approval privileges) is in the interest of an orderly project. If any of these maintainers express in this PR that they intend to make contributions in the next quarter, then they will not be moved to emeritus status.
I propose this vote be open until either an absolute majority of active maintainers (13) votes for the same outcome, or until two weeks has passed (25 Nov 2021), after which a voting majority will determine the outcome (with a tie resulting in no change).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-11 04:32:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3036" class=".btn">#3036</a>
            </td>
            <td>
                <b>
                    [MINOR] updated comment and added link to generateId code in Tessera
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">privacy</span><span class="chip">TeamRevenant</span>
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Added link to relevant Tessera code for generating privacy group ID

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-11 01:58:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3035" class=".btn">#3035</a>
            </td>
            <td>
                <b>
                    Fix sepolia copypasta
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
fix incorrect discovery port on geth sepolia config


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 19:36:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3034" class=".btn">#3034</a>
            </td>
            <td>
                <b>
                    Update Sepolia bootnode, peer logging
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
* update sepolia bootnode to reflect EF's new sepolia boot node
* add peer details to debug logging


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 17:11:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3033" class=".btn">#3033</a>
            </td>
            <td>
                <b>
                    Fix dns discovery issue 
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

We are creating but not starting the dns discovery daemon. After this modification the node find peers instantly.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 16:58:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3032" class=".btn">#3032</a>
            </td>
            <td>
                <b>
                    improve perf trace
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
        Created At 2021-11-10 13:10:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3031" class=".btn">#3031</a>
            </td>
            <td>
                <b>
                    [MINOR] add download link for 21.10.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

added download link and hash for 21.10.1

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 08:27:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3028" class=".btn">#3028</a>
            </td>
            <td>
                <b>
                    Update VoteTallyCache when transitioning to blockheader validatorselectionmode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                TODO:
 - discuss that the cache is overriding validators for parent block (instead of block being produced) - maybe we should only set the cache once the block is successfully created? In reality this shouldn't matter since the parent block should be a contract-mode block and therefore have no cache entry.
 - discuss cache not just getting set once, but every execution of ForkingValidatorProvider.getValidators while producing the transition block.
 - try to recreate bug where network was stopped before node2 imported block, then got InvalidBlock

https://github.com/hyperledger/besu/issues/3019
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 13:13:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3027" class=".btn">#3027</a>
            </td>
            <td>
                <b>
                    [3026] Updating version of disovery dependency 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: Jiri Peinlich <jiri.peinlich@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
The discovery dependency is responsible for handling the v5 version of the discovery process of peers. This PR is updating the version to the latest. The project changed versioning after 0.5.0. The following version was 21.10.0 as can be seen on
the [release page](https://github.com/ConsenSys/discovery/releases).
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3027 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 10:33:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3025" class=".btn">#3025</a>
            </td>
            <td>
                <b>
                    [3011] Calling SignatureAlgorithmFactory::resetInstance before test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: Jiri Peinlich <jiri.peinlich@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
The NodeKeyTest might fail in case the SignatureAlgorithmFactory has an
instance already set from some previous test.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
fixes #3011 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 10:23:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3024" class=".btn">#3024</a>
            </td>
            <td>
                <b>
                    Prepare for 21.10.2-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

gradle.properties to 21.10.2-SNAPSHOT version
and added placeholder in changelog

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 04:48:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3023" class=".btn">#3023</a>
            </td>
            <td>
                <b>
                    Release 21.10.1
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
        Created At 2021-11-09 01:57:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3022" class=".btn">#3022</a>
            </td>
            <td>
                <b>
                    Maintainer: add Taccat Isid 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

I propose to add @taccatisid as a Besu project maintainer.

@taccatisid has contributed with many high quality commits:

Here are their past contributions on Besu project
- https://github.com/hyperledger/besu/pull/2644
- https://github.com/hyperledger/besu/pull/2674
- https://github.com/hyperledger/besu/pull/2717
- https://github.com/hyperledger/besu/pull/2805
- https://github.com/hyperledger/besu/pull/2956

<!-- for non-code contributors -->
@taccatisid also contributed with many high quality actions:

Quality code reviews eg 
- https://github.com/hyperledger/besu/pull/2994
- https://github.com/hyperledger/besu/pull/2971

Voting ends 2 weeks from the publication of this PR or once a majority of the maintainers [vote](https://github.com/hyperledger/besu/blob/main/MAINTAINERS.md#maintainers-approval-process).

For more information on this process see the Becoming a Maintainer section in the MAINTAINERS.md file.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 20:38:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3021" class=".btn">#3021</a>
            </td>
            <td>
                <b>
                    Fix a double execution of the same method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

description in https://github.com/hyperledger/besu/issues/3020

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3020

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 18:09:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3018" class=".btn">#3018</a>
            </td>
            <td>
                <b>
                    JsonUtil.normalizeKeys should handle ArrayNodes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
- Updated JsonUtils to handle ArrayNode. This is important now that we have bft transitions that are specified in an array in the genesis file.

## Fixed Issue(s)
fixes #2856

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 05:15:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3017" class=".btn">#3017</a>
            </td>
            <td>
                <b>
                    [2981] Multi algorithm support for JWT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Frank Li <b439988l@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

This PR allows the user to specify a JWT key algorithm when starting a node with http auth, and the algorithm will then be used with the provided public key.

- Added acceptance tests with login and authorised routes example usage
- Added unit tests for parsing of the public key file and creating JWTAuthOptions
- Added command line argument 'rpc-http-authentication-jwt-algorithm'
- Added test public key - JWT sets
- Added to change log

## Note for reviewers

The deprecation warnings will be flagged by sonar cloud, however it seems we're on a version of vert.x where some methods are flagged as deprecated but the replacement is not available.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #2981 

## Changelog

Add support for additional JWT auth algorithms and associated tests

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 04:39:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3016" class=".btn">#3016</a>
            </td>
            <td>
                <b>
                    separate step for sonar
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dev experience</span><span class="chip">TeamRevenant</span>
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Separate SonarQube into its own step since it uses a restricted context

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 02:24:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3014" class=".btn">#3014</a>
            </td>
            <td>
                <b>
                    More BFT tracing log messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
- Add a trace log message when `BftProtocolManager` receives a subprotocol message. This is the entry-point for BFT related logic in response to the message.

## Fixed Issue(s)
N/A

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 01:43:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3008" class=".btn">#3008</a>
            </td>
            <td>
                <b>
                    When tls is on, use plain framer and handshaker to avoid double encryption
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When tls is on, use passthrough framer and passthrough handshaker to avoid double encryption

Signed-off-by: Saravana Perumal Shanmugam <perusworld@linux.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 19:39:03 +0000 UTC
    </div>
</div>

