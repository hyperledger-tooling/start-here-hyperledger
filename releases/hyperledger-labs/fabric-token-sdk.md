---
layout: default
title: fabric-token-sdk
parent: Hyperledger Labs
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger-labs/fabric-token-sdk
---

# fabric-token-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-token-sdk){: .btn .mr-4 }</span>


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
* additional documentation #3 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/6
* nwo token platform: customisation #4 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/5
* Token Selector: Introduce Concurrency Error #11 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/12
* Streamline Token Transaction Resources Release #10 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/13
* additional documentation by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/15
* additional documentation by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/17
* Refactor Platform Folder Structure #16 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/19
* removing deps to `view/driver` #18 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/20
* additional documentation by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/21
* additional documentation by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/23
* additional documentation by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/26
* Decouple unmarshaling from receiver and export bulk unmarshaling by @yacovm in https://github.com/hyperledger-labs/fabric-token-sdk/pull/29
* clear version for the stack figure? #28 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/30
* tokengen: add ability to generate artifacts #34 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/35
* nwo: token chaincode generation fix param string #36 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/37
* Owner encodes a type #39 by @yacovm in https://github.com/hyperledger-labs/fabric-token-sdk/pull/31
* fabtoken: cleanup and completion #40 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/41
* update fabric smart client dependency to: #43 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/44
* Export Transaction fields by @yacovm in https://github.com/hyperledger-labs/fabric-token-sdk/pull/46
* export verification methods of fabtoken.Validator by @KElkhiyaoui in https://github.com/hyperledger-labs/fabric-token-sdk/pull/49
* update fabric smart client dependency to: #43 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/51
* dlog: membership proof returns errors by @KElkhiyaoui in https://github.com/hyperledger-labs/fabric-token-sdk/pull/50
* Split CI jobs by @yacovm in https://github.com/hyperledger-labs/fabric-token-sdk/pull/54
* add a getter for validation parameters + export unmarshalling method by @KElkhiyaoui in https://github.com/hyperledger-labs/fabric-token-sdk/pull/55
* token/driver api: introduce custom options for Transfer and Issue #42 by @HagarMeir in https://github.com/hyperledger-labs/fabric-token-sdk/pull/52
* Refactor VerifyTransfers by @KElkhiyaoui in https://github.com/hyperledger-labs/fabric-token-sdk/pull/57
* extend issue action #45 by @HagarMeir in https://github.com/hyperledger-labs/fabric-token-sdk/pull/58
* Resurrect go.yml and direct it to merge only by @yacovm in https://github.com/hyperledger-labs/fabric-token-sdk/pull/59
* various improvements #63 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/64
* commit IssueAction by @KElkhiyaoui in https://github.com/hyperledger-labs/fabric-token-sdk/pull/61
* ability to choose wallets and recipient by tms #65 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/66
* various improvements #67 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/68
* update key for issue metadata by @KElkhiyaoui in https://github.com/hyperledger-labs/fabric-token-sdk/pull/69
* minor fix by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/70
* Check if issue metadata entry is already occupied  by @KElkhiyaoui in https://github.com/hyperledger-labs/fabric-token-sdk/pull/73
* Update dependencies and upgrade to Go 1.16 by @yacovm in https://github.com/hyperledger-labs/fabric-token-sdk/pull/74
* Collapse Raw owner (71) by @yacovm in https://github.com/hyperledger-labs/fabric-token-sdk/pull/76
* Revert "Collapse Raw owner" by @yacovm in https://github.com/hyperledger-labs/fabric-token-sdk/pull/78
* close auditor session #79 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/80
* verify #40 by @HagarMeir in https://github.com/hyperledger-labs/fabric-token-sdk/pull/81
* nwo: let the token chaincode being deployed by the nwo fabric p. #82 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/83
* GetManagementService should not panic #85 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/87
* add custom label to public params by @HagarMeir in https://github.com/hyperledger-labs/fabric-token-sdk/pull/88
* Drivers Enhancements #89 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/90
* token processors will not panic anymore when a token by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/91
* Various fixes by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/95
* drivers: use local deserializer to register recipient identities #96 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/97
* ci fix by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/102
* check well-formedness of inputs to token operations #14 by @HagarMeir in https://github.com/hyperledger-labs/fabric-token-sdk/pull/98
* export TCC functions by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/104
* fix module dependency by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/105
* token transaction: application metadata #103 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/108
* token request: generalize auditor field #99 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/109
* FSC dep update by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/110
* translator: adding ability to read the token request by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/112
* upgrade to FSC 1bd8acc7a0fc by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/115
* mathlib integration #1 by @HagarMeir in https://github.com/hyperledger-labs/fabric-token-sdk/pull/113
* rm token/core/math by @HagarMeir in https://github.com/hyperledger-labs/fabric-token-sdk/pull/116
* changes to support the new idemix in FSC by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/117
* use fsc/fabric/services/chaincode package by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/118
* Added FPC support to Token Topology by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/121
* reduce deps to platform/fabric by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/122
* Resolve data races in ZKAT-DLOG transfers by @yacovm in https://github.com/hyperledger-labs/fabric-token-sdk/pull/123
* introduce more abstractions by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/124
* init FPC token chaincode by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/125
* network abstraction by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/126
* additonal network abstraction by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/127
* Parallel zkatdlog by @yacovm in https://github.com/hyperledger-labs/fabric-token-sdk/pull/129
* Test Prove well formed ZLAT-DLOG in parallel by @yacovm in https://github.com/hyperledger-labs/fabric-token-sdk/pull/128
* reduce fabric dependency by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/132
* reduce fabric dep by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/134
* reduce tx size by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/135
* extended fabric identity (idemix) deserializer by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/131
* pp fetcher fix by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/137
* rm off chain by @HagarMeir in https://github.com/hyperledger-labs/fabric-token-sdk/pull/138
* - network package refactored and used in more places by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/140
* get anonymous identity wrt audit info as well by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/141
* fix datarace by @mffrench in https://github.com/hyperledger-labs/fabric-token-sdk/pull/143
* enable race detection by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/144
* TCC extension by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/145
* support for sig metadata by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/146
* reduce logging from error to debug by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/148
* dep sync by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/149
* Cache init params at chaincode startup by @yacovm in https://github.com/hyperledger-labs/fabric-token-sdk/pull/153
* deactivate range proof when it is an ownership transfer by @KElkhiyaoui in https://github.com/hyperledger-labs/fabric-token-sdk/pull/151
* F 150 by @yacovm in https://github.com/hyperledger-labs/fabric-token-sdk/pull/152
* Use mod flag in CI by @yacovm in https://github.com/hyperledger-labs/fabric-token-sdk/pull/155
* update FSC dep by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/156
* new nwo token by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/147
* performance by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/157
* comments to network service by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/158
* fungible token on fabric, sample by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/159
* tokengen should generate also fabtoken parameters #111 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/160
* check finality at the auditor's node by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/161
* ability to lock enrolment ids at audit db level by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/162
* FSC dep update by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/163
* WalletManager Improvements #165 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/166
* mod update by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/168
* nwo: support setup update after key generation #170 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/171
* #179 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/180
* remove dvp integration test by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/182
* remove ttx package #184 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/185
* NFT support by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/174
* F 181 by @KElkhiyaoui in https://github.com/hyperledger-labs/fabric-token-sdk/pull/193
* Test the token transaction release function by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/194
* FIX: nft query engine does not filter properly #198 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/199
* nft: select using wallet #200 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/201
* Orion Integration by @HagarMeir in https://github.com/hyperledger-labs/fabric-token-sdk/pull/175
* NFT integration test and sample by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/197
* Refactoring to make services backend agnostic by @HagarMeir in https://github.com/hyperledger-labs/fabric-token-sdk/pull/209
* Token API Code Documentation by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/206
* cloning instructions by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/210
* nwo token enhancements  by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/211
* fix topology sample by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/214
* remove magic constant 64 for quantity precision #190 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/215
* translator: remove metadata #189 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/216
* sample generate material fix by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/219
* Integrate notifications into token processor by @mbrandenburger in https://github.com/hyperledger-labs/fabric-token-sdk/pull/203
* TCC: reuse embedded params #222 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/223
* Prepare selector for testing by @mbrandenburger in https://github.com/hyperledger-labs/fabric-token-sdk/pull/226
* selector: move certification from the token selector to the token request #224 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/225
* export functions in fungible integration tests #227 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/228
* fix tests by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/229
* tokengen should take in input issuer and auditor public keys #232 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/233
* Fix data race on TMS and expose TMSProvider by @mffrench in https://github.com/hyperledger-labs/fabric-token-sdk/pull/231
* Documentation for FTS_PATH changed as copy paste won't work by @rajat-dlt in https://github.com/hyperledger-labs/fabric-token-sdk/pull/236
* tokengen: add support for custom generator #234 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/235
* tokengen: make GeneratorFunc independent from the global variables #238 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/239
* sample documentation update by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/237
* add func to register issuance wallets by @mffrench in https://github.com/hyperledger-labs/fabric-token-sdk/pull/244
* CI go1.17 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/248
* auditdb: extended transaction tracking #242 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/243
* improve identity and wallet default cache size management by @mffrench in https://github.com/hyperledger-labs/fabric-token-sdk/pull/251
* fix AuditDB redeem bug by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/254
* Namespace is always zkat even if it was changed in the node config #256 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/257
* add missing testdata by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/240
* auditdb: extend to owner wallets #247 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/253
* update FSC dep to latest by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/260
* Doc Correction by @sapthasurendran in https://github.com/hyperledger-labs/fabric-token-sdk/pull/265
* update go.mod to go.1.17 #264 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/266
* TokenSDK Config: returns all TMS configurations by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/268
* Logging cleanup and samples gitignore by @mbrandenburger in https://github.com/hyperledger-labs/fabric-token-sdk/pull/270
* Update old idemix references by @mbrandenburger in https://github.com/hyperledger-labs/fabric-token-sdk/pull/269
* filter metadata by recipient identity #212 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/249
* wallets restructuring #272 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/273
* F 252: zkatdlog crypto library clean up by @KElkhiyaoui in https://github.com/hyperledger-labs/fabric-token-sdk/pull/275
* Remove the need to specify the MSP-ID by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/280
* the recipient to choose a wallet for the tokens to be issued in #284 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/285
* Spelling by @mbrandenburger in https://github.com/hyperledger-labs/fabric-token-sdk/pull/287
* Run goimports by @mbrandenburger in https://github.com/hyperledger-labs/fabric-token-sdk/pull/286
* Tooling enhancement by @mbrandenburger in https://github.com/hyperledger-labs/fabric-token-sdk/pull/288
* ttx: use default network identity if not specified by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/281
* Fix gh actions by @mbrandenburger in https://github.com/hyperledger-labs/fabric-token-sdk/pull/291
* Upgrade to CodeQL v2 by @mbrandenburger in https://github.com/hyperledger-labs/fabric-token-sdk/pull/292
* auditor and issuer are the same node #283 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/289
* Tokengen should also work without signing key of auditor and issuer #299 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/300
* `token\core` improvements by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/297
* use time.NewTimer instead of time.After by @yacovm in https://github.com/hyperledger-labs/fabric-token-sdk/pull/306
* Expose idemix identity cache size in config by @yacovm in https://github.com/hyperledger-labs/fabric-token-sdk/pull/305
* Optimize Idemix pre-provision cache by @yacovm in https://github.com/hyperledger-labs/fabric-token-sdk/pull/304
* F252: token request clean up  by @KElkhiyaoui in https://github.com/hyperledger-labs/fabric-token-sdk/pull/296
* F252: zkatdlog cleanup - add comments and improve error handling by @KElkhiyaoui in https://github.com/hyperledger-labs/fabric-token-sdk/pull/294
* F252: fabtoken cleanup - add comments and enhance error messages by @KElkhiyaoui in https://github.com/hyperledger-labs/fabric-token-sdk/pull/293
* Add recipient signature as acknowledgment  by @sapthasurendran in https://github.com/hyperledger-labs/fabric-token-sdk/pull/298
* Remove GetCachedStateRangeScanIterator by @mbrandenburger in https://github.com/hyperledger-labs/fabric-token-sdk/pull/311
* fix data race in ppm #309 by @Grimnir777 in https://github.com/hyperledger-labs/fabric-token-sdk/pull/310
* Panic Seg Fault with Issue func by @ltxyz in https://github.com/hyperledger-labs/fabric-token-sdk/pull/319
* `token/services/ttx/endorse.go`: EndorseView should store transient immeditately by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/313
* Reduce staticcheck warnings (S1023) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-token-sdk/pull/324
* Reduce staticcheck warnings (ST1019) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-token-sdk/pull/325
* Reduce staticcheck warnings (S1011) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-token-sdk/pull/326
* Reduce staticcheck warnings (S1039) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-token-sdk/pull/327
* Reduce staticcheck warnings (ST1001) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-token-sdk/pull/323
* Reduce staticcheck warnings (SA4010) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-token-sdk/pull/328
* htlc #255 by @HagarMeir in https://github.com/hyperledger-labs/fabric-token-sdk/pull/290
* Reduce staticcheck warnings (SA9003) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-token-sdk/pull/329
* Reduce staticcheck warnings (SA1019) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-token-sdk/pull/333
* Reduce staticcheck warnings (S1038, S1012, S1021, SA4001) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-token-sdk/pull/331
* Reduce staticcheck warnings (SA5007) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-token-sdk/pull/332
* Reduce staticcheck warnings (S1011) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-token-sdk/pull/337
* Reduce staticcheck warnings (SA4022) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-token-sdk/pull/338
* Re-introduce -mod=mod go flag by @yacovm in https://github.com/hyperledger-labs/fabric-token-sdk/pull/344
* Add manual CI test trigger by @mbrandenburger in https://github.com/hyperledger-labs/fabric-token-sdk/pull/342
* Reduce staticcheck warnings (SA4011) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-token-sdk/pull/339
* Reduce staticcheck warnings (U1000) by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-token-sdk/pull/336
* Enable static checks by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-token-sdk/pull/346
* Upgrade Ginkgo v2 by @mbrandenburger in https://github.com/hyperledger-labs/fabric-token-sdk/pull/348
* check that the tokens accepted appear in the vault by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/330
* explicit double spending check by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/335
* translator: remove IssuingValidator #352 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/354
* Fixed missing dependency by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-token-sdk/pull/357
* documentation by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/351
* Rename exchange to htlc by @HagarMeir in https://github.com/hyperledger-labs/fabric-token-sdk/pull/363
* Cleanup deps.go by @alexandrosfilios in https://github.com/hyperledger-labs/fabric-token-sdk/pull/362
* Remove signature metadata action by @HagarMeir in https://github.com/hyperledger-labs/fabric-token-sdk/pull/358
* check public parameters match by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/368
* Interop documentation by @HagarMeir in https://github.com/hyperledger-labs/fabric-token-sdk/pull/360
* FSC dep update by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/373
* Fix: typos by @edwardramsey in https://github.com/hyperledger-labs/fabric-token-sdk/pull/372
* Auditor and Issuer Wallet: Support PKCS11 #320 #355 by @sapthasurendran in https://github.com/hyperledger-labs/fabric-token-sdk/pull/375
* FSC dep update by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/377
* remove "zkat" magic string #107 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/380
* ScanForPreImage Enhancement: Custom Starting Point #378 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/379
* htlc auditing extension by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/369
* Export `ttxdb` SetStatus function by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/376
* double check the use of NewQuantityFromUInt64 #218 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/381
* review htlc terms by @HagarMeir in https://github.com/hyperledger-labs/fabric-token-sdk/pull/382
* Add timeout to Network Finality API #383 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/384
* FSC update by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/385
* add metadata to issue action by @KElkhiyaoui in https://github.com/hyperledger-labs/fabric-token-sdk/pull/387
* Transfer metadata rework by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/386
* check that the public parameters are valid #388 by @KElkhiyaoui in https://github.com/hyperledger-labs/fabric-token-sdk/pull/389
* Issue Action Metadata: Use map #365 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/390
* go1.18 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/391
* commit to go1.18 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/399
* lock error when same hash is used for lock #392 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/393
* missing underlying validation by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/398
* query transaction records by action type and status #396 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/397
* Provide an efficient way to lookup wallet by ID #394 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/395
* Export `SetStatus` function on OnwerDBs by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/407
* ttxdb derivates: failed restart #402 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/405
* Move inactive maintainers to emeritus status by @ryjones in https://github.com/hyperledger-labs/fabric-token-sdk/pull/408
* enhancements pack by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/406
* FTS to now use FSC Fabric Binary Only Implementation by @davidkel in https://github.com/hyperledger-labs/fabric-token-sdk/pull/410
* check that output's quantity is less or equal to max_value. #411 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/414
* FSC update by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/417
* let the token driver decide how to marshal a token request by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/418
* cleanup token request metadata by @HagarMeir in https://github.com/hyperledger-labs/fabric-token-sdk/pull/420
* deprecate balance queries by @HagarMeir in https://github.com/hyperledger-labs/fabric-token-sdk/pull/421
* Expose RegisterIssuerWallet by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/419
* various extensions by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/422
* more checks by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/416
* v0.1.0 by @adecaro in https://github.com/hyperledger-labs/fabric-token-sdk/pull/424

