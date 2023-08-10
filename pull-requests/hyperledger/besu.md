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
                PR <a href="https://github.com/hyperledger/besu/pull/5756" class=".btn">#5756</a>
            </td>
            <td>
                <b>
                    Trigger `OperationTracer` on contexts enter & exit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Extends the `OperationTracer` interface to be triggered on contexts enter & exit.

@daniellehrner @shemnon 

## Fixed Issue(s)

Fixes #5728 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-07 22:25:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5755" class=".btn">#5755</a>
            </td>
            <td>
                <b>
                    EVMTool contract create processing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

The "code" mode of the EVMTool did not support the side effects of a contract create. Expose the TransactionProcessor method that handles that switching.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-07 18:48:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5754" class=".btn">#5754</a>
            </td>
            <td>
                <b>
                    Benchmarking in evmtool
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

Add a new benchmarking sub-command to `evmtool`

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-04 21:54:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5752" class=".btn">#5752</a>
            </td>
            <td>
                <b>
                    Rebase current EIP-6110 prototype to Cancun
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
This is to rebase the existed implementation of EIP-6110 from Shanghai to Cancun. As well, it updates the implementation according to the latest Engine API [specification](https://github.com/ethereum/execution-apis/blob/main/src/engine/experimental/eip6110.md).
Changes include:

- [x] Remove 6110 related changes from `engine_newPayloadV2` and `engine_getPayloadV2`
- [x] Rename `deposits` to `depositReceipts` in `EnginePayloadParameter`
- [x] Introduce `engine_newPayloadV6110` and `engine_getPayloadV6110` that are based on `engine_newPayloadV3` and `engine_getPayloadV3`
- [x] Revamp the existed 6110 acceptance test

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-04 08:32:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5750" class=".btn">#5750</a>
            </td>
            <td>
                <b>
                     23.7.1-RC burn in
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
RC burn-in release of 23.7.1:
 * cherry pick of #5734 performance regression fix
 * changelog revision to reflect 23.7.0 not released
 * change rev to 23.7.1-RC


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-03 20:41:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5749" class=".btn">#5749</a>
            </td>
            <td>
                <b>
                    Update native libraries
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

Use the 0.8.0 version of native libraries, which uses better names for automatic modules for JPMS.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-03 18:23:51 +0000 UTC
    </div>
</div>

