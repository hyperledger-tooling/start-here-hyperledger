---
layout: default
title: firefly-tokens-erc1155
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-tokens-erc1155
---

# firefly-tokens-erc1155 <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-tokens-erc1155){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc1155/pull/123" class=".btn">#123</a>
            </td>
            <td>
                <b>
                    Drop narrow "poolId" formatting in favor of "startId/endId"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Pools on ERC1155 are really just ranges of the token ID space. Going forward,
all pools will be expressed with a `startId` and `endId`. This makes the service
logic much less bound to the specific decisions made in the sample contract
around partitioning it in chunks of exactly 2^128.

The old poolId format such as "F1" or "N2" will still be parsed as expected,
but will not be attached to any new pools.

This is a step toward solving #104 and #98. The remaining work is mainly around
ensuring we _don't_ require a preset factory contract to be configured, and allowing
the user to pass in `startId`/`endId` when creating a pool, which will use them directly
instead of calling `create`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-12 19:09:15 +0000 UTC
    </div>
</div>

