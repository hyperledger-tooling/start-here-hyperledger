---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1101" class=".btn">#1101</a>
            </td>
            <td>
                <b>
                    [ui-version-1.1.2]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Echelberger <eberger727@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-09 18:13:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1099" class=".btn">#1099</a>
            </td>
            <td>
                <b>
                    Add enhancements to Depoy Contract API
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
        Created At 2022-11-08 16:42:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1098" class=".btn">#1098</a>
            </td>
            <td>
                <b>
                    Add forward compatibility with Go 1.19
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-08 16:35:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1096" class=".btn">#1096</a>
            </td>
            <td>
                <b>
                    Idempotent apis
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This feature allows API requests to FireFly Core to be made idempotent.

That is that the caller of the API can specify its own unique identifier (an arbitrary string up to 256 characters) that uniquely identifies the request. So if there is a network connectivity failure, or an abrupt termination of either runtime, the application can safely attempt to resubmit the REST API call and be returned a `409 Conflict` HTTP code.

Examples of how an app might construct such an idempotencyKey include:
- Unique business identifiers from the request that comes into its API up-stream - passing idempotency along the chain
- A hash of the business unique data that relates to the request - maybe all the input data of a blockchain transaction for example, if that payload is guaranteed to be unique.
    > Be careful of cases where the business data might _not_ be unique - like a transfer of 10 coins from A to B... that
    > could happen multiple times, and each would be a separate business transaction. Where as transfer with invoice
    > number abcd1234 of 10 coins from A to B might be perfectly unique.
- A unique identifier of a business transaction generated within the application and stored in its database before submission
    > Here be careful you haven't just moved the problem up one layer. How does that unique ID get generated? Is that
    > itself idempotent?

FireFly already uses an idempotent interface downstream to key plugins:
   - EVMConnect blockchain operations - fully idempotent, using the operation ID
   - Token operations - inherit idempotence from the blockchain connector they communicate with

> Note that the interface between FireFly and EthConnect for blockchain operations is not currently fully idempotent.
> This PR does not make the changes needed for that, and I note that EVMConnect is the recommended choice for
> new FireFly projects.

### Tasks

- [x] Add `idempotencyKey` field to messages
   - Persisted directly on `Message` object
   - Local only - not propagated in `persistBatch` when received remotely
   - Note complexity was in the batching logic, as it's important if the message writer batching has one out of a set of messages that fails the idempotency check, it doesn't fail the whole batch of message/data inserts. To do this without reducing performance for the good case took a bit of extra work
- [x] Add `idempotencyKey` to `invoke` of blockchain smart contracts
    - Persisted on `Transaction` object
- [x] Add `idempotencyKey` to `deploy` of blockchain smart contracts
    - Persisted on `Transaction` object
- [x] Add `idempotencyKey` to `transfer` (/`mint`/`burn`/`approval`) of tokens
    - Persisted on `Transaction` object
- [x] Add `idempotencyKey` to `publish` APIs
- [x] Update e2e tests for Message to test idempotent submission
- [x] Update e2e tests for Tokens to test idempotent submission
- [x] Update e2e tests for Custom contracts to test idempotent submission

> I did look at in this PR, whether I could pass the `idempotencyKey` back to applications on events if they submitted
> them on a request. However, this proved to need more investigation because the `.transaction` field of events is
> only enriched on `transaction_submitted` events. To switch it to be cache-back-queried on every event, and to bloat
> the JSON with the full transaction for all events, felt like a change that needed discussion independent from adding
> the `idempotencyKey` capability to the submission APIs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-08 04:40:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1095" class=".btn">#1095</a>
            </td>
            <td>
                <b>
                    Add endpoint for deploying contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-07 22:14:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1094" class=".btn">#1094</a>
            </td>
            <td>
                <b>
                    Update to go 1.18 and other deps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Pulls in https://github.com/hyperledger/firefly-common/releases/tag/v1.1.4
- Updates all builds and go.mod to 1.18
- Updates docker builds to 1.18
- Also updates other dependencies, and tweaks for those (such as SQLite test case, and re-running Swagger gen)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-07 18:53:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1092" class=".btn">#1092</a>
            </td>
            <td>
                <b>
                    Create new guide for Fabric test-network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a new tutorial for using the FireFly CLI with the Fabric test-network from the fabric-samples repo. CLI changes in https://github.com/hyperledger/firefly-cli/pull/225 are a prerequisite for this tutorial.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-03 14:37:37 +0000 UTC
    </div>
</div>

