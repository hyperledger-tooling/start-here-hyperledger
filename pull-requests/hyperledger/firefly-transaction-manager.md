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
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/41" class=".btn">#41</a>
            </td>
            <td>
                <b>
                    Allow prometheus metrics to be enabled in FFTM
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The initial commit adds a single metric, ff_transaction_submission_error_total, that allows the user to track the number of errors from transaction submissions.

Signed-off-by: Matthew Whitehead <matthew.whitehead@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-18 13:53:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/40" class=".btn">#40</a>
            </td>
            <td>
                <b>
                    adding a flag to support pre signed transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding a boolean flag in the Managed Transaction to indicate whether the transaction is pre-signed. Therefore, the connector can use that flag to call `sendRawTransaction` .
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-17 16:39:19 +0000 UTC
    </div>
</div>

