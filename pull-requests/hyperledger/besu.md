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
                PR <a href="https://github.com/hyperledger/besu/pull/3803" class=".btn">#3803</a>
            </td>
            <td>
                <b>
                    ignore failing test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

This test is consistently passing locally but failing in CI. Ticket here to figure it out - but in the meantime, ignoring it to unblock other PRs. 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-08 23:31:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3800" class=".btn">#3800</a>
            </td>
            <td>
                <b>
                    Initial commit - reputation improvements.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: mark-terry <mark.terry@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Modifies the existing strike/point based behaviour to a more strict point based system.

## Fixed Issue(s)
Part of #3659 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-08 12:40:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3799" class=".btn">#3799</a>
            </td>
            <td>
                <b>
                    Log host and port when starting metrics service.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

The metrics service start message was logging the port twice, rather than the host and port as expected.  This changes the log message to print the correct information in standard host:port format.

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-07 11:04:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3795" class=".btn">#3795</a>
            </td>
            <td>
                <b>
                    [MINOR] Refactor to eliminate deprecated ExpectedException.none
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                refactor tests to use assertThatThrownBy rather than ExpectedException.none

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-06 05:20:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3794" class=".btn">#3794</a>
            </td>
            <td>
                <b>
                    Fix for node returns 5 nodes in 4 node network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change needs to be tested against a test net and maybe mainnet before it can be merged into main.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-06 05:16:45 +0000 UTC
    </div>
</div>

