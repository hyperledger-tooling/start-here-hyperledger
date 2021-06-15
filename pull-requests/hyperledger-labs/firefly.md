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

