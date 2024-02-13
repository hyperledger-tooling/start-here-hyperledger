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
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/108" class=".btn">#108</a>
            </td>
            <td>
                <b>
                    Better logging for transaction writer, and TXUpdate de-dup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Pulls in latest `firefly-common` with fix for https://github.com/hyperledger/firefly-common/pull/125
- Adds operation short id to writer operations to trace them through, and also batch size info
- Merges multiple updates in the same writer batch into a single DB operation
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-13 15:58:30 +0000 UTC
    </div>
</div>

