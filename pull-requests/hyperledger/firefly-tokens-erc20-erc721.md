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
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/70" class=".btn">#70</a>
            </td>
            <td>
                <b>
                    Scrub "namespace" params in favor of more generic data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Partially reverts #59 because it was broken, but also makes the interface
a bit more generic and extensible.

Rather than dictating a namespace param, allow FireFly to pass a
string of data during pool activation, which (if possible) will be stored
locally and returned on all transfer/approval events from that pool. The
behavior is optional and not guaranteed by the connector.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 21:47:37 +0000 UTC
    </div>
</div>

