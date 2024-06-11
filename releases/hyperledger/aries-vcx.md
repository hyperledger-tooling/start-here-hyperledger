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
                    Release 0.64.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.64.0
                </span>
            </td>
            <td>
                # What's Changed
Release 0.64.0 has lots of refactoring, fixes, and dependency updates. did:peer:4 support was added, as well as the move to using upstream anoncreds-rs releases. Release 0.64.0 includes the last of the major contributions supported by the Absa team--major thanks to all of the Absa contributors for all their hard work and contributions to Aries VCX! 

## Features
* Feature/didpeer4 by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/1161
* `did:peer:4` integration, bugfix, improvements by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/1167
* feat: load wallet config from environment variables by @nain-F49FF806 in https://github.com/hyperledger/aries-vcx/pull/1178
* Add setters on `DidDocument`, remove `DidDocumentBuilder` by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/1164

## Refactoring
* refactor: move anoncreds to a separate crate by @xprazak2 in https://github.com/hyperledger/aries-vcx/pull/1175
* refactor: improve mediator routes by @xprazak2 in https://github.com/hyperledger/aries-vcx/pull/1176
* refactor: support json response for mediator base path by @xprazak2 in https://github.com/hyperledger/aries-vcx/pull/1168
* refactor: move wallet to a separate crate by @xprazak2 in https://github.com/hyperledger/aries-vcx/pull/1157
* refactor: move ledger to a separate crate by @xprazak2 in https://github.com/hyperledger/aries-vcx/pull/1172
* refactor: Use `typed-builder` instead of custom one for `VerificationMethod` by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/1162
* Minor aath refactor by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/1159

## Fixes
* [FIX] Loosen "version" restriction on PresentationRequestPayload by @gmulhearn-anonyome in https://github.com/hyperledger/aries-vcx/pull/1212
* fix: allow agent wallet re-creation by @Zzocker in https://github.com/hyperledger/aries-vcx/pull/1184

## CI / Docs
* Simple documentation fixes by @JamesKEbert in https://github.com/hyperledger/aries-vcx/pull/1181
* Update MAINTAINERS.md by @gmulhearn in https://github.com/hyperledger/aries-vcx/pull/1186
* chore: minor readme updates by @JamesKEbert in https://github.com/hyperledger/aries-vcx/pull/1187
* refactor: add new crates to readme by @xprazak2 in https://github.com/hyperledger/aries-vcx/pull/1182
* ci, fix: update path that mediator ci workkflow looks for by @nain-F49FF806 in https://github.com/hyperledger/aries-vcx/pull/1177
* Release 0.64.0 by @JamesKEbert in https://github.com/hyperledger/aries-vcx/pull/1223

## Dependencies
* [Update] Update to anoncreds-rs 0.2 by @gmulhearn-anonyome in https://github.com/hyperledger/aries-vcx/pull/1213
* [FIX] Reduce unnecessary required deps by @gmulhearn-anonyome in https://github.com/hyperledger/aries-vcx/pull/1217
* chore: updating dependabot to support gradle, docker, gha and cargo packages by @rajpalc7 in https://github.com/hyperledger/aries-vcx/pull/1185
* chore(deps): bump anoncreds-clsignatures from 0.3.1 to 0.3.2 in /aries/misc/anoncreds_types by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1200
* chore(deps): update anoncreds-clsignatures requirement from 0.2.0 to 0.3.2 in /aries/misc/indy_ledger_response_parser in the cargo group across 1 directory by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1215
* Update Rust in CI to 1.76 by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/1158
* chore(deps): bump the cargo group with 2 updates by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1216
* chore(deps): bump rustls from 0.21.7 to 0.21.11 by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1183
* chore(deps): bump h2 from 0.3.24 to 0.3.26 by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1174
* chore(deps): bump whoami from 1.4.1 to 1.5.1 by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1173
* Remove codecov job by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/1180

## New Contributors
* @JamesKEbert made their first contribution in https://github.com/hyperledger/aries-vcx/pull/1181
* @Zzocker made their first contribution in https://github.com/hyperledger/aries-vcx/pull/1184
* @rajpalc7 made their first contribution in https://github.com/hyperledger/aries-vcx/pull/1185

**Full Changelog**: https://github.com/hyperledger/aries-vcx/compare/0.63.0...0.64.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-vcx/releases/tag/0.64.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-06-11 03:41:39 +0000 UTC
    </span>
</div>

