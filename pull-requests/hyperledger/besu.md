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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5444" class=".btn">#5444</a>
            </td>
            <td>
                <b>
                    Update dependencies - commons-net
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Refs #5386 
This PR forces the commons-net version to be 3.9.0 but we can't do the same for antlr. antlr version needs to match the version in tuweni. So we need a tuweni release before we can update antlr.
This PR has the version we want but it's not yet released https://github.com/apache/incubator-tuweni/pull/479
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-09 05:40:29 +0000 UTC
    </div>
</div>

