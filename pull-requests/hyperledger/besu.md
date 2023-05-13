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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5442" class=".btn">#5442</a>
            </td>
            <td>
                <b>
                    Fix for block import withdrawals
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
The initial intent of this PR was to fix the withdrawals field missing from the RawBlockIterator class used by the block import subcommand. Ended up introducing a refactor on some of the core methods of Block and BlockBody classes (readFrom and writeTo) aiming to remove duplicated code and reuse the existing logic defined in BlockBody.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #5431
It also fixes all the hive tests broken due to the impossibility of importing blocks (rpc-compat for example) that contained withdrawals via the `blocks import` subcommand.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-08 04:48:06 +0000 UTC
    </div>
</div>

