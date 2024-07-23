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
                    Release 0.65.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.65.0
                </span>
            </td>
            <td>
                Release 0.65.0 most notably adds support for DID Exchange 1.1, as well as updates the AATH (Aries Agent Test Harness) Aries VCX Backchannel to continuously keep the backchannel deployed (see https://aries-interop.info/aries-vcx.html for the latest results), as well as address multiple interoperability issues between Aries VCX and ACA-Py (Aries Cloud Agent Python). This release also updates some scripts and documentation for the mobile demo code to resolve issues and work towards adding support for iOS.

Release 0.65.0 updates the Aries VCX Rust version to 1.79, and performed a large number of internal dependency bumps. This release will be the **final** release with support for the legacy indy-sdk, credx, and indyvdrtools crates and features (see https://github.com/hyperledger/aries-vcx/issues/1250 for more details).

## What's Changed
### DID Exchange
* Support DIDExchange 1.1 #1228 by @gmulhearn in https://github.com/hyperledger/aries-vcx/pull/1230
* Small refactor to the new DIDExchange AnyXYZ wrappers by @gmulhearn in https://github.com/hyperledger/aries-vcx/pull/1249
* [FIX] DIDExchange handlers should do more signature checking #1226 by @gmulhearn-anonyome in https://github.com/hyperledger/aries-vcx/pull/1232

### AATH (Aries Agent Test Harness)
* Update AATH backchannel to build image by @gmulhearn-anonyome in https://github.com/hyperledger/aries-vcx/pull/1221
* Handle trust pings in the AATH backchannel by @gmulhearn in https://github.com/hyperledger/aries-vcx/pull/1254
* (chore) improve AATH readme with some dev instructions by @gmulhearn-anonyome in https://github.com/hyperledger/aries-vcx/pull/1273

### Mobile / UniFFI
* Update uniffi readme by @alberto-instnt in https://github.com/hyperledger/aries-vcx/pull/1259
* Android adjustment & Askar udl impl by @alberto-instnt in https://github.com/hyperledger/aries-vcx/pull/1263
* Android script fix & Askar impl on Kotlin mobile demo by @alberto-instnt in https://github.com/hyperledger/aries-vcx/pull/1270

### Dependencies / CI / Docs
* (chore) update to rust 1.79 by @gmulhearn in https://github.com/hyperledger/aries-vcx/pull/1274
* Removed unused code and suppressed warnings/errors by @alberto-instnt in https://github.com/hyperledger/aries-vcx/pull/1262
* (chore) update all cargo deps by @gmulhearn in https://github.com/hyperledger/aries-vcx/pull/1275
* chore: adjust dependabot config by @JamesKEbert in https://github.com/hyperledger/aries-vcx/pull/1276

#### Dependabot
* chore(deps): bump androidx.camera:camera-camera2 from 1.2.3 to 1.3.4 in /aries/agents/mobile_demo by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1229
* chore(deps): bump androidx.compose:compose-bom from 2022.10.00 to 2022.12.00 in /aries/agents/mobile_demo by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1188
* chore(deps): bump rsa from 0.9.2 to 0.9.6 in the cargo group across 1 directory by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1218
* chore(deps): bump com.google.code.gson:gson from 2.8.9 to 2.11.0 in /aries/agents/mobile_demo/app by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1190
* chore(deps): bump alpine from 3.15.4 to 3.20.0 in /aries/agents/aath-backchannel by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1192
* chore(deps): bump regex from 1.10.3 to 1.10.5 in /aries/misc/anoncreds_types by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1222
* chore(deps): bump org.jetbrains.kotlin.android from 1.7.20 to 1.9.24 in /aries/agents/mobile_demo by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1208
* chore(deps): bump net.java.dev.jna:jna from 5.13.0 to 5.14.0 in /aries/agents/mobile_demo/app by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1205
* chore(deps): bump org.jetbrains.kotlin:kotlin-bom from 1.8.0 to 1.9.24 in /aries/agents/mobile_demo/app by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1204
* chore(deps): bump androidx.activity:activity-compose from 1.5.1 to 1.9.0 in /aries/agents/mobile_demo by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1193
* chore(deps): bump num-bigint from 0.4.4 to 0.4.5 by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1201
* chore(deps): bump curve25519-dalek from 4.1.1 to 4.1.3 in the cargo group by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1231
* chore(deps): bump com.squareup.okhttp3:okhttp from 4.11.0 to 4.12.0 in /aries/agents/mobile_demo/app by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1207
* chore(deps): bump log from 0.4.20 to 0.4.21 in /aries/misc/anoncreds_types by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1198
* chore(deps): bump serde_json from 1.0.111 to 1.0.117 in /aries/misc/anoncreds_types by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1199
* chore(deps): bump tokio from 1.33.0 to 1.38.0 by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1203
* chore(deps): bump typed-builder from 0.16.2 to 0.18.1 by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1211
* chore(deps): bump serde from 1.0.195 to 1.0.203 in /aries/misc/anoncreds_types by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1196
* chore(deps): bump zeroize from 1.6.0 to 1.8.1 by @dependabot in https://github.com/hyperledger/aries-vcx/pull/1209

## New Contributors
* @alberto-instnt made their first contribution in https://github.com/hyperledger/aries-vcx/pull/1259

**Full Changelog**: https://github.com/hyperledger/aries-vcx/compare/0.64.0...0.65.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-vcx/releases/tag/0.65.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-23 05:16:17 +0000 UTC
    </span>
</div>

