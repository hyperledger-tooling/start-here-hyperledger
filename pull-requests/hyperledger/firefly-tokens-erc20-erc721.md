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
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/109" class=".btn">#109</a>
            </td>
            <td>
                <b>
                    Change ERC721 samples to use auto-indexing mint by default
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                With this change, the default "out of the box" sample for ERC721 will _not_ require (or allow) you to pass a token index when minting. It will choose an increasing token index starting from 0.

Via ERC165 support, the connector can now check for 3 different versions of the ERC721WithData interface:
- the current version (V2), which uses auto-indexing on mint and also supports all withData/withURI methods
- the previous version (V1b), which requires explicit indexes, but supports all withData/withURI methods
- the original version (V1a), which requires explicit indexes, and supports withData but not withURI

For the "no data" variant, we have no ERC165 support, so I have destructively replaced the ERC721NoData sample with a new one that uses auto-indexing. Note that it was _just_ replaced in #104 and released as v1.2.0 - I don't really see any need to preserve all the versions of this sample, so I'm just preserving this new one and the original (not the interim one introduced in v1.2.0). This new PR will probably need to become release v1.2.1, and we'll just want to note that the sample in v1.2.0 is not supported.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 17:17:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/108" class=".btn">#108</a>
            </td>
            <td>
                <b>
                    Update README
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add more details on the different smart contract variants supported, and clarify extensions on top of the base fftokens protocol.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 16:25:46 +0000 UTC
    </div>
</div>

