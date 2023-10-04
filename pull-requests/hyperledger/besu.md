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
                PR <a href="https://github.com/hyperledger/besu/pull/5980" class=".btn">#5980</a>
            </td>
            <td>
                <b>
                    Only use the buider to create transactions
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

Remove all the overloaded `Transaction`' constructors, and only allow to create a transaction using the `Builder`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 11:28:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5976" class=".btn">#5976</a>
            </td>
            <td>
                <b>
                    Retry on busy and locktimeout failures for rocksdb transactions
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
Simple default retry policy for rocksdb busy and locktimeout exceptions

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
related to #5911 
related to #5549 
related to #5807
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-02 19:35:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5975" class=".btn">#5975</a>
            </td>
            <td>
                <b>
                    Tests for GraphQL Cancun fields
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Add tests for GraphQL fields added to support cancun. Also, re-work test case inclusion code and update tests impacted by adding a new block to the chain.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-02 17:44:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5974" class=".btn">#5974</a>
            </td>
            <td>
                <b>
                    Target to use about 25MB for the new layered txpool by default
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

Reduce the default memory usage of the txpool, to limit the added amount of memory used by Besu.
There 2 memory limited layers, ready and sparse, so to target 25MB we set the limit for a layer to 12.5MB
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-02 15:44:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5973" class=".btn">#5973</a>
            </td>
            <td>
                <b>
                    [4844] EngineNewPayload - Add Blob Count validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">4844</span>
            </td>
            <td>
                ## PR description
Add Blob Count validation to EngineNewPayload - Fix invalid_blob_count hive tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-02 00:43:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5968" class=".btn">#5968</a>
            </td>
            <td>
                <b>
                    Issue 5544 - Tessera as internal process
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
Fixes #5544 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 11:59:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5967" class=".btn">#5967</a>
            </td>
            <td>
                <b>
                    [4844] FCU Validate badblock before sync
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">4844</span>
            </td>
            <td>
                ## PR description
Validate bad blocks before asking for a new sync
## Fixed Issue(s)
fixes #5950
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 10:35:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5966" class=".btn">#5966</a>
            </td>
            <td>
                <b>
                    Use PendingTransaction in BlockTransactionSelector
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

This is just a refactoring, no functionality change, to have the `PendingTransaction` object during the selection of transactions, since in the `PendingTransaction` there are additional metadata about the candidate transaction that can be used by the selection process, and more will be added in a next PR to better support priority senders.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 09:08:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5964" class=".btn">#5964</a>
            </td>
            <td>
                <b>
                    add plugins summary
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                log a summary of plugins at registration time
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 01:55:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5961" class=".btn">#5961</a>
            </td>
            <td>
                <b>
                    Apply fcu even on invalid payload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes more Hive tests when a payload that is invalid is passed along with an FCU
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 00:11:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5960" class=".btn">#5960</a>
            </td>
            <td>
                <b>
                    Optionally bypass state root verification in reference test worldstate
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
if the passed block header has a stateroot of Hash.ZERO, bypass bonsai state root verification in bonsai reference test worldstate only.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #5934 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-27 20:45:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5959" class=".btn">#5959</a>
            </td>
            <td>
                <b>
                    Priority senders
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

~~This PR is build on top of #5966 so please check it first. [Relative diff](https://github.com/fab-10/besu/compare/main...priority-senders)~~

This PR expand the concept of priority of txs and senders. Currently in Besu by default every tx sent using the RPC API is called _local_, and _local_ is also a synonym for _priority_, that means that the tx does not need to satisfy the min price option and it is selected first when building a block, the txs received via p2p are called _remote_ and haven't any priority.
It is possible to disable this default behavior passing the option `--tx-pool-disable-locals`, and all txs are treated the same.
This simple approach does not works well if Besu is used as a gateway to publish txs for multiple senders, when the node owner what to prioritize only a subset of them, to support this use case, this PR add the `--tx-pool-priority-senders` option, with it is possible to specify the list of senders, whom txs have priority, regardless their origin, both local or remote.

Since _local_ is not always synonym of _priority_, the concepts have been separated, and so a `PendingTransaction` has both attributes as distinct fields, where _local_ is now only used to identify the source and _priority_ is used to apply or not the min price option and during the selection when building a block. To note that txs with priority will be dropped from the pool after the other ones.

To follow the new semantic of `--tx-pool-disable-locals` has been deprecated for removal in favor of `--tx-pool-no-local-priority`

To resume the possibility of mixing the priority options are:
1. Default (no option specified): All txs sent via RPC API are prioritized
2. `--tx-pool-no-local-priority=true`: No tx is prioritized
3. `--tx-pool-priority-senders=sender1,sender2`: All txs sent via RPC API are prioritized + all txs sent by _sender1_ and _sender2_
4. `--tx-pool-no-local-priority=true` `--tx-pool-priority-senders=sender1,sender2`: Only txs sent by _sender1_ and _sender2_ are prioritized

No functional or performance regressions found during the test. 

Comparison with prev release (A this PR, B current stable release)

Block Value
![image](https://github.com/hyperledger/besu/assets/91944855/aa8cecaa-e3a8-41cf-982f-b28b8a003e72)

Txs
![image](https://github.com/hyperledger/besu/assets/91944855/9d617f85-a6fc-4534-b1ad-cbc11e9dc6c4)

Gas used
![image](https://github.com/hyperledger/besu/assets/91944855/b28f2025-948b-47ca-a519-9f1fd767e63d)


## Fixed Issue(s)
Partially fixes #5829 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-27 19:04:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5957" class=".btn">#5957</a>
            </td>
            <td>
                <b>
                    Added toString implementation for TransactionSimulatorResult
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
Added toString implementation for TransactionSimulatorResult

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fix #5942
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-27 09:45:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5955" class=".btn">#5955</a>
            </td>
            <td>
                <b>
                    rlpx - Send empty list instead of Empty Bytes for the Ping and Pong message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                ## PR description
Send empty list instead of Empty Bytes for Ping and Pong message
https://github.com/ethereum/devp2p/blob/master/rlpx.md#ping-0x02
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-27 07:07:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5954" class=".btn">#5954</a>
            </td>
            <td>
                <b>
                    Fixup changelog following 23.7.3 release
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
        Created At 2023-09-27 05:03:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5953" class=".btn">#5953</a>
            </td>
            <td>
                <b>
                    Release 23.7.3
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
        Created At 2023-09-27 02:38:55 +0000 UTC
    </div>
</div>

