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
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/184" class=".btn">#184</a>
            </td>
            <td>
                <b>
                    Fix post-merge build issue related to error codes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See failure here https://github.com/hyperledger/firefly-ethconnect/runs/4301810830?check_suite_focus=true

Combination of #178 post-merge with #177

```
# github.com/hyperledger/firefly-ethconnect/internal/contractgateway
internal/contractgateway/smartcontractgw.go:529:31: undefined: "github.com/hyperledger/firefly-ethconnect/internal/errors".New
make: *** [Makefile:43: deps] Error 2
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 16:56:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/183" class=".btn">#183</a>
            </td>
            <td>
                <b>
                    Do not close a.eventStream, rather handle closed batch dispatcher
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix for https://github.com/hyperledger/firefly-ethconnect/issues/182
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 05:44:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/181" class=".btn">#181</a>
            </td>
            <td>
                <b>
                    Reduce default fetch below 1MB in the case of a small circuit breaker upper bound
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                After considering  in https://github.com/hyperledger/firefly-ethconnect/pull/175#pullrequestreview-813026469a bit of detail, I came to the conclusion this is a step forwards. Given that:
- Sarama only allows querying the HWM that has most recently been obtained via a fetch
- Configuring the producer to actually consume every message, in order to continually fetch, would be very inefficient 

This isn't perfect, as it still requires the consumer to be actively consuming for the circuit breaker to function.
However, in practice I believe it will protect from overflowing the buffer in the common case as even if the chain were stalled, batches of messages will be being consumed and returned with a timeout error periodically.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 02:31:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/180" class=".btn">#180</a>
            </td>
            <td>
                <b>
                    Fix for intermittent failure #179
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix for #179 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 01:17:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/178" class=".btn">#178</a>
            </td>
            <td>
                <b>
                    Add error codes to all ethconnect errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Allocate unique integers to every error
- Include in the errors when printed in the logs
- Wherever possible retain the code-free error in the return on REST `"error": "message goes here"` JSON responses
- Add a separate `"code": "FFEC100049"` on all rest responses
- Add a separate `"errorCode": "FFEC100049"` on replies in the receipt store
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-22 22:07:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/177" class=".btn">#177</a>
            </td>
            <td>
                <b>
                    POST to /subscriptions with in-line event definition
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                FireFly will be handling the storage and management of ABI event types, so we need a base route to `POST` `/subscriptions` that allows the event definition, address etc. to be supplied in-line.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-22 18:24:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/175" class=".btn">#175</a>
            </td>
            <td>
                <b>
                    Add circuit breaker to stop runaway producers losing messages, and immediate receipt option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implementations for:
- [x] #173 
- [x] #176

## Kafka Circuit Breaker

When enabled, the difference between the `offset` of the consumer and the current Kafka `HighWaterMark` of each partition being consumed within the runtime is monitored by a new runtime component

A running average of the size of the consumed messages is kept, to allow an estimation of the byte size of the gap between the offset and high water mark. This is needed as Kafka will roll the buffer based on the size (not the count) of messages, so we need to estimate that.

On startup a log is output showing the configuration.

```
[2021-11-22T04:02:56.465Z]  INFO CircuitBreakerEnabled: trip=6144.00Kb reset=4915.20Kb
```

Under normal consumption, new log entries are logged at most every X seconds (30 by default):

```
[2021-11-22T03:49:36.747Z]  INFO CircuitBreakerHealth: topic=zzzixar21f-zzlcxv8ksq-requests partition=0 offset=45233 hwm=45234 gap=1 gap.estimate=5.73Kb tripped=false lastTripped=never
```

In the case that the circuit breaker trips a log is output as follows - note that it shows the gap in messages, as well as the estimated size of the buffer represented by that gap. The switch trips when this meets an upper threshold.

```
[2021-11-22T01:08:24.551Z]  INFO CircuitBreakerTripped: topic=zzzixar21f-zzlcxv8ksq-requests partition=0 offset=3730 hwm=22513 gap=18783 gap.estimate=8492.70Kb tripped=true lastTripped=2021-11-22T01:08:24.551313415Z
```

When the circuit breaker un-trips (resets), the log output is as follows. This occurs when the gap estimate drops below a fraction of the upper bound - `0.8` (80%) by default:
```
[2021-11-22T01:09:45.179Z]  INFO CircuitBreakerReset: topic=zzzixar21f-zzlcxv8ksq-requests partition=0 offset=11619 hwm=22513 gap=10894 gap.estimate=4915.07Kb tripped=false lastTripped=2021-11-22T01:08:24.551313415Z
```

While tripped, any REST API requests attempting to send messages will receive a `500` error with the following body:

```json
{"error":"Unable to send Kafka message as the gap of 29507 messages between consumer and producer is too large. Estimated at 13312.73Kb"}
```

## Immediate Receipts

A new query parameter on REST API Gateway invocations of contract methods is provided `fly-acktype=receipts` (or `kld-acktype` in Kaleido environments with a custom prefix).

For raw webhooks, this can be supplied as an `ackmode: "receipts"` body parameter.

When specified in async requests, it will be immediately possible to query a receipt object on `/replies/:id`.

- `pending` will be set to `true` (not present in the final receipt once it replaces this entry)
- `msgAck` will be a string containing the Kafka message details
- `headers.type` will be the type of request `SendTransaction` or `DeployContract`
- The rest of the message that has been dispatched to Kafka will be included, with all inputs etc.

Example:

```json
{
  "_id": "97fd6f37-11e9-45d5-4355-4abc77279fef",
  "from": "0x4d1c5d7c4696afd597b2906564ea3aa9e0c382a6",
  "gas": 0,
  "gasPrice": 0,
  "headers": {
    "id": "97fd6f37-11e9-45d5-4355-4abc77279fef",
    "type": "SendTransaction"
  },
  "method": {
    "inputs": [
      {
        "internalType": "int64",
        "name": "someNumber",
        "type": "int64"
      },
      {
        "internalType": "string",
        "name": "someMessage",
        "type": "string"
      }
    ],
    "name": "set",
    "outputs": [],
    "stateMutability": "nonpayable",
    "type": "function"
  },
  "msgAck": "zzzixar21f-zzlcxv8ksq-requests:0:45233",
  "params": [
    "12345",
    "test"
  ],
  "pending": true,
  "receivedAt": 1637552976745,
  "to": "0xbb99253e723891b73b9c18bcc818678f3e29c009",
  "value": 0
}
```

Once the transaction is sent to the blockchain and succeeds/fails, this is replaced with the usual receipt - which is unchanged:

```json
{
  "_id": "97fd6f37-11e9-45d5-4355-4abc77279fef",
  "blockHash": "0x9df474173e82d41ddf03f7db4c2a605a944e0d30b38a326af4588eef0c1806da",
  "blockNumber": "3566",
  "cumulativeGasUsed": "39428",
  "from": "0x4d1c5d7c4696afd597b2906564ea3aa9e0c382a6",
  "gasUsed": "39428",
  "headers": {
    "id": "1faa4e96-4d2c-4ada-58a6-1eb9a51cc379",
    "requestABIId": "",
    "requestId": "97fd6f37-11e9-45d5-4355-4abc77279fef",
    "requestOffset": "zzzixar21f-zzlcxv8ksq-requests:0:45233",
    "timeElapsed": 5.369752082,
    "timeReceived": "2021-11-22T03:49:36.747344301Z",
    "type": "TransactionSuccess"
  },
  "nonce": "45284",
  "receivedAt": 1637552982120,
  "status": "1",
  "to": "0xbb99253e723891b73b9c18bcc818678f3e29c009",
  "transactionHash": "0x110cbf40c547fe5575c4b834115e89437dd335a98536bf869bce726005ae70ef",
  "transactionIndex": "0"
}
```

## Sample App

In case it's useful, here is a simple sample app for streaming messages in at a high pace into a runtime:

```js
const axios = require('axios');
const https = require('https');

