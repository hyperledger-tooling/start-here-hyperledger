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
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc1155/pull/124" class=".btn">#124</a>
            </td>
            <td>
                <b>
                    Add status suffix to readiness probe
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The readiness probe is configured to hit the root of the EVMConnect API - this will give a 405. It needs the status suffix. The ERC20-ERC721 connector already has this suffix.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-22 15:38:20 +0000 UTC
    </div>
</div>

