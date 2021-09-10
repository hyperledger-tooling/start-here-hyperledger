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
                PR <a href="https://github.com/hyperledger/besu/pull/2751" class=".btn">#2751</a>
            </td>
            <td>
                <b>
                    Remove duplication between Qbft protocol schedule and Ibft protocol schedule
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
Remove duplication between Qbft protocol schedule and Ibft protocol schedule

Note: This build on top of the qbft contract vote migration PR, once that is in this will be significantly smaller in changes.
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-10 05:58:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2748" class=".btn">#2748</a>
            </td>
            <td>
                <b>
                    Cleanup metrics connections after idle timeout
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When metrics are in use in teku (which uses besu metrics), and the prometheus service restarts, connections can be left open and never closed.

These connections should close after an idle timeout to avoid causing issues with running out of ports.

Reported in teku issue https://github.com/ConsenSys/teku/issues/4327 .

Signed-off-by: Paul Harris <paul.harris@consensys.net>

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-10 00:51:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2747" class=".btn">#2747</a>
            </td>
            <td>
                <b>
                    merge main into Rayonism
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                dust off the rayonism branch
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 23:01:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2746" class=".btn">#2746</a>
            </td>
            <td>
                <b>
                    Set TransactionGasCalculator in ETC specs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
On #2659 the gas calculator was split but the ETC specification wasn't properly updated, letting 21.7.3 nodes out of consensus.

## Fixed Issue(s)
Fixes #2715

## Changelog

- [ ] Update Ethereum Classic Phoenix and Magneto specs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 20:09:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2745" class=".btn">#2745</a>
            </td>
            <td>
                <b>
                    Add snap protocol message compatibility
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

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 15:29:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2721" class=".btn">#2721</a>
            </td>
            <td>
                <b>
                    [MINOR] Typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixed some typos

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-07 03:59:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2720" class=".btn">#2720</a>
            </td>
            <td>
                <b>
                    Move QBFT CMS creation to block creator
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
Move the CMS creation out of the QbftRound and into a QBFT block creator.

This allows the CMS to be only created the once per block regardless of how many rounds and removes the need for a proposal block behaviour in the qbft round.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-07 02:09:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2717" class=".btn">#2717</a>
            </td>
            <td>
                <b>
                    allow unlocking onchain privacy groups
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Prior to this commit, the only allowed transactions in locked onchain privacy groups were those making the `addParticipants` call to *any* contract--not just the proxy. This commit ensures that:
- while locked, only the group management proxy can be called
- while locked, all functions of the management proxy can be called

Corollary, this commit allows unlocking a group using `unlock` instead of implicitly unlocking it via `addParticipants`. This fixes #2693.

## Fixed Issue(s)

fixes #2693

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-05 22:00:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2716" class=".btn">#2716</a>
            </td>
            <td>
                <b>
                    spike: add benchmark
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

Add a benchmark job based on dockerized caliper. 

Do not merge, rather base a PR on top of this branch.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-05 19:31:16 +0000 UTC
    </div>
</div>

