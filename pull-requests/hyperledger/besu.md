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
                PR <a href="https://github.com/hyperledger/besu/pull/3594" class=".btn">#3594</a>
            </td>
            <td>
                <b>
                    change snapshot version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Frank Li <b439988l@gmail.com>

Change snapshot version to 21.1.3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 05:59:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3592" class=".btn">#3592</a>
            </td>
            <td>
                <b>
                    address some sonar cloud bugs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

constants for strings and check some optionals.
Also changed the engineHttpUrl() method to use the engine host 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 05:14:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3591" class=".btn">#3591</a>
            </td>
            <td>
                <b>
                    Display data storage options in CLI help
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                Signed-off-by: Diego López León <dieguitoll@gmail.com>

## PR description
This is a leftover from #3578 to display the new stable options in the `--help` output
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 04:52:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3590" class=".btn">#3590</a>
            </td>
            <td>
                <b>
                    Do not merge: test tuweni 2.2 RC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Only for testing the tuweni 2.2 RC

Signed-off-by: Stefan Pingel <stefan.pingel@consensys.net>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 04:42:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3589" class=".btn">#3589</a>
            </td>
            <td>
                <b>
                    Release 22.1.2
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
        Created At 2022-03-16 04:30:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3586" class=".btn">#3586</a>
            </td>
            <td>
                <b>
                    Reduce the capacity of the transactions worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The previous queue capacity was too big since currently Besu is able
to process some thousand of transaction messages per second.

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
        Created At 2022-03-15 14:17:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3585" class=".btn">#3585</a>
            </td>
            <td>
                <b>
                    Add group heading to command options
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

This PR continues to group the CLI options together.

- JSON-RPC HTTP
- JSON-RPC WebSockets
- Metrics
- Miner
- Privacy
- Permissions
- Tx poo

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
fixes #2757 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-15 10:30:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3583" class=".btn">#3583</a>
            </td>
            <td>
                <b>
                    Add group heading to command options
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
This PR continues to group the CLI options together. 
- JSON-RPC HTTP
- JSON-RPC WebSockets
- Metrics
- Miner
- Privacy
- Permissions
- Tx pool

## Fixed Issue(s)
fixes #2757 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-14 17:33:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3580" class=".btn">#3580</a>
            </td>
            <td>
                <b>
                    [MINOR] corrections to changelog and typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Fixed some typos including in the CHANGELOG

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-14 01:40:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3579" class=".btn">#3579</a>
            </td>
            <td>
                <b>
                    WebSocket batch test - remove Ignore
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-13 23:43:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3578" class=".btn">#3578</a>
            </td>
            <td>
                <b>
                    Remove -x flag for bonsai CLI options
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
Removes -X from the bonsai flags so users feel safer using the options as bonsai have been tested extensively, note forest will still be the default storage format.

