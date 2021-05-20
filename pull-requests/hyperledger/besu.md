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
                PR <a href="https://github.com/hyperledger/besu/pull/2305" class=".btn">#2305</a>
            </td>
            <td>
                <b>
                    add log blooms for quorum private transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When private transactions are executed in goquorum compatible mode the receipts of these private transactions are stored in place of the public marker transaction. To make these receipts discoverable by calls that use the bloom filters the blooms filters of the private transactions have to be combined with the blooms of the public transactions in the right places. 

Signed-off-by: Stefan Pingel <stefan.pingel@consensys.net>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 07:27:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2304" class=".btn">#2304</a>
            </td>
            <td>
                <b>
                    Add Vijay Michalik to maintainers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Vijay has helped the Besu project through contributions to [user questions](https://chat.hyperledger.org/channel/besu?msg=pEvzRqPLYBvDtbX8m), documentation and [managing issues on the project](https://chat.hyperledger.org/channel/besu?msg=sazaeBhiNpY2Nc5Xk).

Voting ends 2 weeks from the publication of this PR.

For more information on this process see the Becoming a Maintainer section in the MAINTAINERS.md file.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 07:18:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2303" class=".btn">#2303</a>
            </td>
            <td>
                <b>
                    Add Sajida Zouarhi to maintainers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Antoine Toulme <antoine@lunar-ocean.com>
Sajida has started helping manage Github issues and collaborating with the existing maintainers to help coordinate the development of Besu.

Voting ends 2 weeks from the publication of this PR.

For more information on this process see the Becoming a Maintainer section in the MAINTAINERS.md file.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 07:11:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2302" class=".btn">#2302</a>
            </td>
            <td>
                <b>
                    errata discovered in 21.1.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
A couple quick fixes for bugs I found In scale testing 21.1.6 pending transactions:
* baseFee = null was not handled correctly in PendingTransactions.updateBaseFee for a fork block
* the transaction gas budget calculator was 2x'ing the already 2x'd gasLimit at and past fork block

we should probably write some tests that cover these cases, but it is late and the release is already out there...

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog


- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 03:26:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2301" class=".btn">#2301</a>
            </td>
            <td>
                <b>
                    Prepare for version 21.1.7-SNAPSHOT
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
        Created At 2021-05-19 22:00:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2300" class=".btn">#2300</a>
            </td>
            <td>
                <b>
                    Release 21.1.6
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
        Created At 2021-05-19 21:45:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2298" class=".btn">#2298</a>
            </td>
            <td>
                <b>
                    Added PKI module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Adding the PKI module with the initial setup code for keystore configuration.

## Changelog

No need to update the changelog at this moment as this code isn't part of core Besu yet.

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-19 20:32:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2296" class=".btn">#2296</a>
            </td>
            <td>
                <b>
                    Eip 1559 tx sorting refactor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

this is a refactor of PendingTransactions, moving the actual queue out into an interface, and adds a basic implementation that prioritizes by transaction revenue.

The basic implementation keeps just a single transaction pool, without other pre-optimized indexed collections, and simplified locking.  We should quantify the performance of this approach before using this impl.  PR marked as DO NOT MERGE for this reason.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-19 06:53:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2294" class=".btn">#2294</a>
            </td>
            <td>
                <b>
                    GoQuorum ATs: run the estimate gas test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Revert #2282 
Enabling one more passing GoQuorum AT 
See https://github.com/hyperledger/besu/pull/2282

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-19 00:54:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2292" class=".btn">#2292</a>
            </td>
            <td>
                <b>
                    EIP-1559 Transaction Pool Sorting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add transaction sorting as described [here](https://hackmd.io/@adietrichs/1559-transaction-sorting)

## Fixed Issue(s)
fixes #2286

## Changelog
- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-18 22:54:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2289" class=".btn">#2289</a>
            </td>
            <td>
                <b>
                    EIP-3554: Difficulty Bomb Delay to December 1st 2021
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>


## PR description

implemented for london https://eips.ethereum.org/EIPS/eip-3554

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-17 17:29:29 +0000 UTC
    </div>
</div>

