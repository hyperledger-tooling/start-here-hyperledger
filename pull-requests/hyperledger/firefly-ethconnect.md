---
layout: default
title: firefly-ethconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-ethconnect
---

# firefly-ethconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-ethconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/186" class=".btn">#186</a>
            </td>
            <td>
                <b>
                    don't swallow webhook processMsg status codes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                While doing some performance testing for tokens, @awrichar and I noticed that the `429` HTTP code was being swallowed and a `500` was being returned instead. Now, any error code from `processMsg` will be correctly surfaced.  
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 02:50:16 +0000 UTC
    </div>
</div>

