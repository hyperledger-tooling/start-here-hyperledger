---
layout: default
title: caliper
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/caliper
---

# caliper <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/caliper){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1591" class=".btn">#1591</a>
            </td>
            <td>
                <b>
                    Caliper Ethereum documentation overhaul
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Checklist
 - [x]  A link to the issue/user story that the pull request relates to
 - [ ]  How to recreate the problem without the fix
 - [ ]  Design of the fix
 - [ ]  How to prove that the fix works
 - [ ]  Automated tests that prove the fix keeps on working
 - [x]  Documentation

## Issue/User story
Caliper Ethereum documentation was outdated and did not provide information on using the `--caliper-flow-skip-install`  that skips the smart contract installation phase.

## Existing issues
- [x] [GitHub Issues](https://github.com/hyperledger/caliper/issues/1589)

Issue #1589 - Caliper ethereum documentation needs a complete overhaul

## Design of the fix
* Added information on how to use the `--caliper-flow-skip-install` to use pre-deployed contracts. Since the contract configuration on the network config file will differ depending on whether this flag is used, I added a subsection for each use case;
* Added a warning regarding the mandatory usage of `fromAddressSeed` when using more than 1 worker;
* Fixed name mismatches between the network config file keys;
* Added information about the TxStatus type - `getResut()` was not documented;
* Updated references to the old `invokeSmartContract` and `queryState` functions, with the new `sendRequests` function;
* Moved besu-specific warnings to the appropriate sections;
* Removed reference to a "special registry contract", which I haven't found any information about anywhere else.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-04 12:23:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1588" class=".btn">#1588</a>
            </td>
            <td>
                <b>
                    Target organisation for peer gateway docs
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
        Created At 2024-06-01 08:31:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1582" class=".btn">#1582</a>
            </td>
            <td>
                <b>
                    Add Support for Org targeting to peer gateway
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
        Created At 2024-05-31 13:12:12 +0000 UTC
    </div>
</div>