## New Contributors
* @yacovm made their first contribution in https://github.com/hyperledger-labs/fabric-token-sdk/pull/29
* @KElkhiyaoui made their first contribution in https://github.com/hyperledger-labs/fabric-token-sdk/pull/49
* @mffrench made their first contribution in https://github.com/hyperledger-labs/fabric-token-sdk/pull/143
* @rajat-dlt made their first contribution in https://github.com/hyperledger-labs/fabric-token-sdk/pull/236
* @sapthasurendran made their first contribution in https://github.com/hyperledger-labs/fabric-token-sdk/pull/265
* @Grimnir777 made their first contribution in https://github.com/hyperledger-labs/fabric-token-sdk/pull/310
* @ltxyz made their first contribution in https://github.com/hyperledger-labs/fabric-token-sdk/pull/319
* @alexandrosfilios made their first contribution in https://github.com/hyperledger-labs/fabric-token-sdk/pull/324
* @edwardramsey made their first contribution in https://github.com/hyperledger-labs/fabric-token-sdk/pull/372
* @ryjones made their first contribution in https://github.com/hyperledger-labs/fabric-token-sdk/pull/408
* @davidkel made their first contribution in https://github.com/hyperledger-labs/fabric-token-sdk/pull/410

**Full Changelog**: https://github.com/hyperledger-labs/fabric-token-sdk/commits/v0.1.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger-labs/fabric-token-sdk/releases/tag/v0.1.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-11-16 13:23:58 +0000 UTC
    </span>
</div>

