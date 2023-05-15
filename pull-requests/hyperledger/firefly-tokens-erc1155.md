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
                    Allow creating token pools from an existing ERC1155 contract
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

These `startId` and `endId` params can also be passed in on `config` (in
addition to `address`) when creating a token pool, which will generate and
return pool details immediately instead of expecting to call a `create` method.

The old poolId format such as "F1" or "N2" will still be parsed as expected,
but will not be attached to any new pools.

Fixes #104
Fixes #98

**Breaking Change**
There is a minor breaking change in that `info.typeId` on a token pool has
been replaced with `info.startId` for consistency. Any applications that happen
to rely on this field will need to change to the new spelling.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-12 19:09:15 +0000 UTC
    </div>
</div>

