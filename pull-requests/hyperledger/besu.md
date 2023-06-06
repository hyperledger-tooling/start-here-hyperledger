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
                PR <a href="https://github.com/hyperledger/besu/pull/5538" class=".btn">#5538</a>
            </td>
            <td>
                <b>
                    remove PoW header validation if merge is enabled
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
Remove the Attached PoW rule used for the merge, as we are well past merge and this attached version of the PoW rule is causing unnecessary Ethash during chain sync:
![image](https://github.com/hyperledger/besu/assets/1238512/638f5c1f-e523-4ddb-a80a-10e4c3b6488e)


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
relates to #5539 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-06 15:57:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5537" class=".btn">#5537</a>
            </td>
            <td>
                <b>
                    Call operation performance optimizations 
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

- Introduce "undoable" journoled collections: set, map, table, and list
- Move values that are the same or shared across the transaction to
  TxValues record
- Move warm and cold storage to undoable sets and tables.
- Move transient storage to undoable table.
- Move address hashing inside of address with a memoized field.
- lazy create EOF return stack

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 18:04:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5536" class=".btn">#5536</a>
            </td>
            <td>
                <b>
                    EIP - 4844
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implements EIP-4844. 

- introduces a Hardfork class to the protocol schedule system
- new Engine APIs required for CL to work on 4844
- new DataGas type for tracking block cost for 4844 data
- new VersionedHash type to reflect that a versioned hash is not quite a pure sha256
- incorporates wrapped jc-kzg library for KZG point evaluations
- New transaction type, and domain objects for constituent parts to represent the Blobs, KZGCommitments, and Proofs used for 4844
- RLP encoders and decoders to support new transaction type
- gas pricing calculators for the new type of gas
- plugin-api version was changed

- TODO: KZGprecompile tests are failing, likely due to switch to big endian. Test is disabled, investigation ongoing.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 14:57:14 +0000 UTC
    </div>
</div>

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

