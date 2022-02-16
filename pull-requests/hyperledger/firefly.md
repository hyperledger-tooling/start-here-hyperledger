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
                PR <a href="https://github.com/hyperledger/firefly/pull/502" class=".btn">#502</a>
            </td>
            <td>
                <b>
                    Use inline ABI for all Ethconnect contract interactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates all smart contract interactions with Ethconnect so that Ethconnect no longer needs a previously deployed ABI to interact with a given contract. Instead, FireFly now has code that can convert the relevant parts of an FFI into an ABI format. The JSON ABI is used inline in each request to Ethconnect to invoke or query smart contracts or subscribe to events.

Resolves:
- https://github.com/hyperledger/firefly/issues/426
- https://github.com/hyperledger/firefly/issues/425
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 15:37:22 +0000 UTC
    </div>
</div>

