---
layout: default
title: fabric-smart-client
parent: Hyperledger Labs
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger-labs/fabric-smart-client
---

# fabric-smart-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-smart-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v0.1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.1.0
                </span>
            </td>
            <td>
                ## What's Changed
* Fix typo by @tkuhrt in https://github.com/hyperledger-labs/fabric-smart-client/pull/6
* Fix typo by @arsulegai in https://github.com/hyperledger-labs/fabric-smart-client/pull/7
* Continuous Integration Enablement #1 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/10
* Integration Test Infrastructure: Pluggable platforms #3 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/14
* Close GRPC connections from peer & orderer clients by @mffrench in https://github.com/hyperledger-labs/fabric-smart-client/pull/15
* add SECURITY.md and CODE_OF_CONDUCT.md #17 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/18
* NWO: remove generic platform #12 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/16
* Support for the fabric token SDK #20 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/21
* Additional Documentation #2 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/22
* additional documentation by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/25
* ping pong example: additional configuration by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/26
* Restart from genesis if the last transaction committed is a config transaction #4 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/29
* minor fix to documentation #2 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/28
* View GRPC Server: Enforce Signature Verification #27 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/32
* Remove SigService IdentityType #31 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/33
* adding link to github discussion by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/34
* Update docu by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/37
* ViewSDK: DB Driver Pluggability #30 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/36
* Refactor Platform Folder Structure #35 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/38
* additional documentation by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/41
* additional documentation by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/44
* iou sample: additional documentation and comments to the code by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/47
* idemix signer deserializer should check that the nym key matches the secret key #33 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/48
* additional documentation and comments to the code by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/51
* golint fixes, first drop by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/52
* more documentation and comments by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/54
* Support for multiple Fabric Networks #9 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/57
* Support for multiple Fabric Networks #9 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/58
* Support for multiple Fabric Networks #9 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/59
* Support for multiple Fabric Networks #9 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/60
* Call view from REST #39 by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/43
* Support for multiple Fabric Networks #9 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/62
* committer: match the results of the transaction #63 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/64
* compatibility requirements with the fabric token sdk #65 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/66
* committer: fetch each transaction singularly if the block is too big #67 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/68
* Split CI by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/71
* Resurrect go.yml and direct it to merge only by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/72
* nwo: make RegisterResponder use import aliasing #73 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/74
* bug fix #76 #77 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/78
* fabric/core/generic driver: transaction's network not set properly #79 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/80
* view context: run a view with options #83 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/84
* addressing #85 and #86 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/87
* Only run UTs in UT job by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/88
* allow multiple fabric networks to set as default #89 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/90
* nwo: set default fabric network per FSC node #91 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/92
* Update dependencies by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/94
* Upgrade Go version to 1.16 by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/95
* kvs: support delete #97 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/99
* F 61 by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/96
* Remove Alice from network beta and Bob from network alpha by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/104
* Integrate weaver-dlt-interoperability relay #61 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/105
* Introduce client Signing Identity default implementation #102 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/106
* view sdk fails when resolvers aliases are defined #103 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/107
* fabric LocalMembership should first search over the local resolvers #108 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/109
* weaver integration: address generation failure #113 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/114
* Extend ATSA/FSC to support anonymous identity by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/116
* Fabric Private Chaincode support #23 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/112
* Use MSPManager to get verifiers #120 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/121
* Fix CI by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/124
* introduce client identities to invoke views #101 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/122
* cleanup go mod by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/125
* remove token-sdk dep by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/126
* Init module in cc/query by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/127
* fix module name in cc/query by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/128
* go packager: prefix fix by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/129
* check when fabric network service does not exist by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/131
* NWO: Fabric-FPC, more general root path finder by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/132
* fabric-sdk: delivery service #137 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/138
* sdk: failure loading config transaction when restarting #139 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/140
* FPC Integration Enhancements #134 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/143
* vault fails to validate keys containing string(utf8.MaxRune) #144 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/145
* Remove idemix by @ale-linux in https://github.com/hyperledger-labs/fabric-smart-client/pull/115
* imports cleanup by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/148
* Method `CallView` from package `web` able to send correct inputs by @alexshehovcov in https://github.com/hyperledger-labs/fabric-smart-client/pull/150
* Expanded FPC API by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/151
* locking on view/endpoint resolvers by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/154
* Fold cryptogen, artifactsgen into a unified CLI that invokes views by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/155
* Added Fabric topology flexibility by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/156
* Add FPC container logging by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/160
* nwo fabric: support fpc invocation by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/161
* Deduplicate endorsers during discovery by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/159
* nwo improvements by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/162
* fabric envelope, FromBytes method by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/163
* reduce integration infrastructure logging to info by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/164
* vault rws comparison fix by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/169
* fabric envelope logs by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/170
* extended idemix support by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/166
* cleanup context after responding by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/175
* use same tx-id for fpc backend by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/176
* improvements by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/180
* Expose ViewCmd from infrastructure by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/182
* nwo: improved fabric network support by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/181
* Export Infrastructure fields by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/185
* Cache peer connections when invoking chaincode/discovery by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/186
* Revert "Cache peer connections when invoking chaincode/discovery" by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/187
* Revert "Revert "Cache peer connections when invoking chaincode/discovery"" by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/188
* EnableLogPeersToFile on Fabric Topology to enable peer's logs by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/189
* Export Platform by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/190
* Increase default batch size by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/191
* Add command to kill FSC nodes by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/192
* FlowControlBroadcast by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/193
* fix deadlock by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/194
* Do not closeSend by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/195
* Lock when sending by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/196
* Make default KA in CreateGRPCClient zero value by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/199
* Revert "Make default KA in CreateGRPCClient zero value" by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/200
* Add option to redirect FSC to file by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/201
* Maybe fix CI by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/205
* Do not use QSCC to query block, fetch it from peer instead by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/204
* Redirect OSN output to file by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/202
* minor improvements by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/211
* mod update by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/213
* profiling support by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/212
* idemix: adding cache by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/216
* first sample app by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/217
* network cmd improvements by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/218
* Remove unused docker images by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/219
* Remove stack debug from info logger by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/220
* Provide clear error on bad path to crypto files on fabric resolvers #184 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/221
* peer load balancing by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/222
* streanline connection ports by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/225
* FSC identity, use ecdsa with low s #226 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/227
* FPC: generates external builder scripts #230 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/231
* Enable FSC SGX HW support by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/234
* Data race on RegisterIdemixMSP #232 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/233
* Ability to specify the organizations on which to install a FPC by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/235
* nwo.fabric: support for HLE and Prometheus+Graphana by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/236
* minor fix by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/238
* working metrics by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/239
* metrics by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/237
* weaver relay f2f sample by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/240
* larger keys in rw sets by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/242
* add ability to configure idemix cash size #243 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/245
* fix p2p unit-tests flake #246 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/247
* remove debug.Stack logging where not needed by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/250
* streamline sig service logs by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/252
* Orion by @HagarMeir in https://github.com/hyperledger-labs/fabric-smart-client/pull/255
* Attach SGX devices to FPC container by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/253
* orion: update readmes and removed unused interfaces and methods #256 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/258
* README update with clone instructions  by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/260
* Remove wrong rlock release by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/262
* call StartCMDPostNew also for the Generate command by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/265
* NWO must wait that the FSC nodes are fully up and running before starting the tests #266 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/268
* Add event service by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/241
* Add a note on disabling the logger or modifying its configuration by @lebdron in https://github.com/hyperledger-labs/fabric-smart-client/pull/272
* increase namespace length limit in rw sets #273 by @saoussen in https://github.com/hyperledger-labs/fabric-smart-client/pull/274
* Documentation for FTS_PATH changed as copy paste won't work by @rajat-dlt in https://github.com/hyperledger-labs/fabric-smart-client/pull/278
* fabric-sdk: add keep alive config support #279 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/280
* Fix sig deserializer data race by @mffrench in https://github.com/hyperledger-labs/fabric-smart-client/pull/270
* increase namespace length limit to 128 #285 by @saoussen in https://github.com/hyperledger-labs/fabric-smart-client/pull/286
* notify commit/discard tx events #283 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/287
* fix db memory data race by @mffrench in https://github.com/hyperledger-labs/fabric-smart-client/pull/282
* CI go1.17 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/291
* Improve identity cache default by @mffrench in https://github.com/hyperledger-labs/fabric-smart-client/pull/292
* Upgrade libp2p by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/289
* improve GetEphemeralRWSet with namespaces as input #275 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/290
* extract IPs from discovery #293 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/294
* Changed go version requirement in README by @sapthasurendran in https://github.com/hyperledger-labs/fabric-smart-client/pull/296
* update go.mod to go.1.17 #297 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/298
* Enforce GOPATH by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/300
* Fabric upgrade and cleanup by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/295
* RegisterResponder function needs to have two views that should be sent from two different applications #301 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/302
* Pin Fabric 2.2 LTS by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/304
* Run goimports over the code base by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/306
* Move tools deps into tools folder by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/305
* fabric-sdk: use orderers set in the config block by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/307
* view-sdk: enhancements  by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/310
* Refactor nwo docker support by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/308
* Upgrade to CodeQL v2 by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/314
* Rework github actions by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/309
* Add NWO support for existing fabric bins by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/318
* Generate connection.yaml by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/319
* Use time.NewTimer instead of time.After by @yacovm in https://github.com/hyperledger-labs/fabric-smart-client/pull/320
* Removed simple gogo/protobuf/proto dependencies by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-smart-client/pull/321
* Reduce staticcheck warnings (ST1005) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-smart-client/pull/322
* Optimize msp cache by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/324
* Reduce staticcheck warnings (ST1019, S1023) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-smart-client/pull/325
* KVS extensions by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/330
* Remove GetCachedStateRangeScanIterator by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/323
* Reduce staticcheck warnings (SA1019) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-smart-client/pull/328
* Add mbrandenburger to maintainers by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/333
* Reduce staticcheck warnings (ST1001) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-smart-client/pull/332
* Reduce staticcheck warnings (SA1019) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-smart-client/pull/334
* Reduce staticcheck warnings (S1000) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-smart-client/pull/340
* Reduce staticcheck warnings (S1034) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-smart-client/pull/341
* Reduce staticcheck warnings (SA4023) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-smart-client/pull/344
* Reduce staticcheck warnings (S1039) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-smart-client/pull/342
* Revert "Reduce staticcheck warnings (SA4023) (#344)" by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-smart-client/pull/350
* Reduce staticcheck warnings (S1011) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-smart-client/pull/343
* Reduce staticcheck warnings (SA4004) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-smart-client/pull/346
* Reduce staticcheck warnings (SA4023) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-smart-client/pull/351
* Reduce staticcheck warnings (S1021, S1038, S1025, SA4009, S1005, SA9003) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-smart-client/pull/345
* Remove cleaning of non-generated file by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-smart-client/pull/352
* Reduce staticcheck warnings (SA4006) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-smart-client/pull/348
* committer improvements by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/353
* Cleanup integration tests by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/357
* Adding .gitignore to samples by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/356
* Reduce staticcheck warnings (SA9005) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-smart-client/pull/347
* Reduce staticcheck warnings (U1000) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-smart-client/pull/362
* FSC memory enhancements by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/355
* Make ATSA Chaincode receipt struct fields public by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/364
* Enable staticcheck via make checks by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/336
* Upgrade to ginkgo v2 by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/366
* Cleanup deps.go by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-smart-client/pull/371
* Add WithEndorsersByMSPIDs to query chaincode view by @mbrandenburger in https://github.com/hyperledger-labs/fabric-smart-client/pull/370
* Remove need for GOPATH to be set by @davidkel in https://github.com/hyperledger-labs/fabric-smart-client/pull/374
* fabric-sdk: cleanup ordering connection on failure + retry #377 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/379
* fabric-sdk: do not add resolvers for Fabric peers by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/375
* fabric-sdk: support for PKCS11 #281 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/369
* hsm support for mac by @sapthasurendran in https://github.com/hyperledger-labs/fabric-smart-client/pull/383
* view/services/db: orion-based driver by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/303
* Add timeout to Finality API #380 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/388
* Unit tests mocks cleanup #368 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/387
* view comm layer: override ip address #389 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/390
* if no default MSP is set, pick the first by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/392
* minor enhancements by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/394
* Chaincode Event Listening Support by @sapthasurendran in https://github.com/hyperledger-labs/fabric-smart-client/pull/384
* go1.18 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/396
* Minor updates to IOU sample README and code for simplicity and clarity by @bestbeforetoday in https://github.com/hyperledger-labs/fabric-smart-client/pull/399
* commit to go1.18 by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/405
* FSC Improvements by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/403
* Various bug fix by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/409
* fabric ordering: retry also when establishing the connection fails by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/411
* fabric: call discard for unknown tx by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/416
* Fix npe if no core file found by @davidkel in https://github.com/hyperledger-labs/fabric-smart-client/pull/417
* Extensions by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/414
* restructure fsc and fabric driver core to be more intuitive by @davidkel in https://github.com/hyperledger-labs/fabric-smart-client/pull/415
* Minor updates by @mbwhite in https://github.com/hyperledger-labs/fabric-smart-client/pull/422
* enhancement pack by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/421
* NWO to only use Fabric Binaries by @davidkel in https://github.com/hyperledger-labs/fabric-smart-client/pull/426
* sample config with doc by @davidkel in https://github.com/hyperledger-labs/fabric-smart-client/pull/427
* orion cleanup by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/429
* Upgrade chaincode by @sapthasurendran in https://github.com/hyperledger-labs/fabric-smart-client/pull/401
* fix delivery restart by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/430
* keys are sanitised directly by orion, no need for extra sanitization by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/431
* Revert "keys are sanitised directly by orion, no need for extra sanit… by @adecaro in https://github.com/hyperledger-labs/fabric-smart-client/pull/433

