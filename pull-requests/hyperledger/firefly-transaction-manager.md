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
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/102" class=".btn">#102</a>
            </td>
            <td>
                <b>
                    Enhance logging on event dispatch, and resolve edge case panic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Couple of small logging enhancements that would have helped me while investigating a set of logs.

Also addresses a panic with a `nil` `batch` object that I found through adding the Unit Test for my new log, which would happen if we did either of....
- The else to this block (which I've now added a log to):
    https://github.com/hyperledger/firefly-transaction-manager/blob/dcc8484eb3c6f1b6e22d649b74e0f2c29c29c83a/internal/events/eventstream.go#L710
- This `continue`:
    https://github.com/hyperledger/firefly-transaction-manager/blob/dcc8484eb3c6f1b6e22d649b74e0f2c29c29c83a/internal/events/eventstream.go#L720
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 15:49:54 +0000 UTC
    </div>
</div>

