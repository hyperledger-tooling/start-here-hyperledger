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
                PR <a href="https://github.com/hyperledger/besu/pull/5277" class=".btn">#5277</a>
            </td>
            <td>
                <b>
                    Make QBFT validator smart contract mode work with london fork
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should work when gas fees are used as well as for free gas networks

Override the transactionSimulator's default TransactionValidationParams with one that allows for exceeding the account balance (which effectively zeros the baseFee). This mimics the way that eth_estimateGas and eth_call are implemented.

Fixes https://github.com/hyperledger/besu/issues/5249
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 07:50:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5276" class=".btn">#5276</a>
            </td>
            <td>
                <b>
                    Fix including excessDataGas when using a zero base fee
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
Fix including excessDataGas when using a zero base fee

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #5270 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 06:37:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5275" class=".btn">#5275</a>
            </td>
            <td>
                <b>
                    [MINOR] Add log to show where we're reading the jwt from
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
Add a log to print the path where we loaded the engine jwt for better ux.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 00:02:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5274" class=".btn">#5274</a>
            </td>
            <td>
                <b>
                    continue despite test failures
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I would like to propose some blasphemy:

we should run the weekly sonarqube job with gradle --continue so it proceeds on, regardless of test failure.

this week a flaky test failed, and so we got no analysis.
the sonarqube job produces no artifacts of any use, it is meant as a weekly diagnostic, so while blasphemous, I believe this to be safe.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-28 18:41:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5269" class=".btn">#5269</a>
            </td>
            <td>
                <b>
                    Update dependecies to latest version
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

For 23.4-RC

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-24 17:35:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5267" class=".btn">#5267</a>
            </td>
            <td>
                <b>
                    Update netty
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
        Created At 2023-03-24 17:14:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5266" class=".btn">#5266</a>
            </td>
            <td>
                <b>
                    reset cache after heal
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

We found that sometimes after the heal we still have old snapshot in the cache because after the clearTrieLog some transaction pool thread are still running 
The fix is to clear the cache after the snapsync and also add a snapshot of the  new head 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-24 12:14:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5265" class=".btn">#5265</a>
            </td>
            <td>
                <b>
                    Upgrade k8s and snakeyaml libs
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
fixes #5264
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-24 11:31:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5263" class=".btn">#5263</a>
            </td>
            <td>
                <b>
                    Cancel older block creation tasks upon receiving a new one
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

It make sense to have only a block creation task running at any time, but at the moment is it possible (especially on devnets) that two consecutive requests to build a block overlap, with the consequence that first task keeps running until the timeout, even if it is useless, since only the last one is relevant. 
This PR change this behavior, cancelling any existing block creation task, when a new block creation request arrives, and since only one task could be running, a single thread executor is used.
Then a minimum sleep period of 100ms is introduced between retries to reduce the concurrency with the transaction pool, so that it can process more possible candidate transaction for the next retry.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-24 11:04:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5262" class=".btn">#5262</a>
            </td>
            <td>
                <b>
                    Upgrade RocksDB version from 7.7.3 to 8.0.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Upgrade RocksDB version from 7.7.3 to 8.0.0.
Remove deprecated/obsolete RocksDB statistics in version 8.0.0.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-24 08:36:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5261" class=".btn">#5261</a>
            </td>
            <td>
                <b>
                    Use schedule.getForNextBlockHeader in WithdrawalsValidatorProvider
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Part of removing public usages of schedule.getByTimestamp If the parentHeader does not exist, we skip the withdrawals validation however the net result should be to sync in this scenario

Part of #5260 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-24 06:48:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5259" class=".btn">#5259</a>
            </td>
            <td>
                <b>
                    getByBlockNumber replaced by getByBlockHeader on tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
This PR removes the getByBlockNumber from tests and replace it's usage by getByBlockHeader.

## Fixed Issue(s)
Fixes #5165 
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-23 04:36:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5257" class=".btn">#5257</a>
            </td>
            <td>
                <b>
                    additional merkle trie refactoring
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
additional refactoring missed by #5251 
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-22 23:37:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5256" class=".btn">#5256</a>
            </td>
            <td>
                <b>
                    fence repolinter docker action
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
restrict docker based github actions to specific self-hosted runners to prevent docker user from poisoning the filesystem permissions

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-22 18:04:22 +0000 UTC
    </div>
</div>

