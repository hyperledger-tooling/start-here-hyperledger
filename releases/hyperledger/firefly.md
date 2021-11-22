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
                    v0.11.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.11.0
                </span>
            </td>
            <td>
                ## What's Changed
* Move e2e to new routes, and add private/broadcast strong datatype tests by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/260
* Added more tests to the Fabric plugin for 100% coverage by @jimthematrix in https://github.com/hyperledger/firefly/pull/261
* Do not allow UUIDs to be used as names by @awrichar in https://github.com/hyperledger/firefly/pull/262
* Fix logic for transfer+message with waitConfirm=true by @awrichar in https://github.com/hyperledger/firefly/pull/258
* Do not use tokenIndex in E2E test for fungible tokens by @awrichar in https://github.com/hyperledger/firefly/pull/264
* Use firefly_e2e instead of firefly-e2e for container names by @awrichar in https://github.com/hyperledger/firefly/pull/266
* Adjust version for firefly-tokens-erc1155 by @awrichar in https://github.com/hyperledger/firefly/pull/267
* Allow nested RunAsGroup calls by @awrichar in https://github.com/hyperledger/firefly/pull/270
* Split asset manager into multiple files by @awrichar in https://github.com/hyperledger/firefly/pull/268
* New GET routes for tokens by @awrichar in https://github.com/hyperledger/firefly/pull/275
* Add extra columns to token tables for UI support by @awrichar in https://github.com/hyperledger/firefly/pull/276
* Additional E2E coverage for tokens by @awrichar in https://github.com/hyperledger/firefly/pull/274
* introduce FFTime.Time() by @shorsher in https://github.com/hyperledger/firefly/pull/277
* pools-by-connector Add connector field to TokenPoolQueryFactory by @eberger727 in https://github.com/hyperledger/firefly/pull/280
* tokens-by-id getTokenPoolByNameOrID() and getTokenTransfersByID() by @eberger727 in https://github.com/hyperledger/firefly/pull/278
* Update GitHub actions to build every merge to main by @nguyer in https://github.com/hyperledger/firefly/pull/286
* Group token database calls into RunAsGroup wherever possible by @awrichar in https://github.com/hyperledger/firefly/pull/273
* Fix PSQL migration with invalid AUTOINCREMENT by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/289
* Add topic+tag index to messages by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/290
* Add namespace field to token accounts and transfers by @awrichar in https://github.com/hyperledger/firefly/pull/287
* Fix duplicate db migration 00037 by @awrichar in https://github.com/hyperledger/firefly/pull/295
* Update DX dependency, and go deps including bluemonday for CVE-2021-42576 by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/285
* Update docs and add new guides by @nguyer in https://github.com/hyperledger/firefly/pull/284
* Collapse message bools into a new "state" field by @awrichar in https://github.com/hyperledger/firefly/pull/296
* Run E2E tests with matrix including fabric by @nguyer in https://github.com/hyperledger/firefly/pull/242
* Use single quotes for strings in postgres migration by @awrichar in https://github.com/hyperledger/firefly/pull/302
* Small doc updates by @awrichar in https://github.com/hyperledger/firefly/pull/301
* Replace BeforeSend callback with a Prepare method by @awrichar in https://github.com/hyperledger/firefly/pull/283
* remove-member-field Removing member field from operations table by @eberger727 in https://github.com/hyperledger/firefly/pull/300
* Add `?fetchdata` on messages collection to include data, and make consistent with get by ID by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/299
* Allow did:firefly:org/xyz prefix on group input by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/304
* Add scheduled E2E test using latest services by @nguyer in https://github.com/hyperledger/firefly/pull/292
* Add check before writing to websocket channel by @nguyer in https://github.com/hyperledger/firefly/pull/298
* Add jobs for database migration and auto-registration by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/294
* Update assertion on unit test to pass on Go 1.17 by @nguyer in https://github.com/hyperledger/firefly/pull/303
* Only send transfer message if token transfer is successful by @awrichar in https://github.com/hyperledger/firefly/pull/297
* Consume websocket events in "strong datatype" tests by @awrichar in https://github.com/hyperledger/firefly/pull/309
* POST /tokens/<mint | burn | transfers | pools> by @eberger727 in https://github.com/hyperledger/firefly/pull/307
* Split the notions of "token balances" and "token accounts" by @awrichar in https://github.com/hyperledger/firefly/pull/311
* Always pass key and message hash to fftokens connector by @awrichar in https://github.com/hyperledger/firefly/pull/305
* Use WriteByte instead of WriteRune when possible by @awrichar in https://github.com/hyperledger/firefly/pull/314
* Additional cleanup to support tokens UI by @awrichar in https://github.com/hyperledger/firefly/pull/313
* Prometheus Metrics for Mux Router by @hfuss in https://github.com/hyperledger/firefly/pull/321
* Allow specifying pool by name or ID for transfer requests by @awrichar in https://github.com/hyperledger/firefly/pull/320
* Fix COUNT for SQL queries that use DISTINCT by @awrichar in https://github.com/hyperledger/firefly/pull/319
* add build badge by @shorsher in https://github.com/hyperledger/firefly/pull/327
* Replace token pool "validate tx" logic stubs with a new "activate" action by @awrichar in https://github.com/hyperledger/firefly/pull/317
* Upsert optimization by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/325
* Change JSONB columns to BYTEA - issue : Remove use of JSONB columns #324 by @hypefi in https://github.com/hyperledger/firefly/pull/330
* bump UI version to 0.4.1 by @shorsher in https://github.com/hyperledger/firefly/pull/332
* Update dependencies for v0.11.0 release by @nguyer in https://github.com/hyperledger/firefly/pull/333

## New Contributors
* @eberger727 made their first contribution in https://github.com/hyperledger/firefly/pull/280
* @hypefi made their first contribution in https://github.com/hyperledger/firefly/pull/330

**Full Changelog**: https://github.com/hyperledger/firefly/compare/v0.10.1...v0.11.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly/releases/tag/v0.11.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-11-22 16:01:34 +0000 UTC
    </span>
</div>

