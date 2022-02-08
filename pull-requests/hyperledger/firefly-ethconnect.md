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
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/199" class=".btn">#199</a>
            </td>
            <td>
                <b>
                    Protect misconfiguring catchupModeBlockGap < catchupModePageSize and fix catchup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See #198 for the 🤕 behavior you can get if we don't protect against this.

The logic here has an implicit assumption of this rule, so that when we read a page it's never going to extend past the `blockNumber` of the header of the chain at the point we query.

Otherwise, we think:
- Gap to head 1234 is > 250 - so we're in catchup
- Read 5000 (page size) - cool we've read 5000 blocks ... but actually there were only 1234 to read!!!
- ok, now we're not in catchup any more - start reading from where we left off - but that's now skipped a whole bunch of blocks.

https://github.com/hyperledger/firefly-ethconnect/blob/f6c7fe5499d111a25d2301b84efdb8a13db988e2/internal/events/subscription.go#L223-L248
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-04 04:29:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/197" class=".btn">#197</a>
            </td>
            <td>
                <b>
                    Request to be added as a code owner
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Having made significant contributions to this repository, I'd like to formally request being added as a code owner.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-02 01:42:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/196" class=".btn">#196</a>
            </td>
            <td>
                <b>
                    Allow passing an array of ABI methods that might emit an event, when creating a sub
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Two features in this PR related to the `inputs: true` feature on event streams:

### 1. Include `inputSigner` in the response

Return the ethereum address of the `from` that comes back in the `eth_getTransactionByHash` when we're doing the input decoding. This is needed by the FireFly tokens connectors, and currently they have to make an inefficient extra call.

### 2. Add a list of method ABI signatures when subscribing, to avoid need for ABI to be registered

When you are creating a subscription directly, on `POST` `/subscriptions` with an inline Event definition you might still want the inputs to be resolved (the stream has `inputs: true` set).

However, there's no tie between the subscription and an an ABI in the contract registry in this case, so we need a way for you to manually specify an array of all the possible methods that might emit the event you're interested in. Otherwise, there's no way for EthConnect to match the method signature extracted from the transaction, back to a particular method ABI, in order to know how to RLP decode the input data.

This PR propose very simple extension to #177, allowing you to post the payload example below.

`POST` `/subscriptions`
```js
{
  "name": "mysub",
  "stream": "df02bbdd-7038-462e-934d-9b5c7493fcbb",
  "fromBlock": "latest",
  "address": "0x10393D362bEfa1fe52e613801D72Da358C0d76c0",
  "event": {
    "name": "stuffHappened",
    "type": "event",
    "anonymous": false,
    "inputs": [
      {
        "indexed": true,
        "name": "from",
        "type": "address"
      },
      {
        "indexed": true,
        "name": "val1",
        "type": "int64"
      }
    ]
  },
  "methods": [
    {
      "type": "function",
      "name": "doStuff",
      "constant": false,
      "inputs": [
        {
          "name": "val1",
          "type": "int64"
        }
      ],
      "outputs": [],
      "payable": false,
      "stateMutability": "nonpayable"
    }
  ]
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-01 22:51:04 +0000 UTC
    </div>
</div>

