---
layout: default
title: firefly
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/51" class=".btn">#51</a>
            </td>
            <td>
                <b>
                    Dynamic config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a new `/config` endpoint which can be used for dynamically adding or modifying config at runtime via a REST API. Any change in configuration will result in a restart of all services and plugins (not the process itself though).

Due to how powerful (dangerous) the new configuration endpoints are, they have been moved to a separate “admin” HTTP listener which will listen on a separate port, if enabled at all. By default, it is disabled. To enable the admin endpoints, add the following lines to your firefly.core config:

```yaml
admin:
  enabled: true
  address: 0.0.0.0
  port: 5001
```

To set a configuration key make a `PUT` request to `/admin/api/v1/config/{key}` with a JSON request body.


For example, if you want to set the HTTP URL for ethconnct, you would make a `PUT` request to `/admin/api/v1/config/blockchain.ethereum.ethconnect` with a request body of:

```json
{
  "url": "http://some_url"
}
```

The payload will be merged with any existing config. This means that it is not possible to _remove_ configuration keys that are present in the config file, via the REST API.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 01:58:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/50" class=".btn">#50</a>
            </td>
            <td>
                <b>
                    first pass of Github Pages documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-08 21:58:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/49" class=".btn">#49</a>
            </td>
            <td>
                <b>
                    Add private send API route
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Example `POST` to `/api/v1/namespaces/{ns}/send/message`

```json
{
  "data": [{
      "value": "hello world"
  }],
  "group": {
    "members": [
      {"identity": "org_0"},
      {"identity": "org_1"}
    ],
    "name": "mygroup1"
  }
}
```

There are a few bug fixes in the PR from testing end to end, particularly around ensuring the groupid propagates through the layers where it needs to.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-08 21:37:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/48" class=".btn">#48</a>
            </td>
            <td>
                <b>
                    Fix logic for querying "local" flag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-08 15:23:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/47" class=".btn">#47</a>
            </td>
            <td>
                <b>
                    HTTP Data Exchange plugin connections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Fills out the Data Exchange interfaces
  - Get endpoint info (to broadcast)
  - Add peer (from broadcast)
  - Upload blob (streaming interface - ns+UUID)
  - Download blob (streaming interface - ns+UUID)
  - Send message (in-line bytes)
  - Send blob (must already be uploaded - not yet fully integrated with core in this PR)

- Implements the integration with https://github.com/kaleido-io/firefly-dataexchange-https
  - HTTPS + WebSockets using the standard clients already built into core

- Implements batch off-chain message transfer
  - Messages are used for the transfer of the `batch` data
  - The heavy lifting was already complete in #42, so this just joins the dots of sending data and processing events

- Nodes now have `name` and `owner` (not an identity)
  - This is because for Data Exchange, there is a `peerID` as well. So it's not possible to reconcile a single identity with a node
  - So now instead when a message arrives over the private data exchange, we can use the `peerID` to lookup the node, and then resolve the identity matching that
  - We traverse up the tree, so if a batch arrives signed by an org, and that org has a parent, we are will to accept that message from any node that is owned by any org as you move up the hierarchy.

- Groups no longer have a UUID (or a description)
  - Instead are identified via a `hash` combining:
    - The list of members
    - The ledger (Fabric channel etc.)
    - An application specified `name`
  - This means all referring objects, like `Message` etc. now use a Bytes32 rather than UUID to refer across
  - This was important, to allow applications to simply define+use groups without waiting for propagation and agreement on which ID wins. Now it doesn't matter which group initiation message is sent first, as all the definitions are the same, and the later ones will be ignored. It just matters that the same member list is used in each. The name is optional.

- Rewind support for the event aggregator in the case of off-chain data arriving after a batch pin on-chain TX
  - Simply rewinds the `offset` back to the earliest offset in the batch that arrived
  - We re-process any `pin` entries since then, that aren't already marked `dispatched`

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-08 14:51:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/46" class=".btn">#46</a>
            </td>
            <td>
                <b>
                    add namespace filter to TransactionFactory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 - allows transaction queries to be filtered by namespace
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-08 14:27:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/42" class=".btn">#42</a>
            </td>
            <td>
                <b>
                    Gen2 pluggable Private Messaging [Pm] interface + API naming updates based on feedback
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Adds the `private messaging [Pm]` Private Messaging Interface
- Updates the aggregator for the gen2 private messaging support
  - Renames `blocked` to `pins` to be the sequence of pinning operations, in the blockchain derived order
    - For broadcast this includes hashed topics as the `context`
    - For private messaging this is a masked `pin` that is a function of the `topic`+`group`+`sender`+`nonce`
  - Introduces `nextpins` within private groups, so everyone knows what the next message from each sender is
     - Without leaking a static identifier between transactions to the chain
- API updates, driven primarily by feedback from @awrichar @jimthematrix @nguyer :
  -`author` -> `signer` on `Transaction` - as it contains the onchain identity (resolved via the `[Ii]` plugin)
  - `recipient` -> `member` on `Group`
  - `topic` -> `tag` on `Message` - this is a single value, that classifies the message and how it should be processed
  - `context` -> `topics` on `Message` - this is the stream that links together multiple messages that must be ordered
     - Added plural here, as we regularly see business requirements to merge topics (group data mapping use cases etc.)
- Solidity updates
 - Single transaction for all pinned batches
 - New fields are:
   - `Namespace` - in the clear namespace
   - `TransactionID` - the UUID generated in FireFly for the transaction
   - `BatchID` - the UUID generated in FireFly for the batch
   - `BatchHash` - the SHA256 hash of the batch (broadcast or private)
   - `PayloadRef` - for broadcast only, the off-chain public storage reference to get the batch contents
   - `Contexts` - an array of every context in the batch, which are masked for private transfers
- Event updates - reconciled event types
   - `message_confirmed` - happens on the namespace of the message (including `ff_system` for definitions)
   - `message_invalid` - if a message is rejected at a point we know what it is - such as due to schema validation
   - `namespace_confirmed` - occurs on the namespace when a broadcasted namespace is confirmed
   - `namespace_confirmed` - occurs on the namespace of a datatype when a new datatype is confirmed
   - `group_confirmed` - occurs in the private group, on the namespace, when a group creation is confirmed

Example ethereum representation of the batch pin transaction.
This is a broadcast, and in this case the same topic in every message.

```json
{
    "namespace": "default",
    "uuids": "0xb67d5c84ab8d43ea8600fc108645db1bf4e9989e3fc840d08175ec1d08891ee4",
    "batchHash": "0x16b78c32f8c728611ded3f2dfe84108ad75f88a2cf0297770c8875a85c1485c0",
    "payloadRef": "0x387f34a30f68a94ef571a2a69c147ecf3ea978a712d0054dcf1e1a4abe2471da",
    "contexts": [
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f",
        "0x37a8eec1ce19687d132fe29051dca629d164e2c4958ba141d5f4133a33f0688f"
    ]
}
```

In PR chain with #40 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-02 21:06:47 +0000 UTC
    </div>
</div>