const BASE_URL = 'https://xyz.example.com/';
const USERNAME = 'xxxxxx';
const PASSWORD = 'xxxxxx;
const INSTANCE_ADDRESS = '0xbb99253e723891b73b9c18bcc818678f3e29c009';
const FROM_ADDRESS = '0x4d1c5d7c4696afd597b2906564ea3aa9e0c382a6';

const MAX_SOCKETS = 50;
const MAX_PROMISES = 200;
const TOTAL_MESSAGES = 10000;

const client = axios.create({
  httpsAgent: new https.Agent({
    maxSockets: MAX_SOCKETS,
  }),
  auth: {
    username: USERNAME,
    password: PASSWORD,
  },
  baseURL: BASE_URL
});

async function run() {

  let i = 0;
  const inflight = {};
  while (i < TOTAL_MESSAGES) {
    if (Object.keys(inflight).length < MAX_PROMISES) {
      const reqNo = ++i;
      inflight[`${reqNo}`] = (client.request({
        url: `instances/${INSTANCE_ADDRESS}/set`,
        method: 'POST',
        data: {
          "someMessage": `Test ${reqNo}`,
          "someNumber": reqNo,
        },
        params: {
          'kld-from': FROM_ADDRESS,
          'kld-sync': 'false',
          'kld-acktype': 'receipt',
        }
      })
        .then(({status})  => console.log(`PASS - ${reqNo} [${status}]`))
        .catch(err => console.log(`FAIL - ${reqNo} [${err.response && err.response.status}]: ${(err.response && err.response.data && JSON.stringify(err.response.data)) || err.message}`))
        .then(() => reqNo)
      );
    } else {
      const reqNo = await Promise.any(Object.values(inflight))
      delete inflight[reqNo]
    }
  }

}

run().catch(err => {
  console.error(err.stack);
  process.exit(1);
});
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-21 16:47:03 +0000 UTC
    </div>
</div>

