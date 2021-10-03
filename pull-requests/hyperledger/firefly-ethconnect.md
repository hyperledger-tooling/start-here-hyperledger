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
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/155" class=".btn">#155</a>
            </td>
            <td>
                <b>
                    Add extra nil checks and logging surrounding contract caching
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
        Created At 2021-10-01 16:39:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/154" class=".btn">#154</a>
            </td>
            <td>
                <b>
                    Added support for inline schema of transactions and events payload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This allows ethconnect to be used with contracts that it doesn't have ABIs for, by passing the schema for the transaction payload or event inline.

### Sending Transactions
In the `POST /contracts/:address/:method` requests:
```json
{
    "$schema":  {
      "type": "function",
      "name": "put",
      "stateMutability": "nonpayable",
      "inputs": [
        {
          "name": "x",
          "type": "uint256",
          "internalType": "uint256"
        }
      ],
      "outputs": []
    },
    "x": "12346"
}
```

### Subscribing to Events
In the `POST /contracts/:address/:event/subscribe` requests:
```json
{
    "$schema": {
      "anonymous": false,
      "inputs": [
        {
          "internalType": "uint256",
          "name": "data",
          "type": "uint256"
        }
      ],
      "name": "DataStore",
      "type": "event"
    },
    "stream": "es-9655024d-85cc-4f56-7773-ab6d96fc861e"
}
```

In the above examples, the ethconnect instance does not need to know anything about the contract at `:address` either in the remote registry or in the local ABI store.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 02:25:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/152" class=".btn">#152</a>
            </td>
            <td>
                <b>
                    Updates to avoid timing windows in WebSocket eventstream resulting in blocked streams in edge case reconnect scenario
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We've seen a hard to diagnose pattern of logs, that seem to result in an event stream getting stuck:

```
[2021-09-28T00:55:53.412Z]  INFO WS/d82a5fe8-8356-4ce9-7b3b-c749d0498deb: Connected
[2021-09-28T00:55:53.525Z]  WARN es-45c43457-c322-4883-41ad-d256af5b9325: Is currently blocked. InFlight=808 BatchSize=50
```

```
[2021-09-28T01:07:49.695Z] ERROR WS/d82a5fe8-8356-4ce9-7b3b-c749d0498deb: Error: websocket: close 1006 (abnormal closure): unexpected EOF
[2021-09-28T01:07:49.695Z]  INFO WS/d82a5fe8-8356-4ce9-7b3b-c749d0498deb: Disconnected
[2021-09-28T01:07:49.695Z]  INFO WS/d82a5fe8-8356-4ce9-7b3b-c749d0498deb: Closing
[2021-09-28T01:07:49.695Z] ERROR es-45c43457-c322-4883-41ad-d256af5b9325: Batch 1 attempt 1 failed. ErrorHandling=block BlockedRetryDelay=30s
[2021-09-28T01:07:49.695Z]  INFO WS/d82a5fe8-8356-4ce9-7b3b-c749d0498deb: Disconnected
[2021-09-28T01:07:50.132Z]  WARN es-45c43457-c322-4883-41ad-d256af5b9325: Is currently blocked. InFlight=808 BatchSize=50
[2021-09-28T01:07:51.133Z]  WARN es-45c43457-c322-4883-41ad-d256af5b9325: Is currently blocked. InFlight=808 BatchSize=50
[2021-09-28T01:07:52.134Z]  WARN es-45c43457-c322-4883-41ad-d256af5b9325: Is currently blocked. InFlight=808 BatchSize=50
[2021-09-28T01:07:53.134Z]  WARN es-45c43457-c322-4883-41ad-d256af5b9325: Is currently blocked. InFlight=808 BatchSize=50
[2021-09-28T01:07:54.134Z]  WARN es-45c43457-c322-4883-41ad-d256af5b9325: Is currently blocked. InFlight=808 BatchSize=50
[2021-09-28T01:07:54.890Z]  INFO WS/e3dbcfa5-1e71-47d6-5719-e2b3b1e880c8: Connected
[2021-09-28T01:07:55.135Z]  WARN es-45c43457-c322-4883-41ad-d256af5b9325: Is currently blocked. InFlight=808 BatchSize=50
```

This PR provides a very speculative change that _might_ fix this.

The `cycleTopic ` code assumes it's safe to close the `t.closingChannel` and then create a new one, at the same time another thread is spinning around a retry loop.
I'm speculating that isn't actually safe, and it's possible the loop comes back round and ends up getting the wrong `t.closingChannel` when it comes back round here in some timing condition:
https://github.com/hyperledger/firefly-ethconnect/blob/8545f1c09d5fc9829508dac9a08d8c57210079eb/internal/events/websockets.go#L47

The result is the _next_ disconnect doesn't actually wake the loop, because it's listening on the wrong `t.closingChannel`.

So this PR does two things:

1. ~Stops closing the channel, instead does a non-blocking push of a `bool` down the channel~
  - See below, removed channel completely
2. Adds extra logging to hopefully see more information, if this problem re-occurs with the speculative fix in place
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 03:16:12 +0000 UTC
    </div>
</div>

