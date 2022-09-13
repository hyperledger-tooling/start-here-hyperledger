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
                    v1.1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.1.0
                </span>
            </td>
            <td>
                ## Migration from v1.0

Please see the detailed [Migration Guide](https://github.com/hyperledger/firefly/wiki/Migration-Guide-for-v1.1.0) in the Wiki.

## Highlights

### [Read the release blog here](https://www.hyperledger.org/blog/2022/09/12/hyperledger-firefly-v1-1-is-now-available)

![Intro to FireFly v1](https://user-images.githubusercontent.com/6660217/189673243-6547ecc9-e76d-4f8b-9cfb-a3535dc70c12.png)

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
* Use API framework newly moved to cmomon with extension points by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/851
* Return definition rejection reasons as errors by @awrichar in https://github.com/hyperledger/firefly/pull/813
* Move /admin/api to /spi and PUT->PATCH by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/842
* Restore FireFly contract version, update UI version by @awrichar in https://github.com/hyperledger/firefly/pull/853
* Fix github.ref in prereleased action by @nguyer in https://github.com/hyperledger/firefly/pull/852
* Update README.md by @viswatejagajulavarthy in https://github.com/hyperledger/firefly/pull/854
* Add namespace to pins by @awrichar in https://github.com/hyperledger/firefly/pull/856
* Remove redundant payloadRef field on Batch Pin by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/858
* Use firefly-signer library and allow numbers expressed as strings by @nguyer in https://github.com/hyperledger/firefly/pull/837
* Use a separate orchestrator for each namespace by @awrichar in https://github.com/hyperledger/firefly/pull/855
* Push namespace info to token connector, handle batch events by @awrichar in https://github.com/hyperledger/firefly/pull/861
* Remove namespace from identity manager, network map, and group manager calls by @awrichar in https://github.com/hyperledger/firefly/pull/862
* Further cleanup of namespace params to managers and database plugin by @awrichar in https://github.com/hyperledger/firefly/pull/864
* Update token connector versions by @awrichar in https://github.com/hyperledger/firefly/pull/867
* Remove unneeded BatchManager references by @awrichar in https://github.com/hyperledger/firefly/pull/850
* Update builder to go 1.17 and docs by @nguyer in https://github.com/hyperledger/firefly/pull/868
* Updating Create Listener Docs to Use eventPath by @hfuss in https://github.com/hyperledger/firefly/pull/860
* Move event plugin init to namespace manager by @awrichar in https://github.com/hyperledger/firefly/pull/863
* Resolve DX operations via requestID (not event ID) by @awrichar in https://github.com/hyperledger/firefly/pull/872
* Create firefly contract subscription per namespace by @shorsher in https://github.com/hyperledger/firefly/pull/865
* Remove namespace param from remaining manager calls by @awrichar in https://github.com/hyperledger/firefly/pull/875
* Add shorsher as a code owner by @awrichar in https://github.com/hyperledger/firefly/pull/869
* Handle namespace validation at the route level rather than at data manager by @awrichar in https://github.com/hyperledger/firefly/pull/876
* Remove "namespace" as a query param from all routes by @awrichar in https://github.com/hyperledger/firefly/pull/877
* Convert more callback handlers to be namespace-specific by @awrichar in https://github.com/hyperledger/firefly/pull/874
* Collapse batchpin.Submitter into multiparty.Manager by @awrichar in https://github.com/hyperledger/firefly/pull/880
* Move SubmitNetworkAction and RootOrg config to Multiparty Manager by @awrichar in https://github.com/hyperledger/firefly/pull/881
* surface URI as parameter for token mint by @shorsher in https://github.com/hyperledger/firefly/pull/879
* Enable non-multiparty namespaces by @awrichar in https://github.com/hyperledger/firefly/pull/878
* Track blockchain callback handlers per namespace by @awrichar in https://github.com/hyperledger/firefly/pull/883
* FAQ and FireFly Tutorial Updates by @trevorsc19 in https://github.com/hyperledger/firefly/pull/857
* Move FFI/ABI conversion code to signer and common by @nguyer in https://github.com/hyperledger/firefly/pull/866
* Add E2E tests for gateway mode by @nguyer in https://github.com/hyperledger/firefly/pull/887
* Add sqlite to Docker image by @awrichar in https://github.com/hyperledger/firefly/pull/893
* Fix logs from E2E test invocation by @awrichar in https://github.com/hyperledger/firefly/pull/892
* Custom contract subscriptions now utilize namespaces by @shorsher in https://github.com/hyperledger/firefly/pull/891
* Add basic auth support by @nguyer in https://github.com/hyperledger/firefly/pull/894
* Only start each plugin once by @awrichar in https://github.com/hyperledger/firefly/pull/901
* Support tokens only namespaces by @shorsher in https://github.com/hyperledger/firefly/pull/896
* Map namespace between local name and remote name by @awrichar in https://github.com/hyperledger/firefly/pull/895
* Change default contracts to network version 2 by @awrichar in https://github.com/hyperledger/firefly/pull/890
* Stop orchestrator for ff_system when moving to network V2 by @awrichar in https://github.com/hyperledger/firefly/pull/884
* Commonize blockchain code by @shorsher in https://github.com/hyperledger/firefly/pull/902
* E2E suite cleanup by @awrichar in https://github.com/hyperledger/firefly/pull/904
* Tokens plugins now support a remote name by @shorsher in https://github.com/hyperledger/firefly/pull/900
* Strip down namespace object and clean up APIs by @awrichar in https://github.com/hyperledger/firefly/pull/898
* added documentation for connecting firefly to a remote fabric chaincode by @satoshi-u in https://github.com/hyperledger/firefly/pull/908
* remove namespace from `sender_contracts` by @shorsher in https://github.com/hyperledger/firefly/pull/903
* Build Docker once to share with all E2E jobs by @awrichar in https://github.com/hyperledger/firefly/pull/909
* Add E2E tests for contract termination by @awrichar in https://github.com/hyperledger/firefly/pull/899
* Small Docker build enhancements by @awrichar in https://github.com/hyperledger/firefly/pull/910
* Properly handle remote->local namespace mapping in blockchain plugin by @awrichar in https://github.com/hyperledger/firefly/pull/911
* Update UI version by @awrichar in https://github.com/hyperledger/firefly/pull/912
* Fix test coverage gaps in operations manager by @awrichar in https://github.com/hyperledger/firefly/pull/914
* Use "poolData" instead of "namespace" in fftokens by @awrichar in https://github.com/hyperledger/firefly/pull/913
* Allow multiple copies of things on different namespaces by @awrichar in https://github.com/hyperledger/firefly/pull/915
* Add admin and config fields to E2E testState by @awrichar in https://github.com/hyperledger/firefly/pull/917
* E2E test for tokens only namespaces by @shorsher in https://github.com/hyperledger/firefly/pull/919
* Fixes Incorrect Route in the `broadcast_data`Tutorial by @JeffNeff in https://github.com/hyperledger/firefly/pull/922
* Add the V1 migration test to integration runs by @awrichar in https://github.com/hyperledger/firefly/pull/921
* Add node-specific suffix to DX endpoint "id" by @awrichar in https://github.com/hyperledger/firefly/pull/916
* Pin golangci-lint to v1.47.3 instead of latest by @awrichar in https://github.com/hyperledger/firefly/pull/932
* Add multi-tenancy E2E test by @awrichar in https://github.com/hyperledger/firefly/pull/918
* super small typo by @sebgoa in https://github.com/hyperledger/firefly/pull/924
* add E2E test for token plugins with remote names by @shorsher in https://github.com/hyperledger/firefly/pull/920
* Minor cleanup of namespace comments/struct descriptions by @awrichar in https://github.com/hyperledger/firefly/pull/927
* Updates for EVMConnect support (with EthConnect cross-compatibility) by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/923
* Wait up to 1000ms to lock sqlite database by @awrichar in https://github.com/hyperledger/firefly/pull/928
* Update .gitignore: ignoring .idea path by @kmilodenisglez in https://github.com/hyperledger/firefly/pull/937
* Fix bugs with Operations (and other minor fixes) by @awrichar in https://github.com/hyperledger/firefly/pull/935
* Update Viper to support camelCase nested keys by @awrichar in https://github.com/hyperledger/firefly/pull/930
* Remove unneeded sleep from txcommon test by @awrichar in https://github.com/hyperledger/firefly/pull/945
* update integration test to use new e2e suites by @shorsher in https://github.com/hyperledger/firefly/pull/938
* Add deprecation warning for old node config by @awrichar in https://github.com/hyperledger/firefly/pull/946
* fixing the example firefly core command by @Chengxuan in https://github.com/hyperledger/firefly/pull/950
* Distinguish "message not available" from "message missing data" by @awrichar in https://github.com/hyperledger/firefly/pull/953
* Advertise full node name (with suffix) to DX by @awrichar in https://github.com/hyperledger/firefly/pull/942
* Properly match operation updates to the plugin that generated them by @awrichar in https://github.com/hyperledger/firefly/pull/955
* Add BLOCKCHAIN_CONNECTOR env var and add evmconnect to manifest by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/949
* Store full details of EVMConnect/EthConnect updates for Token ops by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/948
* Destroy sysmessaging package 💥 by @awrichar in https://github.com/hyperledger/firefly/pull/926
* Changes to support E2E tests with confirmations, where requests might be slow by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/960
* Update to latest dependencies ready for V1.1 alpha.3 by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/963
* bump ui to 1.1 alpha 3 by @shorsher in https://github.com/hyperledger/firefly/pull/965
* Performance improvements for batch lookups by @awrichar in https://github.com/hyperledger/firefly/pull/967
* Messages that fail validation should be rejected by @awrichar in https://github.com/hyperledger/firefly/pull/956
* Update to firefly-signer v0.9.13 by @nguyer in https://github.com/hyperledger/firefly/pull/969
* Update to firefly-signer v0.9.15 by @nguyer in https://github.com/hyperledger/firefly/pull/970
* Fix group race condition, optimize transaction cache by @awrichar in https://github.com/hyperledger/firefly/pull/971
* fix integration matrix `exclude` by @shorsher in https://github.com/hyperledger/firefly/pull/973
* Add cache for operations by @awrichar in https://github.com/hyperledger/firefly/pull/972
* Adjust defaults for all cache items that don't expose a Size by @awrichar in https://github.com/hyperledger/firefly/pull/975
* Only query operations from the database if there were cache misses by @awrichar in https://github.com/hyperledger/firefly/pull/976
* Leverage transaction cache in a few more places by @awrichar in https://github.com/hyperledger/firefly/pull/974
* Use optimistic inserts for blockchain events by @awrichar in https://github.com/hyperledger/firefly/pull/977
* Create config migration script by @awrichar in https://github.com/hyperledger/firefly/pull/934
* Add nil check for blobReceiver during WaitStop by @awrichar in https://github.com/hyperledger/firefly/pull/980
* add nil check for aggregator during WaitStop by @shorsher in https://github.com/hyperledger/firefly/pull/981
* bump reset polling to 60seconds by @shorsher in https://github.com/hyperledger/firefly/pull/983
* Update firefly_node.md by @Liadc in https://github.com/hyperledger/firefly/pull/987
* Fix bugs when running with an old config file by @awrichar in https://github.com/hyperledger/firefly/pull/984
* Restore camelCase key names by @awrichar in https://github.com/hyperledger/firefly/pull/988
* Add /pins/rewind API for requesing manual rewind by @awrichar in https://github.com/hyperledger/firefly/pull/991
* Wait for server to exit, before restarting for reset by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/994
* Propagate the underlying parse error by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/992
* Do not rely on "topic" to be present in event streams by @awrichar in https://github.com/hyperledger/firefly/pull/999
* Manifest updates for v1.1.0-rc.1 by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1000
* Update CLI to v1.1.0-rc.1 by @nguyer in https://github.com/hyperledger/firefly/pull/1001
* Upgrade firefly-common to v1.1.1 by @awrichar in https://github.com/hyperledger/firefly/pull/1003
* Replace namespace.remotename with namespace.multiparty.networkname by @awrichar in https://github.com/hyperledger/firefly/pull/947
* Add e2e test which attempts to register an invalid identity by reusing a key by @anna-jackson in https://github.com/hyperledger/firefly/pull/996
* Ensure new namespaces are up during multi_tenancy test by @awrichar in https://github.com/hyperledger/firefly/pull/1009
* Ensuring Empty List is Provided for FFDX Init on Zero Peer Nodes by @hfuss in https://github.com/hyperledger/firefly/pull/1004
* Update readme for local dev set up by @Chengxuan in https://github.com/hyperledger/firefly/pull/961
* Add reference doc on identities by @awrichar in https://github.com/hyperledger/firefly/pull/997
* Add tool for auditing blockchain event order by @awrichar in https://github.com/hyperledger/firefly/pull/1002
* Add firefly-signer to manifest by @nguyer in https://github.com/hyperledger/firefly/pull/1015
* add another account for fabric by @anna-jackson in https://github.com/hyperledger/firefly/pull/1018
* Verify integrity of group for private messages by @awrichar in https://github.com/hyperledger/firefly/pull/1006
* adds `fetchreference` to /events/:id by @shorsher in https://github.com/hyperledger/firefly/pull/1017
* Allow any plugin to terminate the system on a bad event by @awrichar in https://github.com/hyperledger/firefly/pull/1021
* Clean up event manager unit tests by @awrichar in https://github.com/hyperledger/firefly/pull/1019
* Use advisory lock instead of exclusive lock on events table by @awrichar in https://github.com/hyperledger/firefly/pull/1027
* Allow null signer on transfers to account for non-archive indexing of historical transactions by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1026
* Add status information for subscriptions & contract listeners by @shorsher in https://github.com/hyperledger/firefly/pull/1028
* Update manifest for v1.1.0-rc.2 by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1033
* update event docs by @shorsher in https://github.com/hyperledger/firefly/pull/1031
* Prevent panic on ff_system namespace for synchronous token pool creation in V1.0 migrated env by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1036
* Routes to directly publish blob/JSON data to shared storage (IFPS etc.) by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1034
* remove legacy namespace query for organizations by @shorsher in https://github.com/hyperledger/firefly/pull/1035
* Allow gateway init with DX and Shared Storage plugins + /data APIs by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1037
* Create a centralised cache manager by @Chengxuan in https://github.com/hyperledger/firefly/pull/1005
* [address-resolver-route] POST /verifiers/resolve by @eberger727 in https://github.com/hyperledger/firefly/pull/1038
* Namespaces reference section + moonbeam docs by @shorsher in https://github.com/hyperledger/firefly/pull/1012
* Add tutorial for Polygon testnet by @nguyer in https://github.com/hyperledger/firefly/pull/966
* Update Good First Issue Link by @nguyer in https://github.com/hyperledger/firefly/pull/1010
* Update manifest for v1.1.0-rc.3 by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1040
* Fix sequence query in auditevents by @awrichar in https://github.com/hyperledger/firefly/pull/1043
* Properly enforce uniqueness of BatchPin blockchain events by @awrichar in https://github.com/hyperledger/firefly/pull/1047
* adding test cases for cache init errors by @Chengxuan in https://github.com/hyperledger/firefly/pull/1044
* Consistently fall back to ff_system for legacy identity lookups by @awrichar in https://github.com/hyperledger/firefly/pull/1048
* Handle FFTM new style acks with batchNumber by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1050
* update public chain docs by @shorsher in https://github.com/hyperledger/firefly/pull/1046
* Update manifest for v1.1.0 by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1053

## New Contributors
* @teaglebuilt made their first contribution in https://github.com/hyperledger/firefly/pull/793
* @viswatejagajulavarthy made their first contribution in https://github.com/hyperledger/firefly/pull/854
* @trevorsc19 made their first contribution in https://github.com/hyperledger/firefly/pull/857
* @satoshi-u made their first contribution in https://github.com/hyperledger/firefly/pull/908
* @JeffNeff made their first contribution in https://github.com/hyperledger/firefly/pull/922
* @sebgoa made their first contribution in https://github.com/hyperledger/firefly/pull/924
* @kmilodenisglez made their first contribution in https://github.com/hyperledger/firefly/pull/937
* @Chengxuan made their first contribution in https://github.com/hyperledger/firefly/pull/950
* @Liadc made their first contribution in https://github.com/hyperledger/firefly/pull/987
* @anna-jackson made their first contribution in https://github.com/hyperledger/firefly/pull/996

**Full Changelog**: https://github.com/hyperledger/firefly/compare/v1.0.4...v1.1.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly/releases/tag/v1.1.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-09-12 12:57:15 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v1.1.0-rc.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.1.0-rc.4
                </span>
            </td>
            <td>
                ## What's Changed
* Fix sequence query in auditevents by @awrichar in https://github.com/hyperledger/firefly/pull/1043
* Properly enforce uniqueness of BatchPin blockchain events by @awrichar in https://github.com/hyperledger/firefly/pull/1047
* adding test cases for cache init errors by @Chengxuan in https://github.com/hyperledger/firefly/pull/1044
* Consistently fall back to ff_system for legacy identity lookups by @awrichar in https://github.com/hyperledger/firefly/pull/1048
* Handle FFTM new style acks with batchNumber by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1050


**Full Changelog**: https://github.com/hyperledger/firefly/compare/v1.1.0-rc.3...v1.1.0-rc.4
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly/releases/tag/v1.1.0-rc.4" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-09-09 23:21:55 +0000 UTC
    </span>
</div>

