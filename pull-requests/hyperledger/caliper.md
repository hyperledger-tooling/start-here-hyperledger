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
                PR <a href="https://github.com/hyperledger/caliper/pull/1585" class=".btn">#1585</a>
            </td>
            <td>
                <b>
                    Implementation of Issue #1497 - Allow the Ethereum connector to use an already deployed contract
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
 - [ ]  Documentation - any JSDoc, website, or Stackoverflow answers?


## Issue/User story
Issue #1497 - Allow the Ethereum connector to use an already deployed contract

## Existing issues
- [x] [GitHub Issues](https://github.com/hyperledger/caliper/issues/1497)

## Design of the fix
To use a contract that is already deployed, an optional 'address' key may be specified on the [Contract Definition file](https://hyperledger.github.io/caliper/vNext/ethereum-config/#contract-definition-file). The new connector reads the 'address' key from the Contract Definition File, and if it exists, it does not deploy a new contract.

## Validation of the fix
Working on my local Besu network

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-31 17:45:05 +0000 UTC
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

