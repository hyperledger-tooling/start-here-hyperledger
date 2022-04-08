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
                    0.7.4-rc0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.7.4-rc0
                </span>
            </td>
            <td>
                This release consists largely of internal fixes with a few minor enhancements. There has been a lot of groups exercising ACA-Py and the updates made in this release are a reflection of those efforts. We have PRs that have been contributed by 16 different people, which is very likely a record for a single ACA-Py release.

For more context of the changes in this release, please see the [CHANGELOG.md](https://github.com/hyperledger/aries-cloudagent-python/blob/0.7.4-rc0/CHANGELOG.md) file. Below is a generated list of the PRs.

## What's Changed
* Doh....update the date in the Changelog for 0.7.3 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1592
* Added missed new module -- upgrade -- to the RTD generated docs by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1593
* Update aries-askar patch version to at least 0.2.4 as 0.2.3 does not include backward compatibility by @acuderman in https://github.com/hyperledger/aries-cloudagent-python/pull/1603
* Replace blank credential/presentation exchange states with abandoned state by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1605
* DID updates for endorser by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1601
* Update aiohttp dependency by @acuderman in https://github.com/hyperledger/aries-cloudagent-python/pull/1606
* style: format with stable black release by @TimoGlastra in https://github.com/hyperledger/aries-cloudagent-python/pull/1615
* feat: enable webhook events for mediation records by @TimoGlastra in https://github.com/hyperledger/aries-cloudagent-python/pull/1614
* Auto-promote author did to public after endorsing by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1607
* Upgrade ConfigArgParse to version 1.5.3 by @WadeBarnes in https://github.com/hyperledger/aries-cloudagent-python/pull/1627
* Fix for non-revoc proof with no timestamp by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1628
* Move database operations inside the session context by @acuderman in https://github.com/hyperledger/aries-cloudagent-python/pull/1633
* feat: query connections by their_public_did by @TimoGlastra in https://github.com/hyperledger/aries-cloudagent-python/pull/1637
* Fix auto connection response not being properly mediated by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1638
* Pin markupsafe at version 2.0.1 by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1642
* feat: accept taa using startup parameter --accept-taa by @TimoGlastra in https://github.com/hyperledger/aries-cloudagent-python/pull/1643
* Update Endorser documentation by @chumbert in https://github.com/hyperledger/aries-cloudagent-python/pull/1646
* Performance demo updates by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1647
* Fixes and cleanups for issue-credential 1.0 by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1619
* Fix usage of send_credential_ack by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1653
* Add cred_def_id to metadata when using an Endorser by @frostyfrog in https://github.com/hyperledger/aries-cloudagent-python/pull/1655
* docs: supported features attribution by @TimoGlastra in https://github.com/hyperledger/aries-cloudagent-python/pull/1654
* Revert change to send_credential_ack return value by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1660
* Add "sent" key to both Schema and Cred Defs when using Endorsers by @frostyfrog in https://github.com/hyperledger/aries-cloudagent-python/pull/1663
* fix: always notify if revocation notification record exists by @TimoGlastra in https://github.com/hyperledger/aries-cloudagent-python/pull/1665
* Fixes for credential details in issue-credential webhook responses by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1668
* Qualify did exch connection lookup by role by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1670
* Add pre-commit as optional developer tool by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1671
* [#1674] Add basic DOCKER_ENV logging for run_demo by @tdiesler in https://github.com/hyperledger/aries-cloudagent-python/pull/1675
* Remove references to play with von by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1688
* Endorser support for updating DID endpoints on ledger by @frostyfrog in https://github.com/hyperledger/aries-cloudagent-python/pull/1696
* platform target in run tests. by @burdettadam in https://github.com/hyperledger/aries-cloudagent-python/pull/1697
* Fix DIF PresExch and OOB request_attach delete unused connection by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1676
* Fix: DIF proof proposal when creating bound presentation request [Issue#1687] by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1690
* Add auto_verify flag in present-proof protocol by @DaevMithran in https://github.com/hyperledger/aries-cloudagent-python/pull/1702
* Fix: update IndyLedgerRequestsExecutor logic - multitenancy and basic base wallet type  by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1700
* Allow use of SEED when creating local wallet DID Issue-1682 by @DaevMithran in https://github.com/hyperledger/aries-cloudagent-python/pull/1705
* Add an integration test for mixed proof with a revocable cred and a n… by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1672
* Multitenancy Docs Update by @MonolithicMonk in https://github.com/hyperledger/aries-cloudagent-python/pull/1706
* Feature/undelivered events by @mepeltier in https://github.com/hyperledger/aries-cloudagent-python/pull/1694
* Fix: present-proof v2 send-proposal [issue#1474] by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1667
* run_docker start - pass environment variables by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1715
* Fix DIFPresFormatHandler returning invalid V20PresExRecord on presentation verification by @rmnre in https://github.com/hyperledger/aries-cloudagent-python/pull/1645
* Fixes for v7.3.0 - Issue#1597 by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1711
* Fix order of operations connecting faber to endorser by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1716
* did-exchange implicit request pthid update & invitation key verification by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1599
* Prep for adding the 0.7.4-rc0 tag by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1722

## New Contributors
* @frostyfrog made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1655
* @tdiesler made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1675
* @MonolithicMonk made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1706
* @mepeltier made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1694
* @rmnre made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1645

**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.7.3...0.7.4-rc0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.7.4-rc0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-04-07 20:28:06 +0000 UTC
    </span>
</div>

