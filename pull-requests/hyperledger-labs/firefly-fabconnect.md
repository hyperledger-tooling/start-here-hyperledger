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
                PR <a href="https://github.com/hyperledger-labs/firefly-fabconnect/pull/30" class=".btn">#30</a>
            </td>
            <td>
                <b>
                    Event stream support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Overview
The event stream feature enhances the fabric SDK's event pub/sub in the following ways:
- supports delivery channels that are friendly to microservices architecture and consumptions from a remote client using standard HTTP transports, with websockets (implemented in this PR) and webhooks (started in this PR but incomplete)
- REST endpoints to manage a flexible resource model to subscribe to various events:
  - `EventStream` represents a communication channel b/w the client and the fabconnect server, can be websocket or webhook based
  - `Subscription` represents a specification on events of interest, which are created under an event stream

# Examples
## Create a websocket based event stream
```
POST http://localhost:3000/eventstreams
{
    "name": "stream-1",
    "type": "websocket",
    "websocket": {
        "topic": "test-1"
    }
}
response:
{
    "created": "2021-08-03T11:35:15Z",
    "id": "es-ea547efa-8b64-4b90-76dc-88317afc352b",
    "name": "stream-1",
    "path": "/eventstreams/es-ea547efa-8b64-4b90-76dc-88317afc352b",
    "suspended": false,
    "type": "websocket",
    "batchSize": 1,
    "batchTimeoutMS": 5000,
    "errorHandling": "skip",
    "blockedReryDelaySec": 30,
    "websocket": {
        "topic": "test-1"
    },
    "timestampCacheSize": 1000
}
```

## Create a subscription and assign a Topic
```
POST http://localhost:3000/eventstreams/es-ea547efa-8b64-4b90-76dc-88317afc352b/subscriptions
{
    "channel": "default-channel",
    "name": "sub-1",
    "signer": "signer105",
    "fromBlock": "25"
}
response:
{
    "created": "2021-08-03T11:35:51Z",
    "id": "sb-a9091298-1277-4257-5914-075329317f11",
    "channel": "default-channel",
    "path": "/subscriptions/sb-a9091298-1277-4257-5914-075329317f11",
    "name": "sub-1",
    "stream": "es-ea547efa-8b64-4b90-76dc-88317afc352b",
    "signer": "signer105",
    "fromBlock": "25",
    "filter": {}
}
```

## Connect to the websocket endpoint from the client app
```
$ wscat --connect http://localhost:3000/ws
Connected (press CTRL+C to quit)
> {"type":"listen","topic":"test-1"}
< [{"chaincodeId":"","blockNumber":36,"transactionId":"91a171b81f77c5a8e478d3c39c9752a94a18c0ccb7ef1cad1dc489c9f4023397","eventName":"","payload":null,"subId":"","signature":""}]

> {"type":"ack","topic":"test-1"}
< [{"chaincodeId":"","blockNumber":37,"transactionId":"095c45657e7a884c6ea5a659c8ef87e8e97758ebb10d71bb26e159bc2f95cd64","eventName":"","payload":null,"subId":"","signature":""}]

> {"type":"listen","topic":"test-1"}
> 
```

# Remaining Work
The following work items are still needed to complete the event stream feature:
- webhooks support (#31)
- event payload unmarshaling (#32)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-04 02:35:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-fabconnect/pull/25" class=".btn">#25</a>
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
                Signed-off-by: Jan Rock <jan.rock@me.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-30 21:20:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-fabconnect/pull/24" class=".btn">#24</a>
            </td>
            <td>
                <b>
                    Identity support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Note: not focusing on tests right now so that the FireFly integration can proceed sooner, which is an important exercise to inform the architectural validation to accommodate multiple ledger technologies

## Create (register)
```
$ curl -H "Content-Type: application/json" -d '{"name":"user102","type":"client"}' http://localhost:3000/identities | jq
{
  "name": "user102",
  "secret": "nzzoCYRTxaRj"
}
```

including error handling:
```
$ curl -H "Content-Type: application/json" -d '{"name":"user102","type":"client"}' http://localhost:3000/identities | jq
{
  "error": "failed to register user: failed to register user: Response from server: Error Code: 0 - Registration of 'user102' failed: Identity 'user102' is already registered\n"
}
```

## Enroll
```
$ curl -H "Content-Type: application/json" -d '{"secret":"nzzoCYRTxaRj"}' http://localhost:3000/identities/user102/enroll 
{
  "name": "",
  "success": true
}
```

## List
```
g$ curl http://localhost:3000/identities | jq
[
  {
    "name": "admin",
    "maxEnrollments": -1,
    "type": "client",
    "affiliation": "",
    "caname": ""
  },
  {
    "name": "u0cr3kb8sl",
    "maxEnrollments": 1,
    "type": "orderer",
    "affiliation": "",
    "caname": ""
  },
  {
    "name": "u0cr3kb8sl-admin",
    "maxEnrollments": 1,
    "type": "admin",
    "affiliation": "",
    "caname": ""
  },
```

## Get
```
$ curl http://localhost:3000/identities/user102 | jq
{
  "name": "user102",
  "maxEnrollments": -1,
  "type": "client",
  "affiliation": "",
  "caname": "u0vgwu9s00"
}
```

## Using a newly registered and enrolled signing identity to submit transactions
```
$ curl -H "Content-Type: application/json" -d '{"headers":{"type":"SendTransaction","channel":"default-channel","signer":"user102"},"chaincode":"asset_transfer","func":"CreateAsset","args":["asset1016","yellow","10","Tom","1300"]}' http://localhost:3000/transactions | jq
{
  "sent": true,
  "id": "1621fcad-d42e-4489-7956-2d056901850c"
}

[2021-07-29T18:28:15.316-04:00]  INFO --> POST /transactions
[2021-07-29T18:28:15.316-04:00]  INFO Request handler accepted message. MsgID: 1621fcad-d42e-4489-7956-2d056901850c Type: SendTransaction
[2021-07-29T18:28:15.316-04:00]  INFO In-flight 1000001 added. signer=user102 before=0
[2021-07-29T18:28:15.316-04:00]  INFO <-- POST /transactions [202]:
{"sent":true,"id":"1621fcad-d42e-4489-7956-2d056901850c"}
[2021-07-29T18:28:16.068-04:00]  INFO TX: Sent OK [0.75s]
[2021-07-29T18:28:16.170-04:00]  INFO Obtained receipt after 101.97ms - average time to receipt: 101.97ms
[2021-07-29T18:28:16.170-04:00]  INFO Receipt for f39a3c720c8013b654527258332d05c5ea341e05939e2f42d7516554ee74fb9c obtained after 0.10s Success=true
[2021-07-29T18:28:16.170-04:00]  INFO Received reply message. requestId='1621fcad-d42e-4489-7956-2d056901850c' reqOffset='' type='TransactionSuccess': 
[2021-07-29T18:28:16.171-04:00]  INFO 1621fcad-d42e-4489-7956-2d056901850c: Inserted receipt into receipt store
[2021-07-29T18:28:16.171-04:00]  INFO In-flight 1000001 complete. signer=user102 sub=true before=1 after=0
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-30 13:06:51 +0000 UTC
    </div>
</div>

