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

