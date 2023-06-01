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
                PR <a href="https://github.com/hyperledger/besu/pull/5523" class=".btn">#5523</a>
            </td>
            <td>
                <b>
                    Fix code availability in grapqh
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5502" class=".btn">#5502</a>
            </td>
            <td>
                <b>
                    run non-mainnet ATs on PRs, split into sub groups
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Run all ATs on PRs, but split into 
* mainnet
* Clique + BFT
* Privacy + Permissioning
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 00:50:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5501" class=".btn">#5501</a>
            </td>
            <td>
                <b>
                    Release 23.4.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 23.4.1
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 00:49:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5500" class=".btn">#5500</a>
            </td>
            <td>
                <b>
                    Specify optional scheme (ws or wss) in Ethstats url option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
- Allow scheme (ws:// or wss://) optionally to be specified in ethstats url. If user specify the scheme, the connection logic doesn't need to switch from ssl to non-ssl on each retry logic.
- Change order of ethstats service start after main ethereum loop is up because ethstats service needs local node address.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #5494 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-25 23:36:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5499" class=".btn">#5499</a>
            </td>
            <td>
                <b>
                    Revert "Add plugin API to select Transactions (#5396)"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit 65bcc557e41cca2568588a21441aa5d8658a5e79.

Due to breaking Clique (in the ATs at least)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-25 22:33:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5498" class=".btn">#5498</a>
            </td>
            <td>
                <b>
                    Stop evaluating txs for sender after the first skipped one
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

This PR is built on top of  #5492 and #5491 so check them first.

This PR introduce a simple optimization to avoid to waste time validating transactions that will not be selected during the current block creation process. 
Basically if a sender have more than one prioritized candidate transactions, and for some reason any of them is not selected during the block creation process, it make no sense to keep evaluating any more transaction after the skipped one, since it will not be selected due to the nonce gap.

Enabling the selection stats implemented in #5492 is it possible to see the difference before and after this PR, the wasted validation work that we are removing is represented by the `INVALID_TRANSIENT(NONCE_TOO_HIGH)` label.

Before
```
Selection stats: Totals[Evaluated=2000, Selected=109, Skipped=1891, Dropped=0]; Detailed[INVALID_TRANSIENT(GAS_PRICE_BELOW_CURRENT_BASE_FEE)=1712, INVALID_TRANSIENT(NONCE_TOO_HIGH)=158, INVALID_TRANSIENT(TX_TOO_LARGE_FOR_REMAINING_GAS)=21, SELECTED=109]
```

After
```
Selection stats: Totals[Evaluated=1743, Selected=126, Skipped=1617, Dropped=0]; Detailed[INVALID_TRANSIENT(GAS_PRICE_BELOW_CURRENT_BASE_FEE)=1600, INVALID_TRANSIENT(TX_TOO_LARGE_FOR_REMAINING_GAS)=17, SELECTED=126]
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-25 09:26:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5497" class=".btn">#5497</a>
            </td>
            <td>
                <b>
                    Remove maybeHead from BackwardSyncContext
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                # Summary of Changes

* Remove what appears to be a redundant global variable, `maybeHead`. When backwards sync is performed, this can cause besu to incorrectly jump back to a much older block instead of a recent block.
* Add logging to help debug these issues

# Context 

This is a partial fix for issues noticed on recent nimbus-besu combos: https://github.com/hyperledger/besu/issues/5411
Note, there are still issues due to nimbus behaviour, so there is instability when restarting Nimbus for a period of about an hour where it gets in sync but falls out again repeatedly.

It should prevent the issue where we see large "reorgs" in the logs e.g.:
```
{"@timestamp":"2023-04-27T00:47:24,241","level":"WARN","thread":"vert.x-worker-thread-0","class":"DefaultBlockchain","message":"Chain Reorganization +192 new / -0 old
       Old - hash: 0xbca29e861aabf1b975cde3ee6f147a86ad8de3bfab1a39bfb2d98594a72eb63d, height: 3368145
       New - hash: 0xd1fb6c37bf03b2ed56bfd07699e9097119f143b600f4a33e4010edee3261a75a, height: 3368337
  Ancestor - hash: 0xbca29e861aabf1b975cde3ee6f147a86ad8de3bfab1a39bfb2d98594a72eb63d, height: 3368145","throwable":""}
{"@timestamp":"2023-04-27T00:47:24,670","level":"WARN","thread":"nioEventLoopGroup-3-9","class":"DefaultBlockchain","message":"Chain Reorganization +0 new / -192 old
       Old - hash: 0xd1fb6c37bf03b2ed56bfd07699e9097119f143b600f4a33e4010edee3261a75a, height: 3368337
       New - hash: 0xbca29e861aabf1b975cde3ee6f147a86ad8de3bfab1a39bfb2d98594a72eb63d, height: 3368145
  Ancestor - hash: 0xbca29e861aabf1b975cde3ee6f147a86ad8de3bfab1a39bfb2d98594a72eb63d, height: 3368145","throwable":""}
  ```
  
because instead of rewinding back to an incorrectly maintained `maybeHead` hash, it will rewind back to the hash that was given to it in the FCU or newPayload.

Note, we still see these reorgs when Prysm lock-steps syncs in batches of ~50 newPayloads

# Testing

This goal of this testing was to ensure the node could get back into sync in each scenario (and also explore the various CL syncing strategies but that's not relevant for this PR). Testing was done on Sepolia, unless otherwise mentioned

- Initial Sync (performs backwards sync as last stage)
- Scenario 1: CL restart
- Scenario 2: CL short downtime: 30 - 120 mins
- Scenario 3: CL long downtime: 7 hours
- Scenario 4: Besu short downtime: 30 - 60 mins
- Scenario 5: Besu long downtime: 3 - 5 hours
- Scenario 6: Besu longer downtime: 20 hours

| Scenario/CL | Nimbus | Teku | Prysm | Lighthouse | Lodestar | Nimbus Mainnet | Teku Mainnet |
--|--|--|--|--|--|--|--|
| Initial Sync | ✅  | ✅ | ✅  | ✅  | ✅  | ✅ | ✅  |
| Scenario 1 | ✅  | ✅ | ✅  | ✅  | ✅  | ✅  | ✅  |
| Scenario 2 | ✅  | ✅ | ✅  | ✅  | ✅  |
| Scenario 3 |  | ✅ | ❓* |  |   |
| Scenario 4 | ✅  | ✅ | ✅  | ✅  |  |
| Scenario 5 |  | ✅ |  ✅ |  | ✅  |
| Scenario 6 |  | ✅ |  ✅  |  |  |

* Prysm Scenario 3 was a 43 hour downtime. With Prysm's lock-step it is a slow recovery (so not actually backwards sync anyway)...it was quicker to recover by resyncing prysm.

# Impact

Scenario 1 with Nimbus (the main driver for this fix) before and after the fix:

BEFORE
<img width="1612" alt="nimbus-without-fix" src="https://github.com/hyperledger/besu/assets/2893793/18cf7810-034c-41a9-bc86-5b2ddb8d350e">

AFTER
<img width="1607" alt="nimbus-with-fix" src="https://github.com/hyperledger/besu/assets/2893793/95934c65-4c09-446f-862c-0db83c38f56f">

After being restarted, Nimbus on Sepolia takes some time to find peers, so it is maybe getting more towards Scenario 2. No lock-step is attempted, instead Nimbus causes a few small backward syncs with some halts in between. 
The main difference with before is that besu is only backward syncing a few blocks rather than many hundreds due to the Besu bug.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-25 07:31:43 +0000 UTC
    </div>
</div>

