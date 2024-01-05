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
                PR <a href="https://github.com/hyperledger/besu/pull/6353" class=".btn">#6353</a>
            </td>
            <td>
                <b>
                    WIP: QBFT + shanghai support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Implement shanghai support for QBFT and IBFT chains

## Fixed Issue(s)
Fixes https://github.com/hyperledger/besu/issues/5446
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-04 17:42:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6352" class=".btn">#6352</a>
            </td>
            <td>
                <b>
                    Rel 24.1.0-RC2 cherry pick - cancun
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
small cherry-pick to mark Cancun as finalized

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-04 17:05:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6351" class=".btn">#6351</a>
            </td>
            <td>
                <b>
                    finalized cancun spec
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
        Created At 2024-01-04 16:07:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6350" class=".btn">#6350</a>
            </td>
            <td>
                <b>
                    Migrate BFT tests to junit 5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                builds on #6339 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-04 07:55:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6347" class=".btn">#6347</a>
            </td>
            <td>
                <b>
                    Set build version to 24.1.0-SNAPSHOT
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
bump gradle properties version and adjust changelog to match release

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-03 20:23:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6345" class=".btn">#6345</a>
            </td>
            <td>
                <b>
                    Use synchronized call to access the chain head block in estimateGas()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Optimistically get the chain head block without taking a lock. If that fails, retry under the lock.

This is an identical fix to https://github.com/hyperledger/besu/pull/6143.

I did consider making a more generic helper/util function to wrap the logic for any place in the code that needs it, but looking through the code I can't see any other cases where the a failed attempt to get the chain head block results in an internal error or exception. Most others treat it as optional and just retry on the next go round.

## Fixed Issue(s)
Fixes https://github.com/hyperledger/besu/issues/6344
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-03 16:06:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6343" class=".btn">#6343</a>
            </td>
            <td>
                <b>
                    Make RPC reason settable, pass execution failure reason in RPC error message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR adds a setter for the `reason` field in `JsonRpcError`.

If a caller sets the `reason`, it is appended to the message for the error that is taken from the `RpcErrorType` enums.

It also adds a new `RpcErrorType` of `EXECUTION_HALTED` to be used during transaction simulations (e.g. during `eth_estimateGas()` calls) so a failed gas estimation doesn't just return `INTERNAL_ERROR` when there's a problem with the execution.

The specific example I hit this in was using a Shanghai smart contract with the `JUMP0` opcode against a QBFT Besu node (QBFT doesn't currently support Shanghai).

## Fixed Issue(s)
Fixes #4914 
(See also https://github.com/hyperledger/besu/pull/5706 which improves the error messages sent back to the user for reverted transactions)

## TODO before taking out of draft
 - [x] Unit test fixes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-03 14:44:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6341" class=".btn">#6341</a>
            </td>
            <td>
                <b>
                    Update dependencies
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
        Created At 2024-01-03 13:06:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6340" class=".btn">#6340</a>
            </td>
            <td>
                <b>
                    Fix trielog shipping issue during self destruct
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

Fix trielog shipping issue during self destruct 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-03 11:27:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6339" class=".btn">#6339</a>
            </td>
            <td>
                <b>
                    TestWatcher junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                migrate the TestWatcher functionality from junit 4 Rule to junit 5

fixes #6348

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-03 07:05:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6338" class=".btn">#6338</a>
            </td>
            <td>
                <b>
                    [MINOR] migrate controller builder test junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #5571 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-03 01:38:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6337" class=".btn">#6337</a>
            </td>
            <td>
                <b>
                    [MINOR] made directory structure of subcommands tests match source
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                tidying up
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-03 00:32:39 +0000 UTC
    </div>
</div>

