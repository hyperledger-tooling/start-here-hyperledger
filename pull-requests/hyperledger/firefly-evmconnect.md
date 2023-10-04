---
layout: default
title: firefly-evmconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-evmconnect
---

# firefly-evmconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-evmconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/101" class=".btn">#101</a>
            </td>
            <td>
                <b>
                    Do not block startup to check chain head
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #98

Depends on https://github.com/hyperledger/firefly-signer/pull/48 (was causing a panic in UTs)

Instead of checking the chain head in-line in `EventStreamStart()` function, this change pushes that `preStartProcessing` code down into the `streamLoop` that gets started asynchronously.

This means we don't block FFTM from starting up.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 18:17:18 +0000 UTC
    </div>
</div>

