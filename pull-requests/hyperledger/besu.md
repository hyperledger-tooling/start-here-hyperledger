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
                PR <a href="https://github.com/hyperledger/besu/pull/3728" class=".btn">#3728</a>
            </td>
            <td>
                <b>
                    remove TTD depth limit for ancestorIsValidTerminalProofOfWork
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

remove TTD search depth limit.  Ideally we will set a recent finalized block when we finish backward sync (and fast and snap sync as well), as that will be more performant than scanning through blocks looking for TTD when we do not have a finalized block.  However, removing this limit will prevent us from incorrectly failing an `engine_forkchoiceUpdate` call post-sync when there is a significant distance between HEAD and TTD.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#3727

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 20:45:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3726" class=".btn">#3726</a>
            </td>
            <td>
                <b>
                    3621 parent timestamps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Adds lastValidHash as optional param to failing ForkChoiceResults
- Controversial:  fails on timestamps that are not greater than parents. This was requested when discovered in a differential fuzz test against Geth, however the means of handling this and returning the error to the CL is still under discussion

fixes #3677 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 17:54:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3723" class=".btn">#3723</a>
            </td>
            <td>
                <b>
                    Move 2 Maintainers to Emeritus Status
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I propose moving the following maintainers to Emeritus status, pursuant to the inactivity clause. These maintainers have had no activity in the past 6 months, as identified by an automated report run by the Hyperledger Foundation:

@abdelhamidbakhta  - last github action (a PR review) was 6 Jun 2021
@RatanRSur  - last github commit was 7 Oct 2021

We very much appreciate their contributions but moving their status to emeritus (and thus revoking PR approval privileges) is in the interest of an orderly project. If any of these maintainers express in this PR that they intend to make contributions in the next quarter, then they will not be moved to emeritus status.

I propose this vote be open until either an absolute majority of active maintainers (14) votes for the same outcome, or until two weeks has passed (26 Apr 2022), after which a voting majority will determine the outcome (with a tie resulting in no change).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 17:25:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3720" class=".btn">#3720</a>
            </td>
            <td>
                <b>
                    revert to TransactionDB to resolve 'busy' exception 
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
Revert to TransactionDB to resolve 'busy' exception from OptimisticTransactionDB.  

As I understand it, we originally went to OptimisticTransctionDB in order to support `deleteRange()` for our implementation of `RocksDBColumnarKeyBValueStore.clear()`.  In light of the change to the `clear` implementation in #3634, we do not need to use OptimisticTransactionDB.  

Currently in Draft while testing and while discussing the merits of sticking with OptimisticTransactionDB for locking performance.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3719

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-11 16:48:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3718" class=".btn">#3718</a>
            </td>
            <td>
                <b>
                    [DO NOT MERGE] Test another implementation of Arrays.fill
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Performance test : Test another implementation of Arrays.fill
Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-11 12:47:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3712" class=".btn">#3712</a>
            </td>
            <td>
                <b>
                    Fix save worldstate issue on bonsai and fastsync
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Fix a bug that caused the worldstate to be missing during a fastsync and prevented it from completing properly

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 11:06:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3711" class=".btn">#3711</a>
            </td>
            <td>
                <b>
                    Fix NPE in DeFramer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                Signed-off-by: Frank Li <b439988l@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Catch an NPE using optionals and complete the future nicely with an exception

## Fixed Issue(s)
Fixes #3637 

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 04:45:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3710" class=".btn">#3710</a>
            </td>
            <td>
                <b>
                    add snapsync as beta feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

This PR enables the snapsync as client. It works with Bonsai but there are still some limitations and possible optimizations.
I will test with Forest

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 09:28:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3709" class=".btn">#3709</a>
            </td>
            <td>
                <b>
                    lgtm yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Added config file for LGTM
Note the LGTM failure is the "main build" which is building off main branch - which still has OOM. But the "merge build" ie building off this PR, is passing. 

Current report: https://lgtm.com/projects/g/hyperledger/besu/logs/rev/pr-935719d01d715dea5db84d624ce75b5505b7708f/lang:java/stage:Build%20main_fe673431fab8c6439e6eb0e83f6545a1583afaeb

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 08:44:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3708" class=".btn">#3708</a>
            </td>
            <td>
                <b>
                    Not null annotations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                replace jetbrains with javax.annotation.Nonnull

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 07:01:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3707" class=".btn">#3707</a>
            </td>
            <td>
                <b>
                    Feature/bonsai fast sync clear flat db
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
During fast sync on bonsai, clear only the flat database rather than the entire bonsai worldstate.  

DRAFT: while testing bonsai fast-sync account db clearing and lazy reads on goerli and mainnet


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Along with #3684 , fixes #3694 

## Documentation


- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 05:19:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3705" class=".btn">#3705</a>
            </td>
            <td>
                <b>
                    vertx 4.2.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Update vertx dependency

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 01:59:22 +0000 UTC
    </div>
</div>

