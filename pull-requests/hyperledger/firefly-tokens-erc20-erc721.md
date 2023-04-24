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
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/131" class=".btn">#131</a>
            </td>
            <td>
                <b>
                    Add REST call and event batch size metrics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a variety of metrics and will close https://github.com/hyperledger/firefly-tokens-erc20-erc721/issues/89 when its complete.

The approach I've used is to add to the existing log interceptor and use that as a point to capture inbound API metrics. The renamed `logging-and-metrics` interceptor exposes methods to set/inc/observe other metrics e.g. relating to blockchain calls and event processing.

A few more details of the approach I've used are in the issue.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-18 14:04:16 +0000 UTC
    </div>
</div>

