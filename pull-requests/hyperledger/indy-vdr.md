---
layout: default
title: indy-vdr
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-vdr
---

# indy-vdr <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-vdr){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/242" class=".btn">#242</a>
            </td>
            <td>
                <b>
                    Faster pool refresh
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Capture additional information about the state proof multi-signature verification.
- After performing a successful status request, prioritize the responding nodes when performing a subsequent catchup request. This helps to avoid delays waiting for nodes that are no longer active.
- Adjust default configuration parameters: ack_timeout -> 5 seconds, read timeout -> 30 seconds, connection request limit -> 10 requests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-01 19:01:17 +0000 UTC
    </div>
</div>

