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
                    0.7.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.7.3
                </span>
            </td>
            <td>
                This release includes some new AIP 2.0 features (Revocation Notification and Discover Features 2.0), a major new feature for those using Indy ledger (multi-ledger support), a new "version upgrade" process that automates updating data in secure storage required after a new release, and a fix for a critical bug in some mediator scenarios. The release also includes several new pieces of documentation (upgrade processing, storage database information and logging) and some other documentation updates that make the ACA-Py Read The Docs site useful again. And of course, some recent bug fixes and cleanups are included.

For more context of the changes in this release, please see the [CHANGELOG.md](/CHANGELOG.md) file. Below is a generated list of the PRs.

## What's Changed
* Fix TypeError by @gorgsenegger in https://github.com/hyperledger/aries-cloudagent-python/pull/1494
* Add RTD configs to get generator working by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1496
* DIF PresExch - ProblemReport and "is_holder" by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1493
* Remove Streetcred references by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1504
* Discover Features Protocol: v1_0 refactoring and v2_0 implementation by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1500
* Fix warnings when generating ReadTheDocs by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1509
* Fix error when connection request is received (askar, public invitation) by @baegjae in https://github.com/hyperledger/aries-cloudagent-python/pull/1508
* Fix TypeError when calling credential_definitions_fix_cred_def_wallet… by @gorgsenegger in https://github.com/hyperledger/aries-cloudagent-python/pull/1515
* Fix AttributeError by @gorgsenegger in https://github.com/hyperledger/aries-cloudagent-python/pull/1516
* Fix bug when getting credentials on askar-profile by @baegjae in https://github.com/hyperledger/aries-cloudagent-python/pull/1510
* added logging documentation by @chriamue in https://github.com/hyperledger/aries-cloudagent-python/pull/1519
* Multiple Indy Ledger support and State Proof verification by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1425
* OOB: Fixes issues with multiple public explicit invitation and unused 0160 connection by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1525
* Display QR code when generating/displaying invites on startup by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1526
* Fix error when removing a wallet on askar-profile by @baegjae in https://github.com/hyperledger/aries-cloudagent-python/pull/1518
* Fix DIF Presentation Request Input Validation by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1517
* Delete unused ConnRecord generated - OOB invitation  `(use_exising_connection)` by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1521
* added documentation for wallet storage databases by @chriamue in https://github.com/hyperledger/aries-cloudagent-python/pull/1523
* Implement Revocation Notification v1.0 by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1464
* Add Revocation notification support to alice/faber by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1527
* Fix integration tests (revocation notifications) by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1528
* Fix connection record response for mobile by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1469
* Enable WS Pings for WS Inbound Transport by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1530
* Outbound Queue - more usability improvements by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1501
* ConnRecord tags - `their_public_did` and `invitation_msg_id` by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1543
* Fix validation for range checks by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1538
* Remove required dependencies from multi-ledger code by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1550
* Update demo requirements by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1551
* PR#1543 Follow up - Adding invitation_msg_id and their_public_did back to record_value. by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1553
* Await asyncio.sleeps by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1558
* Updates to Changelog, RTD and version for the 0.7.3-RC0 release by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1535
* Add alias field to didexchange invitation UI by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1561
* Typo vdr service name by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1563
* chore: update pydid to ^0.3.3 by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1562
* Update docker scripts to use new & improved docker IP detection by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1565
* DiscoveryExchangeRecord RECORD_TOPIC typo fix by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1566
* Fix the inconsistency of invitation_msg_id between invitation and response by @baegjae in https://github.com/hyperledger/aries-cloudagent-python/pull/1564
* Multi ledger: IndyDID resolver bug fix by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1569
* fix: use invitation key for connection query by @TimoGlastra in https://github.com/hyperledger/aries-cloudagent-python/pull/1570
* Add fix for #1575 to allow OPTIONS method to work with x-api-key by @jcourt562 in https://github.com/hyperledger/aries-cloudagent-python/pull/1576
* OOB connection_reuse webhooks by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1581
* Multiple Indy Ledger - Askar Fixes and Cleanup by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1583
* ACA-Py Upgrade command implementation by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1557
* Fix for Test Harness --version issue by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1589
* Allow public invites for alice/faber demo by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1574
* Add credential_revoked state by @DaevMithran in https://github.com/hyperledger/aries-cloudagent-python/pull/1545
* Fixes for revocable credential issuance by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1591
* Updates for final Release 0.7.3 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1573

## New Contributors
* @gorgsenegger made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1494
* @chriamue made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1519

**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.7.2...0.7.3
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.7.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-01-10 21:34:04 +0000 UTC
    </span>
</div>

