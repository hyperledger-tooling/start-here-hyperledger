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
                PR <a href="https://github.com/hyperledger/besu/pull/5492" class=".btn">#5492</a>
            </td>
            <td>
                <b>
                    Detailed transaction selection stats for layered txpool
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

Expand the transaction selection result adding more fine grained info specifically about the reason a transaction is skipped or tagged as invalid, and also specify if the selection ended due to block full or block over min occupancy ratio.
These results are also collected so at the end of the selection we can log detailed stats, that are useful to understand which are the main reasons for a transaction not to be selected, and so improve the way transactions are prioritized, to avoid proposing these transactions in the first place.

Stats are logged at debug level, and here it is a sample:
```
Selection stats: Totals[Evaluated=425, Selected=272, Skipped=153, Dropped=0]; Detailed[BLOCK_OCCUPANCY_ABOVE_THRESHOLD (stop=true, discard=false)=1, SELECTED (stop=false, discard=false)=272, INVALID_TRANSIENT (stop=false, discard=false)(GAS_PRICE_BELOW_CURRENT_BASE_FEE)=152]
```

This helped spotting some optimizations and understand [the effect of `min-block-occupancy-ratio` on PoS networks](https://github.com/hyperledger/besu/pull/5492)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-24 12:27:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5491" class=".btn">#5491</a>
            </td>
            <td>
                <b>
                    Ignore min-block-occupancy-ratio option when on PoS
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

[`min-block-occupancy-ratio` option ](https://besu.hyperledger.org/en/stable/public-networks/reference/cli/options/#min-block-occupancy-ratio) make sense on PoW networks where you need to be faster that other nodes in finding a block, so you can set be satisfied when the block produced is enough filled, but on PoS you do not need to compete with other nodes, since you have an allocated slot to produce the block, so in this case make sense to always try to fill the block, until the remaining gas is less than the minimum needed for the smaller transaction.
So for PoS the `min-block-occupancy-ratio` option is ignored since we always try to fill 100% of the block.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-24 08:37:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5483" class=".btn">#5483</a>
            </td>
            <td>
                <b>
                    Remove TOML table headings before checking for valid config parameters
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR modifies the TOML parsing function `checkUnknownOptions()` to remove TOML headings before checking if all of the attributes are valid. E.g. for the following file:

```
[TxPool]
tx-pool-max-size = 1024
```

the `TxPool` TOML parameter will be removed and ignored as per the discussion in the related issue.

## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/5482

Remaining tasks before PR review:

- [ ] Add unit test
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-23 14:52:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5479" class=".btn">#5479</a>
            </td>
            <td>
                <b>
                    Remove bonsai accumulator trielogfactory
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
Fixes a refactor omission.  TrieLogFactory was still statically constructed and used in accumulator.  This would lead to besu writing trie logs to its database with the default TrieLog serializer rather than one (potentially) configured via plugin.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-19 19:18:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5476" class=".btn">#5476</a>
            </td>
            <td>
                <b>
                    Implement debug_getRawReceipts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                ## PR description
Implements the `debug_getRawReceipts` RPC method. This allows retrieving all receipts in a block in one call without the overhead of computing derived values. Return value is a plain array of RLP encoded receipts from the block.  e.g:

```shell
cast rpc debug_getRawReceipts latest
["0x7ef9010c0182fa0db9010000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000c08353766d"]
```

Method is included in https://ethereum.github.io/execution-apis/api-documentation/ though not with a lot of detail.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-19 10:35:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5475" class=".btn">#5475</a>
            </td>
            <td>
                <b>
                    Blobdb for static data
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

This PR is built on top of https://github.com/hyperledger/besu/pull/5471, so check it first.

This PR introduces optimizations for RocksDB column families that contain static data, i.e. key value entries that are never changed, but only added, like an append log storage, the best example is the blockchain storage, that benefit if [BlobDB ](https://github.com/facebook/rocksdb/wiki/BlobDB) is used for them, since the write amplification is highly reduced, with the result of faster initial sync and less wear out of SSD.

Preliminary test shows that checkpoint sync is faster with BlobDB enabled, more tests are ongoing, and will share the results later.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #4607 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-19 09:29:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5474" class=".btn">#5474</a>
            </td>
            <td>
                <b>
                    remove old EF bootnodes
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
This PR removes old EF bootnodes .Would like someone from the EF team validate this before we move forward with that.
@skylenet @parithosh Could please confirm these bootnodes don't exist anymore?


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-19 05:20:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5473" class=".btn">#5473</a>
            </td>
            <td>
                <b>
                    Invalid transaction type - report to user
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">RPC</span><span class="chip">ux</span>
            </td>
            <td>
                If transaction validation fails because of "Invalid transaction type", report that error back to the user (previously was "invalid params")
This will make situations like this easier to troubleshoot -
https://discord.com/channels/905194001349627914/938504958909747250/1108931495797727354
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-19 03:50:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5471" class=".btn">#5471</a>
            </td>
            <td>
                <b>
                    Introduce variables storage
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

This is the first PR of a series to reorganize the data in db, in order to pave the way to future optimizations.
The first goal that we want to achieve is the optimization of the db for data that is static, leveraging [the BlobDB](https://github.com/facebook/rocksdb/wiki/BlobDB) feature.
For static data like blockchain or trie logs, BlobDB is a better choice since it reduces a lot the write amplification during compaction, with the result of faster initial sync and less wear out of the disk.

Now we have variable data mixed with static data in the blockchain column family, and this is not optimal, so this PR moved the _variabiles_ into the dedicated column family `VARIABLES` that we can further optimize for frequently changing data in future.

The PR is meant to keep backward compatibility and is able to migrate existing variables to the new location on startup. 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-18 15:45:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5470" class=".btn">#5470</a>
            </td>
            <td>
                <b>
                    Add more backwards sync logging to debug nimbus issue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Using this PR to deploy the code on a test node, may or may not want to merge this logging
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-17 23:31:04 +0000 UTC
    </div>
</div>

