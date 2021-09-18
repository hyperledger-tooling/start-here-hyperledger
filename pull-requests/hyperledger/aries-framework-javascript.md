---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/458" class=".btn">#458</a>
            </td>
            <td>
                <b>
                    Feature/offline message retrieval
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds access to sending a trust ping via the connectionsModule and allows passing of trust ping message arguments (to be able to set response requested, for instance).
Fixes mediation websocket reconnect exponential backoff incrementing behavior. 
Fixes mediation to allow queued messages to be picked up from an ACA-Py Mediator. ACA-Py as a mediator only will deliver messages from the undelivered queue if a message does not trigger a response, such as a trust ping with response requested: false. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-18 00:09:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/457" class=".btn">#457</a>
            </td>
            <td>
                <b>
                    fix(core): using query-string to parse URLs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Took the advice of @TimoGlastra ans used query-string for parsing URLs. 



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 15:48:07 +0000 UTC
    </div>
</div>

