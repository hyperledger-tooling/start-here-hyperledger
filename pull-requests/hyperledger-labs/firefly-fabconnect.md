---
layout: default
title: firefly-fabconnect
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-fabconnect
---

# firefly-fabconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-fabconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-fabconnect/pull/23" class=".btn">#23</a>
            </td>
            <td>
                <b>
                    README.md and .gitignore small improvement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                README.md - Added Makefile tag with a list of initial commands
.gitignore - OS specific, Goland .idea folder
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-29 21:17:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-fabconnect/pull/20" class=".btn">#20</a>
            </td>
            <td>
                <b>
                    Tx submit and event receipt tracking
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For async requests, added more complete support for submitting Fabric transactions and tracking the transaction status event, and saving the result in the receipt store.

Example request:
```
curl -H "Content-Type: application/json" -d '{"headers":{"type":"SendTransaction","channel":"default-channel","signer":"user2"},"chaincode":"asset_transfer","func":"CreateAsset","args":["asset1014","yellow","10","Tom","1300"]}' http://localhost:3000/transactions?fly-sync=true | jq

{
  "sent": true,
  "id": "008185fd-5a28-4e1a-4526-d8f9d8f5cc18"
}
```

```
$ curl http://localhost:3000/receipts/41c0c0a4-46a8-4c46-7289-90705ea70436 |jq
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   347  100   347    0     0   338k      0 --:--:-- --:--:-- --:--:--  338k
{
  "_id": "41c0c0a4-46a8-4c46-7289-90705ea70436",
  "headers": {
    "id": "218310d6-b915-4e52-4cd0-fc147265c49a",
    "requestId": "41c0c0a4-46a8-4c46-7289-90705ea70436",
    "requestOffset": "",
    "timeElapsed": 1.056184,
    "timeReceived": "2021-07-27T18:53:11.317501Z",
    "type": "TransactionSuccess"
  },
  "receivedAt": 1627411992373
}
```

For sync requests, the end to end transaction processing also works now.

```
$ curl -H "Content-Type: application/json" -d '{"headers":{"type":"SendTransaction","channel":"default-channel","signer":"user2"},"chaincode":"asset_transfer","func":"CreateAsset","args":["asset1014","yellow","10","Tom","1300"]}' http://localhost:3000/transactions?fly-sync=true | jq

{
  "headers": {
    "id": "1572b6aa-75a8-4c7c-6f6a-6f1b911c38aa",
    "type": "TransactionSuccess",
    "timeReceived": "2021-07-27T19:42:02.957407Z",
    "timeElapsed": 1.05154,
    "requestOffset": "",
    "requestId": ""
  }
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-27 21:15:42 +0000 UTC
    </div>
</div>

