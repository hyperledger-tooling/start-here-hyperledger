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
                PR <a href="https://github.com/hyperledger/firefly-fabconnect/pull/81" class=".btn">#81</a>
            </td>
            <td>
                <b>
                    Fill in event fields from transactions that do not publish events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If a transaction does not publish an event, the event object published by the event stream has mostly empty fields:

```
{
    "chaincodeId": "",
    "blockNumber": 12,
    "transactionId": "",
    "transactionIndex": 0,
    "eventIndex": 0,
    "eventName": "",
    "payload": "",
    "timestamp": 1645073064291071927,
    "subId": "sb-f2d3ed2e-2f34-4b79-7763-87755a3f8391"
  }
```

The fields `chaincodeId` and `transactionId` should be filled in from the transaction object that contained the event.

After the fix, the fields are filled in:

```
{
    "chaincodeId": "_lifecycle",
    "blockNumber": 12,
    "transactionId": "052935d3e4debb3e67b40249153ec006f2d419b058df7f604b9b3311796b8934",
    "transactionIndex": 0,
    "eventIndex": 0,
    "eventName": "",
    "payload": "",
    "timestamp": 1645073064291071927,
    "subId": "sb-f2d3ed2e-2f34-4b79-7763-87755a3f8391"
  }
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-03 19:33:02 +0000 UTC
    </div>
</div>

