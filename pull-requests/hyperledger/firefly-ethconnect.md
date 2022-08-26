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
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/227" class=".btn">#227</a>
            </td>
            <td>
                <b>
                    Add additional idempotence check to cover Kafka server restart, while EthConnect stays running
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                EthConnect works on an "at target" nonce allocation (see comparision with "at source" in
[readme of FFTM](https://github.com/hyperledger/firefly-transaction-manager/blob/main/README.md#nonce-management)), meaning it gives an "at least once" delivery assurance to the blockchain, backed by Apache Kafka.

In the case that the REST API Gateway is tuned for high performance, with an in-flight count in the many hundreds, and the Kafka servers are restarted, the consumer groups might redeliver many messages. This is undesirable.

EthConnect already has the concept of an idempotency key, on the front-side of the REST API Gateway, using `ackmode` as added in #175 to get an immediate receipt, combined with supplying your own custom ID. However, that is only checked in the REST API Gateway boundary layer today.

See the following diagram as a reference, showing how a Kafka at-least-once redelivery results in this duplication:
![EthConnect at-least-once issue (1)](https://user-images.githubusercontent.com/6660217/186766456-c229e16c-a22b-4846-9e81-9af879e5eda1.jpg)

This PR proposes adding an additional idempotency check, at the point we receive the message from Kafka. Note this does not change the fundamental nature of the "at target" architecture from being at-least-once, and in some failure scenarios (for full idempotent delivery e2e with Ethereum nonces you would need the "at source" ordering architecture of https://github.com/hyperledger/firefly-evmconnect based on the new FFTM architecture).

But this PR does protect against something like a planned HA rolling restart of a Kafka cluster, from causing redelivery.

![ethconnect_kafka_idempotency_enhancement](https://user-images.githubusercontent.com/6660217/186765590-2d643579-efa8-43fe-b64d-2a80808e17b1.jpg)

The new check is only enabled when:
- `fly-ackmode=receipt` has been specified in the transaction submission via the APIs described in #175 
- The REST API Gateway and the Kafka<->Ethereum module are co-located in the same address space

The check covers two scenarios:
1. The transaction is already in-flight in TX Processor when the redelivery occurs
2. The transaction has already been assigned a transaction hash when the redelivery occurs

> One complexity in the change, was making it so the two different components could both access the receipt store. For that I moved out a new package called `receipts`.
 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 20:50:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/226" class=".btn">#226</a>
            </td>
            <td>
                <b>
                    Fix potential deadlock broadcasting to a closed WS connection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Port of https://github.com/hyperledger/firefly-transaction-manager/pull/28 to EthConnect codebase, which shares this WS socket management code.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 12:13:49 +0000 UTC
    </div>
</div>

