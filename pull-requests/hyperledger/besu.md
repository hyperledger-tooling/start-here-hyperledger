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
                PR <a href="https://github.com/hyperledger/besu/pull/6401" class=".btn">#6401</a>
            </td>
            <td>
                <b>
                    log a different warning if pruning is enabled with BONSAI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                log "ignored" if enabled with BONSAI vs "deprecated" if enabled with FOREST

fixes #6400
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-14 21:50:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6397" class=".btn">#6397</a>
            </td>
            <td>
                <b>
                    Upgrade Mockito
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
        Created At 2024-01-12 17:59:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6396" class=".btn">#6396</a>
            </td>
            <td>
                <b>
                    Upgrade Guava dependency
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

Upgrade Guava to 33.0.0, since it introduces a change in the Supplier class, the memory consumption estimation of a pending transaction has been updated to take in account the new layout of the class.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-12 11:16:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6395" class=".btn">#6395</a>
            </td>
            <td>
                <b>
                    Fix typo in SUPPORT.md
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

fix `Hyperlegder` to `Hyperledger`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-12 08:29:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6394" class=".btn">#6394</a>
            </td>
            <td>
                <b>
                    Trie log prune using TrieLogEvent
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
This PR aims to make the pruning logic async as this feature does not need to be in the synchronous.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Part of #5390 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-12 07:50:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6392" class=".btn">#6392</a>
            </td>
            <td>
                <b>
                    reduce machine size for clique/BFT ATs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                same change as was made in #6384 for permissioning ATs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-12 04:26:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6390" class=".btn">#6390</a>
            </td>
            <td>
                <b>
                    Use mining beneficiary from protocol spec in TraceServiceImpl
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

instead of using coinbase from block header as mining beneficiary, we use the protocol spec to retrieve it

## Fixed Issue(s)
fixes #6389 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-11 23:53:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6387" class=".btn">#6387</a>
            </td>
            <td>
                <b>
                    [MINOR] Fix pki tests condition check on mac
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Fix pki tests condition check on mac

## Fixed Issue(s)
see https://github.com/hyperledger/besu/pull/6235
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-11 02:25:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6384" class=".btn">#6384</a>
            </td>
            <td>
                <b>
                    Fix test flackyness of acceptanceTestsPermissioning 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">flake</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

`NodeSmartContractPermissioningAcceptanceTest` could fail due to the fact that if a node is not in sync txs are not accepted, since the txpool is disabled, so before interacting with the node we must wait for all the nodes in the test to be in sync.
Also tuned Circle CI to execute acceptanceTestsPermissioning serially, to avoid to spawn too many Besu processes and in that way it is enough to use a medium executor, as last thing slowed a bit the block creation to make synchronization easier.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-10 20:57:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6383" class=".btn">#6383</a>
            </td>
            <td>
                <b>
                    Bump to nex release snapshot 24.1.1
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
bump release version to 24.1.1-SNAPSHOT
add/edit/move changelog entries
TBA links for 24.1.0
add missing changelog entry for 23.10.2

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-10 18:29:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6382" class=".btn">#6382</a>
            </td>
            <td>
                <b>
                    In fluent APIs correct Tangerine Whistle definition.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The fluent API incorrectly added the code size limit in Tangerine Whistle instead of first adding it in Spurious Dragon.

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
        Created At 2024-01-10 18:14:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6381" class=".btn">#6381</a>
            </td>
            <td>
                <b>
                    Introduce TransactionEvaluationContext to pass data between selectors and plugin
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

Some tx selector plugins needs more context about the current tx being evaluated, for example the current minGasPrice, or the effective price of the tx and possibly more data in the future, for this we introduce the TransactionEvaluationContext to hold that data and pass it across all the selectors and the plugin. Another advantage of this context is to avoid to compute multiple time the same data, in case it is needed in more that one selector.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-10 13:15:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6380" class=".btn">#6380</a>
            </td>
            <td>
                <b>
                    Make transaction pool configurable in acceptance tests
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
        Created At 2024-01-10 13:10:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6379" class=".btn">#6379</a>
            </td>
            <td>
                <b>
                    Ignore bin files when running the spdx license check
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
Ignore generated files in `bin/` directories when running the SPDX license check.  Visual Studio Code generates build files in various bin directories, which causes this check to fail.  
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-09 21:29:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6378" class=".btn">#6378</a>
            </td>
            <td>
                <b>
                    Upgrade `com.fasterxml.jackson` dependencies
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

