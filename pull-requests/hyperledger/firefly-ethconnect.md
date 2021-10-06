---
layout: default
title: firefly-ethconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-ethconnect
---

# firefly-ethconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-ethconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/157" class=".btn">#157</a>
            </td>
            <td>
                <b>
                    ES Subscriptions: Store checkpoint after a stale subscription is processed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * We update the checkpoint block for a subscription when it's stale. However, we also need to store the checkpoint after since any restart must pick up from that point on.
* Set initial block height for stream when non-zero. Noticed we were not storing the "starting" block height when a custom value is configured when creating a stream
* Update deps

Fixes: https://github.com/hyperledger/firefly-ethconnect/issues/156
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-06 17:57:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/155" class=".btn">#155</a>
            </td>
            <td>
                <b>
                    Add extra nil checks and logging surrounding contract caching
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
        Created At 2021-10-01 16:39:02 +0000 UTC
    </div>
</div>

