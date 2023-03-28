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
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/128" class=".btn">#128</a>
            </td>
            <td>
                <b>
                    Retry logic for blockchain calls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes https://github.com/hyperledger/firefly-tokens-erc20-erc721/issues/126 

PR https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/122 discussed the idea of retrying token URI lookup calls but in the end it was decided it was out of scope.

The changes in this PR are an attempt to provide a pragmatic approach to making any blockchain calls (which will include those driven by `tokenURI()`) retryable based on whether a given blockchain call returns an error that matches the configured regex pattern. For example setting the pattern to `.*ECONNREFUSED.*` causes the blockchain call to retry after a back-off delay.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-27 13:24:11 +0000 UTC
    </div>
</div>

