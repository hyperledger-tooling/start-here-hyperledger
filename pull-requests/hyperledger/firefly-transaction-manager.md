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
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/99" class=".btn">#99</a>
            </td>
            <td>
                <b>
                    Fixing a nonce conflict issue when the cached nonce expired.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There is a problem when two different batches of transaction inserts happen in parallel, one of them will read the incorrect nonce back from the DB + the nonce callback when the cached nonce expires. 

The fix in the PR is to check the expired cached nonce first to avoid pending transactions that have clashing nonces between them.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-02 07:46:31 +0000 UTC
    </div>
</div>

