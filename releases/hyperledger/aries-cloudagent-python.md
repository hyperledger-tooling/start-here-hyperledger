---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    0.7.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.7.0
                </span>
            </td>
            <td>
                Another significant release, this version adds support for multiple new protocols, credential formats, and extension methods.

- Support for [W3C Standard Verifiable Credentials](https://www.w3.org/TR/vc-data-model/) based on JSON-LD using LD-Signatures and [BBS+ Signatures](https://w3c-ccg.github.io/ldp-bbs2020/), contributed by [Animo Solutions](https://animo.id/) - [#1061](https://github.com/hyperledger/aries-cloudagent-python/pull/1061)
- [Present Proof V2](https://github.com/hyperledger/aries-rfcs/tree/master/features/0454-present-proof-v2) including support for [DIF Presentation Exchange](https://identity.foundation/presentation-exchange/) - [#1125](https://github.com/hyperledger/aries-cloudagent-python/pull/1125)
- Pluggable DID Resolver (with a did:web resolver) with fallback to an external DID universal resolver, contributed by [Indicio](https://indicio.tech/) - [#1070](https://github.com/hyperledger/aries-cloudagent-python/pull/1070)
- Updates and extensions to ledger transaction endorsement via the [Sign Attachment Protocol](https://github.com/hyperledger/aries-rfcs/pull/586), contributed by [AyanWorks](https://www.ayanworks.com/) - [#1134](https://github.com/hyperledger/aries-cloudagent-python/pull/1134), [#1200](https://github.com/hyperledger/aries-cloudagent-python/pull/1200)
- Upgrades to Demos to add support for Credential Exchange 2.0 and W3C Verifiable Credentials [#1235](https://github.com/hyperledger/aries-cloudagent-python/pull/1235)
- Alpha support for the Indy/Aries Shared Components ([indy-vdr](https://github.com/hyperledger/indy-vdr), [indy-credx](https://github.com/hyperledger/indy-shared-rs) and [aries-askar](https://github.com/hyperledger/aries-askar)), which enable running ACA-Py without using Indy-SDK, while still supporting the use of Indy as a ledger, and Indy AnonCreds verifiable credentials [#1267](https://github.com/hyperledger/aries-cloudagent-python/pull/1267)
- A new event bus for distributing internally generated ACA-Py events to controllers and other listeners, contributed by [Indicio](https://indicio.tech/) - [#1063](https://github.com/hyperledger/aries-cloudagent-python/pull/1063)
- Enable operation without Indy ledger support if not needed
- Performance fix for deployments with large numbers of DIDs/connections [#1249](https://github.com/hyperledger/aries-cloudagent-python/pull/1249)
- Simplify the creation/handling of plugin protocols [#1086](https://github.com/hyperledger/aries-cloudagent-python/pull/1086), [#1133](https://github.com/hyperledger/aries-cloudagent-python/pull/1133), [#1226](https://github.com/hyperledger/aries-cloudagent-python/pull/1226)
- DID Exchange implicit invitation handling [#1174](https://github.com/hyperledger/aries-cloudagent-python/pull/1174)
- Add support for Indy 1.16 predicates (restrictions on predicates based on attribute name and value) [#1213](https://github.com/hyperledger/aries-cloudagent-python/pull/1213)
- BDD Tests run via GitHub Actions [#1046](https://github.com/hyperledger/aries-cloudagent-python/pull/1046)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.7.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-07-15 11:42:15 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    0.7.0-rc1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.7.0-rc1
                </span>
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.7.0-rc1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-07-08 20:24:11 +0000 UTC
    </span>
</div>

