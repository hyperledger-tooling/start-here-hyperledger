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
                PR <a href="https://github.com/hyperledger/besu/pull/5986" class=".btn">#5986</a>
            </td>
            <td>
                <b>
                    Validation ordering
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - corrects a number of validation errors by adjusting priority of evaluations
- covers and corrects a subtle issue where besu would propose bad blocks in the event of a re-org prior to a proposal which restored blob transactions to mempool.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-04 22:03:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5985" class=".btn">#5985</a>
            </td>
            <td>
                <b>
                    Transaction detachedCopy to optimize txpool memory usage
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

When a tx is decoded from RLP, some of its fields are reference to slices of the encoded RLP byte array, the latter could be shared by many transactions at the same time, for example when decoding the block body, every tx object keep a reference to the large RLP byte array, that could be hundred of KB long, the same happens when we receive a bunch on txs via p2p in the same message.
This approach works fine if the tx objects are short lived, since it means allocating and copying less data around, but does not fit well for pending txs, since they could live much longer in the txpool and a single tx could keep a reference to a large byte array, while actually only it only needs a small portion of it.

This PR solve this memory inefficiency, by creating a _detachedCopy_ of the tx when this is added to the txpool. A _detachedCopy_ is a copy that does not share any byte array with others. This also changes previous assumptions on the estimation of the amount of memory used by a pending tx, so the calculation have been updated and extended to cover also the Blob tx estimation.

relates #5977 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-04 12:57:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5983" class=".btn">#5983</a>
            </td>
            <td>
                <b>
                    [MINOR] Expose getSize to transaction interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Exposes getSize to transaction interface so it can be used by plugins
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-04 05:48:13 +0000 UTC
    </div>
</div>

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
Simple default retry policy for rocksdb busy and locktimeout exceptions.

**This may or may not remedy the busy exceptions encountered in the listed issues, but it will at a minimum provide better signal regarding whether these are transient issues due to compaction, or more systemic issues

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

fixes #5977 
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

