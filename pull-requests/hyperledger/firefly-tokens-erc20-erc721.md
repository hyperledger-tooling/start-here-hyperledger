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
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/37" class=".btn">#37</a>
            </td>
            <td>
                <b>
                    Add compatibility with local truffle
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-29 14:41:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/36" class=".btn">#36</a>
            </td>
            <td>
                <b>
                    Allow activation to register from a custom block number
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Allow `blockNumber` to be optionally included in the ERC-20/ERC-721 custom `config` section
- Allow `poolConfig` to be passed by FireFly during `activate`
    - This will require (non-breaking) changes on the FireFly core API contract too
- Create the EthConnect subscriptions from the specified `blockNumber` in preference above all other block numbers
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 18:17:04 +0000 UTC
    </div>
</div>

