---
layout: default
title: firefly-cordaconnect
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-cordaconnect
---

# firefly-cordaconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-cordaconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cordaconnect/pull/5" class=".btn">#5</a>
            </td>
            <td>
                <b>
                    Add support for eventstream, REST layer, fix cordapp and readme update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR includes
- [x] spring boot application `connector`
   - [x] eventstream management REST APIS for corda, similar to ethconnect
   - [x] WebSockets support to listen on corda events
   - [x] REST API to interact with firefly cordapp (`/broadcastBatch`) 
   - [x] Swagger support for REST endpoints 
- [x] Fixes to firefly cordapp (adds missing logic inside firefly-flows cordapp)
- [x] Updates to readme

Signed-off-by: amit panghal <amit.panghal@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-24 21:23:58 +0000 UTC
    </div>
</div>

