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
                PR <a href="https://github.com/hyperledger/besu/pull/5534" class=".btn">#5534</a>
            </td>
            <td>
                <b>
                    Feature addition for tracing private transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Draft PR for adding priv_traceTransaction API

## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/5280
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 07:17:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5532" class=".btn">#5532</a>
            </td>
            <td>
                <b>
                    Remove push metrics port from effective ports
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This results in a port conflict check however the push metrics port refers to a push gateway for besu to connect to rather than a port it is serving itself.

If you run besu with push metrics [following this guide](https://besu.hyperledger.org/en/stable/public-networks/how-to/monitor/metrics/#run-prometheus-with-besu-in-push-mode) then the bug fixed by this PR is that you have to run besu first, followed by the push gateway.

Now you can start either besu or push gateway in any order.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-04 20:54:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5531" class=".btn">#5531</a>
            </td>
            <td>
                <b>
                    Move ethstats server request to trace
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
        Created At 2023-06-04 20:43:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5529" class=".btn">#5529</a>
            </td>
            <td>
                <b>
                    logging cleanup, giant new payload.
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
Moved newPayload logging to trace

## Fixed Issue(s)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-02 14:54:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5527" class=".btn">#5527</a>
            </td>
            <td>
                <b>
                    Prevent rocksdb segfaults when accessing closed storage
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
gate transaction access on whether the underlying storage has closed.  This prevents segfaults at shutdown when we close rocksdb, but there are async processes attempting to access the db.

Currently evaluating to ensure there is no noticeable performance regression.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#5362 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-01 23:56:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5526" class=".btn">#5526</a>
            </td>
            <td>
                <b>
                    preload only when value changed
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
        Created At 2023-06-01 11:25:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5525" class=".btn">#5525</a>
            </td>
            <td>
                <b>
                    [MINOR] switch QBFT tests to Junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                statemachine tests have plenty of unnecessary mockings so did not unpick that as part of this PR, went with lenient mockings instead.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-01 08:11:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5523" class=".btn">#5523</a>
            </td>
            <td>
                <b>
                    Fix code availability in graphQL
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
This PR loads the account code when we still have the ws snapshot available. This avoids the issue caused in graph
QL api when we try to fetch the Account code in the AccountAdapter and the ws snapshot is already closed.
Another possibility would be to pass the block number to the AccountAdapter and get another open another snapshot to query the accounts code and storage in the AccountAdapter which has the enough context to know what slot is being requested.
This can be attempted in a separate PR and if we decide to move forward with that we can transfer this tiny change to the AccountAdapter as well. 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Partially fixes #5516 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-01 02:29:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5522" class=".btn">#5522</a>
            </td>
            <td>
                <b>
                    Make docker commands easier to debug during upload and manifest creation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                Debugging for https://github.com/hyperledger/besu/issues/5521

Print out commands being executed

Separate out docker push and docker manifest push commands for release to make it easier to spot which one fails in #5521 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-31 22:31:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5520" class=".btn">#5520</a>
            </td>
            <td>
                <b>
                    [4844] wip - added versioned hashes checking
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                refs #5487 
still TBD whether this is added to V2 or V3. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-31 06:46:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5519" class=".btn">#5519</a>
            </td>
            <td>
                <b>
                    4844 devnet 5b
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                rebased from main
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-31 00:36:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5517" class=".btn">#5517</a>
            </td>
            <td>
                <b>
                    Log worldstate availability
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

PR adds debug logging to worldstate access path, and a warning when we try to access closed worldstate.
Added in response to #5456, and seems suitable to add to main.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-30 19:45:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5514" class=".btn">#5514</a>
            </td>
            <td>
                <b>
                    PR checklist - remove checkbox for non-mainnet ATs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                these are now run in CI on each PR per #5502 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-30 01:37:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5513" class=".btn">#5513</a>
            </td>
            <td>
                <b>
                    Update Tuweni to 2.4.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Updates Tuweni to 2.4.1, updating group ID to io.tmio.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-29 21:03:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5512" class=".btn">#5512</a>
            </td>
            <td>
                <b>
                    refactor txpool options
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ux</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Add all tx-pool CLI options under a single group https://github.com/hyperledger/besu/issues/5466

## Fixed Issue(s)
Fixes, #5466 


Result
![Screenshot 2023-05-30 at 19 40 37](https://github.com/hyperledger/besu/assets/99179176/f3d7a5e6-6290-4caa-96db-c7642536e265)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-29 18:24:18 +0000 UTC
    </div>
</div>

