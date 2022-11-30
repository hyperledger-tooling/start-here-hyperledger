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
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/43" class=".btn">#43</a>
            </td>
            <td>
                <b>
                    Update FF every time there is an error, or interesting change in state
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Note this is an interim change, and we should fully implement https://github.com/hyperledger/firefly/issues/1108 such that only a transition of the _state_ to `Error` would result in a WebSocket update (not simply us writing an error to our local state from a single execution of the polling loop).

This PR:
1. Fixes the problem that we didn't propagate error updates at all
2. Introduces a more complete history list, that includes when we submitted the transaction, when we got a receipt etc.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-27 19:03:17 +0000 UTC
    </div>
</div>

