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
                    v1.1.0-alpha.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.1.0-alpha.3
                </span>
            </td>
            <td>
                ## What's Changed
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

## New Contributors
* @viswatejagajulavarthy made their first contribution in https://github.com/hyperledger/firefly/pull/854
* @trevorsc19 made their first contribution in https://github.com/hyperledger/firefly/pull/857
* @satoshi-u made their first contribution in https://github.com/hyperledger/firefly/pull/908
* @JeffNeff made their first contribution in https://github.com/hyperledger/firefly/pull/922
* @sebgoa made their first contribution in https://github.com/hyperledger/firefly/pull/924
* @kmilodenisglez made their first contribution in https://github.com/hyperledger/firefly/pull/937
* @Chengxuan made their first contribution in https://github.com/hyperledger/firefly/pull/950

**Full Changelog**: https://github.com/hyperledger/firefly/compare/v1.1.0-alpha.2...v1.1.0-alpha.3
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly/releases/tag/v1.1.0-alpha.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-08-15 20:39:58 +0000 UTC
    </span>
</div>

