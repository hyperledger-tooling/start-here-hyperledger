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
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/134" class=".btn">#134</a>
            </td>
            <td>
                <b>
                    Async event enrichment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR aims to improve the concurrency of event-enrichment.

Today when a batch of events is received from the token connector, each event is processed synchronously. In the case of an NFT transfer event, processing that event involves a call to `getTokenURI()` which requires communication with the chain via the blockchain connector. These calls can be made in parallel so long as the original order of the events is maintained when the batch is sent on to FireFly core.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-27 08:57:35 +0000 UTC
    </div>
</div>

