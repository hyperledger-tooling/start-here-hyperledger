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
                PR <a href="https://github.com/hyperledger/besu/pull/3429" class=".btn">#3429</a>
            </td>
            <td>
                <b>
                    RocketChat -> Discord
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Replace Rocket Chat links with Discord. Reworded some links.

This does remove the badge from the top of the README. Requires Discord admin to setup if we want the equivalent for Discord. https://shields.io/category/chat

Fixes #3428 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-15 04:47:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3425" class=".btn">#3425</a>
            </td>
            <td>
                <b>
                    Replace Log4j2 with Logback
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
As a continuation of the work made on #3285 this PR completely removes Log4j2 as a project dependency, substituting its behaviour with Logback

This has been split into the following commits:
- [HEAD~6](https://github.com/diega/besu/commit/logback~6): renames leftover method from #3285
- [HEAD~5](https://github.com/diega/besu/commit/logback~5): removes Log4j2 usage dependencies relying on the `Log4j2ConfiguratorUtil` (this is for simplifying the last diff)
- [HEAD~4](https://github.com/diega/besu/commit/logback~4): replace Log4j2 `ThreadContext` usage with Slf4j's `MDC`
- [HEAD~3](https://github.com/diega/besu/commit/logback~3): this is to avoid problems with `ch.qos.logback.classic.Level` which deserializes silently to `DEBUG` level by default when an invalid value gets passed (e.g. `FATAL`)
- [HEAD~2](https://github.com/diega/besu/commit/logback~2): for the same reason than before, the level values are filtered by the received string
- [HEAD~1](https://github.com/diega/besu/commit/logback~1): addresses [java:S116](https://sonarcloud.io/organizations/hyperledger/rules?open=java%3AS116&rule_key=java%3AS116) Sonar rule
- [HEAD](https://github.com/diega/besu/commit/logback): replaces Log4j2 dependency with Logback. Removes custom Log4j2 management for dealing with ANSI colors by using conditionals in the Logback config file.

## TODO
- [ ] configure Splunk in `logback.xml` properly (cc @atoulme) 

## Documentation changes
[Configure logging](https://besu.hyperledger.org/en/stable/HowTo/Monitor/Logging/) wiki page will need to be updated. [This](https://logback.qos.ch/manual/configuration.html#configFileProperty) doc page explains how to override the default location of the configuration file. 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-14 14:57:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3424" class=".btn">#3424</a>
            </td>
            <td>
                <b>
                    Add backward sync unit tests missing from previous PR #3410
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Code originally written by gezero on the merge branch

Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

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
        Created At 2022-02-14 14:49:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3423" class=".btn">#3423</a>
            </td>
            <td>
                <b>
                    FullSync Future should stop when total terminal difficulty is reached
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jiri Peinlich <jiri.peinlich@gmail.com>

The Full sync future should finish executing once the terminal total difficulty is reached. Note that we will not stop syncing exactly at the TTD but we will finish syncing the current batch of blocks.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-14 13:47:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3421" class=".btn">#3421</a>
            </td>
            <td>
                <b>
                    Improve closing behavior of JsonResponseStreamer, and make clear it i…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …s managed bt the ObjectWriter

Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

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
        Created At 2022-02-14 10:25:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3419" class=".btn">#3419</a>
            </td>
            <td>
                <b>
                    3378 websocket engine
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
Websocket for Engine APIs can be configured separately.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3378 
## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-13 22:00:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3416" class=".btn">#3416</a>
            </td>
            <td>
                <b>
                    Reduce log level for invalid transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
When evaluating transactions to include in a block, a warn log message was evaluated for any transction found to be invalid. This was excessively noisy if the base fee had increased as many transactions were considered invalid.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-13 08:43:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3415" class=".btn">#3415</a>
            </td>
            <td>
                <b>
                    [Issue-3115] Fix mining beneficiary acceptance tests
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
Fix acceptance tests related to *bft mining beneficiaries:
* Only set genesis config if it is not already set.  
* Throw if test attempts to verify an empty `Cluster`.
* Configure genesis file with appropriate keys for consensus type ("ibft2", "qbft").

## Fixed Issue(s)
Part of #3115 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-12 19:35:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3413" class=".btn">#3413</a>
            </td>
            <td>
                <b>
                    Lgtm alert x 1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix 1 LGTM alerts 
* check null privacyPluginParams in BesuCommand

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-11 21:33:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3412" class=".btn">#3412</a>
            </td>
            <td>
                <b>
                    Merge: extend block creation and mining to support The Merge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Code originally written by garyschulte on the merge branch.
Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

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
        Created At 2022-02-11 16:02:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3411" class=".btn">#3411</a>
            </td>
            <td>
                <b>
                    Extend validateAndProcessBlock to return an error message in case of …
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …failure

This message can then be used to send a more detailed response to the RPC
caller of ExecutePayload API.

Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
https://github.com/hyperledger/besu/issues/3145

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-11 14:29:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3410" class=".btn">#3410</a>
            </td>
            <td>
                <b>
                    Merge: port of backward sync
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Code originally written by gezero on the merge branch
Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

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
        Created At 2022-02-11 13:55:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3409" class=".btn">#3409</a>
            </td>
            <td>
                <b>
                    Bug 3343
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

When asking for the forkId for the chain head sometimes we may return
null. In those cases return an empty list.


## Fixed Issue(s)

fixes 3343

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-11 06:49:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3405" class=".btn">#3405</a>
            </td>
            <td>
                <b>
                    fix NPE, issue 3335
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                https://github.com/hyperledger/besu/issues/3335
Signed-off-by: Stefan Pingel <stefan.pingel@consensys.net>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-11 03:18:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3404" class=".btn">#3404</a>
            </td>
            <td>
                <b>
                    Fix order in MAINTAINERS.md
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
        Created At 2022-02-11 03:05:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3403" class=".btn">#3403</a>
            </td>
            <td>
                <b>
                    Publish kintsugi final image
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
tagging tweak

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-11 02:47:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3402" class=".btn">#3402</a>
            </td>
            <td>
                <b>
                    Publish kintsugi final tag
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
update snapshot so that the docker image tag will reflect it is a kintsugi artifact

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-11 00:47:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3401" class=".btn">#3401</a>
            </td>
            <td>
                <b>
                    add kintsugi to publishDocker
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

add kintsugi as a branch we publish to docker from.  This is likely the only commit this branch will get as the network is nearing end-of-life

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-10 23:05:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3399" class=".btn">#3399</a>
            </td>
            <td>
                <b>
                    Response streaming: stop on IO error and remove queue management
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Queue management is removed, since it is not working at the moment,
and can cause deadlock, will be reimplemented later if needed.
Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3381
## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-10 13:36:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3397" class=".btn">#3397</a>
            </td>
            <td>
                <b>
                    Reject locally-sourced frontier transactions below the minimum gas price when not mining
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Reject locally-sourced frontier transactions below the minimum gas price when not mining.

Brings back some of the functionality that was taken out by https://github.com/hyperledger/besu/pull/1743

The main problem is that if you're not mining and send zero priced frontier transactions to the node it will fill up the transaction pool. 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-10 11:14:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3396" class=".btn">#3396</a>
            </td>
            <td>
                <b>
                    update open telemetry to 1.6.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

I updated all open telementry libs from 1.5.0 to 1.6.0 but that broke some ATs with NoClassDefFound https://app.circleci.com/pipelines/github/hyperledger/besu/13070/workflows/d1c5ed54-3cf9-4afc-a9f3-a9474a27468b/jobs/72564

So I reverted  'io.opentelemetry:opentelemetry-proto:1.5.0-alpha'

I am not 100% sure this combination of libs will work nicely together. But all tests pass

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 18:16:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3393" class=".btn">#3393</a>
            </td>
            <td>
                <b>
                    Add terminal block check to forkchoiceUpdated and executePayload
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
add check for descends from terminal block to engine_executePayload and engine_forkchoiceUpdated

* move isTerminalPoWBlock to TransitionUtils for re-use
* add check for isTerminalPoWBlock and recursion to MergeCoordinator
* expose latestValidAncestorDescendsFromTerminal in MergeMiningCoordinator interface
* remove unused parameter classes
* rename existing parameter classes to Engine* instead of Execution*

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3262 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 02:27:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3392" class=".btn">#3392</a>
            </td>
            <td>
                <b>
                    Merge: add terminal block number and hash to genesis config options
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ported from the merge branch.

Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

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
        Created At 2022-02-08 17:40:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3391" class=".btn">#3391</a>
            </td>
            <td>
                <b>
                    MERGE: new payload API for Kiln testnet
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
        Created At 2022-02-08 15:11:50 +0000 UTC
    </div>
</div>

