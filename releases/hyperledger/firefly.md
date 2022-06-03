---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v1.1.0-alpha.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.1.0-alpha.1
                </span>
            </td>
            <td>
                ## What's Changed
* Clean up API spec for token approvals by @awrichar in https://github.com/hyperledger/firefly/pull/775
* Add first step of FireFly Transaction Manager support - separate URL for submit by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/751
* Fix bugs with token approvals by @awrichar in https://github.com/hyperledger/firefly/pull/778
* [ui-v1.0.1] manifest by @eberger727 in https://github.com/hyperledger/firefly/pull/776
* Update manifest.json by @nguyer in https://github.com/hyperledger/firefly/pull/781
* Token transfer/approval protocolId should be unique for each connector by @awrichar in https://github.com/hyperledger/firefly/pull/780
* Default for token approvals should be "approved: true" by @awrichar in https://github.com/hyperledger/firefly/pull/782
* update cobra short and long descriptions by @shorsher in https://github.com/hyperledger/firefly/pull/785
* update init logging branding by @shorsher in https://github.com/hyperledger/firefly/pull/786
* Remove non-definition items from DefinitionHandler by @awrichar in https://github.com/hyperledger/firefly/pull/789
* Update Tokens Tutorials by @nguyer in https://github.com/hyperledger/firefly/pull/777
* Refactor to move common utility code out to firefly-common by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/791
* Fix links in documentation by @teaglebuilt in https://github.com/hyperledger/firefly/pull/793
* Allow namespace to be omitted from URLs by @awrichar in https://github.com/hyperledger/firefly/pull/792
* Do not init apiserver config, until after config reset by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/794
* Remove old ERC21/ERC721 contracts (no longer used by test) by @awrichar in https://github.com/hyperledger/firefly/pull/797
* sync core with firefly-common by @shorsher in https://github.com/hyperledger/firefly/pull/805
* De-duplicate existing token approvals in database migration by @awrichar in https://github.com/hyperledger/firefly/pull/810
* Message "state" should be read-only by @awrichar in https://github.com/hyperledger/firefly/pull/801
* Add reference docs generation for types by @nguyer in https://github.com/hyperledger/firefly/pull/811
* Define config schema for namespaces.predefined by @awrichar in https://github.com/hyperledger/firefly/pull/798
* Remove unused parameters from blockchain plugin interface by @awrichar in https://github.com/hyperledger/firefly/pull/819
* Include component name when initialization fails by @awrichar in https://github.com/hyperledger/firefly/pull/824
* Add new Docker tags for release channels by @nguyer in https://github.com/hyperledger/firefly/pull/815
* Add language tag to FFM, FFE, FFC, etc by @nguyer in https://github.com/hyperledger/firefly/pull/818
* Address coverage gap for "Capabilities" method by @awrichar in https://github.com/hyperledger/firefly/pull/825
* Docs internationalization by @nguyer in https://github.com/hyperledger/firefly/pull/822
* Move plugin configuration under `plugins` section by @shorsher in https://github.com/hyperledger/firefly/pull/821
* Factor out Namespace Manager by @awrichar in https://github.com/hyperledger/firefly/pull/826
* Possible to see clash on port 6000 for metrics server by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/829
* Additional type docs by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/816
* Adde custom onchain logic docs for Fabric plus refactoring by @jimthematrix in https://github.com/hyperledger/firefly/pull/784
* Fix link to events reference by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/831
* Add version support to docs site by @nguyer in https://github.com/hyperledger/firefly/pull/830
* Fix relative links in reference descriptions docs by @nguyer in https://github.com/hyperledger/firefly/pull/832
* Namespace config validation by @shorsher in https://github.com/hyperledger/firefly/pull/833
* Disable external link checking when building docs, due to unreliable external servers by @nguyer in https://github.com/hyperledger/firefly/pull/839
* Support migration of the FireFly contract from one location to another by @awrichar in https://github.com/hyperledger/firefly/pull/820
* fabconnect async calls + setting broadcast/private message header types by @shorsher in https://github.com/hyperledger/firefly/pull/841
* Update README with missing links, and bit of a restructure by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/835
* Allow extra options to pass through to blockchain connectors by @nguyer in https://github.com/hyperledger/firefly/pull/844
* Verify namespace for all broadcast/private message requests by @awrichar in https://github.com/hyperledger/firefly/pull/843
* Update dependency versions by @nguyer in https://github.com/hyperledger/firefly/pull/845
* Move all identity APIs under /namespaces by @awrichar in https://github.com/hyperledger/firefly/pull/804
* Enhancements to migration/network version behavior by @awrichar in https://github.com/hyperledger/firefly/pull/849

## New Contributors
* @teaglebuilt made their first contribution in https://github.com/hyperledger/firefly/pull/793

**Full Changelog**: https://github.com/hyperledger/firefly/compare/v1.0.0...v1.1.0-alpha.1
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly/releases/tag/v1.1.0-alpha.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-06-02 18:27:33 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v1.0.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.0.2
                </span>
            </td>
            <td>
                ## Summary
Fix invocations on custom Fabric chaincode, which were not properly reporting success/failure status back to FireFly (along with other minor bugfixes).

## What's Changed
* De-duplicate existing token approvals in database migration by @awrichar in https://github.com/hyperledger/firefly/pull/809
* Backport docs generation and versioning code for 1.0 stream by @nguyer in https://github.com/hyperledger/firefly/pull/834
* default fabconnect calls to async by @shorsher in https://github.com/hyperledger/firefly/pull/836
* set message header type for broadcast/private by @shorsher in https://github.com/hyperledger/firefly/pull/838


**Full Changelog**: https://github.com/hyperledger/firefly/compare/v1.0.1...v1.0.2
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly/releases/tag/v1.0.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-05-27 20:53:30 +0000 UTC
    </span>
</div>

