---
layout: default
title: firefly-tokens-erc20-erc721
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-tokens-erc20-erc721
---

# firefly-tokens-erc20-erc721 <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-tokens-erc20-erc721){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/83" class=".btn">#83</a>
            </td>
            <td>
                <b>
                    Port eventstream changes from erc1155
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Mostly a port of https://github.com/hyperledger/firefly-tokens-erc1155/pull/94

Note that stream names in this repo do not contain a reference to the contract address, as they do in ERC1155. In the case of this connector, there are actually many different contracts (one optional factory and many deployed instances) - so it may be more difficult to detect if one changed. I've left the stream naming unchanged in this PR, just ported the slightly altered event stream logic.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-23 20:05:18 +0000 UTC
    </div>
</div>

