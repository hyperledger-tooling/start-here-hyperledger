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
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/75" class=".btn">#75</a>
            </td>
            <td>
                <b>
                    fix: Update to latest firefly-common resty
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **NOTE** This is an draft as it relies on a PR in firefly-common and firefly-transaction-manager
- https://github.com/hyperledger/firefly-common/pull/65
- https://github.com/hyperledger/firefly-transaction-manager/pull/77
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-20 15:43:43 +0000 UTC
    </div>
</div>

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

