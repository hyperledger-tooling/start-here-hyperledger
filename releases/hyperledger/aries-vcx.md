---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Release 0.63.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.63.0
                </span>
            </td>
            <td>
                # Removed
* remove libvcx_core and vcx_napi_rs crates by @xprazak2 in https://github.com/hyperledger/aries-vcx/pull/1145
* remove mediated connection and agency client by @xprazak2 in https://github.com/hyperledger/aries-vcx/pull/1147

# Refactor
* Use `did_parser_nom` instead of legayc `did_parser` by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/1150
* refactor: use BaseWallet instead of a specific wallet type by @xprazak2 in https://github.com/hyperledger/aries-vcx/pull/1122
* Do not include logger implementation in aries-vcx by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/1149
* Refactor aries-agent-rust by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/1153
* Embed aath backchannel into repo by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/1155

# Changes
* change: simplify didcore components, did-exchange protocol by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/1075

# Features
* feat: add wallet migration to askar by @xprazak2 in https://github.com/hyperledger/aries-vcx/pull/1144

# Packages
* Bump h2 from 0.3.21 to 0.3.24 by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1109
* chore(deps): bump mio from 0.8.8 to 0.8.11 by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1143


**Full Changelog**: https://github.com/hyperledger/aries-vcx/compare/0.62.0...0.63.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-vcx/releases/tag/0.63.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-03-17 22:28:13 +0000 UTC
    </span>
</div>

