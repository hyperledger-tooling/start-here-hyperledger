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
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/109" class=".btn">#109</a>
            </td>
            <td>
                <b>
                    Fix propagation of `blockNumber` to EVMConnect (and batch logging tweak)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - We weren't passing `blockNumber` down
- We were assuming on the internal struct it had to be a number, where FFTM should not be opinionated
   - Noting that for EVM it can be `"latest"`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 20:30:30 +0000 UTC
    </div>
</div>

