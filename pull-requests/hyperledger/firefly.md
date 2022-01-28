---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/457" class=".btn">#457</a>
            </td>
            <td>
                <b>
                    Add route for /transactions/{txnid}/status
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
        Created At 2022-01-27 22:11:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/456" class=".btn">#456</a>
            </td>
            <td>
                <b>
                    Allow calling JSONObject() on nil JSONAny
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix for #453 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 20:45:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/452" class=".btn">#452</a>
            </td>
            <td>
                <b>
                    Remove deprecated APIs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Proposal to do this removal for `v0.12.0`

Fixes #407 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 17:32:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/451" class=".btn">#451</a>
            </td>
            <td>
                <b>
                    Updated documentation to make it more useful
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I've added some changes in firefly documentation which I think will make it more useful and informative.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 13:35:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/448" class=".btn">#448</a>
            </td>
            <td>
                <b>
                    Add Blockchain Transaction IDs to FireFly Transaction objects and add blockchain IDs to events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Adds a string-array field of `blockchainIds` on the `transaction` object
  - Backed by a comma-separated field
  - Alphabetically sorted on each `UpsertTransaction` with lower-case only text, and no duplicates
  - Updated when blockchain operations complete
  - Updated when blockchain events arrive that are correlated with a blockchain transaction
  - In all current FireFly transaction types, should be zero or one blockchain transactions
  - Future extensibility to more
- Adds a structured `blockNumber/transactionIndex/eventIndex/subEventNumber` convention to all event IDs
   - Example `000000654321/000010/00002` would be:
      - Block number: `654321`
      - Transaction index: `10`
      - Log index (ethereum) / event number (fabric): `2`
   - The convention with padding (12/6/6/6 zeros) is intended to provide an alphabetically sortable list
   - For Fabric this feature depends on fixing https://github.com/hyperledger/firefly-fabconnect/issues/74
   - Tokens connectors are going to have tweaks to ensure the same number of zeros / separators for consistency
   - The final `subEventNumber` is reserved for protocols that batch logical events (such as transfers) in an data array emitted by a single event

Transaction example from E2E:

```js
{
  "id": "264200de-188a-4aae-92e7-1e5345604345",
  "namespace": "default",
  "type": "batch_pin",
  "created": "2022-01-25T22:01:08.9671519Z",
  "status": "Succeeded",
  "blockchainIds": [
    "0xb819561e2149c6a77a1de8a971895e486e064f45da26e1c48d2b4263eccffc43"
  ]
}
```

To which the following Blockchain event is associated:

```json
{
  "id": "8b85311c-b51f-4b69-bbbf-083ac4728db4",
  "sequence": 22,
  "source": "ethereum",
  "namespace": "default",
  "name": "BatchPin",
  "protocolId": "000000000031/000000/000000",
  "output": {
    "author": "0xce1fde1c97d3db88dbb83af16ac3b0efefeba80d",
    "batchHash": "0xb605c7d5238dd01fa594cab74db229a997e2c7c5150eeb43288ecdac30b62b97",
    "contexts": [
      "0x2a30597d4aca075c164bfb02c44de63802d66f1422295aa6b7ce8b0daa12c470"
    ],
    "namespace": "default",
    "payloadRef": "QmWC6JQnpoYAsWj6junfwaiq8DvQgoLBMQt2nkoaYmxzaZ",
    "timestamp": "1643148068",
    "uuids": "0x264200de188a4aae92e71e5345604345af60568cd62c48e69cadce0d498d0584"
  },
  "info": {
    "address": "0x3A4e59b55979d0D196aB39471DfA706b0a0CEce9",
    "blockNumber": "31",
    "logIndex": "0",
    "signature": "BatchPin(address,uint256,string,bytes32,bytes32,string,bytes32[])",
    "subId": "sb-51267be5-775c-4d22-6d72-b8a85675187b",
    "timestamp": "1643148068",
    "transactionHash": "0xb819561e2149c6a77a1de8a971895e486e064f45da26e1c48d2b4263eccffc43",
    "transactionIndex": "0x0"
  },
  "timestamp": "2022-01-25T22:01:08Z",
  "tx": {
    "type": "batch_pin",
    "id": "264200de-188a-4aae-92e7-1e5345604345"
  }
}
```

