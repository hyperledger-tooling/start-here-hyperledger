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
                In PR chain with #1094 

- [x] Add `idempotencyKey` field to messages
   - Persisted directly on `Message` object
   - Local only - not propagated in `persistBatch` when received remotely
   - Note complexity was in the batching logic, as it's important if the message writer batching has one out of a set of messages that fails the idempotency check, it doesn't fail the whole batch of message/data inserts. To do this without reducing performance for the good case took a bit of extra work
- [x] Add `idempotencyKey` to `invoke` of blockchain smart contracts
    - Persisted on `Transaction` object
- [x] Add `idempotencyKey` to `deploy` of blockchain smart contracts
    - Persisted on `Transaction` object
- [x] Add `idempotencyKey` to `transfer` (/`mint`/`burn`) of tokens
    - Persisted on `Transaction` object
- [x] Add `idempotencyKey` to `publish` APIs
- [x] Update e2e tests for Message to test idempotent submission
- [ ] Update e2e tests for Tokens to test idempotent submission
- [ ] Update e2e tests for Custom contracts to test idempotent submission
- [ ] Add `idempotencyKey` to events deliveries
    - Where either the transaction or referenced-message has one set
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

