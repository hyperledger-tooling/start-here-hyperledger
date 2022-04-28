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
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/5" class=".btn">#5</a>
            </td>
            <td>
                <b>
                    Block based receipt detection in confirmation mgr, and optional change listener
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In PR chain with #4 

- Adds `transactionHashes` to block info on `ffcapi`
- Moves receipt detection to confirmation manager
  - Checks once explicitly when TX added to confirmation manager
  - Then by detecting inclusion in block hashes
- Makes the change listener optional
  - Not needed when FFTM is the only component updating these operations in FF Core (common case)
- Updates the config for clarity for above
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 17:47:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/4" class=".btn">#4</a>
            </td>
            <td>
                <b>
                    Do not expect txHash until send, and keep history of errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - `TransactionHash` can only be known at the `send` phase
- It's really helpful for debug to keep a rolling list of errors from the policy manager in the `Operation`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-22 22:39:58 +0000 UTC
    </div>
</div>

