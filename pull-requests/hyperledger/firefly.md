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
                PR <a href="https://github.com/hyperledger/firefly/pull/1418" class=".btn">#1418</a>
            </td>
            <td>
                <b>
                    Enable contract listeners with multiple filters
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">migration_consideration</span>
            </td>
            <td>
                This PR adds the ability to listen to multiple types of events on the same contract listener, by adding an array of listeners, rather than a single event signature/location per listener. The old way of creating a listener is still accepted by the API, but it will always be returned in the filters array now. **This is a migration concern that needs to be documented.**

## Open questions
One thing I'm not sure about here, is that this PR as-is removes the uniqueness constraint on listeners by topic/location/signature. It now allows multiples. I'm not sure if this is a problem or not. I can add that constraint back, but it would likely require some more sophisticated DB changes. Which brings me to the next point...

Right now all the filters for a contract listener get serialized to JSON and stored in a single column. I lated realized this means we lose the ability to query/filter (no pun intended) by signature, location, etc. which we used to do, in order to check for duplicates. I'm not sure if this is required or not, but wanted to call it out.

## Example

### Create contract listener request
```json
{
    "filters": [
        {
            "interface": {
                "id": "aaa0e410-2b5b-4815-a80a-a18f2ae59f7d"
            },
            "eventPath": "BatchPin",
            "location": {
                "address": "0xb0cd60ade460e797e0c9d206290ac4ed45672c60"
            }
        }
    ],
    "name": "CustomBatchPin",
    "options": {
        "firstEvent": "oldest"
    },
    "topic": "batch-pin"
}
```

### Create contract listener response
```json
{
    "id": "acc0d227-1da4-4d0d-bbe0-0c60f754158f",
    "namespace": "default",
    "name": "CustomBatchPin",
    "backendId": "018b258a-0c2c-07c0-5d59-50583ae91f1e",
    "created": "2023-10-12T20:18:06.012167Z",
    "filters": [
        {
            "event": {
                "name": "BatchPin",
                "description": "",
                "params": [
                    {
                        "name": "author",
                        "schema": {
                            "type": "string",
                            "details": {
                                "type": "address",
                                "internalType": "address"
                            },
                            "description": "A hex encoded set of bytes, with an optional '0x' prefix"
                        }
                    },
                    {
                        "name": "timestamp",
                        "schema": {
                            "oneOf": [
                                {
                                    "type": "string"
                                },
                                {
                                    "type": "integer"
                                }
                            ],
                            "details": {
                                "type": "uint256",
                                "internalType": "uint256"
                            },
                            "description": "An integer. You are recommended to use a JSON string. A JSON number can be used for values up to the safe maximum."
                        }
                    },
                    {
                        "name": "action",
                        "schema": {
                            "type": "string",
                            "details": {
                                "type": "string",
                                "internalType": "string"
                            }
                        }
                    },
                    {
                        "name": "uuids",
                        "schema": {
                            "type": "string",
                            "details": {
                                "type": "bytes32",
                                "internalType": "bytes32"
                            },
                            "description": "A hex encoded set of bytes, with an optional '0x' prefix"
                        }
                    },
                    {
                        "name": "batchHash",
                        "schema": {
                            "type": "string",
                            "details": {
                                "type": "bytes32",
                                "internalType": "bytes32"
                            },
                            "description": "A hex encoded set of bytes, with an optional '0x' prefix"
                        }
                    },
                    {
                        "name": "payloadRef",
                        "schema": {
                            "type": "string",
                            "details": {
                                "type": "string",
                                "internalType": "string"
                            }
                        }
                    },
                    {
                        "name": "contexts",
                        "schema": {
                            "type": "array",
                            "details": {
                                "type": "bytes32[]",
                                "internalType": "bytes32[]"
                            },
                            "items": {
                                "type": "string",
                                "description": "A hex encoded set of bytes, with an optional '0x' prefix"
                            }
                        }
                    }
                ]
            },
            "location": {
                "address": "0xb0cd60ade460e797e0c9d206290ac4ed45672c60"
            },
            "interface": {
                "id": "aaa0e410-2b5b-4815-a80a-a18f2ae59f7d"
            },
            "signature": "BatchPin(address,uint256,string,bytes32,bytes32,string,bytes32[])"
        }
    ],
    "topic": "batch-pin",
    "options": {
        "firstEvent": "oldest"
    }
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-12 20:56:15 +0000 UTC
    </div>
</div>

