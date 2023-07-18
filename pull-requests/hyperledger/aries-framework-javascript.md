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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1508" class=".btn">#1508</a>
            </td>
            <td>
                <b>
                    fix(samples): mediator wallet and http transport
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds `IndySdkModule` to `Agent` modules in order to allow it to have a default Wallet and Storage implementation (it could be Askar once we solve the performance issue for node <18 and/or drop support for it).

In `HttpInboundTransport`, It also moves content-type validation to the specific endpoint rather than the whole HTTP server. This is needed to allow using an invitation endpoint.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-12 18:30:05 +0000 UTC
    </div>
</div>

