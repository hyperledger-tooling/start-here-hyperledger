---
layout: default
title: firefly-fabconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-fabconnect
---

# firefly-fabconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-fabconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-fabconnect/pull/51" class=".btn">#51</a>
            </td>
            <td>
                <b>
                    Added workflow to build and publish docker image
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
        Created At 2021-09-27 18:03:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-fabconnect/pull/50" class=".btn">#50</a>
            </td>
            <td>
                <b>
                    Added data type support to tx input and event subscription
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Transaction Input
payload schema can be specified in the `headers` section of the request body. Complex types are supported for chaincodes that takes structs as input:
```
{
    "headers": {
        "type": "SendTransaction",
        "payloadSchema": {
            "type": "array",
            "prefixItems": [{
                "name": "id", "type": "string"
            }, {
                "name": "color", "type": "string"
            }, {
                "name": "size", "type": "string"
            }, {
                "name": "owner", "type": "string"
            }, {
                "name": "appraisal", "type": "object",
                "properties": {
                    "appraisedValue": {
                        "type": "integer"
                    },
                    "inspected": {
                        "type": "boolean"
                    }
                }
            }]
        }
    },
    "func": "CreateAsset",
    "args": {
        "owner": "Tom",
        "appraisal": {
            "appraisedValue": 123000,
            "inspected": true
        },
        "size": "10",
        "id": "asset205",
        "color": "red"
    }
}
```
## Event Payload
Previously, the event payload is always send to the listening client as the byte array originally obtained from Fabric's event object:

```
{
    "chaincodeId": "asset_transfer",
    "blockNumber": 126,
    "transactionId": "ff1c69f8e891a6aa43378ecd2a914f4a0ea3f3cfb23247ecc298a2e66a5c5970",
    "eventName": "AssetCreated",
    "payload": "eyJJRCI6ImFzc2V0MTA2OSIsImNvbG9yIjoieWVsbG93Iiwic2l6ZSI6MTAsIm93bmVyIjoiVG9tIiwiYXBwcmFpc2VkVmFsdWUiOjEzMDB9",
    "subId": "sb-6366481d-1495-4a89-6e57-b9403d781208"
  }
```

With the enhancement, a `payloadType` property can be specified during event subscription, that can provide one of 3 types to instruct the event processor in fabconnect to unmarshal the byte array before sending to the client:
- `string`: the byte array will be encoded as UTF-8 strings,
```
{
    "chaincodeId": "asset_transfer",
    "blockNumber": 131,
    "transactionId": "c38dc609f86298e2ef407cc645aeec134fb08cbe283565501bb8b38103fcaee0",
    "eventName": "AssetCreated",
    "payload": "{\"ID\":\"asset1074\",\"color\":\"yellow\",\"size\":10,\"owner\":\"Tom\",\"appraisedValue\":1300}",
    "subId": "sb-ad7adeb7-5f40-4157-51b9-5caa35a1fd4d"
  }
```
- `stringifiedJSON`: the byte array will be encoded as fully expanded string maps,
```
{
    "chaincodeId": "asset_transfer",
    "blockNumber": 130,
    "transactionId": "83be13b68874253655eefde7cb992b4b53bea7b919eed742f91a08b802aadd98",
    "eventName": "AssetCreated",
    "payload": {
      "ID": "asset1073",
      "appraisedValue": 1300,
      "color": "yellow",
      "owner": "Tom",
      "size": 10
    },
    "subId": "sb-bb06eaaf-cc71-422b-581a-b3ded393d63d"
  }
```
- `bytes`: which is the default, the byte array is left alone without any further treatment

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-24 14:23:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-fabconnect/pull/49" class=".btn">#49</a>
            </td>
            <td>
                <b>
                    Remove references to labs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-23 20:27:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-fabconnect/pull/47" class=".btn">#47</a>
            </td>
            <td>
                <b>
                    Gateway client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added support to use the gateway implementation in the SDK (client-side gateway) that works with a Fabric peer that has the discovery service turned on, in order to minimize the required information inside the connection profile.

This works when `useGatewayClient: true` is configured. If not set or set to `false`, then the original support of solely relying on the connection profile is used.

Another bool configuration parameter `useGatewayServer` is added but is ineffective right now. It's for the Fabric 2.4 support for server-side gateway which makes the target peer a "submitting peer", in order to minimize the burden of the client SDKs in coordinating the peers selection and transaction proposals submission. Support for it will be added in a future PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-21 19:38:46 +0000 UTC
    </div>
</div>

