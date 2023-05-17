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
                
            </td>
            <td>
                ## PR description
Body Size Limit for BodyHandler in Vert.x Route: A limit on body size for the BodyHandler is introduced to prevent memory overuse and improve application robustness. (Set to 100MB)

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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5449" class=".btn">#5449</a>
            </td>
            <td>
                <b>
                    Implement Limit on Resource-Intensive Batch Requests in JSON RPC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span><span class="chip">mainnet</span><span class="chip">RPC</span>
            </td>
            <td>
                ## PR description

This Pull Request introduces a new limitation mechanism for batch requests in Besu's JSON RPC that are deemed resource-intensive. Non-resource-intensive methods can be called without restrictions, while resource-intensive requests are now subject to a limit, which is defined by Besu's `JsonRpcConfiguration`. Currently, the `eth_call` method is the only one marked as resource-intensive.

Changes

- Introduced a limit on the number of resource-intensive requests that can be executed in a batch of JSON RPC requests within Besu. The limit is configurable.
- Implemented an optional command-line interface parameter `rpc-http-max-resource-intensive-per-batch-size` allowing users to manually adjust the resource-intensive request limit as per their needs.
- Established a new error response mechanism. If the number of resource-intensive requests exceeds the set limit, all subsequent resource-intensive requests will receive a specific error.

For instance, given the limit of 1 for the resource-intensive eth_call method, the response to this batch of requests would be:

Request
```
[
  {"jsonrpc":"2.0", "method":"eth_call", "params":[{/*parameters for eth_call*/}], "id":1},
  {"jsonrpc":"2.0", "method":"eth_call", "params":[{/*parameters for eth_call*/}], "id":2},
  {"jsonrpc":"2.0", "method":"eth_getTransactionCount", "params":[{/*parameters for eth_getTransactionCount*/}], "id":3},
  {"jsonrpc":"2.0", "method":"eth_getBlockByNumber", "params":[{/*parameters for eth_getBlockByNumber*/}], "id":4}
]
```
Response:
```
[
  {
    "jsonrpc": "2.0",
    "id": 1,
    "result": { /* result of first eth_call */ }
  },
  {
    "jsonrpc": "2.0",
    "id": 2,
    "error": {
      "code": -32005,
      "message": "Resource-Intensive Request Limit Exceeded",
    }
  },
  {
    "jsonrpc": "2.0",
    "id": 3,
    "result": { /* result of eth_getTransactionCount */ }
  },
  {
    "jsonrpc": "2.0",
    "id": 4,
    "result": { /* result of eth_getBlockByNumber */ }
  }
]
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-12 04:32:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5448" class=".btn">#5448</a>
            </td>
            <td>
                <b>
                    Fix 'locahost' typo in log config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Fix minor typo in log host default value

## Fixed Issue(s)
None
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-11 16:16:32 +0000 UTC
    </div>
</div>

