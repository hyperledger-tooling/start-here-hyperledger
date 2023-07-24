---
layout: default
title: firefly-ethconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-ethconnect
---

# firefly-ethconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-ethconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/235" class=".btn">#235</a>
            </td>
            <td>
                <b>
                    Add synchronized flag to subscriptions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a new flag to a subscription to indicate whether ETHConnect is still catching up or has caught up to the configured block height gap, and is keeping up with the chain head. When you do a `GET` on a subscription you will now see a `synchronized` field like this:

```json
    {
        "created": "2023-07-24T17:02:29Z",
        "id": "sb-6e37fa9f-1a8c-48e1-6159-0f15701e15e5",
        "path": "/subscriptions/sb-6e37fa9f-1a8c-48e1-6159-0f15701e15e5",
        "name": "default_BatchPin_3078626437333333",
        "stream": "es-900f1d84-22fd-470f-54cd-b87d3e9e475a",
        "filter": {
            "address": [
                "0xbd7333f75351fe1bfc0e6f0bf2c01fc185beaf4a"
            ],
            "topics": [
                [
                    "0x805721bc246bccc732581be0c0aa2dd8f7ec93e97ba4b307be84428c98b0a12f"
                ]
            ]
        },
        "event": {
            "type": "event",
            "name": "BatchPin",
            "inputs": [
                {
                    "name": "author",
                    "type": "address",
                    "internalType": "address"
                },
                {
                    "name": "timestamp",
                    "type": "uint256",
                    "internalType": "uint256"
                },
                {
                    "name": "namespace",
                    "type": "string",
                    "internalType": "string"
                },
                {
                    "name": "uuids",
                    "type": "bytes32",
                    "internalType": "bytes32"
                },
                {
                    "name": "batchHash",
                    "type": "bytes32",
                    "internalType": "bytes32"
                },
                {
                    "name": "payloadRef",
                    "type": "string",
                    "internalType": "string"
                },
                {
                    "name": "contexts",
                    "type": "bytes32[]",
                    "internalType": "bytes32[]"
                }
            ],
            "outputs": null
        },
        "fromBlock": "latest",
        "synchronized": true
    }
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 17:55:12 +0000 UTC
    </div>
</div>

