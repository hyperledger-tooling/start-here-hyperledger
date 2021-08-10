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
                PR <a href="https://github.com/hyperledger-labs/firefly-fabconnect/pull/35" class=".btn">#35</a>
            </td>
            <td>
                <b>
                    Kafka integration test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @jimthematrix Kafka integration test as we discussed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-09 22:44:40 +0000 UTC
    </div>
</div>

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
- event payload unmarshaling (#32)
- event filtering (#33)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-04 02:35:13 +0000 UTC
    </div>
</div>

