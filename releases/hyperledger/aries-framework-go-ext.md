---
layout: default
title: aries-framework-go-ext
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/aries-framework-go-ext
---

# aries-framework-go-ext <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go-ext){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Release v1.0.0-rc.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    component/vdr/orb/v1.0.0-rc.1
                </span>
            </td>
            <td>
                ## What's Changed
* Add basic settings file by @ryjones in https://github.com/hyperledger/aries-framework-go-ext/pull/1
* feat: Adds global checks by @soluchok in https://github.com/hyperledger/aries-framework-go-ext/pull/5
* ci: Adds codecov.yaml file by @soluchok in https://github.com/hyperledger/aries-framework-go-ext/pull/8
* feat: Adds MySQL storage implementation by @soluchok in https://github.com/hyperledger/aries-framework-go-ext/pull/6
* feat: Adds Couchdb storage implementation by @soluchok in https://github.com/hyperledger/aries-framework-go-ext/pull/7
* test: Common test package for storage by @soluchok in https://github.com/hyperledger/aries-framework-go-ext/pull/11
* test: Adds common tests (couchdb, mysql) by @soluchok in https://github.com/hyperledger/aries-framework-go-ext/pull/10
* refactor: Enables testpackage and nlreturn linters by @soluchok in https://github.com/hyperledger/aries-framework-go-ext/pull/13
* chore: Update aries-framework-go dependency by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/15
* feat:  Adds MongoDB storage implementation. by @pfeairheller in https://github.com/hyperledger/aries-framework-go-ext/pull/17
* chore: Updates Codecov by @soluchok in https://github.com/hyperledger/aries-framework-go-ext/pull/29
* refactor: MySQL uses now own errors by @soluchok in https://github.com/hyperledger/aries-framework-go-ext/pull/32
* issue:  Fix mongodb storage driver tests by @pfeairheller in https://github.com/hyperledger/aries-framework-go-ext/pull/33
* feat:  Adds AMQP Inbound Transport by @pfeairheller in https://github.com/hyperledger/aries-framework-go-ext/pull/16
* feat: Trustbloc DID method support by @soluchok in https://github.com/hyperledger/aries-framework-go-ext/pull/35
* Feature:  An Implementation of VDR for resolving DIDs against an Indy ledger by @pfeairheller in https://github.com/hyperledger/aries-framework-go-ext/pull/34
* fix: Lint script not working with modules with local import replace by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/39
* BUG:  Fix Makefile so lint runs locally by @pfeairheller in https://github.com/hyperledger/aries-framework-go-ext/pull/42
* feat: Add sidetree client by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/37
* chore: add vdr-sidetree workflow by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/43
* feat: Partial CouchDB implementation of new storage interface by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/41
* feat: Query method for new CouchDB storage implementation by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/47
* feat: GetBulk method for new CouchDB storage implementation by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/49
* feat: Batch method for new CouchDB storage implementation by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/51
* chore: Use DocResolution from aries did package by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/52
* chore: remove project codecov status check by @troyronda in https://github.com/hyperledger/aries-framework-go-ext/pull/53
* chore: prepare codecov settings split by @troyronda in https://github.com/hyperledger/aries-framework-go-ext/pull/54
* fix: GetPublicKeyJWK bug by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/56
* chore: updare aries revision by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/57
* chore: Add WithRecoveryCommitment and WithUpdateCommitment by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/59
* chore: move vdr trustbloc from trustbloc-did-method by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/60
* chore: Support adding sidetree purposes by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/61
* fix: Load genesis files in trustbloc vdr initialization by @Moopli in https://github.com/hyperledger/aries-framework-go-ext/pull/62
* chore: Add repolint by @troyronda in https://github.com/hyperledger/aries-framework-go-ext/pull/63
* fix: Unable to retrieve certain keys - new CouchDB store implementation by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/64
* feat: Update CouchDB implementation based on latest Aries dependencies by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/66
* feat: Partial MySQL implementation of new storage interface by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/68
* feat: Update aries-framework-go, only use new storage interface now by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/70
* fix: CouchDB and MySQL storage Go module paths by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/71
* chore: Updates aries revision by @soluchok in https://github.com/hyperledger/aries-framework-go-ext/pull/72
* fix: CouchDB documents don't store if key was previously deleted by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/73
* feat: MySQL implementation of interface methods needed by Aries agent by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/74
* fix: MySQL provider "store not found" errors when prefix is used by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/75
* chore: update sidetree-core by @sandrask in https://github.com/hyperledger/aries-framework-go-ext/pull/77
* fix: MySQL not storing binary data correctly by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/82
* fix: Binary data not storing correctly with CouchDB storage provider by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/83
* chore: Update Aries dependencies to v0.1.6 by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/84
* chore: go mod tidy for vdr trusbloc by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/85
* chore: Update common storage test suite version by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/86
* feat: Improvements to CouchDB document storage by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/87
* chore: remove kms from create trustbloc vdr by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/89
* test: add bdd test for trutbloc vdr by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/92
* feat: add basic orb vdr by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/93
* fix: Prevent storage of invalid tag names, update storage tests commit by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/94
* feat: add AnchorOrigin to sidetree request (create,recover) by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/96
* test: add basic bdd test for orb vdr by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/95
* feat: use aries jwk for sidetree client by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/98
* test: add bdd test for orb vdr (update, recover, deactivate) by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/97
* chore: update trustbloc vdr to use latest aries by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/99
* feat: add discovery domain for orb vdr by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/100
* fix: remove hardcoded operation in url by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/101
* test: add bdd test for vdr orb discovery by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/102
* feat: add Shared Resolution Domain validation by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/103
* fix: send empty body for GET by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/104
* feat: CouchDB provider support for query sorting and initial page by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/105
* chore: update afgo, go version to 1.16 where necessary, and golangci-lint by @Moopli in https://github.com/hyperledger/aries-framework-go-ext/pull/106
* feat: Index creation retries and better logging by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/107
* chore: update to latest orb by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/108
* feat: mysql Batch() by @llorllale in https://github.com/hyperledger/aries-framework-go-ext/pull/110
* fix: mysql batch by @llorllale in https://github.com/hyperledger/aries-framework-go-ext/pull/111
* fix: fix trustbloc vdr client to work with recent changes to sidetree client by @Moopli in https://github.com/hyperledger/aries-framework-go-ext/pull/112
* chore: orb - preload JSONLD contexts by @llorllale in https://github.com/hyperledger/aries-framework-go-ext/pull/113
* chore: update latest AFG by @Baha-sk in https://github.com/hyperledger/aries-framework-go-ext/pull/114
* chore: update to orb v0.1  by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/115
* fix: get resolution endpoints from configure domain by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/116
* chore: update to latest aries by @Moopli in https://github.com/hyperledger/aries-framework-go-ext/pull/117
* chore: update orb revision by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/118
* chore: update afgo version by @Moopli in https://github.com/hyperledger/aries-framework-go-ext/pull/119
* fix: orb vdr docs by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/120
* chore: update to latest orb by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/125
* chore: update to latest vct and orb by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/126
* feat: Support for Iterator TotalItems in CouchDB by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/128
* chore: update active maintainer list by @troyronda in https://github.com/hyperledger/aries-framework-go-ext/pull/127
* fix: CouchDB TotalItems not correct when tag values are empty by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/129
* feat: resolve orb did using IPNS by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/130
* test: add test for did orb ipns by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/131
* feat: get latest anchor origin by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/132
* feat: resolve webcas in orb vdr by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/133
* chore: update to latest orb by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/134
* chore: update to latest orb by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/135
* chore: rename webfinger response struct by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/136
* fix: Race condition in MySQL storage provider by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/137
* fix: ipns config by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/138
* chore: Updates vct by @soluchok in https://github.com/hyperledger/aries-framework-go-ext/pull/139
* fix: Fixes bdd tests by @soluchok in https://github.com/hyperledger/aries-framework-go-ext/pull/140
* chore: Update storage implementations to pass new common tests by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/145
* feat: MongoDB/DocumentDB storage provider by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/148
* added nil check for nym reply by @0xArdi in https://github.com/hyperledger/aries-framework-go-ext/pull/149
* chore: update AFGO by @aholovko in https://github.com/hyperledger/aries-framework-go-ext/pull/150
* chore: Update Go Mongo driver version by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/151
* fix: temp workaround for cyclic deps by @aholovko in https://github.com/hyperledger/aries-framework-go-ext/pull/152
* fix: cleanup deps by @aholovko in https://github.com/hyperledger/aries-framework-go-ext/pull/153
* chore: update AFGO by @aholovko in https://github.com/hyperledger/aries-framework-go-ext/pull/154
* chore: update sidetree dependency by @aholovko in https://github.com/hyperledger/aries-framework-go-ext/pull/155
* chore: update AFGO for sidetree vdr by @aholovko in https://github.com/hyperledger/aries-framework-go-ext/pull/156
* chore: update AFGO by @aholovko in https://github.com/hyperledger/aries-framework-go-ext/pull/158
* chore: add timeout for http client by @rolsonquadras in https://github.com/hyperledger/aries-framework-go-ext/pull/159
* docs: Fix incorrect MongoDB provider documentation by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/161
* fix: allow creating/updating doc with base58 pub keys in vdr/sidetree by @Moopli in https://github.com/hyperledger/aries-framework-go-ext/pull/162
* chore: update orb vdr to latest sidetree vdr by @Moopli in https://github.com/hyperledger/aries-framework-go-ext/pull/163
* fix: allow creating docs with base58 keys in orb vdr by @Moopli in https://github.com/hyperledger/aries-framework-go-ext/pull/164
* feat: Reuse MongoDB connection across stores by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/165
* test: Update common tests and interface version by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/166
* updated indy vdr component to be compliant with v0.1.6 aries by @0xArdi in https://github.com/hyperledger/aries-framework-go-ext/pull/160
* feat: GetStoreConfig can now be used to check for underlying database by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/168
* chore: Store JSON strings as string instead of binary in MongoDB by @bstasyszyn in https://github.com/hyperledger/aries-framework-go-ext/pull/169
* chore: use orb discovery client by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/170
* fix: Detect transient error when setting indexes using DocumentDB by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/171
* feat: Increase max data size for MySQL storage provider by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/172
* fix: Retry on transient Put and Batch errors for MongoDB by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/173
* feat: resolve did from https hint by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/175
* chore: avoid adding current keys when update did by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/176
* fix: Large integer storage not working correctly with MongoDB provider by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/177
* chore: Update storage SPI and tests commit versions by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/178
* chore: enable UPDATE_DOCUMENT_STORE_ENABLED for orb by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/179
* chore: add temp solution updated did from cache by @rolsonquadras in https://github.com/hyperledger/aries-framework-go-ext/pull/181
* chore: update to release versions by @rolsonquadras in https://github.com/hyperledger/aries-framework-go-ext/pull/183
* chore: Add commitment to KeyRetriever interface by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/184
* chore: check for error did not found by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/185
* feat: add option to return when did is anchored or updated by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/186
* feat: allow vdr to accept did with verification methods by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/187
* feat: resolve hl cas links by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/188
* feat: Support for querying for two tags at once with MongoDB by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/189
* feat: Query using less than or greater than operators with MongoDB by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/190
* chore: enable RESOLVE_FROM_ANCHOR_ORIGIN for orb by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/191
* feat: use round robin for orb domains by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/192
* feat: add UnanchoredMaxLifeTime option by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/194
* fix: check TransactionTime in checkUnanchoredDIDTime by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/195
* fix: read unix time in utc by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/196
* fix: Error when storing JSON to DocumentDB that use dots in field names by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/197
* feat: check max usage for cached update DID by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/198
* fix: Dots in nested array objects not escaping for DocumentDB by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/199
* chore: update to latest orb by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/200
* fix: don't set RecipientKeys and RoutingKeys if empty by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/202
* chore: add verify resolution result option by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/201
* feat: Support for faster InsertOne command in MongoDB Batch call by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/203
* chore: add tracing for vdr read by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/204
* feat: Wrap MongoDB duplicate key error by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/205
* chore: update maintainers list by @troyronda in https://github.com/hyperledger/aries-framework-go-ext/pull/208
* chore: configure http client in orb vdr by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/209
* chore: add option for custom http client by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/210
* chore: update to latest aries by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/211
* chore: add custom http client option by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/212
* fix: sidetree vdr by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/214
* chore: update to latest sidetree vdr by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/213
* chore: update http2 for http client by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/215
* feat: Allow for more than two tags in query for MongoDB by @bstasyszyn in https://github.com/hyperledger/aries-framework-go-ext/pull/216
* chore: update to latest orb by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/217
* chore: update orb to latest by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/218
* chore: remove check for published DID when update by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/219
* fix: vdr resolve to work with http hint by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/220
* chore: update to latest orb by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/221
* feat: add support to resolve with versionId or versionTime by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/222
* fix: replace GetSigningKey with GetSigner by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/223
* chore: Replace GetSigningKey with GetSigner in orb VDR by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/224
* Partial PostgreSQL storage provider implementation by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/225
* chore: support Ed25519VerificationKey2020 in VDR by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/226
* feat: PostgreSQL provider SetStoreConfig, Close and Query support by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/228
* chore: update  by @Moopli in https://github.com/hyperledger/aries-framework-go-ext/pull/231
* chore: update orb vdr to latest afgo and sidetree vdr by @Moopli in https://github.com/hyperledger/aries-framework-go-ext/pull/232
* fix: add dbname in right location in connect string by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/233
* chore: update afgo and edge-core dependencies to 0.1.8 by @Moopli in https://github.com/hyperledger/aries-framework-go-ext/pull/234
* chore: complete release for orb vdr by @Moopli in https://github.com/hyperledger/aries-framework-go-ext/pull/235
* fix: postgres default db by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/237
* chore: update to latest orb by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/238
* fix: Return error when using duplicate tag names in MongoDB and CouchDB by @DRK3 in https://github.com/hyperledger/aries-framework-go-ext/pull/239
* chore: update to latest aries in sidetree vdr by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/240
* chore: update to latest orb revision by @fqutishat in https://github.com/hyperledger/aries-framework-go-ext/pull/241

