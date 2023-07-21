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
                    Release 0.57.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.57.0
                </span>
            </td>
            <td>
                # Changes
* Remove vcx_schema_prepare_for_endorser by @mirgee in https://github.com/hyperledger/aries-vcx/pull/860

# New components
* Feature/credx issuer by @bobozaur in https://github.com/hyperledger/aries-vcx/pull/854
* Sovrin-specific DDO facade by @mirgee in https://github.com/hyperledger/aries-vcx/pull/871
* Implementation of did:peer:2 DID method by @mirgee in https://github.com/hyperledger/aries-vcx/pull/883
* Support peer:did:3 by @mirgee in https://github.com/hyperledger/aries-vcx/pull/886
* Feature/cred migrator by @bobozaur in https://github.com/hyperledger/aries-vcx/pull/867
* libvcx implementation profiles by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/892

# Fixes
* Fix ci by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/876
* Fix 877: Connection Requests with empty DIDDoc pubkey controller by @gmulhearn-anonyome in https://github.com/hyperledger/aries-vcx/pull/878

# Refactoring
* Split BaseLedger trait by @mirgee in https://github.com/hyperledger/aries-vcx/pull/861
* Issue #847: Prover Handler Types by @gmulhearn in https://github.com/hyperledger/aries-vcx/pull/848
* Split IndyVdrLedger and IndySdkLedger by @mirgee in https://github.com/hyperledger/aries-vcx/pull/862
* Remove reliance of IndyVdrLedger on global state by @mirgee in https://github.com/hyperledger/aries-vcx/pull/863
* Refactor/do not consume profile by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/872
* Make DidDocument's service generic over method-specific fields by @mirgee in https://github.com/hyperledger/aries-vcx/pull/865
* Minor DDO service builder improvement by @mirgee in https://github.com/hyperledger/aries-vcx/pull/868
* Refactor basewallet and corresponding consumers by @tech-bash in https://github.com/hyperledger/aries-vcx/pull/843
* Remove unnecessary bound on DDO service by @mirgee in https://github.com/hyperledger/aries-vcx/pull/879
* Inject only required components, not entire profiles by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/873
* Remove unused lockfiles by @mirgee in https://github.com/hyperledger/aries-vcx/pull/882
* Make PeerDid generic over numalgo by @mirgee in https://github.com/hyperledger/aries-vcx/pull/887
* Refactor/testing by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/880
* Refactor dealing with tails_dir in tests by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/897
* Cleanup/constant by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/898

# Dependencies
* Update dependencies and AriesMessage Deserialize impl by @bobozaur in https://github.com/hyperledger/aries-vcx/pull/894

# Improvements
* Enable compiling the workspace with --tests --all-features by @mirgee in https://github.com/hyperledger/aries-vcx/pull/890

# CI
* CI: Skip test-android job by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/885
* Tweak CI to fix build-docker-android on main branch by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/899

**Full Changelog**: https://github.com/hyperledger/aries-vcx/compare/0.56.0...0.57.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-vcx/releases/tag/0.57.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-07-19 10:08:53 +0000 UTC
    </span>
</div>

