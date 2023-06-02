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
                PR <a href="https://github.com/hyperledger/besu/pull/5515" class=".btn">#5515</a>
            </td>
            <td>
                <b>
                    [4844] Remove SSZ
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
        Created At 2023-05-30 01:55:27 +0000 UTC
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
                    Update Tuweni to 2.4.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Updates Tuweni to 2.4.0, updating group ID to io.tmio.

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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5509" class=".btn">#5509</a>
            </td>
            <td>
                <b>
                    Record empty responses when retrying a peer task
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

`AbstractRetryingPeerTask` has a way to understand if the result of a try is empty, but it only uses this information to discriminate if the result is a partial one, instead is very useful to also use the emptiness information to demote the peer and eventually disconnect it in case it sends too many useless responses, as done in this PR.
In the making of this PR, I discovered that there were opportunities to improve the code and simplify the writing of retrying tasks, so I refactored and documented the code so that any class extending `AbstractRetryingPeerTask` should not set the final task result by themself, but instead implements the `emptyResult` and `successfulResult` to report the status of the request, so that the final setting of the task result is always a duty of `AbstractRetryingPeerTask`, removing the different approaches used before.

relates to #5415 and #5271


## Tests

- [ ] Checkpoint Sync
- [ ] Snap Sync
- [ ] Fast Sync
- [ ] Full sync
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-29 10:35:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5508" class=".btn">#5508</a>
            </td>
            <td>
                <b>
                    Use retry switching peer for world state download tasks
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

Built on top of #5509, so please check it first. [Link to only see diff again #5509](https://github.com/fab-10/besu/compare/demote-peer-with-empty-responses-when-retrying...fab-10:besu:use-retry-switching-peer)

With this PR all the world state download tasks used by snap sync are updated to use the retry switching peer strategy, to reduce the chance that we keep sending requests to the same bad peer.

relates to https://github.com/hyperledger/besu/issues/5415 and #5271
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-29 09:28:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5507" class=".btn">#5507</a>
            </td>
            <td>
                <b>
                    Revert the revert of the tx selection commit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The original PR (#5396) caused a problem when running on Frontier. The world state update was committed too late and the receipt was created with the old world state root hash. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-29 05:13:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5506" class=".btn">#5506</a>
            </td>
            <td>
                <b>
                    RPC - default to internal error not invalid params
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                see #4212 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-29 04:20:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5505" class=".btn">#5505</a>
            </td>
            <td>
                <b>
                    GraphQL: Migrate Long types to strings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Migrate from EIP specified numeric values to execution-spec specified
string values.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 19:32:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5504" class=".btn">#5504</a>
            </td>
            <td>
                <b>
                    Prepare for next version
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
        Created At 2023-05-26 04:38:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5503" class=".btn">#5503</a>
            </td>
            <td>
                <b>
                    Change disconnect peer message to debug level.
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
Change the peer disconnect message to debug level. Since that's not useful to end users.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 01:28:42 +0000 UTC
    </div>
</div>

