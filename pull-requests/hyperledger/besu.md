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

Built on top of #6377 

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
This PR will establish a new cache within the Transaction class to house all computed senders for their respective transaction hashes. This PR is expected to improve block processing time, given that the majority of transaction senders are determined when Besu fills its transaction pool.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6365" class=".btn">#6365</a>
            </td>
            <td>
                <b>
                    One permissioning AT to junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                refs #6262 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-08 01:13:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6363" class=".btn">#6363</a>
            </td>
            <td>
                <b>
                    Import export trie log
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
This PR extends the x-trie-log subcommand to allow exporting and importing of a trie log.

This PR is built on top of https://github.com/hyperledger/besu/pull/6303



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-08 00:03:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6362" class=".btn">#6362</a>
            </td>
            <td>
                <b>
                    migrate clique tests fully to junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                fixes #6261
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-07 23:20:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6360" class=".btn">#6360</a>
            </td>
            <td>
                <b>
                    fix: use UID 1000 for besu user (#6358)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

The openjdk-latest Docker image is using UID 1001 for besu, because its base image `ubuntu:23.10` now contains a default "ubuntu" user with UID 1000. (This UID change causes the besu user with UID 1001 to not have access to files created for past versions with UID 1000.)

This PR removes the default ubuntu user and explicitly uses UID 1000 when creating the besu user.

**Note that this change will re-break file permissions for people who've already changed besu file ownership from 1000 -> 1001 when upgrading to 23.10.3, as the besu user goes back to UID 1000, as it was in versions prior to 23.10.3.**

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->



## Fixed Issue(s)

Fixes #6358
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-07 09:34:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6359" class=".btn">#6359</a>
            </td>
            <td>
                <b>
                    fixing trielog generation when selfdestruct/create2 on same block
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

This PR fixes a bug in the generation of the trie log when we have a selfdestruct and create2 of the same account in the same block, and if this contract contains a non-empty storage. This bug occurred on the mainnet, and we were able to reproduce the bug and validate that the fix resolves the problem. We had a previous PR to fix this bug but it was not completly fixed on this one

This bug was fixed when we create the trie log with a persistent BonsaiWorldstate, but not with a non-persistent BonsaiWorldstate, which is what happens with the call of the newPayload method. BackwardSync uses the persistent worldstate, and that's why the BackwardSync unlocks the situation.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#6357 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-06 22:33:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6356" class=".btn">#6356</a>
            </td>
            <td>
                <b>
                    Fix docker detection on Mac
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
uses `/.dockerenv` as a fallback detector mechanism for DockerDetector.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #6139

prior to this PR, when running besu on docker desktop on Mac, besu would fail to recognize it was running inside docker without specifying a nat-method or when using  `--nat-method=AUTO` 

on Mac M2, using docker desktop:
```
2024-01-06 01:23:27.514+00:00 | main | INFO  | RunnerBuilder | Detecting NAT service.
...
2024-01-06 01:23:27.629+00:00 | main | INFO  | DockerNatManager | Starting docker NAT manager.
```



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-06 01:49:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6354" class=".btn">#6354</a>
            </td>
            <td>
                <b>
                    Improve the high spec flag
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
Improve the high spec flag (`Xplugin-rocksdb-high-spec-enabled`) by limiting it to only few column families.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-05 09:13:07 +0000 UTC
    </div>
</div>

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
Implement shanghai support for QBFT and IBFT chains.

Summary of the changes:

- Pass the `protocolSchedule` into the `BftContext` so it can check if `shanghai` is enabled
- Add a new `createBlock(...)` function to `BftBlockCreator` that allows BFT block creators to use the `AbstractBlockCreator` `createBlock(...)` function that takes a list of withdrawals
  - Use this to create blocks that have an (empty) list of withdrawals if shanghai _is_ enabled
  - Use the original `createBlock(...)` implementation when shanghai _isn't_ enabled
- Change the way the BFT block validator for a given protocol schedule is selected, using the parent header and timestamp instead of block number
  - **I need to better understand how BFT round, chain height & sequence number relate to protocol schedule. This change is still WIP**

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
                BFT tests now use Junit 5
before: acceptanceTestsCliqueBft 65 tests [example](https://app.circleci.com/pipelines/github/hyperledger/besu/26075/workflows/990c39ad-cf35-43ff-ad65-cdb87bf46f7d/jobs/170967)
after: acceptanceTestsCliqueBft 65 tests [example](https://app.circleci.com/pipelines/github/hyperledger/besu/26094/workflows/e8411b37-8abd-46f2-a02f-089dc91dfb9c/jobs/171128) 
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

