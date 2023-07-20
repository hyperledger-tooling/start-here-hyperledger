---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1371" class=".btn">#1371</a>
            </td>
            <td>
                <b>
                    Log full payload of critical EVMConnect actions at DEBUG level
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The payloads that flow between `firefly-core` and `firefly-evmconnect` are a very important contract in FireFly, and there's complex translation that happens (FFI <-> ABI etc. and other things in the operation like the `from` address and `location`).
For debugging it's very important to be able to see the exact payload, and important enough you shouldn't need to enable `trace` level and take the cost of logging _every_ payload exchange between microservices to see it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-19 15:07:07 +0000 UTC
    </div>
</div>