## New Contributors
* @ryjones made their first contribution in https://github.com/hyperledger/aries-framework-go-ext/pull/1
* @soluchok made their first contribution in https://github.com/hyperledger/aries-framework-go-ext/pull/5
* @DRK3 made their first contribution in https://github.com/hyperledger/aries-framework-go-ext/pull/15
* @pfeairheller made their first contribution in https://github.com/hyperledger/aries-framework-go-ext/pull/17
* @fqutishat made their first contribution in https://github.com/hyperledger/aries-framework-go-ext/pull/37
* @troyronda made their first contribution in https://github.com/hyperledger/aries-framework-go-ext/pull/53
* @Moopli made their first contribution in https://github.com/hyperledger/aries-framework-go-ext/pull/62
* @sandrask made their first contribution in https://github.com/hyperledger/aries-framework-go-ext/pull/77
* @llorllale made their first contribution in https://github.com/hyperledger/aries-framework-go-ext/pull/110
* @Baha-sk made their first contribution in https://github.com/hyperledger/aries-framework-go-ext/pull/114
* @0xArdi made their first contribution in https://github.com/hyperledger/aries-framework-go-ext/pull/149
* @aholovko made their first contribution in https://github.com/hyperledger/aries-framework-go-ext/pull/150
* @rolsonquadras made their first contribution in https://github.com/hyperledger/aries-framework-go-ext/pull/159
* @bstasyszyn made their first contribution in https://github.com/hyperledger/aries-framework-go-ext/pull/169

**Full Changelog**: https://github.com/hyperledger/aries-framework-go-ext/commits/component/vdr/orb/v1.0.0-rc.1
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-framework-go-ext/releases/tag/component/vdr/orb/v1.0.0-rc.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-04-12 20:08:51 +0000 UTC
    </span>
</div>

