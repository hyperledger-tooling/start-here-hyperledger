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
                PR <a href="https://github.com/hyperledger/firefly-fabconnect/pull/64" class=".btn">#64</a>
            </td>
            <td>
                <b>
                    Chaincode Query and TransactionById support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Chaincode Query
```
POST /query

{
    "headers": {
        "signer": "user4",
        "channel": "default-channel",
        "chaincode": "asset_transfer"
    },
    "func": "GetAllAssets",
    "args": []
}
```

Response:
```
{
    "headers": {
        "id": "9b92d3e5-6bee-433c-63d8-303b09784779",
        "type": "QuerySuccess",
        "timeReceived": "2021-12-19T20:12:45.979664Z",
        "timeElapsed": 0.037289,
        "requestOffset": "",
        "requestId": ""
    },
    "result": [
        {
            "ID": "asset-151713",
            "appraisedValue": 1300,
            "color": "yellow",
            "owner": "Tom",
            "size": 5
        },
        {
            "ID": "asset-583666",
            "appraisedValue": 1300,
            "color": "yellow",
            "owner": "Tom",
            "size": 5
        }
    ]
}
```

## Get Transaction By ID
```
GET /transactions/:id?fly-channel=<channel-id>&fly-signer=<signer>
```

Response:
```
{
    "headers": {
        "id": "785bdd6d-ab76-4b0d-74df-bbeffccbb1e3",
        "type": "QuerySuccess",
        "timeReceived": "2021-12-20T14:10:46.803715Z",
        "timeElapsed": 0.154484,
        "requestOffset": "",
        "requestId": ""
    },
    "result": {
        "transactions": [
            {
                "chaincodeProposal": {
                    "input": {
                        "args": [
                            "CreateAsset",
                            "asset015",
                            "red",
                            "10",
                            "Tom",
                            "123000"
                        ],
                        "isInit": false
                    }
                },
                "payload": {
                    "action": {
                        "proposalResponsePayload": {
                            "extension": {
                                "events": {
                                    "chaincodeId": "asset_transfer",
                                    "eventName": "AssetCreated",
                                    "payload": "{\"ID\":\"asset015\",\"color\":\"red\",\"size\":10,\"owner\":\"Tom\",\"appraisedValue\":123000}",
                                    "txId": "e0ba85200c7539b3726f05a3e278a66e6954f135dbd58182c6511377918a2d47"
                                }
                            },
                            "proposalHash": "Fj5LrScc7gKcODjUsYv4+O8cV7cS42zsfqy2PEuRpbw="
                        }
                    },
                    "chaincodeProposalPayload": {
                        "input": {
                            "chaincodeId": {
                                "name": "asset_transfer"
                            },
                            "input": {
                                "args": [
                                    "CreateAsset",
                                    "asset015",
                                    "red",
                                    "10",
                                    "Tom",
                                    "123000"
                                ],
                                "isInit": false
                            },
                            "type": 0
                        }
                    }
                }
            }
        ],
        "type": "EndorserTransaction"
    }
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-19 20:15:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-fabconnect/pull/63" class=".btn">#63</a>
            </td>
            <td>
                <b>
                    Fix event subscription when since is 0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jim Zhang <jim.zhang@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-18 21:14:58 +0000 UTC
    </div>
</div>

