---
layout: default
title: aries-framework-swift
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/aries-framework-swift
---

# aries-framework-swift <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-swift){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v1.2.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.2.3
                </span>
            </td>
            <td>
                Many bugs are fixed including revocation handling and mediator message pickup.

## What's Changed
* feature: Support invitation short url by @conanoc in https://github.com/hyperledger/aries-framework-swift/pull/16
* fix the error of ACA-py agent not accepting OOB response by @conanoc in https://github.com/hyperledger/aries-framework-swift/pull/19
* enable AgentConfig codable. by @kukgini in https://github.com/hyperledger/aries-framework-swift/pull/26
* refactor: Prepare to support multiple pools by @kukgini in https://github.com/hyperledger/aries-framework-swift/pull/31
* ProofAttributeInfo.names should be an array type by @kukgini in https://github.com/hyperledger/aries-framework-swift/pull/47
* Support build on XCode 14 by @conanoc in https://github.com/hyperledger/aries-framework-swift/pull/49
* Fix crash when there are multiple attributes to prove by @conanoc in https://github.com/hyperledger/aries-framework-swift/pull/50
* Fix ack message expect response problem by @kukgini in https://github.com/hyperledger/aries-framework-swift/pull/51
* fix revocation registry delta deserialize error. by @kukgini in https://github.com/hyperledger/aries-framework-swift/pull/52
* fix unable to download tails file error when tails directory not exists. by @kukgini in https://github.com/hyperledger/aries-framework-swift/pull/53
* filter out revoked credentials from requested credentials when auto s… by @kukgini in https://github.com/hyperledger/aries-framework-swift/pull/54
* Fix typo by @conanoc in https://github.com/hyperledger/aries-framework-swift/pull/58
* Assert the mediator invitation url is same to that of mediation record by @conanoc in https://github.com/hyperledger/aries-framework-swift/pull/59
* Delete mediation record if it's not ready by @conanoc in https://github.com/hyperledger/aries-framework-swift/pull/60
* Fix implicit pickup by @conanoc in https://github.com/hyperledger/aries-framework-swift/pull/61

**Full Changelog**: https://github.com/hyperledger/aries-framework-swift/compare/v1.2.2...v1.2.3
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-framework-swift/releases/tag/v1.2.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-08-18 01:03:06 +0000 UTC
    </span>
</div>

