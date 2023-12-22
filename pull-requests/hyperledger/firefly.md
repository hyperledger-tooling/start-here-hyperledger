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
                PR <a href="https://github.com/hyperledger/firefly/pull/1437" class=".btn">#1437</a>
            </td>
            <td>
                <b>
                    Update tezos stack creation doc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Related to [PR#279](https://github.com/hyperledger/firefly-cli/pull/279)

^^ @denisandreenko 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-22 09:58:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1436" class=".btn">#1436</a>
            </td>
            <td>
                <b>
                    Reflect through submissionRejected JSON body from FFTM/EVMConnect
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                On invoke contract or deploy contract, with `idempotencyKey` set, we were previously leaving operation status as `Initialized` after failing to submit a transaction due to a `revert` during transaction submission.

This PR allows the blockchain connectors to return a `submissionRejected: true` boolean in the JSON response to the submission, to state that the failure is not a temporary infrastructure issue that is retryable in nature, and rather a rejection of the transaction as invalid. In that case, the status will be `Failed`.

FF Core part of https://github.com/hyperledger/firefly/issues/1435

Works with https://github.com/hyperledger/firefly-transaction-manager/pull/104

Depends on the following (new E2E test should fail without these):
- https://github.com/hyperledger/firefly/pull/1436
- https://github.com/hyperledger/firefly-transaction-manager/pull/104
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-21 16:12:05 +0000 UTC
    </div>
</div>

