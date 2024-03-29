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
                    0.12.0rc2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.12.0rc2
                </span>
            </td>
            <td>
                Release 0.12.0 is a relative large release but currently with no breaking changes. We expect there will be breaking changes (at least in the handling of endorsement) before the 0.12.0 release is finalized, hence the minor version update.

The `rc0` release candidate introduced a regression via [PR \#2705] that has been reverted in `rc1` and later via [PR \#2789]. Further investigation is needed to determine how to accomplish the goal of [PR \#2705] ("feat: inject profile") without the regression. The `rc2` and later releases address a regression related to the sending of a revocation notification from the issuer to the holder of a newly revoked credential, fixed in [PR \#2814].

[PR \#2814]: https://github.com/hyperledger/aries-cloudagent-python/pull/2705
[PR \#2705]: https://github.com/hyperledger/aries-cloudagent-python/pull/2705
[PR \#2789]: https://github.com/hyperledger/aries-cloudagent-python/pull/2789

Much progress has been made on `did:peer` support in this release, with the handling of inbound [DID Peer] 1 added, and inbound and outbound support for DID Peer 2 and 4. The goal of that work is to eliminate the remaining places where "unqualified" DIDs remain, and to enable the "connection reuse" in the Out of Band protocol when using DID Peer 2 and 4 DIDs. Work continues in supporting ledger agnostic [AnonCreds], and the new [Hyperledger AnonCreds Rust] library. Attention was also given in the release to the handling of JSON-LD [Data Integrity Verifiable Credentials], with more expected before the release is finalized. In addition to those updates, there were fixes and improvements across the codebase.

The most visible change in this release is the re-organization of the ACA-Py documentation, moving the vast majority of the documents to the folders within the `docs` folder -- a long overdue change that will allow us to soon publish the documents on [https://aca-py.org](https://aca-py.org) directly from the ACA-Py repository, rather than from the separate [aries-acapy-docs](https://github.com/hyperledger/aries-acapy-docs) currently being used.

A big developer improvement is a revamping of the test handling to eliminate ~2500 warnings that were previously generated in the test suite.  Nice job [@ff137](https://github.com/ff137)!

[DID Peer]: https://identity.foundation/peer-did-method-spec/
[AnonCreds]: https://www.hyperledger.org/projects/anoncreds
[Hyperledger AnonCreds Rust]: https://github.com/hyperledger/anoncreds-rs
[Data Integrity Verifiable Credentials]: https://www.w3.org/TR/vc-data-integrity/

### 0.12.0rc2 Breaking Changes

There are no breaking changes in 0.12.0rc2.

## What's Changed
* Initial code migration from anoncreds-rs branch by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2596
* Bump aiohttp from 3.8.6 to 3.9.0 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2635
* Feature Suggestion: Include a Reason When Constraints Cannot Be Applied by @Ennovate-com in https://github.com/hyperledger/aries-cloudagent-python/pull/2630
* Fix: RevRegEntry Transaction Endorsement by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/2558
* fix: update broken demo dependency by @mrkaurelius in https://github.com/hyperledger/aries-cloudagent-python/pull/2638
* Bump cryptography from 41.0.5 to 41.0.6 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2636
* Integrate Anoncreds rs into credential and presentation endpoints by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2632
* Initial migration of anoncreds revocation code by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2643
* feat: add did:jwk resolver by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2645
* Feat: DIDX Implicit Request auto-accept and Delete OOB Invitation related records by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/2642
* Add ConnectionProblemReport handler by @usingtechnology in https://github.com/hyperledger/aries-cloudagent-python/pull/2600
* Update integration tests for anoncreds-rs by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2651
* Connection and DIDX Problem Reports by @usingtechnology in https://github.com/hyperledger/aries-cloudagent-python/pull/2653
* feat: support resolving did:peer:1 received in did exchange by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2611
* Slight improvement to credx proof validation error message by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2655
* Update snyk workflow to execute on Pull Request by @usingtechnology in https://github.com/hyperledger/aries-cloudagent-python/pull/2658
* refactor: make ldp_vc logic reusable by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2533
* Additional anoncreds integration tests by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2660
* Tweak scope of GHA integration tests by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2662
* fix: link to raw content change from master to main by @Ennovate-com in https://github.com/hyperledger/aries-cloudagent-python/pull/2663
* Ensure "preserve_exchange_records" flags are set. by @usingtechnology in https://github.com/hyperledger/aries-cloudagent-python/pull/2664
* fix: open-api generator script by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2661
* Anoncreds - Add unit testing by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2672
* Fix: Change To Use Timezone Aware UTC datetime by @Ennovate-com in https://github.com/hyperledger/aries-cloudagent-python/pull/2679
* Cache TAA by wallet name by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2676
* Improve Per Tenant Logging: Fix issues around default log file path by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/2659
* Return 404 when schema not found by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2683
* Update dependencies by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/2686
* Add unit tests for anoncreds revocation by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2688
* chore(deps): Bump jwcrypto from 1.5.0 to 1.5.1 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2689
* Emit did:peer:2 for didexchange by @Jsyro in https://github.com/hyperledger/aries-cloudagent-python/pull/2687
* did peer 4 resolution by @Jsyro in https://github.com/hyperledger/aries-cloudagent-python/pull/2692
* Remove if condition which checks if the `credential.type` array is equal to 1 by @PatStLouis in https://github.com/hyperledger/aries-cloudagent-python/pull/2670
* Improve api documentation and error handling by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2690
* Add did web method type as a default option by @PatStLouis in https://github.com/hyperledger/aries-cloudagent-python/pull/2684
* fix: update constants in TransactionRecord by @amanji in https://github.com/hyperledger/aries-cloudagent-python/pull/2698
* Remove tiny-vim from being added to the container image to reduce reported vulnerabilities from scanning by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2699
* fix: save multi_use to the DB for OOB invitations by @frostyfrog in https://github.com/hyperledger/aries-cloudagent-python/pull/2694
* Update legacy bcgovimages references. by @WadeBarnes in https://github.com/hyperledger/aries-cloudagent-python/pull/2700
* Feature/emit did peer 4 by @Jsyro in https://github.com/hyperledger/aries-cloudagent-python/pull/2696
* feat: inject profile by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2705
* chore(deps): Bump jinja2 from 3.1.2 to 3.1.3 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2707
* feat: make VcLdpManager pluggable by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2706
* Update RTD requirements after security vulnerability recorded by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2712
* fix: minor type hint corrections for VcLdpManager by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2704
* Integration test for did:peer by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2713
* Fix subwallet record removal by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/2721
* Remove exception on connectionless presentation problem report handler by @loneil in https://github.com/hyperledger/aries-cloudagent-python/pull/2723
* Fix incorrect Sphinx search library version reference by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2716
* Update the SupportedRFCs Document to be up to date by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2722
* Upgrade anoncreds to 0.2.0.dev7 by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2719
* Update devcontainer documentation by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2729
* 0.12.0rc0 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2732
* docs: create design doc for adding W3C VC format support by @tra371 in https://github.com/hyperledger/aries-cloudagent-python/pull/2674
* Upgrade anoncred-rs to version 0.2.0-dev8 by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2734
* bump pydid to v 0.4.3 by @PatStLouis in https://github.com/hyperledger/aries-cloudagent-python/pull/2737
* Enable presentation issuance/verification through vc-api endpoints by @PatStLouis in https://github.com/hyperledger/aries-cloudagent-python/pull/2710
* Upgrade anoncreds to 0.2.0-dev9 by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2741
* Relax validation of holder DID when submitting a credential request by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2731
* chore(deps): Bump aiohttp from 3.9.1 to 3.9.2 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2745
* chore: pin black version by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2747
* Breaking - remove endorser capability to write ledger transactions by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2720
* Update BBS+ context to bypass redirections by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2739
* Anoncreds schema endorsement by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2715
* Fix pytest collection errors when anoncreds package is not installed by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/2750
* Add cached copy of BBS v1 context by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/2749
* Remove asynctest dependency and fix "coroutine not awaited" warnings by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2755
* Update anoncreds to 0.2.0-dev10 by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2758
* Upgrade anoncreds to version 0.2.0-dev11 by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2763
* Move emit events to profile and delay sending until after commit by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2760
* ⬆️ Update pytest-asyncio to 0.23.4  by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2764
* Reorganize the ACA-Py Documentation Files by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2765
* Anoncreds - Cred Def and Revocation Endorsement by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2752
* Tweaks to MD files to enable aca-py.org publishing by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2771
* Implement B006 rule by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2775
* :arrow_up: Upgrade pytest to 8.0 by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2773
* fix: partial revert of ConnRecord schema change by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2746
* Add Dependabot configuration by @WadeBarnes in https://github.com/hyperledger/aries-cloudagent-python/pull/2783
* chore(deps): Bump the all-actions group with 10 updates by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2784
* Anoncreds revoke and publish-revocations endorsement by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2782
* Demo description of reuse in establishing a connection by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2787
* Revert profile inject by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2789
* Revert profile injection for VcLdpManager on vc-api endpoints by @PatStLouis in https://github.com/hyperledger/aries-cloudagent-python/pull/2794
* feature/per tenant settings by @amanji in https://github.com/hyperledger/aries-cloudagent-python/pull/2790
* Add known issues section to Multiledger.md documentation by @esune in https://github.com/hyperledger/aries-cloudagent-python/pull/2788
* Bump pyld version to 2.0.4 by @PatStLouis in https://github.com/hyperledger/aries-cloudagent-python/pull/2795
* Fix deprecation warnings by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2756
* Change middleware registration order by @PatStLouis in https://github.com/hyperledger/aries-cloudagent-python/pull/2796
* 0.12.0rc1 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2799
* 0.12.0rc1-tweak by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2800
* Author subwallet setup automation by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2791
* Add anoncreds multitenant endorsement integration tests by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2801
* Get and create anoncreds profile when using anoncreds subwallet by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2803
* Update publish-docs to operate on main and on branches prefixed with docs-v by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2804
* Publish docs GHActions tweak by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2806
* More updates to get docs publishing by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2810
* Eliminate the double workflow event by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2811
* Create revocation notification after list entry written to ledger by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2812
* Fix anoncreds non-endorsement revocation by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2814
* chore(deps): Bump the all-actions group with 3 updates by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2815
* Allow for crids in event payload to be integers by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2819
* FIX: GHA update for doc publishing, fix doc file that was blanked by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2820
* Send revocation list instead of rev_list object - Anoncreds by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2821
* chore(deps): Bump cryptography from 42.0.3 to 42.0.4 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2805
* 0.12.0rc2 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2825

## New Contributors
* @mrkaurelius made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2638
* @jamshale made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2672
* @PatStLouis made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2670
* @tra371 made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2674

**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.11.0...0.12.0rc2
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.12.0rc2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-03-06 03:11:12 +0000 UTC
    </span>
</div>

