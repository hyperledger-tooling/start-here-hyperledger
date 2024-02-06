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
                PR <a href="https://github.com/hyperledger/besu/pull/6501" class=".btn">#6501</a>
            </td>
            <td>
                <b>
                    Deprecate --Xp2p-peer-lower-bound
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                Deprecate CLI option --Xp2p-peer-lower-bound and remove usage

Fixes #6376
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-31 03:46:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6500" class=".btn">#6500</a>
            </td>
            <td>
                <b>
                    [MINOR] remove duplicate setting of default values for CLI options
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                where the default is number/boolean/string, just leave it to the initialized value for the actual field.

same as was done for Sync Options in #6499
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-31 01:44:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6499" class=".btn">#6499</a>
            </td>
            <td>
                <b>
                    Flat db heal - deprecate CLI option and set to always true
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * set flat db healing enabled to true always
* remove duplicate setup of default values from Sync Options class

refs #6157
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-31 01:26:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6498" class=".btn">#6498</a>
            </td>
            <td>
                <b>
                    Filter Discovered peers for ipv6 support
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
updates PeerDiscoveryAgent to 
* use existing NetworkUtility to filter for any/none peers
* fall back to source address if ipv6 is not supported (like in a docker container)

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #6475 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-31 01:01:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6496" class=".btn">#6496</a>
            </td>
            <td>
                <b>
                    [Refactor] Move graphqloptions to its own class
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Move GraphQl options options to its own class

## Fixed Issue(s)
see https://github.com/hyperledger/besu/issues/6428
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-30 21:46:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6493" class=".btn">#6493</a>
            </td>
            <td>
                <b>
                    add profile info to help footer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #6430 

depends on #6449

![Screenshot 2024-01-30 at 3 21 48 pm](https://github.com/hyperledger/besu/assets/2627919/81aef27d-340e-4bb4-8207-20788071812d)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-30 05:20:56 +0000 UTC
    </div>
</div>

