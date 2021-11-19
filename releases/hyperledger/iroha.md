---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Hyperledger Iroha v1.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    1.3.0
                </span>
            </td>
            <td>
                # Hyperledger Iroha v1.3

Here is the list of changes that were implemented since Iroha v1.2.1:

## Features:

### Subscription engine #813

Subscription engine singleton #849
SE features update #914:
- thread pool
- subscribers creator
- weak connectivity between Engine and Subscribers
- engine is disposable
- switch between sync and async single-thread tasks
[Additional schedulers to dispatcher](https://github.com/hyperledger/iroha/commit/dd250b1e46ad48b5118911db4e43e2a8fc61c113)
[Stack-created subscriber is not allowed](https://github.com/hyperledger/iroha/commit/bbf35f85a12bf6400255a4e6d61a1a871e954468)
Is busy fixup #1366
Atomic busy check #1370
Repeat implementation #1410

Fixed thread pool tasks balancer #1271

### Metrics #943
- Add CMake files to .clang-format-ignore
- Disable prometheus-cpp logs
- Extend WSV to countDomains(), countTransactions(), countPeers()
- `-fno-lto` to link GCC-10 and clang with civetweb which was built with GCC-9
- Tests dependant on ametsuchi are linked against sync_subscription, not async
Metrics Uptime #1471

Prometheus metrics sample #841
Documentation #1346

### GitHub Actions #1028
A script to request tags of docker repository from DockerHub using curl and jq #1288
Improvements and fixes #1291, #1313, #1343, #1357, #1284, #1157, #1039
Fixed CI and automatic builds #1450, #1567, #1578, #1589
Better cathegories in CTest logs #1564

### RocksDB #1084

Added rocksdb initialization and basic functionality #954
RocksDB implementation for WsvCommand and WsvQuery #976
RocksDB implementation of Indexer #983
RocksDB command executor #1013
`Invalid precision` test fix for RocksDB implementation #1089
Fix: Read precision in SubstractAssetQuantity #1091
Specific query executor #1049
Block Store #1304
RocksDB cache #1335
Print current DB status on exit #1410
Memory leaks fixes #1410

### Tools for Migration to RocksDB
``wsv_checker`` #1294
Migration-tool #1320
Adding the tools to Docker #1426
Tests for tools iroha_migrate, iroha_wsv_diff #1597

### Proposal Creation Timeout #1011:
- Replace round delay with proposal creation timeout
- Send batches to current and next rounds
- Decouple Yac and OnDemandOrdering from rxcpp
- Asynchronous proposal request

### Optional gRPC Parameters #1048

### Additional Commands and Queries for Burrow #1326
*Implemented by this year's Hyperledger intern @Ayush-Jalan with @Baziorek as a mentor*
Documentation on new commands #1334
Missing queries integration to Burrow #1443

### Queries extension by modifing TxPaginationMeta #1092
*Implemented by this year's Hyperledger intern @Pawlak00 with @Baziorek as a mentor*
Extending ``GetPendingTransactions`` #1300


### Other Features

Async dispatcher implementation #962
Default log manager now reports config-file issues #951
Now CanAddPeer permission also allows the user to remove peers #1362


## Fixes

`reinterpret_pointer_cast` fix for clang build #909
No `--drop-state`  flag is needed for the first run anymore #900 (+ test fix #925)
Enabled `reinterpret_pointer_cast` for apple platform only to fix build #932
AmetsuchiTest: added condition for prepared block tests #952
`reinterpret_pointer_cast` moved to `iroha` namespace #1000
Iroha no longer freezes in GRPC when message of more than 4 MB are sent to it #1003
FlatFile: made the file close before rename #1012
Synchronization fix #1073
[Postgres_options_test fix](https://github.com/hyperledger/iroha/commit/989e6ade15fd5b4c0711d55c4d84a7d5c7397cf5)
Ordering Service batches cache + small block fixup #1327
Fixed integration tests #1347, 
Fixed integration tests #1347, #1378
Query permission test fix #1380
Fixed add_peer_test #1408
RocksDBWsvQuery: fixed buffer reuse in getPeerByPublicKey #1505
Fixed MST expiration #1488, #1489, #1490, #1521, #1557
YAC logical fixes #1410
Ordering Service removing duplicated transactions #1410
Prevented Ordering Service server from creating blocks when there are not enough transactions in the pool #1581
Restoring WSV Fix #1528, #1472
`GetTransactions` request fix #1410 
`on_demand_os_client_grpc` test freeze fix #1410 

## Infrastructure

Increase Windows CI disk size #918
Remove outdated usages of master branch #924
Fixed CI badge #1367
Added missing brew dep #1336
Added scripts/fix-dco.sh #1303

## Refactoring

Refactored YAC #1110
Removed `boost::adaptors::filter` which could be dereferenced multiple times causing performance decrease #869
Remove rxcpp #1004
Internal storage refactoring #1410 

## Docs

Fixed Links #912
Additional Information About Configuration + Small Documentation Build Fixes #879
PR template change #1002
Added description of metrics flags #1006
Fixed Config example in Docs #1037, #1360
Block Path Config Description #1080
Updated documentation requirements #1359, #1159
Configuration Fix #1360
Removed Doxygen build #1377
Docs: Migration Tool and WSV Checker Use #1412
Fixed Build Instructions #1503
Fixed Starting Container Instructions for RocksDB Iroha #1600

Main team preparing the release: @kuvaldini, @iceseer, @LiraLemur 

**Results of the Performance Testing can be found [here](https://wiki.hyperledger.org/display/iroha/Release+1.3.0)**
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/iroha/releases/tag/1.3.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-11-12 15:10:48 +0000 UTC
    </span>
</div>

