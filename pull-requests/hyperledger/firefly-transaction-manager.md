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
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/62" class=".btn">#62</a>
            </td>
            <td>
                <b>
                    Pull policy loop into transaction handler
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For https://github.com/hyperledger/firefly-transaction-manager/issues/57

Works done:
1. Created a new class called `TransactionHandler`, this includes the old policy engine + policy loop + nonce management
1. High level e2e test and external configuration file remained unchanged
1. Added EventHandler interface for capturing all of the managed transaction processing events
2. Kept the TransactionHandler interface as simple as possible for easy understanding.  
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-15 15:52:00 +0000 UTC
    </div>
</div>

