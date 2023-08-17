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
                PR <a href="https://github.com/hyperledger/besu/pull/5765" class=".btn">#5765</a>
            </td>
            <td>
                <b>
                    fix: prioritize fork error over missing payload fields
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * prioritize fork error over missing payload fields
* additional rpc error code for unsupported fork per https://github.com/ethereum/execution-apis/pull/426/files

fixes #5738
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-17 01:01:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5764" class=".btn">#5764</a>
            </td>
            <td>
                <b>
                    23.7.1-RC2 cherry-pick
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
cherry-pick #5749 into RC2

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-16 19:35:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5763" class=".btn">#5763</a>
            </td>
            <td>
                <b>
                    EvmTool fixes
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

A mixed collection of EVMTool fixes
* Ensure ECDSA algo is pre-configured
* used clamped math in an old gas calculator
* use correct gas calculator in fluent APIs

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-15 15:26:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5762" class=".btn">#5762</a>
            </td>
            <td>
                <b>
                    Make the `MessageFrame.isWarm(...)` method family public
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addresses #5761 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 23:34:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5760" class=".btn">#5760</a>
            </td>
            <td>
                <b>
                    Cancun genesis tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - fixes genesis block calculations when started post cancun
- refactors engine api tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 22:38:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5759" class=".btn">#5759</a>
            </td>
            <td>
                <b>
                    Migrate DataGas to BlobGas
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

In all places move from DataGas to BlobGas when talking about 4844 gas.

This addresses the issue I've seen with multiple PRs for blob gas testing having to update JSON fields ad-hoc.  This PR changes them all in one go.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 18:33:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5758" class=".btn">#5758</a>
            </td>
            <td>
                <b>
                    Eip4788 parentBeaconBlockRoot 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Adds support for EIP 4788 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-13 23:50:20 +0000 UTC
    </div>
</div>

