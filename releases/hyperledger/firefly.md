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
                    v1.3.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.3.0
                </span>
            </td>
            <td>
                ## What's Changed
* Allow a message to contain two data items with the same hash by @awrichar in https://github.com/hyperledger/firefly/pull/1182
* remove near tutorial by @shorsher in https://github.com/hyperledger/firefly/pull/1183
* Fix typo in private & broadcast blob upload docs by @matthew1001 in https://github.com/hyperledger/firefly/pull/1185
* Fix configuration dynamic reload logic by @Chengxuan in https://github.com/hyperledger/firefly/pull/1194
* remove redundant reset by @Chengxuan in https://github.com/hyperledger/firefly/pull/1195
* Fix nightly integration tests by @nguyer in https://github.com/hyperledger/firefly/pull/1190
* Fix path in Fabric test-network tutorial by @nguyer in https://github.com/hyperledger/firefly/pull/1184
* Fail gracefully when inserting many data rows on sqlite by @awrichar in https://github.com/hyperledger/firefly/pull/1198
* Add "txid" and "txparent" to messages by @awrichar in https://github.com/hyperledger/firefly/pull/1163
* Call Features() getter to read DB provider features by @matthew1001 in https://github.com/hyperledger/firefly/pull/1197
* Fix spelling of "sequence" rewind and clarify API description by @awrichar in https://github.com/hyperledger/firefly/pull/1209
* Replace "UpsertBatch" with "InsertOrGetBatch" by @awrichar in https://github.com/hyperledger/firefly/pull/1208
* Re-poll immediately on full batch by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1204
* [tokens] Only Use broadcastName for Multi-Party Namespaces by @onelapahead in https://github.com/hyperledger/firefly/pull/1203
* [resolver] Unit Test for URL Encoding Key by @onelapahead in https://github.com/hyperledger/firefly/pull/1214
* Run Solidity tests on GitHub PRs by @awrichar in https://github.com/hyperledger/firefly/pull/1201
* Fix logging of blockchain event inserts by @awrichar in https://github.com/hyperledger/firefly/pull/1215
* Ensure cached transaction gets updated with new blockchain IDs by @awrichar in https://github.com/hyperledger/firefly/pull/1216
* `/api/v1/nextpins` route, complementing the `/api/v1/pins` route in problem diagnosis by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1212
* Correction of typos by @denisandreenko in https://github.com/hyperledger/firefly/pull/1218
* Propagate API context to announce in sync token pool creation cases by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1222
* Ensure that when we broadcast we use the org identity, not the default NS identity by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1223
* Add "intent" to address resolver plugin interface and API by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1226
* Do not reject messages from an unrecognized identity by @awrichar in https://github.com/hyperledger/firefly/pull/1224
* Fix minor typos and API example in docs by @matthew1001 in https://github.com/hyperledger/firefly/pull/1229
* Use the channel and signer to query transaction details from fabconnect by @matthew1001 in https://github.com/hyperledger/firefly/pull/1225
* Add version to log output and fix Dockerfile to include it by @nguyer in https://github.com/hyperledger/firefly/pull/1189
* Fix archive name for integration test logs by @nguyer in https://github.com/hyperledger/firefly/pull/1235
* Add an indxed column and simple query API for distinct sub-paths by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1236
* Validate and restore listeners on startup, and allow deletion if not found in connector by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1234
* Allow FireFly core to start, even if an individual Namespace cannot initialize by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1231
* Allow pinning a message to any blockchain contract invoke by @awrichar in https://github.com/hyperledger/firefly/pull/1213
* Cleanup around batches and transactions by @awrichar in https://github.com/hyperledger/firefly/pull/1202
* Resubmit any operations not yet in "Pending" state when an idempotency key clash is detected by @matthew1001 in https://github.com/hyperledger/firefly/pull/1230
* Actually start the legacy "ff_system" namespace when needed by @awrichar in https://github.com/hyperledger/firefly/pull/1246
* Do not update operations once they enter succeeded/failed state by @awrichar in https://github.com/hyperledger/firefly/pull/1257
* Add support for evmconnect's "execution reverted" error code by @awrichar in https://github.com/hyperledger/firefly/pull/1249
* Update CLI to v1.2.1 by @awrichar in https://github.com/hyperledger/firefly/pull/1260
* Fix coverage gaps from new operation update logic by @awrichar in https://github.com/hyperledger/firefly/pull/1259
* Allow operations to change between "Failed" and "Succeeded" by @awrichar in https://github.com/hyperledger/firefly/pull/1265
* Update rpc endpoints in polygon_testnet.md  by @Chengxuan in https://github.com/hyperledger/firefly/pull/1268
* Try out large runners to see if they are faster. by @ryjones in https://github.com/hyperledger/firefly/pull/1269
* Pass `key` on queries to blockchain, after resolving with an intent to query by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1271
* Re-establish active subscriptions after dynamic Namespace reload by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1242
* Update Swagger UI used in the docs site by @nguyer in https://github.com/hyperledger/firefly/pull/1258
* Check message on-chain consistency before initializing context by @awrichar in https://github.com/hyperledger/firefly/pull/1251
* Add guide for rotating DX certs by @nguyer in https://github.com/hyperledger/firefly/pull/1181
* Fix updating Contract APIs by @nguyer in https://github.com/hyperledger/firefly/pull/1275
* Fix timing issue between Init and ConfigReload of Namespace Manager by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1280
* Fix 1287 by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1288
* Address coverage gap, and issue with intent propagation found via it by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1281
* Accept private groupinit messages from any signing key by @awrichar in https://github.com/hyperledger/firefly/pull/1282
* Do not retry after a rejected message by @awrichar in https://github.com/hyperledger/firefly/pull/1278
* chore(ci): switch to dedicated Firefly runners by @ryjones in https://github.com/hyperledger/firefly/pull/1286
* Add proper WHERE clause to contract API updates by @awrichar in https://github.com/hyperledger/firefly/pull/1292
* chore: remove deprecated config by @EnriqueL8 in https://github.com/hyperledger/firefly/pull/1289
* Remove duplicates prior to adding unique index on contract API ID by @awrichar in https://github.com/hyperledger/firefly/pull/1293
* Handle duplicate pool locators properly by @awrichar in https://github.com/hyperledger/firefly/pull/1295
* Retry tokens events consistent with FFDX, as we cannot push back nack by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1296
* feat: Upgrade to latest ffresty with mTLS by @EnriqueL8 in https://github.com/hyperledger/firefly/pull/1290
* Fix unique indexes for transfers/approvals to be per-namespace by @awrichar in https://github.com/hyperledger/firefly/pull/1299
* fix: missing test coverage by @EnriqueL8 in https://github.com/hyperledger/firefly/pull/1300
* Confirm group init messages during dispatch by @awrichar in https://github.com/hyperledger/firefly/pull/1309
* Update to Go v1.19 by @nguyer in https://github.com/hyperledger/firefly/pull/1233
* Update firefly-common v1.2.11 and firefly-signer v1.1.8 by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1314
* Do not allow a batch to contain messages from different signing keys by @awrichar in https://github.com/hyperledger/firefly/pull/1313
* Derive batch signing key from messages in the batch by @awrichar in https://github.com/hyperledger/firefly/pull/1316
* Separate "define" and "publish" for token pools, and allow deleting unpublished pools by @awrichar in https://github.com/hyperledger/firefly/pull/1261
* feat: background start for connector plugins by @EnriqueL8 in https://github.com/hyperledger/firefly/pull/1315
* Unset handlers when namespaces are deleted (but not when they are just reloaded) by @nguyer in https://github.com/hyperledger/firefly/pull/1318
* chore(docs): fix discord link by @ryjones in https://github.com/hyperledger/firefly/pull/1320
* Separate "define" and "publish" for contract interfaces, and allow deleting unpublished interfaces by @awrichar in https://github.com/hyperledger/firefly/pull/1279
* Clean up remaining definition tests by @awrichar in https://github.com/hyperledger/firefly/pull/1321
* Separate "define" and "publish" for contract APIs, and allow deleting unpublished APIs by @awrichar in https://github.com/hyperledger/firefly/pull/1322
* Do not perform key resolution when looking up multiparty root org by @awrichar in https://github.com/hyperledger/firefly/pull/1329
* Add unit test for "delete contract API" route by @awrichar in https://github.com/hyperledger/firefly/pull/1327
* Perform nextpin calculations for both confirmed and rejected messages by @awrichar in https://github.com/hyperledger/firefly/pull/1326
* Process batch of events from Blockchain connector, in a single DB TX by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1331
* fix: multiple named tuple result from contract by @EnriqueL8 in https://github.com/hyperledger/firefly/pull/1333
* Move idempotency key architecture docs into main docs site by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1334
* Use a more optimistic approach when inserting token transfer events by @matthew1001 in https://github.com/hyperledger/firefly/pull/1291
* Update idempotency.md to fix sentence by @matthew1001 in https://github.com/hyperledger/firefly/pull/1335
* Surface message rejection reason to API by @awrichar in https://github.com/hyperledger/firefly/pull/1336
* Update Fabric chaincode Dockerfile by @lanasta in https://github.com/hyperledger/firefly/pull/1302
* Fix coverage drop in aggregator by @awrichar in https://github.com/hyperledger/firefly/pull/1337
* feat: TLS Configs for Webhooks by @EnriqueL8 in https://github.com/hyperledger/firefly/pull/1330
* docs: add mTLS section by @EnriqueL8 in https://github.com/hyperledger/firefly/pull/1325
* Fix uniqueness check in InsertOrGetFFI to match indexes by @awrichar in https://github.com/hyperledger/firefly/pull/1346
* FabConnect does not / can not set transactionIndex and eventIndex by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1345
* Use NetworkName instead of Name for definition topics by @awrichar in https://github.com/hyperledger/firefly/pull/1351
* feat: expose retry and HTTP options for webhooks by @EnriqueL8 in https://github.com/hyperledger/firefly/pull/1353
* Add E2E test for indexing an existing ERC1155 by @awrichar in https://github.com/hyperledger/firefly/pull/1352
* Remove token pools from the cache upon deletion by @awrichar in https://github.com/hyperledger/firefly/pull/1356
* Docs improvements by @ssmirr in https://github.com/hyperledger/firefly/pull/1348
* Do not set operation state to failed if we get a 409 - leave unchanged by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1361
* Postgres concurrency:true by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1342
* Batch insert of events all the way to the DB operations by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1343
* Further optimize blockchain transaction inserts to DB by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1354
* Add fftokens docs on /deactivatepool by @awrichar in https://github.com/hyperledger/firefly/pull/1332
* Automatically check operation status when querying pending transaction by @nguyer in https://github.com/hyperledger/firefly/pull/1341
* feat: batching events and webhook plugin support by @EnriqueL8 in https://github.com/hyperledger/firefly/pull/1359
* Log full payload of critical EVMConnect actions at DEBUG level by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1371
* Add httpOptions.proxyURL option to Subscription by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1372
* Detect partial success when performing batch insert of blockchain events by @awrichar in https://github.com/hyperledger/firefly/pull/1377
* Correctly parse blockchain subscription name when delivering events by @awrichar in https://github.com/hyperledger/firefly/pull/1378
* Add unit test for LIKE filters with escaped characters by @awrichar in https://github.com/hyperledger/firefly/pull/1364
* Prevent inserting token transfers with invalid blockchain event refs by @awrichar in https://github.com/hyperledger/firefly/pull/1386
* Update CODEOWNERS and MAINTAINERS.md by @nguyer in https://github.com/hyperledger/firefly/pull/1373
* Enrich events for contract deploy success/failure by @awrichar in https://github.com/hyperledger/firefly/pull/1391
* Two functions with the same param types, but different names, cannot share a cache entry by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1389
* Do not expect to retrieve local org during definition handling by @awrichar in https://github.com/hyperledger/firefly/pull/1398
* handle update for unpublished API by @Chengxuan in https://github.com/hyperledger/firefly/pull/1395
* Replace token pool "confirmed" state with "active" bool by @awrichar in https://github.com/hyperledger/firefly/pull/1305
* Enhance OpenAPI interface, for namespace-local APIs, and extra routing options by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1400
* Update README.md by @nguyer in https://github.com/hyperledger/firefly/pull/1399
* Fix SQL migration conflict and coverage gaps by @nguyer in https://github.com/hyperledger/firefly/pull/1401
* Tezos plugin support by @denisandreenko in https://github.com/hyperledger/firefly/pull/1402
* Update manifest by @denisandreenko in https://github.com/hyperledger/firefly/pull/1403
* check enabled for organization creation in non-multiparty system by @arinddas in https://github.com/hyperledger/firefly/pull/1405
* Fix table of contents view by @denisandreenko in https://github.com/hyperledger/firefly/pull/1409
* Fix database migration order by @nguyer in https://github.com/hyperledger/firefly/pull/1407
* Handle idempotent retry after error during initializing phase by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1406
* Add docs for AND/OR option by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1413
* namespace scoped web sockets by @hosie in https://github.com/hyperledger/firefly/pull/1419
* Documentation for working with the Tezos Blockchain by @denisandreenko in https://github.com/hyperledger/firefly/pull/1412
* Include "detail" param in Swagger for GET operation by @awrichar in https://github.com/hyperledger/firefly/pull/1420
* Call ResolveFFI from GenerateFFI by @awrichar in https://github.com/hyperledger/firefly/pull/1423
* DA-539 Update tezos docs by @denisandreenko in https://github.com/hyperledger/firefly/pull/1426
* Fix JSON schema output for custom contracts by @nguyer in https://github.com/hyperledger/firefly/pull/1427
* Definition conflicts should be HTTP 409 by @awrichar in https://github.com/hyperledger/firefly/pull/1430
* Add name/version if not specified by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1432
* Reflect through submissionRejected JSON body from FFTM/EVMConnect by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1436
* chore: start upgrade to firefly-common 1.4.1 by @SamMayWork in https://github.com/hyperledger/firefly/pull/1440
* typo: Inpsect vs Inspect by @torrespro in https://github.com/hyperledger/firefly/pull/1417
* Publish FFI with children by @nguyer in https://github.com/hyperledger/firefly/pull/1425
* Correct uniqueness lookup for nil location by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1433
* Docs/tezos by @denisandreenko in https://github.com/hyperledger/firefly/pull/1438
* Update log level in config auto reload by @nguyer in https://github.com/hyperledger/firefly/pull/1424
* Enable batch delivery over WebSockets by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1447
* feat: Add an API to allow for querying events under a subscription with additional filtering by @SamMayWork in https://github.com/hyperledger/firefly/pull/1452
* fix-1297 by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1298
* log: add debug logs for webhook by @EnriqueL8 in https://github.com/hyperledger/firefly/pull/1380
* Add Tezos connector to README by @alex-semenyuk in https://github.com/hyperledger/firefly/pull/1464
* DA-587 Update tezos docs (FFI section) by @denisandreenko in https://github.com/hyperledger/firefly/pull/1456
* Update comment to reflect availability with WebSockets by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1449
* Tezos Connector map converter by @alex-semenyuk in https://github.com/hyperledger/firefly/pull/1451
* fix: Merge ID into PATCH calls for identity if one is not provided by @SamMayWork in https://github.com/hyperledger/firefly/pull/1458
* fix: Status call returns properly when node is not registered but organisation is by @SamMayWork in https://github.com/hyperledger/firefly/pull/1467
* Update the FF manifest by @denisandreenko in https://github.com/hyperledger/firefly/pull/1448
* Intermittent unit tests by @Philip-21 in https://github.com/hyperledger/firefly/pull/1463
* adding vuln checks for high/critical severity by @ssmirr in https://github.com/hyperledger/firefly/pull/1462
* Update dependencies. Update to Go 1.21 by @nguyer in https://github.com/hyperledger/firefly/pull/1454
* Add map example to Tezos docs by @alex-semenyuk in https://github.com/hyperledger/firefly/pull/1468
* Fix contract method not found error by @nguyer in https://github.com/hyperledger/firefly/pull/1473
* Use non-root user in Docker image by @nguyer in https://github.com/hyperledger/firefly/pull/1439
* Update firefly-common by @nguyer in https://github.com/hyperledger/firefly/pull/1476
* Use separate event stream per namespace by @nguyer in https://github.com/hyperledger/firefly/pull/1388
* Update manifest.json by @nguyer in https://github.com/hyperledger/firefly/pull/1477
* Fix AssetManager startup retry by @nguyer in https://github.com/hyperledger/firefly/pull/1484
* Update UI to v1.3.0 by @nguyer in https://github.com/hyperledger/firefly/pull/1482
* Fix build tag in release GitHub action by @nguyer in https://github.com/hyperledger/firefly/pull/1480
* Upgrade to hardhat-toolbox for batch bin and custom pin contracts by @nguyer in https://github.com/hyperledger/firefly/pull/1479
* DeployContract implementation for Tezos connector by @alex-semenyuk in https://github.com/hyperledger/firefly/pull/1481
* Update Tezos documentation by @alex-semenyuk in https://github.com/hyperledger/firefly/pull/1488
* Update webhook docs by @EnriqueL8 in https://github.com/hyperledger/firefly/pull/1471
* feat: Add metrics for messaging when performing a token transfer by @EnriqueL8 in https://github.com/hyperledger/firefly/pull/1490
* Fix broken links at docs  by @alex-semenyuk in https://github.com/hyperledger/firefly/pull/1489
* Allow cancelling a batch that is stuck in dispatch by @awrichar in https://github.com/hyperledger/firefly/pull/1487
* Add documentation to outline how EVM revert errors are handled by @matthew1001 in https://github.com/hyperledger/firefly/pull/1493
* Update manifest.json for v1.3.0 by @nguyer in https://github.com/hyperledger/firefly/pull/1494
* update blockchain connector docs to match the latest by @Chengxuan in https://github.com/hyperledger/firefly/pull/1498
* Update the FF error docs to be in a more suitable place in the nav and give clearer out-of-the-box examples by @matthew1001 in https://github.com/hyperledger/firefly/pull/1499
* Upgrade psql client dependency by @nguyer in https://github.com/hyperledger/firefly/pull/1504
* Update token connectors by @nguyer in https://github.com/hyperledger/firefly/pull/1495
* Send start msg on reconnect for token connectors by @EnriqueL8 in https://github.com/hyperledger/firefly/pull/1502
* Add base API url to contract api result by @EnriqueL8 in https://github.com/hyperledger/firefly/pull/1501
* fix metrics when recording length of confirmed event by @EnriqueL8 in https://github.com/hyperledger/firefly/pull/1496
* Update manifest with evmconnect 1.3.8 by @EnriqueL8 in https://github.com/hyperledger/firefly/pull/1505
* Move doc site to new Hyperledger template by @nguyer in https://github.com/hyperledger/firefly/pull/1503
* docs: Prepare documentation for FireFly v1.3.0 by @SamMayWork in https://github.com/hyperledger/firefly/pull/1461

## New Contributors
* @denisandreenko made their first contribution in https://github.com/hyperledger/firefly/pull/1218
* @EnriqueL8 made their first contribution in https://github.com/hyperledger/firefly/pull/1289
* @lanasta made their first contribution in https://github.com/hyperledger/firefly/pull/1302
* @ssmirr made their first contribution in https://github.com/hyperledger/firefly/pull/1348
* @arinddas made their first contribution in https://github.com/hyperledger/firefly/pull/1405
* @hosie made their first contribution in https://github.com/hyperledger/firefly/pull/1419
* @SamMayWork made their first contribution in https://github.com/hyperledger/firefly/pull/1440
* @torrespro made their first contribution in https://github.com/hyperledger/firefly/pull/1417
* @alex-semenyuk made their first contribution in https://github.com/hyperledger/firefly/pull/1464
* @Philip-21 made their first contribution in https://github.com/hyperledger/firefly/pull/1463

**Full Changelog**: https://github.com/hyperledger/firefly/compare/v1.2.2...v1.3.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly/releases/tag/v1.3.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-04-25 16:12:46 +0000 UTC
    </span>
</div>

