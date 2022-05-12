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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3793" class=".btn">#3793</a>
            </td>
            <td>
                <b>
                    Add code hash check to fast sync
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

add  a check in CodeNodeDataRequest to ensure code is not only present, but matches the expected hash.  This is necessary for bonsai databases since the code is stored by account hash rather than code hash.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-05 22:28:48 +0000 UTC
    </div>
</div>