Event example from E2E:

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-25 21:41:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/447" class=".btn">#447</a>
            </td>
            <td>
                <b>
                    contract_invoke Transaction should mirror status of contract_invoke Operation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fundamental question: is this the right place for this logic to live, or is this propagating an anti-pattern?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-25 21:03:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/446" class=".btn">#446</a>
            </td>
            <td>
                <b>
                    Add convenience URL /transactions/{txnid}/blockchainevents
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
        Created At 2022-01-25 19:41:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/444" class=".btn">#444</a>
            </td>
            <td>
                <b>
                    Restore Transaction reference on TokenTransfer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Although transfers initiated outside of FireFly will NOT have a Transaction, it's
still useful to track Transactions for those transfers initiated by FireFly. This
is needed for tracking of async transfer requests, filtering transfers, etc.

Partially reverts 0e654d2a7b9960e3d2a4946c788f80e5052e056e
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 23:17:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/443" class=".btn">#443</a>
            </td>
            <td>
                <b>
                    Rename /contracts/events to /blockchainevents
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also move the query helpers from Contract Manager to Orchestrator, as this
has become a generic construct that spans more than one manager/plugin.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 22:52:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/441" class=".btn">#441</a>
            </td>
            <td>
                <b>
                    Create a Transaction and Operation for contract invoke requests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #393
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 19:14:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/439" class=".btn">#439</a>
            </td>
            <td>
                <b>
                    v0.11.x backport: Ready state changes require a bump to the message to re-sequence it
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport_v0.11.x</span>
            </td>
            <td>
                Backport of #438 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-23 21:33:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/438" class=".btn">#438</a>
            </td>
            <td>
                <b>
                    Ready state changes require a bump to the message to re-sequence it
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-candidate</span><span class="chip">backport-complete</span>
            </td>
            <td>
                Fixes the core symptom reported in #421 

> Note that this does not implement the full change to batches described in the discussion on that issue.
> However, when that change happens, this fix will still be applicable.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-23 17:41:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/436" class=".btn">#436</a>
            </td>
            <td>
                <b>
                    Add AddressResolver to Ethereum for key-to-address mapping
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a REST-pluggable interface to the ethereum Blockchain plugin, that allows it to resolve non-Address strings (such as hierarchical HD wallet addresses) into ethereum addresses.

This supports a common configuration for signing as follows:

```
┌------------┐            ┌------------┐                ┌------------┐                ┌------------┐
|            |            |            |                |            |                |            |
|            |            |            |                |            |                |            |
|  FireFly   | -- REST -> | EthConnect | -- JSON/RPC -> |   Signer   | -- JSON/RPC -> |    Node    |
|            |            |            |   (unsigned)   |            |    (signed)    |            |
|            |            |            |                |            |                |            |
└-----┬------┘            └------------┘                └-----┬------┘                └------------┘
      |                                                       |
      └---------- Resolve non-address signing key ID ---------┘
```

Note that much of the FireFly relies on one-time resolution of the signing key, into a string
that is stored in database objects for later signing.

So once the interface has been used to resolve the key the target microservice **must**
reliably retain knowledge of the resolved address such that it can be used to perform
the actual transaction signing.

> The original input string is discarded by FireFly after resolution
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-23 02:01:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/435" class=".btn">#435</a>
            </td>
            <td>
                <b>
                    Fail transaction when token transfer operation fails
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #434
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 21:29:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/432" class=".btn">#432</a>
            </td>
            <td>
                <b>
                    v0.11.x backport: Fixing Websocket Connections when Prometheus Metrics Enabled + containerd update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport_v0.11.x</span>
            </td>
            <td>
                See #371

Also contains #414 `go.mod` update
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 03:36:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/431" class=".btn">#431</a>
            </td>
            <td>
                <b>
                    v0.11.x backport: Fix token account listing on Postgres
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport_v0.11.x</span>
            </td>
            <td>
                See #422 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 03:25:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/430" class=".btn">#430</a>
            </td>
            <td>
                <b>
                    v0.11.x backport: Add ping/pong heartbeating to WSClient, and fix concurrent map on config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport_v0.11.x</span>
            </td>
            <td>
                See https://github.com/hyperledger/firefly/pull/420
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 03:16:20 +0000 UTC
    </div>
</div>

