---
layout: default
title: iroha-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-javascript
---

# iroha-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-javascript/pull/88" class=".btn">#88</a>
            </td>
            <td>
                <b>
                    fix: isomorphic client transports
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Client should work both in Node.js & Web. I achieved this seamlessly introducing 2 new packages - `@iroha2/client-isomorphic-ws` (WebSocket) and `*-fetch` (Fetch API).

And now I am pretty sure that client works in Web thanks to new Cypress test.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-29 10:28:27 +0000 UTC
    </div>
</div>

