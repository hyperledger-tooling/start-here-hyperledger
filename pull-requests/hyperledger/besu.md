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
                PR <a href="https://github.com/hyperledger/besu/pull/6130" class=".btn">#6130</a>
            </td>
            <td>
                <b>
                    Add `rpc-gas-cap` to CLI options
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
This PR introduces the CLi option`rpc-gas-cap` which allows users to limit the amount of gas used by the  RPC methods `eth_call` and `eth_getEstimateGas`. 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #6042 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-06 14:47:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6127" class=".btn">#6127</a>
            </td>
            <td>
                <b>
                    Log missing chain head as warning, not trace
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Change `CHAIN_HEAD_NOT_AVAILABLE` to a warning, not a trace log entry

## Fixed Issue(s)
Fixes #6126 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-06 11:02:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6122" class=".btn">#6122</a>
            </td>
            <td>
                <b>
                    [#5561]migrate tests to junit5
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
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-05 02:36:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6121" class=".btn">#6121</a>
            </td>
            <td>
                <b>
                    5571migrate tests to junit5
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
issue #5571 
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-05 00:10:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6119" class=".btn">#6119</a>
            </td>
            <td>
                <b>
                    Update RPCs for yParity
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

* Update the GraphQL and JSON-RPC endpoints to provide `yParity` instead of `v` for non-legacy transactions.
* Update the JSON-RPC tests to use the Hive data. 
* Add JSON-RPC tests for Shanghai and Cancun blocks/fields.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-03 17:29:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6117" class=".btn">#6117</a>
            </td>
            <td>
                <b>
                    clean up the ProcessableBlockHeader
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

This removes a few fields that don't make sense and that are not used in the existing core/ProcessableBlockHeader class. 
This introduces a interface ProcessableBlockHeader in the plugin module.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-03 03:43:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6116" class=".btn">#6116</a>
            </td>
            <td>
                <b>
                    Pipeline for debug RPC endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Increase efficiency by using pipeline for debug block endpoints

Refs #5322 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-03 02:20:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6114" class=".btn">#6114</a>
            </td>
            <td>
                <b>
                    Reference Tests v13
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

v13 of the official Ethereum Reference Tests.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-02 15:06:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6110" class=".btn">#6110</a>
            </td>
            <td>
                <b>
                    [MINOR] - Add 23.10.1 correct changelog
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add 23.10.1 final changelog

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-01 03:36:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6109" class=".btn">#6109</a>
            </td>
            <td>
                <b>
                    Restore javadoc and sources jar as trusted artifacts
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

Makes Idea happy again as documented here https://docs.gradle.org/6.8.3/userguide/dependency_verification.html#sec:skipping-javadocs

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-31 10:58:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6108" class=".btn">#6108</a>
            </td>
            <td>
                <b>
                    [IGNORE] loading test for trie log pruner
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
        Created At 2023-10-30 21:05:40 +0000 UTC
    </div>
</div>

