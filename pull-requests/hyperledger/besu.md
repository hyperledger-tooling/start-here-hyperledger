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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5467" class=".btn">#5467</a>
            </td>
            <td>
                <b>
                    JsonRpcHttpService - Add BodyHandler limit size 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span><span class="chip">TeamRevenant</span><span class="chip">mainnet</span><span class="chip">RPC</span>
            </td>
            <td>
                ## PR description
Body Size Limit for BodyHandler in Vert.x Route: A limit on body size for the BodyHandler is introduced to prevent memory overuse and improve application robustness. (Set to 5MB)

`--rpc-http-max-request-content-length ` overrides the limit. 



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-17 02:10:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5465" class=".btn">#5465</a>
            </td>
            <td>
                <b>
                    handle cases where dagger besuComponent is null
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
fix cases where BesuCommand is constructed without a dagger context

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-16 23:32:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5462" class=".btn">#5462</a>
            </td>
            <td>
                <b>
                    Fix Docker image failing to start Besu with NoClassDefFoundError for org.xerial.snappy.Snappy
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
Fix Besu failing to start when using Docker 23.4.0 due to `NoClassDefFoundError` for `org.xerial.snappy.Snappy`.

The cause was that we are using an older version of glibc for some Docker images due to the older version of the Ubuntu distro being used.

Changes
- Updated docker images to use Ubuntu 22.04 so that a newer version of glibc is used. This fixes an issue with snappy library where the library cannot be loaded.
- Included ca-certificates-java as a separate install to fix Java install issue on Ubuntu https://github.com/adoptium/installer/issues/105

Related to the update of the snappy library https://github.com/xerial/snappy-java/issues/417#issuecomment-1513916298

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #5463 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-16 04:45:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5458" class=".btn">#5458</a>
            </td>
            <td>
                <b>
                    JSON array handling Improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span><span class="chip">mainnet</span><span class="chip">RPC</span>
            </td>
            <td>
                ## PR description

- Separation of JsonObjectHandler and JsonArrayHandler: JsonObjectHandler and JsonArrayHandler are now distinct classes, enhancing code readability and maintainability.

- Optimised JSON RPC Array Request Processing: Outputs of individual requests are now directly written to the JsonGenerator

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-15 23:55:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5457" class=".btn">#5457</a>
            </td>
            <td>
                <b>
                    Change to more user-friendly message
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
Following the suggestion (https://github.com/hyperledger/besu/pull/5452#discussion_r1193426313) and changing to a more user-friendly message.
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
FIxes #5416 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-15 22:53:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5454" class=".btn">#5454</a>
            </td>
            <td>
                <b>
                    Log access denied error separately to other IO exceptions so cause is clearer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR logs `AccessDeniedException`s separately to generic `IOException`s when loading static node config.

## Fixed Issue(s)
Possibly fixes https://github.com/hyperledger/besu/issues/3986 (it looks there have been various commits that have improved the behaviour described in the issue. I think this PR further improves it by differentiating between access denied and general file IO issues, but whether it can actually be closed I'm not sure. Maybe the PR reviewer can comment on that and remove this `fixes` statement if they think the issue needs to remain open)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-15 10:45:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5453" class=".btn">#5453</a>
            </td>
            <td>
                <b>
                    Only create DB data dir if it doesn't already exist
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR skips creation of the database directory if it exists. While the call to `Files.createDirectories()` (which we use to initialise it if the DB needs creating) should be a no-op in this case, symlinks cause it to fail so the safer thing to do is confirm that the directory doesn't actually exist before making that call.

## Fixed Issue(s)
Fixed https://github.com/hyperledger/besu/issues/4043
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-15 09:58:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5452" class=".btn">#5452</a>
            </td>
            <td>
                <b>
                    Add info log to indicate Besu is waiting on CL to be synced
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
Add a info log so users can better understand why besu isn't doing anything when it's actually waiting on CL to send a FCU. 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #5416 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-15 03:25:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5451" class=".btn">#5451</a>
            </td>
            <td>
                <b>
                    Restore transactions from disk searially to avoid blocking other threads
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

I could happen that when restoring many transactions from disk, to have Vertx thread blocked exception, to avoid that is it safer to restore transactions serially than in parallel.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-12 10:11:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5450" class=".btn">#5450</a>
            </td>
            <td>
                <b>
                    Layered txpool reconcile sender
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

Added a general way to detect nonce discrepancies between world state and the txpool view for a sender, that could happen during the small amount of time during block import when the world state is update while the txpool still does not process the confirmed txs, or when there is a reorg and the sender nonce goes back, and if a nonce discrepancy is detected the txs for the sender are reconciled according with the world state nonce.

The new solution replace the solution that was in place to handle reorg, since it is general and covers all the cases of nonce discrepancies.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #5447 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-12 09:42:03 +0000 UTC
    </div>
</div>

