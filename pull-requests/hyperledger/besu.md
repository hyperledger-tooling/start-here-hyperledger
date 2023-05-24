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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5469" class=".btn">#5469</a>
            </td>
            <td>
                <b>
                    Log more info about proposed blocks
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

at INFO level, instead of only logging this

```
Fetch block proposal by identifier: 0x0068a2d68ca65973, hash: 0x450b0b3269e8a90df99e41bd2436ac69e45b66d24c7a79e5c96448892becb137, number: 9017061, coinbase: 0x3826539cbd8d68dcf119e80b994557b4278cec9f, transaction count: 72
```

this is logged, additions are: the start of the block creation, and when the proposal is fetched the gas used and the reward.

```
Start building proposals for block 9017061 identified by 0x0068a2d68ca65973
Fetch block proposal by identifier: 0x0068a2d68ca65973, hash: 0x450b0b3269e8a90df99e41bd2436ac69e45b66d24c7a79e5c96448892becb137, number: 9017061, coinbase: 0x3826539cbd8d68dcf119e80b994557b4278cec9f, transaction count: 72, gas used: 38.80%, reward: 19.00 finney
```

at DEBUG level every time a better block is found logs more info about the block
```
{"@timestamp":"2023-05-17T17:22:48,970","level":"DEBUG","thread":"PoS-Block-Builder-0","class":"PostMergeContext","message":"Current best proposal for block 9017091: txs 26, gas used 22.37%, reward 10.22 finney","throwable":""}
{"@timestamp":"2023-05-17T17:22:49,482","level":"DEBUG","thread":"PoS-Block-Builder-0","class":"PostMergeContext","message":"Current best proposal for block 9017091: txs 29, gas used 22.98%, reward 13.12 finney","throwable":""}
{"@timestamp":"2023-05-17T17:22:50,493","level":"DEBUG","thread":"PoS-Block-Builder-0","class":"PostMergeContext","message":"Current best proposal for block 9017091: txs 35, gas used 25.36%, reward 15.16 finney","throwable":""}
{"@timestamp":"2023-05-17T17:22:51,000","level":"DEBUG","thread":"PoS-Block-Builder-0","class":"PostMergeContext","message":"Current best proposal for block 9017091: txs 37, gas used 27.19%, reward 15.16 finney","throwable":""}
{"@timestamp":"2023-05-17T17:22:51,546","level":"DEBUG","thread":"PoS-Block-Builder-0","class":"PostMergeContext","message":"Current best proposal for block 9017091: txs 38, gas used 27.56%, reward 15.93 finney","throwable":""}
{"@timestamp":"2023-05-17T17:22:51,990","level":"DEBUG","thread":"PoS-Block-Builder-0","class":"PostMergeContext","message":"Current best proposal for block 9017091: txs 40, gas used 27.70%, reward 16.30 finney","throwable":""}
{"@timestamp":"2023-05-17T17:22:52,554","level":"DEBUG","thread":"PoS-Block-Builder-0","class":"PostMergeContext","message":"Current best proposal for block 9017091: txs 44, gas used 29.18%, reward 18.18 finney","throwable":""}
{"@timestamp":"2023-05-17T17:22:53,024","level":"DEBUG","thread":"PoS-Block-Builder-0","class":"PostMergeContext","message":"Current best proposal for block 9017091: txs 46, gas used 29.46%, reward 18.33 finney","throwable":""}
{"@timestamp":"2023-05-17T17:22:53,503","level":"DEBUG","thread":"PoS-Block-Builder-0","class":"PostMergeContext","message":"Current best proposal for block 9017091: txs 50, gas used 30.56%, reward 20.86 finney","throwable":""}
{"@timestamp":"2023-05-17T17:22:54,003","level":"DEBUG","thread":"PoS-Block-Builder-0","class":"PostMergeContext","message":"Current best proposal for block 9017091: txs 53, gas used 31.07%, reward 21.66 finney","throwable":""}
{"@timestamp":"2023-05-17T17:22:55,007","level":"DEBUG","thread":"PoS-Block-Builder-0","class":"PostMergeContext","message":"Current best proposal for block 9017091: txs 54, gas used 31.14%, reward 22.66 finney","throwable":""}
{"@timestamp":"2023-05-17T17:22:55,528","level":"DEBUG","thread":"PoS-Block-Builder-0","class":"PostMergeContext","message":"Current best proposal for block 9017091: txs 57, gas used 31.57%, reward 23.27 finney","throwable":""}
{"@timestamp":"2023-05-17T17:22:56,838","level":"DEBUG","thread":"PoS-Block-Builder-0","class":"PostMergeContext","message":"Current best proposal for block 9017091: txs 62, gas used 34.31%, reward 29.26 finney","throwable":""}
{"@timestamp":"2023-05-17T17:22:57,285","level":"DEBUG","thread":"PoS-Block-Builder-0","class":"PostMergeContext","message":"Current best proposal for block 9017091: txs 64, gas used 34.93%, reward 31.24 finney","throwable":""}
{"@timestamp":"2023-05-17T17:22:57,713","level":"DEBUG","thread":"PoS-Block-Builder-0","class":"PostMergeContext","message":"Current best proposal for block 9017091: txs 66, gas used 35.24%, reward 33.10 finney","throwable":""}
{"@timestamp":"2023-05-17T17:22:58,811","level":"DEBUG","thread":"PoS-Block-Builder-0","class":"PostMergeContext","message":"Current best proposal for block 9017091: txs 69, gas used 43.41%, reward 34.15 finney","throwable":""}
```


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-17 17:26:27 +0000 UTC
    </div>
</div>

