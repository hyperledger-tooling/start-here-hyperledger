---
layout: default
title: perun-eth-backend
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/perun-eth-backend
---

# perun-eth-backend <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/perun-eth-backend){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-eth-backend/pull/45" class=".btn">#45</a>
            </td>
            <td>
                <b>
                    Draft: Introduce Egoistic Funding 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR introduced "egoistic funding" where one participant can be tagged to be egoistic using the `EgoisticPart` array (which does not change the funder interface) such that it waits until all other participants have deposited their amounts before continuing to deposit.

The background to this is that in PerunX, the hub should not deposit until the client has deposited its funds to prevent losses due to gas costs if the client never actually deposits.
As a consequence, the Perun Websocket Backend needs to be adapted that one of the participants can register as egoistic (maybe even in the `Initialize` message?) and the WebSocket Backend provides information this to the funder.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-19 12:26:58 +0000 UTC
    </div>
</div>

