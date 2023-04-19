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
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/74" class=".btn">#74</a>
            </td>
            <td>
                <b>
                    include from field on eth_call
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                calling `query` function on a contract API is always resulting in `sender` being passed as `0x0` because the `from` field is not included in the RPC call.

If `options.from` is provided to firefly core, it is being passed down to evmconnect but it is not being included in the RPC call in the case where the type is `query`. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-14 00:17:18 +0000 UTC
    </div>
</div>

