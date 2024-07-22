---
layout: default
title: firefly-signer
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-signer
---

# firefly-signer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-signer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/68" class=".btn">#68</a>
            </td>
            <td>
                <b>
                    Expose API to directly call HashStruct from EIP-712 and M+N dims
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Allows use of the EIP-712 hashing algorithm for the data itself, without needing to also supply a domin.
- Allows querying `M` and `N` dimensions of parsed Elementary Types
- Fixes issue where we could have a `Component` array containing a nil entry on the case of extra parameters on input
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-15 21:13:14 +0000 UTC
    </div>
</div>