Jackson 2.15 by default limits the length of input string to a value that is lower than the string length used in some of our test, so now we need to explicitly tune this value. Setting max int since this is only related to tests. 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-09 15:56:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6377" class=".btn">#6377</a>
            </td>
            <td>
                <b>
                    Upgrade dependencies
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

Update all dependencies that do not require code changes.

Dependencies that require code changes will be updated in separate PR.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-09 12:57:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6375" class=".btn">#6375</a>
            </td>
            <td>
                <b>
                    Add a sender cache to Transaction
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
This PR will create a new cache within the Transaction class to house all computed senders for their respective transaction hashes. 
When receiving the newPayload call, it calculates asynchronously and in parallel all the transaction hashes and senders.
This PR is expected to improve block processing time, given that either the transaction sender is determined when Besu fills its transaction pool or with the asynchronous tasks. 

**The cache memory footprint**

The cache is defined with this pair hash -> address, for 100_000 entries, it consumes currently less than 20 MiB.
<img width="937" alt="image" src="https://github.com/hyperledger/besu/assets/5099602/bc0be6e5-988f-4b71-9d99-f501d9cc3a99">

We can find below the CPU profiling with and without this PR.

**Without this PR**
<img width="1719" alt="image" src="https://github.com/hyperledger/besu/assets/5099602/0a0569da-2b26-462e-acd9-3c4b6ff4cc9d">


**With this PR**
<img width="1719" alt="image" src="https://github.com/hyperledger/besu/assets/5099602/a0b4e853-48a1-4f5b-bdf4-b5f6804303cf">


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-09 10:13:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6373" class=".btn">#6373</a>
            </td>
            <td>
                <b>
                    full sync - don't fail startup if sync-min-peers specified
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Log a warning instead of failing startup

fixes #6327 

Before:
```
➜  b2 git:(sync-min-peers) ✗ besu --sync-mode="full" --sync-min-peers=1
2024-01-09 12:17:57.498+10:00 | main | INFO  | Besu | Starting Besu
2024-01-09 12:17:57.866+10:00 | main | ERROR | Besu | Failed to start Besu
picocli.CommandLine$ParameterException: --sync-min-peers can't be used with FULL sync-mode [--sync-min-peers]
	at org.hyperledger.besu.cli.util.CommandLineUtils.failIfOptionDoesntMeetRequirement(CommandLineUtils.java:129)
```
and startup fails.

After:

```
➜  b2 git:(sync-min-peers) ✗ besu --sync-mode="full" --sync-min-peers=1
2024-01-09 12:24:50.728+10:00 | main | INFO  | Besu | Starting Besu
2024-01-09 12:24:51.539+10:00 | main | WARN  | Besu | --sync-min-peers is ignored in FULL sync-mode
2024-01-09 12:24:51.818+10:00 | main | INFO  | Besu | Connecting to 0 static nodes.
```
and startup continues
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-09 06:08:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6372" class=".btn">#6372</a>
            </td>
            <td>
                <b>
                    Added alias --sync-min-peers for --fast-sync-min-peers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add an alias for fast-sync-min-peers

refs #6327 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-09 02:15:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6371" class=".btn">#6371</a>
            </td>
            <td>
                <b>
                    merges in 23.10.3-hotfix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * trigger a BWS if we do not have a valid worldstate available during fcU raise log rolling failure loglevel to error from debug
* fixing on selfdestruct


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-08 19:28:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6368" class=".btn">#6368</a>
            </td>
            <td>
                <b>
                    chore: fix typos
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
        Created At 2024-01-08 04:14:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6367" class=".btn">#6367</a>
            </td>
            <td>
                <b>
                    [MINOR] Move bootnodes logging to RunnerBuilder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Move bootnodes logging to RunnerBuilder so that we always log the actual bootnodes being used. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-08 01:59:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6366" class=".btn">#6366</a>
            </td>
            <td>
                <b>
                    [MINOR] readme - fixed link to logging docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #6342 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-08 01:51:33 +0000 UTC
    </div>
</div>

