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

This Pull Request introduces a new limitation mechanism for batch requests in Besu's JSON RPC that are deemed resource-intensive. Non-resource-intensive methods can be called without restrictions, while resource-intensive requests are now subject to a limit, which is defined by Besu's `JsonRpcConfiguration`.

Changes

- Introduced a limit on the number of resource-intensive requests that can be executed in a batch of JSON RPC requests within Besu. The limit is configurable.
- Implemented an optional command-line interface parameter `rpc-http-max-resource-intensive-per-batch-size` allowing users to manually adjust the resource-intensive request limit as per their needs.
- Established a new error response mechanism. If the number of resource-intensive requests exceeds the set limit, all subsequent resource-intensive requests will receive a specific error.

For instance:

```
[
  {"jsonrpc":"2.0", "method":"eth_call", "params":[{/*parameters for eth_call*/}], "id":1},
  {"jsonrpc":"2.0", "method":"eth_call", "params":[{/*parameters for eth_call*/}], "id":2},
  {"jsonrpc":"2.0", "method":"eth_getTransactionCount", "params":[{/*parameters for eth_getTransactionCount*/}], "id":3},
  {"jsonrpc":"2.0", "method":"eth_getBlockByNumber", "params":[{/*parameters for eth_getBlockByNumber*/}], "id":4}
]
```
Given the limit of 1 for the resource-intensive eth_call method, the response to this batch of requests would be:

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
      "code": -32600,
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5440" class=".btn">#5440</a>
            </td>
            <td>
                <b>
                    TrieLogFactory plugin support
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

PR does some plumbing to get TrieLogs and TrieLogFactory into the plugin-api, such that we can have a pluggable TrieLog serializer/deserializer and event observer.  Having trielogs in plugin-api also facilitates trielog push and pull to remote services.

notable changes/rearrangement:

* in plugin-api/services
  * adds TrieLogService 
  * adds plugin-api/services/trielog package:
    * TrieLog, now plugin interface for TrieLogLayer
    * TrieLog.LogTuple, now plugin interface for BonsaiValue
    * TrieLogEvent
    * TrieLogObserver
    * TrieLogAccumulator, now plugin interface for BonsaiWorldStateUpdateAccumulator

* in data types:
  * moves StorageSlotKey, into data-types
  * adds AccountValue, in data-types, now interface  for StateTrieAccountValue and BonsaiAccount
    
* writeRlp and writeInnerRlp moved from BonsaiValue into TrieLogFactory
* TrieLog now exposes the account, code, and storage maps directly rather than only via stream
    

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes protocol-misc # 756
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-06 02:35:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5439" class=".btn">#5439</a>
            </td>
            <td>
                <b>
                    Add option to send SNI header in TLS ClientHello message [#4894]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                ## PR description

Adds an option to send an SNI header on a TLS ClientHello message. Given the existing exposed options for the `TLSConfiguration`, I went for the `--Xp2p-tls-*` prefix for the new sni header option, instead of `p2p-tls-clienthello-sni` as it was stated in #4894 . Please let me know if you prefer otherwise.

* add --Xp2p-tls-clienthello-sni option to enable the SNI header

## Fixed Issue(s)
fixes hyperledger#4894
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-05 09:59:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5438" class=".btn">#5438</a>
            </td>
            <td>
                <b>
                    Enable blobs on Blockchain and trie log column families
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
Enable blobs on Blockchain and trie log column families.
Only values that are bigger than 4 KiB are written to Blobs

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-05 09:09:06 +0000 UTC
    </div>
</div>