## Changelog
Add to breaking changes (should we support the -X flag for a little longer?)

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-13 23:37:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3577" class=".btn">#3577</a>
            </td>
            <td>
                <b>
                    Added --version flag to subcommands [#2762]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Davide Savazzi <davide@davidesavazzi.net>

## PR description

Added --version flag to subcommands. Added a test for each subcommand.

## Fixed Issue(s)

fixes #2762

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-13 16:35:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3575" class=".btn">#3575</a>
            </td>
            <td>
                <b>
                    add execution engine endpoints to docker ports
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
add 8550 and 8551 to the besu image Dockerfiles

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3574 

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-12 00:46:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3573" class=".btn">#3573</a>
            </td>
            <td>
                <b>
                    Update TTD for Kiln
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## PR description

The TTD for Kiln has been updated. This PR adds the new one to the Kiln genesis file
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-11 15:45:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3572" class=".btn">#3572</a>
            </td>
            <td>
                <b>
                    [SNAPSYNC] Add range proof validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">snapsync</span>
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

This PR will be followed by many PRs to add snapsync compatibility to Besu.

This PR add the range proof validation that will be necessary later

NB: This feature is still experimental and may still change a lot. More tests will be added later when it will be close to the final version 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-11 08:50:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3571" class=".btn">#3571</a>
            </td>
            <td>
                <b>
                    [MINOR] xl executor for quorum ATs (nightly)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Revert back to the xlarge executor for Quorum ATs

Last time these tests were consistently passing, the config looked like this https://github.com/hyperledger/besu/commit/1c39d4814327b8b095a8801adcb2332a12e19bb6

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-11 05:24:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3569" class=".btn">#3569</a>
            </td>
            <td>
                <b>
                    Warn if consensus client doesn't call transition configuration endpoint within 120 seconds
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
Adds a QoS timer behavior to `engine_exchangeTransitionConfigurationV1` rpc method 

[implements 120 second QoS warning](https://github.com/ethereum/execution-apis/blob/main/src/engine/specification.md#specification-3)

If the RPC method is not configured, there will be no such warning.  

Example log warning:

`2022-03-10 19:40:30.853-08:00 | vert.x-eventloop-thread-1 | WARN  | EngineExchangeTransitionConfiguration | not called in 120 seconds, consensus client may not be connected`

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3561

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-11 03:51:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3568" class=".btn">#3568</a>
            </td>
            <td>
                <b>
                    Added debug logging.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Mark Terry <mark.terry@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Added some debug logging to clarify the state when the IllegalArgumentException is thrown while downloading headers.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Related to #3336 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-11 00:04:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3567" class=".btn">#3567</a>
            </td>
            <td>
                <b>
                    Revert "upgrade vertx (#3530)"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit 9d2d87e954f5f74007d64dffd11a5f2f742d938b.

Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Revert the version of vertx just in case it is responsible for the change in behaviour of the WebSocket batch request test
## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-10 23:53:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3566" class=".btn">#3566</a>
            </td>
            <td>
                <b>
                    ignore flaky test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Ignoring flaky websocket batch test 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-10 23:45:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3565" class=".btn">#3565</a>
            </td>
            <td>
                <b>
                    remove requirement for CL to have zero blocknumber
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
Super simple PR to remove zero blocknumber requirement CL TransitionConfiguration


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#3560 

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-10 23:23:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3564" class=".btn">#3564</a>
            </td>
            <td>
                <b>
                    updated tests to ensure hex values are returned
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Uses Quantity for consistent formatting.

## Fixed Issue(s)
fixes #3563 

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-10 21:55:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3559" class=".btn">#3559</a>
            </td>
            <td>
                <b>
                    Add headings to Besu help
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sandra Wang <yx97.wang@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
fixes #2757 
## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-10 16:08:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3556" class=".btn">#3556</a>
            </td>
            <td>
                <b>
                    modified batch request test to avoid async complete issue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Send 2 x the same request as the batch. The request of "" seems to cause different behaviour.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-10 04:32:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3554" class=".btn">#3554</a>
            </td>
            <td>
                <b>
                    Stratum mining errata
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
This PR addresses a couple bits of additional plumbing to ensure transitionCoordinator correctly routes stratum ethash observers


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#3541

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-10 03:11:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3553" class=".btn">#3553</a>
            </td>
            <td>
                <b>
                    added trace logging of parameter RPC calls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

LOG.trace of all supplied RPC params

## PR description

Fixes 

## Changelog #3528 

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-10 02:49:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3552" class=".btn">#3552</a>
            </td>
            <td>
                <b>
                    update picocli
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span><span class="chip">dependencies</span>
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Update versions
* pico CLI
* gRPC
* mockito
* kubernetes client

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-10 01:54:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3551" class=".btn">#3551</a>
            </td>
            <td>
                <b>
                    added extra info to issue template
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Added some suggestions for extra info that may be relevant especially for smart contract related issues.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-10 01:02:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3550" class=".btn">#3550</a>
            </td>
            <td>
                <b>
                    Refactor TomlAuth  with AuthenticatioProvider
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: Sandra Wang <yx97.wang@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
This PR is to refactor authenticationprovider dependencies
If I am not mistaken, this would be the last PR for issue#2766

## Fixed Issue(s)
fixes: #2766 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-09 20:32:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3548" class=".btn">#3548</a>
            </td>
            <td>
                <b>
                    check types before providing a PowMiningCoordinator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Adds conditionals around assumptions on type of MiningCoordinator

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3541 

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-09 17:32:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3547" class=".btn">#3547</a>
            </td>
            <td>
                <b>
                    add kiln network, add network option for fast-sync capable
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
* Add kiln network 
* add NetworkName enum param for whether a named network can fast sync or not
* set kiln to full-sync only (for now)

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#3545

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-09 17:17:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3546" class=".btn">#3546</a>
            </td>
            <td>
                <b>
                    Richer return information for Precompiled Contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description

Allow precomiled contracts to return richer information instead of
results/fail. System/precompile contracts can now revert, fail, refund
gas, etc. instead of just succeed or fail.

This also had the nice effect of removing some hard-coded names for privacy contracts in the EVM code, which decouples it from privacy and frees up privacy for easier evolution.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-09 17:07:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3544" class=".btn">#3544</a>
            </td>
            <td>
                <b>
                    Always show privacyGroupId on PrivateTransactionReceipt
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - This is to provide a clearer way of knowing which `privacyGroupId` a private transaction ended up in.

Signed-off-by: Antony Denyer <git@antonydenyer.co.uk>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-09 11:12:43 +0000 UTC
    </div>
</div>

