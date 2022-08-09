---
layout: default
title: aries-acapy-plugin-toolbox
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/aries-acapy-plugin-toolbox
---

# aries-acapy-plugin-toolbox <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-plugin-toolbox){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    0.3.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.3.0
                </span>
            </td>
            <td>
                Compatible with ACA-Py 0.7.4.

## What's Changed
* chore: add documents required by repolint by @dbluhm in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/59
* Use event bus to send notifications to Admin connections by @dbluhm in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/60
* fix: ledger not ready on get taa accept request by @dbluhm in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/64
* Fix presentation and issuance errors by @dbluhm in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/66
* fix: basic messages not sending to recipients by @dbluhm in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/67
* Check in integration test progress by @dbluhm in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/70
* refactor: simplify logging by @dbluhm in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/72
* fix: add assign_thread_from function to ReceiveInvitationHandler by @cjhowland in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/74
* Test/int/connections by @cjhowland in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/75
* Test/int/schemas by @cjhowland in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/77
* fix: presentation as holder failure on cred retrieval by @dbluhm in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/78
* fix: replace ngrok with localtunnel by @dbluhm in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/82
* Integration tests part II by @dbluhm in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/85
* chore: replaced reference to "master" with "main" by @frostyfrog in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/87
* Test/add integration testing for credentials-get-list by @cjhowland in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/94
* feat:added_connections_unit_test by @PeterStrob in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/95
* Trustping Protocol and Integration Test updates by @dbluhm in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/96
* Update CONTRIBUTING.md by @ryjones in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/97
* feat:added_connections_GetListHandler_test by @PeterStrob in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/99
* feat: Add revocation support to credentials by @frostyfrog in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/88
* Add presentation request to the "get-matching-credentials" call by @frostyfrog in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/100
* fix: Switch from Sovrin StagingNet to BuilderNet by @frostyfrog in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/103
* feat:added updatehandler test by @PeterStrob in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/102
* fix: demo mediator use undelivered queue by @dbluhm in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/101
* Support ACA-Py 0.7.1 by @dbluhm in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/86
* feat:added_StorageError_check_to_updatehandler_test by @PeterStrob in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/104
* feat/added_deletehandler_unit_test by @PeterStrob in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/105
* feat:added create invitation handler unit test by @PeterStrob in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/107
* chore: Update readme with tip to install the Indy SDK by @frostyfrog in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/108
* doc: Add information about starting ACA-Py with config by @frostyfrog in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/109
* feat: update tunnels in demo to use simplified service by @dbluhm in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/106
* feat:added presentation exchange flow integration test by @PeterStrob in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/110
* Feat/added receiveinvitationhandler.test by @PeterStrob in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/111
* refactor: simplify docker and demos by @dbluhm in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/112
* Fix message delivery to open session by @dbluhm in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/92
* fix: acapy-endpoint.sh to send correct ws endpoint to ACA-Py by @frostyfrog in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/113
* feat: add docker-compose for agent local connections by @cjhowland in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/114
* Feature/aca py 0.7.3rc0 by @frostyfrog in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/116
* Feat/credential-issued and presentation-received notification messages by @cjhowland in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/117
* feat: update to 0.7.3 of ACA-Py by @dbluhm in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/119
* fix: holder cred-get-list returns only holder creds by @dbluhm in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/120
* docs: handling interlaced QR code by @mepeltier in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/121
* Feature/oob didex admin by @PeterStrob in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/123
* Feat/custom pres req reject by @mepeltier in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/124
* feat: update mediator wallet to bypass encoding problems for demo by @mepeltier in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/126
* Fix/admin trustping demo by @mepeltier in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/127
* feat: replace connections with oob for invites in all demo configs by @mepeltier in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/128
* test: update acapy-client in int tests by @dbluhm in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/129
* Test/int/connection reuse by @cjhowland in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/130
* feat: Upgrade to ACA-Py 0.7.4 by @frostyfrog in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/132

## New Contributors
* @frostyfrog made their first contribution in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/87
* @PeterStrob made their first contribution in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/95
* @mepeltier made their first contribution in https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/121

**Full Changelog**: https://github.com/hyperledger/aries-acapy-plugin-toolbox/compare/v0.1.0...v0.3.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-acapy-plugin-toolbox/releases/tag/v0.3.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-07-11 19:57:18 +0000 UTC
    </span>
</div>

