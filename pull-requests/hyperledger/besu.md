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
                PR <a href="https://github.com/hyperledger/besu/pull/2547" class=".btn">#2547</a>
            </td>
            <td>
                <b>
                    Privacy plugin pmt signer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Allow plugin users to sign privacy marker transactions
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-19 12:37:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2545" class=".btn">#2545</a>
            </td>
            <td>
                <b>
                    Tx replacement rules
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
refactor of transaction replacement rules:
* split into gasPrice and 1559FeeMarket rules
* consider maxFeePerGas as well as maxPriorityFeePerGas in the transaction bump logic for 1559 fee market

1559 fee market logic is effectively:
* replace when BOTH:
  * new effective price  > prior effective price plus percent bump 
  * new effective priority fee is >= prior effective priority fee
* OR, replace when BOTH:
  * new effective price == prior effective price 
  * new effective priority fee > prior effective priority fee plus percent bump
* ELSE, don't replace



## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
fixes #2529

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-15 22:43:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2543" class=".btn">#2543</a>
            </td>
            <td>
                <b>
                    update changelog with 21.7.1 download link
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

post release CHANGELOG update

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 19:16:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2542" class=".btn">#2542</a>
            </td>
            <td>
                <b>
                    Prepare for version 21.7.2-SNAPSHOT
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
        Created At 2021-07-14 17:40:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2541" class=".btn">#2541</a>
            </td>
            <td>
                <b>
                    Release 21.7.1
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
        Created At 2021-07-14 17:09:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2539" class=".btn">#2539</a>
            </td>
            <td>
                <b>
                    [Spike] QBFT transaction-based voting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">enhancement</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
Spike for Qbft transaction based voting. This won't be merged as, it will be broken up into smaller PRs.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 04:31:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2538" class=".btn">#2538</a>
            </td>
            <td>
                <b>
                    ATs: update Tessera docker image version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Update to Tessera 21.7.0 in container tests setup

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 00:54:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2537" class=".btn">#2537</a>
            </td>
            <td>
                <b>
                    Add Justin Florentine as a maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Justin has made significant [commits](https://github.com/hyperledger/besu/commits?author=jflo) improving the quality and features of besu, this PR adds him as a maintainer.

Voting ends 2 weeks from the publication of this PR or once a majority of the maintainers [vote](https://github.com/hyperledger/besu/blob/master/MAINTAINERS.md#maintainers-approval-process).  

For more information on this process see the Becoming a Maintainer section in the MAINTAINERS.md file.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-13 22:02:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2536" class=".btn">#2536</a>
            </td>
            <td>
                <b>
                    p2p tls support (command line options and acceptance tests)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is the final part of the changes to support p2p over tls. this has command line options to support p2p over tls enablement and acceptance tests to cover them as well.
The keystores are generated using scripts from https://github.com/perusworld/besu-isolated-networks/blob/p2p-over-ssl/scripts/gen-at-keys.sh

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-13 17:00:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2535" class=".btn">#2535</a>
            </td>
            <td>
                <b>
                    update RPC methods : fill gasPrice for post london 1559 transaction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

For 1559 transactions returned on the rpc, we need to fill the gasPrice field as follows:
- effectivePriorityFeePerGas


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-13 14:26:59 +0000 UTC
    </div>
</div>

