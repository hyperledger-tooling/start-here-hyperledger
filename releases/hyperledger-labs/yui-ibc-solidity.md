---
layout: default
title: yui-ibc-solidity
parent: Hyperledger Labs
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger-labs/yui-ibc-solidity
---

# yui-ibc-solidity <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-ibc-solidity){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v0.3.33
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.3.33
                </span>
            </td>
            <td>
                ## What's Changed
* Fix to ensure `proposedConnectionHops` of MsgChannelUpgradeTry matches existing upgrade's one by @bluele in https://github.com/hyperledger-labs/yui-ibc-solidity/pull/286
* Add ERC-165 to IIBCModule by @bluele in https://github.com/hyperledger-labs/yui-ibc-solidity/pull/284

## For IBC Module Developers

After #284, the module developers must either inherit `IBCAppBase` or implement ERC-165 to support `IIBCModule` interface explicitly in their modules.

**Full Changelog**: https://github.com/hyperledger-labs/yui-ibc-solidity/compare/v0.3.32...v0.3.33
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/releases/tag/v0.3.33" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-22 01:10:58 +0000 UTC
    </span>
</div>

