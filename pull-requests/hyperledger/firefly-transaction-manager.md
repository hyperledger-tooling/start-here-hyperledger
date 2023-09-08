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
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/101" class=".btn">#101</a>
            </td>
            <td>
                <b>
                    Start debug server before we start processing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Notices when debugging an issue, that even though a debug listener was configured, there wasn't one running. Turns out the runtime was hitting a problem establishing its event streams, before starting the debug server.

This PR proposes:
- Starting the debug server earlier
- Using the standard `httpserver` config structure and go routine
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-08 16:01:51 +0000 UTC
    </div>
</div>

