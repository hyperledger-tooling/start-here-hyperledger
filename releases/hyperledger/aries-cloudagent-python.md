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
                    0.7.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.7.4
                </span>
            </td>
            <td>
                0.7.4 is a significant release focused on stability and production deployments. As the "patch" release number (0.7.3 to 0.7.4) indicates, there were no breaking changes in the Admin API, but a huge volume of updates and improvements.  Highlights of this release include:

- A major performance and stability improvement resulting from the now recommended use of [Aries Askar](https://github.com/bcgov/aries-askar) instead of the Indy-SDK.
- There are significant improvements and tools for dealing with revocation-related issues.
- A lot of work has been on the handling of Hyperledger Indy transaction endorsements.
- ACA-Py now has a pluggable persistent queues mechanism in place, with Redis and Kafka support available (albeit with work still to come on documentation).

In addition, there are a significant number of general enhancements, bug fixes, documentation updates and code management improvements.

This release is a reflection of the many groups stressing ACA-Py in production environments, reporting issues and the resulting solutions. We also have a very large number of contributors to ACA-Py, with this release having PRs from 22 different individuals. A big thank you to all of those using ACA-Py, raising issues and providing solutions.

More details about this release, including the major updates and a categorized list of PRs, can be found in the [Change Log file](https://github.com/hyperledger/aries-cloudagent-python/blob/main/CHANGELOG.md#074).

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
* Duplicate checking for schema and cred def by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1721
* Adds support to faber demo for returning json response in connectionless proof-requests by @amanji in https://github.com/hyperledger/aries-cloudagent-python/pull/1720
* Allow deletion of invalid V20PresExRecord - failing schema validation by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1718
* Use provided connection_id if provided by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1726
* feat: create new JWT tokens and invalidate older for multitenancy by @TimoGlastra in https://github.com/hyperledger/aries-cloudagent-python/pull/1725
* Allow specifying key derivation method on sub-wallet create by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1719
* feat: allow querying default mediator from base wallet by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1729
* Fix iteration over key list, update Askar to 0.2.5 by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1740
* Fixes logic for web hook formatter in Faber demo by @amanji in https://github.com/hyperledger/aries-cloudagent-python/pull/1739
* Documentation on existing language wrappers for aca-py by @etschelp in https://github.com/hyperledger/aries-cloudagent-python/pull/1738
* Updates to Changelog for 0.7.4. RC1 release by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1747
* Fixing the intro paragraph and heading in the changelog of this 0.7.4RC1 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1752
* 0.7.4-RC1 Changelog intro paragraph - fix copy/paste error by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1753
* Added async with for mediator record delete by @dejsenlitro in https://github.com/hyperledger/aries-cloudagent-python/pull/1749
* fix: Resolve Revocation Notification environment variable name collision by @frostyfrog in https://github.com/hyperledger/aries-cloudagent-python/pull/1751
* [#1745] Fetch from --genesis-url likely to fail in composed container… by @tdiesler in https://github.com/hyperledger/aries-cloudagent-python/pull/1746
* Redis PQ Cleanup by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1659
* Some ReadTheDocs File updates by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1770
* 0.7.4-rc2 update by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1771
* Adds `transport_id` variable assignment back to outbound enqueue method by @amanji in https://github.com/hyperledger/aries-cloudagent-python/pull/1776
* Replace async workaround within document loader by @frostyfrog in https://github.com/hyperledger/aries-cloudagent-python/pull/1774
* Feature: Add the ability to deny specific plugins from loading by @frostyfrog in https://github.com/hyperledger/aries-cloudagent-python/pull/1737
* Document impact of multi-ledger on TAA acceptance by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1778
* fix: add a close statement to ensure session is closed on error by @reflectivedevelopment in https://github.com/hyperledger/aries-cloudagent-python/pull/1777
* Fix tails server upload multi-ledger mode by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1785
* Feat/revocation notification v2 by @frostyfrog in https://github.com/hyperledger/aries-cloudagent-python/pull/1734
* feat: Add filter param to connection list for invitations by @frostyfrog in https://github.com/hyperledger/aries-cloudagent-python/pull/1797
* feat: support connectionless exchange by @TimoGlastra in https://github.com/hyperledger/aries-cloudagent-python/pull/1710
* Additional endpoints to get revocation details and fix "published" status by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1783
* Fix: Duplicated schema and cred_def - Askar and Postgres by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1800
* Fix: Inbound Transport is_external attribute by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1802
* Adjust revocation registry update procedure to shorten transactions by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1804
* Fix put_file when the server returns a redirect by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1808
* Fix missing webhook handler by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1816
* Changelog, version and ReadTheDocs updates for 0.7.4-rc3 release by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1817
* Fix IssuerCredRevRecord state update on revocation publish by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1827
* Fix: Present Proof v2 - check_proof_vs_proposal update to support proof request with restrictions by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1820
* Fix external Outbound Transport loading code by @frostyfrog in https://github.com/hyperledger/aries-cloudagent-python/pull/1812
* Prover - verification outcome from presentation ack message by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1757
* Fix: present-proof v1 send-proposal flow by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1811
* Add troubleshooting document, include initial examples - ledger connection, out-of-sync RevReg by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1818
* Update POST /present-proof/send-request to POST /present-proof-2.0/send-request by @lineko in https://github.com/hyperledger/aries-cloudagent-python/pull/1824
* Update pyjwt to 2.4 by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1829
* Update changelog and version for 0.7.4-rc4 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1830
* Enable pip-audit by @ryjones in https://github.com/hyperledger/aries-cloudagent-python/pull/1831
* Use local deps only by @ryjones in https://github.com/hyperledger/aries-cloudagent-python/pull/1834
* Multi-tenancy stale wallet clean up by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1692
* Improve typing of settings and add plugin settings object by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1833
* 0.7.4-rc5 changelog, version and ReadTheDocs updates by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1838
* Set prefix for integration test demo agents; some code cleanup by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1840
* Only run on main repo by @ryjones in https://github.com/hyperledger/aries-cloudagent-python/pull/1845
* Fix handling of non-revocable credential when timestamp is specified (askar/credx) by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1847
* Use default wallet type askar for alice/faber demo and bdd tests by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1761
* Fix a typo in DevReadMe.md by @feknall in https://github.com/hyperledger/aries-cloudagent-python/pull/1844
* Update the Supported RFCs document for 0.7.4 release by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1846
* 0.7.4 Release Changelog and version update by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1849

## New Contributors
* @frostyfrog made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1655
* @tdiesler made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1675
* @MonolithicMonk made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1706
* @mepeltier made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1694
* @rmnre made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1645
* @etschelp made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1738
* @reflectivedevelopment made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1777
* @lineko made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1824
* @feknall made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1844

**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.7.3...0.7.4
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.7.4" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-06-30 17:53:07 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    0.7.4-rc5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.7.4-rc5
                </span>
            </td>
            <td>
                **NOTE** We expect 0.7.4-rc5 will the be the last Release Candidate prior to the official 0.7.4 release.

**NOTE:** 0.7.4-rc4 contains a fix for a revocation-related issue introduced in 0.7.4-rc3. We recommend updating to 0.7.4-rc4 immediately if you have been using 0.7.4-rc3.

- See issue: [\#1823](https://github.com/hyperledger/aries-cloudagent-python/issues/1823)
- See Pull Request: [\#1827](https://github.com/hyperledger/aries-cloudagent-python/pull/1827)

The 0.7.4 release consists largely of internal fixes to ACA-Py, big increases in performance resulting from the now recommended use of [Aries Askar](https://github.com/bcgov/aries-askar) instead of the Indy-SDK, improvements and tools for dealing with revocation-related issues, plus a number of general enhancements. There have been a lot of groups exercising ACA-Py and the updates made in this release are a reflection of those efforts. We have PRs that have been contributed by 21 different people.

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
* Duplicate checking for schema and cred def by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1721
* Adds support to faber demo for returning json response in connectionless proof-requests by @amanji in https://github.com/hyperledger/aries-cloudagent-python/pull/1720
* Allow deletion of invalid V20PresExRecord - failing schema validation by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1718
* Use provided connection_id if provided by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1726
* feat: create new JWT tokens and invalidate older for multitenancy by @TimoGlastra in https://github.com/hyperledger/aries-cloudagent-python/pull/1725
* Allow specifying key derivation method on sub-wallet create by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1719
* feat: allow querying default mediator from base wallet by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1729
* Fix iteration over key list, update Askar to 0.2.5 by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1740
* Fixes logic for web hook formatter in Faber demo by @amanji in https://github.com/hyperledger/aries-cloudagent-python/pull/1739
* Documentation on existing language wrappers for aca-py by @etschelp in https://github.com/hyperledger/aries-cloudagent-python/pull/1738
* Updates to Changelog for 0.7.4. RC1 release by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1747
* Fixing the intro paragraph and heading in the changelog of this 0.7.4RC1 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1752
* 0.7.4-RC1 Changelog intro paragraph - fix copy/paste error by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1753
* Added async with for mediator record delete by @dejsenlitro in https://github.com/hyperledger/aries-cloudagent-python/pull/1749
* fix: Resolve Revocation Notification environment variable name collision by @frostyfrog in https://github.com/hyperledger/aries-cloudagent-python/pull/1751
* [#1745] Fetch from --genesis-url likely to fail in composed container… by @tdiesler in https://github.com/hyperledger/aries-cloudagent-python/pull/1746
* Redis PQ Cleanup by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1659
* Some ReadTheDocs File updates by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1770
* 0.7.4-rc2 update by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1771
* Adds `transport_id` variable assignment back to outbound enqueue method by @amanji in https://github.com/hyperledger/aries-cloudagent-python/pull/1776
* Replace async workaround within document loader by @frostyfrog in https://github.com/hyperledger/aries-cloudagent-python/pull/1774
* Feature: Add the ability to deny specific plugins from loading by @frostyfrog in https://github.com/hyperledger/aries-cloudagent-python/pull/1737
* Document impact of multi-ledger on TAA acceptance by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1778
* fix: add a close statement to ensure session is closed on error by @reflectivedevelopment in https://github.com/hyperledger/aries-cloudagent-python/pull/1777
* Fix tails server upload multi-ledger mode by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1785
* Feat/revocation notification v2 by @frostyfrog in https://github.com/hyperledger/aries-cloudagent-python/pull/1734
* feat: Add filter param to connection list for invitations by @frostyfrog in https://github.com/hyperledger/aries-cloudagent-python/pull/1797
* feat: support connectionless exchange by @TimoGlastra in https://github.com/hyperledger/aries-cloudagent-python/pull/1710
* Additional endpoints to get revocation details and fix "published" status by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1783
* Fix: Duplicated schema and cred_def - Askar and Postgres by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1800
* Fix: Inbound Transport is_external attribute by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1802
* Adjust revocation registry update procedure to shorten transactions by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1804
* Fix put_file when the server returns a redirect by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1808
* Fix missing webhook handler by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1816
* Changelog, version and ReadTheDocs updates for 0.7.4-rc3 release by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1817
* Fix IssuerCredRevRecord state update on revocation publish by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1827
* Fix: Present Proof v2 - check_proof_vs_proposal update to support proof request with restrictions by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1820
* Fix external Outbound Transport loading code by @frostyfrog in https://github.com/hyperledger/aries-cloudagent-python/pull/1812
* Prover - verification outcome from presentation ack message by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1757
* Fix: present-proof v1 send-proposal flow by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1811
* Add troubleshooting document, include initial examples - ledger connection, out-of-sync RevReg by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1818
* Update POST /present-proof/send-request to POST /present-proof-2.0/send-request by @lineko in https://github.com/hyperledger/aries-cloudagent-python/pull/1824
* Update pyjwt to 2.4 by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1829
* Update changelog and version for 0.7.4-rc4 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1830
* Enable pip-audit by @ryjones in https://github.com/hyperledger/aries-cloudagent-python/pull/1831
* Use local deps only by @ryjones in https://github.com/hyperledger/aries-cloudagent-python/pull/1834
* Multi-tenancy stale wallet clean up by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1692
* Improve typing of settings and add plugin settings object by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1833
* 0.7.4-rc5 changelog, version and ReadTheDocs updates by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1838

## New Contributors
* @frostyfrog made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1655
* @tdiesler made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1675
* @MonolithicMonk made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1706
* @mepeltier made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1694
* @rmnre made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1645
* @etschelp made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1738
* @reflectivedevelopment made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1777
* @lineko made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1824

**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.7.3...0.7.4-rc5
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.7.4-rc5" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-06-24 00:12:02 +0000 UTC
    </span>
</div>

