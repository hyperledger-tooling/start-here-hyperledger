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
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/152" class=".btn">#152</a>
            </td>
            <td>
                <b>
                    Provide a blocking mode for async msgs, and add more intuitive POST routes returning types not messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implements #112 

- Does _lots_ of dependency work to allow the sync-async bridge to be callable from broadcast/privatemessaging/networkmap
  - Adds a `syshandlers` package for the system event handlers that we previously bundled into `events`
  - Adds a `sysmessaging` that abstracts broadcast/private sends, and reply exchanges
  - Updates the orchestrator initialixation order to manage passing things between the internal components
- Deprecates all the old routes
- Adds new routes that:
  - Are all grouped on the path with the resources they create
  - Consistently return the object type that is the input
  - Have a `?confirm` option to block until the confirmation event arrives (or a 500 on the case it's rejected)
- Leaves the old routes there functioning exactly as today
  - Gives time for the CLI setup, and other consumers to move to the new routes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-09 02:50:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/151" class=".btn">#151</a>
            </td>
            <td>
                <b>
                    bump ui to v0.2.0
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
        Created At 2021-08-06 18:10:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/150" class=".btn">#150</a>
            </td>
            <td>
                <b>
                    Add optional counts to all filtered collection queries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #13 

Example results from a query of `http://localhost:5000/api/v1/namespaces/ff_system/messages?count&limit=2`

```json
{
  "count": 2,
  "total": 4,
  "items": [
    {
      "header": {
        "id": "40f30f03-c8d9-4c4c-984f-8023e36f5f02",
        "type": "definition",
        "txtype": "batch_pin",
        "author": "0x1cde1feef9ed07737d1e180208e3fb4014d0a5d4",
        "created": "2021-08-05T16:37:38.870531541Z",
        "namespace": "ff_system",
        "topics": [
          "ff_org_0x1cde1feef9ed07737d1e180208e3fb4014d0a5d4"
        ],
        "tag": "ff_define_node",
        "datahash": "e33cd600ea094ed8aac8ee0ef8b813f1ef8775fe15d95c2d00a512fef31d59b6"
      },
      "hash": "2641ea3ff8a92722507ada5c7fdd4a3efa479365827b5dd059588494e646ec74",
      "batch": "38c26dde-e09f-4f56-a896-b130afd6ddc3",
      "pending": false,
      "confirmed": "2021-08-05T16:37:48.34491Z",
      "data": [
        {
          "id": "eeb09caf-c26d-40fc-ab1b-4df36ee56103",
          "hash": "3dd6ab8545be3571b6b33abce8372db8ebbbd68766bf66d4e0211dbbc6788698"
        }
      ]
    },
    {
      "header": {
        "id": "75395af0-5c8c-4065-add6-74f48ba285a9",
        "type": "definition",
        "txtype": "batch_pin",
        "author": "0x1cde1feef9ed07737d1e180208e3fb4014d0a5d4",
        "created": "2021-08-05T16:37:30.816714921Z",
        "namespace": "ff_system",
        "topics": [
          "ff_org_0x1cde1feef9ed07737d1e180208e3fb4014d0a5d4"
        ],
        "tag": "ff_define_organization",
        "datahash": "128fe5e4add78e8e996834ab81acd8077ee6ed4ff37a0c9a948e142dae365377"
      },
      "hash": "cc59cba89f8e9798e1428edd8cf445fa7565944d1da79b99384ffbd808640819",
      "batch": "54cc3f0c-8c5b-40ff-bd3e-ec96dc5e02e4",
      "pending": false,
      "confirmed": "2021-08-05T16:37:38.586237Z",
      "data": [
        {
          "id": "144affec-10d4-43de-a68c-b04aac71f69c",
          "hash": "f784833b8c1ded6db1394847c4313ed7b8f86bf2f47217a1d178bd4f08370a90"
        }
      ]
    }
  ]
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-04 21:52:29 +0000 UTC
    </div>
</div>

