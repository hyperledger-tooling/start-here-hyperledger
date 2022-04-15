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
                PR <a href="https://github.com/hyperledger/besu/pull/3729" class=".btn">#3729</a>
            </td>
            <td>
                <b>
                    fix ethstats issue
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

- Fix a problem in the retry mechanism meant that we could send a large number of requests at the same time.
- Setting the default port to 3000 if it is not put in the flag

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #3570

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-14 13:50:36 +0000 UTC
    </div>
</div>

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

