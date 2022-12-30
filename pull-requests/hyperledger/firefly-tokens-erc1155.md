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
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc1155/pull/105" class=".btn">#105</a>
            </td>
            <td>
                <b>
                    Support passing an ABI directly in any mint/burn/transfer/approval call
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In a chain with #103.
Part of [FIR-16](https://github.com/hyperledger/firefly-fir/pull/16).

Companion to https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/104 - see notes there for a general description of this enhancement.

**Breaking Changes**
The `info.baseUri` field will no longer be populated when creating a non-fungible pool. Similar to the notes on the ERC20/721 PR, this is done because it relies on a non-standard method in the contract, is perceived to be rarely used, and can be worked around by directly invoking the underlying contract method.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-30 14:56:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc1155/pull/103" class=".btn">#103</a>
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
                Companion to https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/103
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-29 17:34:37 +0000 UTC
    </div>
</div>

