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
                PR <a href="https://github.com/hyperledger/besu/pull/4035" class=".btn">#4035</a>
            </td>
            <td>
                <b>
                    re-add a sync check before accepting/processing remote transactions
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
Re-adds a check to ensure the node is ready to accept and process remote transactions

* uses SyncState::isInitialSyncPhaseDone 
* adds safe handling of chain head parameters when processing transactions

relates to #3937

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #4030 


## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-30 20:42:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4034" class=".btn">#4034</a>
            </td>
            <td>
                <b>
                    [Issue-3867] Limit outbound eth message sizes
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
Builds on #4002.

Add logic to limit the size of outbound `eth` subprotocol messages.  

## Fixed Issue(s)
Fixes #3867

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-30 20:40:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4033" class=".btn">#4033</a>
            </td>
            <td>
                <b>
                    Move Taccat to Emeritus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I propose moving Taccat from Active Maintainer to Emeritus Maintainer status, pursuant to the inactivity clause. Taccat has had no activity in the past 6 months, as identified by an automated report run by the Hyperledger Foundation:

@taccatisid  - [last github action](https://github.com/ryjones/gal-besu/blob/main/reports/GAL-taccatisid.md) (a PR create) was 17 Dec 2021

We very much appreciate their contributions but changing status to emeritus (and thus revoking PR approval privileges) is in the interest of an orderly project. If Taccat expresses in this PR that they intend to make contributions in the next quarter, then they will not be moved to emeritus status.

I propose this vote be open until either an absolute majority of active maintainers (13) votes for the same outcome, or until two weeks has passed (14 July 2022), after which a voting majority will determine the outcome (with a tie resulting in no change).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-30 16:50:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4032" class=".btn">#4032</a>
            </td>
            <td>
                <b>
                    turns down logging output to debug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-30 14:22:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4031" class=".btn">#4031</a>
            </td>
            <td>
                <b>
                    Revert "Upgrade OpenTelemetry (#3675)"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit 78717ade1d45902c13e77e84bc201338e159c3c4.

Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Issues with "Failed to connect" errors 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-29 23:50:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4027" class=".btn">#4027</a>
            </td>
            <td>
                <b>
                    Return transaction type for legacy transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## PR description

Instead of omitting the transaction type when serializing a legacy transaction, we return the spec conform value of `0x0`.

## Fixed Issue(s)

fixes #4025 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 13:38:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4026" class=".btn">#4026</a>
            </td>
            <td>
                <b>
                    Add terminal block hash and number to Ropsten genesis file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Add terminal block hash and number to Ropsten genesis file, and also require that peers on Ropsten must have that block

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
        Created At 2022-06-28 13:09:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4024" class=".btn">#4024</a>
            </td>
            <td>
                <b>
                    Add Sepolia TTD and DNS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                ## PR description

Adds the correct TTD and DNS config to the Sepolia config file

## Fixed Issue(s)
fixes #4021 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 09:06:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4023" class=".btn">#4023</a>
            </td>
            <td>
                <b>
                    Print full exception when NatService fails to configure automaticially
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                https://github.com/hyperledger/besu/issues/3787

Signed-off-by: Antony Denyer <git@antonydenyer.co.uk>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 08:56:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4019" class=".btn">#4019</a>
            </td>
            <td>
                <b>
                    allow upgrade whether websockets enabled or not
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>
fixes #3948 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 00:16:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4018" class=".btn">#4018</a>
            </td>
            <td>
                <b>
                    Updates to DNS discovery
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Diego López León <dieguitoll@gmail.com>

## PR description
This PR adds a new implementation for [EIP-14159](https://eips.ethereum.org/EIPS/eip-1459) replacing [DNSDaemon](https://github.com/apache/incubator-tuweni/blob/main/dns-discovery/src/main/kotlin/org/apache/tuweni/discovery/DNSDaemon.kt) from Tuweni with a new one, vert.x based.
This new implementation provides the following benefits:
- Random tree traversal
- Batched discovery
- Periodic traversal continues from last state
- Non blocking implementation, based on vert.x DNS client 

## Fixed Issue(s)
Fixes #1707

## Notes
This is sent as a draft to gather feedback on this implementation. How often should we check the DNS for new peers? How many leaves should be attempted to connect per branch? Should this parameters need to be parameterized through the CLI? Based on the willingness to merge this proposal I would finish the specification by adding support to linked trees

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-27 19:33:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4017" class=".btn">#4017</a>
            </td>
            <td>
                <b>
                    warning invalid sync mode option [#3884]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Warning displayed to the user when an invalid sync-mode option passed to besu.
Removed the custom converter that was allowing invalid options to be passed converting them to null in the end.

## Fixed Issue(s)
Fixes #3884

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-27 01:16:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4013" class=".btn">#4013</a>
            </td>
            <td>
                <b>
                    When on PoS the head can be only be updated by ForkchoiceUpdate
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

When executing a newPayload or build a new block, we do not need to move
the chain head and update the world state, since this will be done by a
following forkchoice update call, but we still need to validate the block
and doing so we can also prepare everything for the future call, so we do
not need to re-execute everything, but only update the pointers, so that the
response to the forkchoice update call is quick.

Moreover on block proposal do only a validation of the block without storing or remembering nothing, to avoid saving data that could be stale, for example the empty block that is always proposed, is useless if another better block is produced later.

Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #3957

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-24 15:02:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4011" class=".btn">#4011</a>
            </td>
            <td>
                <b>
                    Update reference tests to the latest version and include test for gray glacier
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span><span class="chip">mainnet</span>
            </td>
            <td>
                The reference tests for Gray Glacier are included to ensure that our implementation is correct.

Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-24 11:45:25 +0000 UTC
    </div>
</div>

