---
layout: default
title: firefly-transaction-manager
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-transaction-manager
---

# firefly-transaction-manager <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-transaction-manager){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/104" class=".btn">#104</a>
            </td>
            <td>
                <b>
                    Require policy engines to map failures during submission to idempotency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See https://github.com/hyperledger/firefly/issues/1435

The implementation here:
- Requires the policy manager implementations to return a new boolean
- Provides a mapping from the `ErrorReason` information that FFCAPI implementations already provide
- Uses a `submissionRejected` boolean on the response back to core (so `false` means it is retryable)
- Updates to latest `firefly-common`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-21 15:20:19 +0000 UTC
    </div>
</div>