## New Contributors
* @tkuhrt made their first contribution in https://github.com/hyperledger-labs/fabric-smart-client/pull/6
* @arsulegai made their first contribution in https://github.com/hyperledger-labs/fabric-smart-client/pull/7
* @adecaro made their first contribution in https://github.com/hyperledger-labs/fabric-smart-client/pull/10
* @mbrandenburger made their first contribution in https://github.com/hyperledger-labs/fabric-smart-client/pull/37
* @yacovm made their first contribution in https://github.com/hyperledger-labs/fabric-smart-client/pull/43
* @ale-linux made their first contribution in https://github.com/hyperledger-labs/fabric-smart-client/pull/115
* @alexshehovcov made their first contribution in https://github.com/hyperledger-labs/fabric-smart-client/pull/150
* @HagarMeir made their first contribution in https://github.com/hyperledger-labs/fabric-smart-client/pull/255
* @lebdron made their first contribution in https://github.com/hyperledger-labs/fabric-smart-client/pull/272
* @saoussen made their first contribution in https://github.com/hyperledger-labs/fabric-smart-client/pull/274
* @rajat-dlt made their first contribution in https://github.com/hyperledger-labs/fabric-smart-client/pull/278
* @sapthasurendran made their first contribution in https://github.com/hyperledger-labs/fabric-smart-client/pull/296
* @alexandrosfilios made their first contribution in https://github.com/hyperledger-labs/fabric-smart-client/pull/321
* @davidkel made their first contribution in https://github.com/hyperledger-labs/fabric-smart-client/pull/374
* @bestbeforetoday made their first contribution in https://github.com/hyperledger-labs/fabric-smart-client/pull/399
* @mbwhite made their first contribution in https://github.com/hyperledger-labs/fabric-smart-client/pull/422

**Full Changelog**: https://github.com/hyperledger-labs/fabric-smart-client/commits/v0.1.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger-labs/fabric-smart-client/releases/tag/v0.1.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-11-16 12:51:41 +0000 UTC
    </span>
</div>

