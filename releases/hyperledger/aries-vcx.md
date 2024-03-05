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
                    Release 0.62.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.62.0
                </span>
            </td>
            <td>
                # Features
* DID Exchange Protocol by @mirgee in https://github.com/hyperledger/aries-vcx/pull/928
* feat: implement new wallet trait for askar by @xprazak2 in https://github.com/hyperledger/aries-vcx/pull/1085
* DID parser using nom by @mirgee in https://github.com/hyperledger/aries-vcx/pull/1099
* anoncreds-rs integration by @mirgee in https://github.com/hyperledger/aries-vcx/pull/1110

# Enhancements
* Add backtrace capturing, prototype a test err handling by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/1022
* Add mediator coordination messages to aries-vcx messages crate by @nain-F49FF806 in https://github.com/hyperledger/aries-vcx/pull/1052
* feature: Derive Display for all aries messages by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/1069

# Fixes
* Indifferent to b64url padding in indy-utils by @gmulhearn-anonyome in https://github.com/hyperledger/aries-vcx/pull/1055
* fix(message_macros):  explicit lifetime declaration by @nain-F49FF806 in https://github.com/hyperledger/aries-vcx/pull/1077
* fix: didcomm message forwarding by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/1081
* fix: Mediated Connection - Decrypt invitation request at Invitee's as No-Auth by @mkempa in https://github.com/hyperledger/aries-vcx/pull/1087
* fix: #1053 Base64URLSafe padded and unpadded decoding by @lukewli-anonyome in https://github.com/hyperledger/aries-vcx/pull/1083

# Refactoring
* Split test code by @bobozaur in https://github.com/hyperledger/aries-vcx/pull/1023
* Refactor ServiceBuilder by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/1021
* Refactor and modify OutOfBandReceiver by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/1038
* Did peer refactoring, new display macro by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/1034
* refactor: encryption envelope by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/1070
* refactor: encryption envelope APIs, tests by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/1082
* Add justfile by @mirgee in https://github.com/hyperledger/aries-vcx/pull/1125
* Type requested credentials by @mirgee in https://github.com/hyperledger/aries-vcx/pull/1130
* feat: add new Wallet trait, implement for indy wallet by @xprazak2 in https://github.com/hyperledger/aries-vcx/pull/1084
* feat(actions): add input in publish image action and default it to ghcr.io by @PanGan21 in https://github.com/hyperledger/aries-vcx/pull/1142

## New Contributors
* @xprazak2 made their first contribution in https://github.com/hyperledger/aries-vcx/pull/1051
* @mkempa made their first contribution in https://github.com/hyperledger/aries-vcx/pull/1087
* @lukewli-anonyome made their first contribution in https://github.com/hyperledger/aries-vcx/pull/1083
* @vuittont60 made their first contribution in https://github.com/hyperledger/aries-vcx/pull/1098
* @PanGan21 made their first contribution in https://github.com/hyperledger/aries-vcx/pull/1142

**Full Changelog**: https://github.com/hyperledger/aries-vcx/compare/0.61.0...0.62.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-vcx/releases/tag/0.62.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-03-05 07:30:57 +0000 UTC
    </span>
</div>

