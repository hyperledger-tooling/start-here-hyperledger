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
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/103" class=".btn">#103</a>
            </td>
            <td>
                <b>
                    Split tokens service logic into multiple helpers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In anticipation of [FIR-16](https://github.com/hyperledger/firefly-fir/pull/16), which is likely to complicate the connector further, it seems like we're overdue for splitting up the logic in this file.

Goal here is to split without changing any current functionality (although some changes were needed to achieve a clean break, particularly around ABI mapping). Unit tests, Nest E2E tests, and FireFly E2E tests passed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-21 13:46:58 +0000 UTC
    </div>
</div>

