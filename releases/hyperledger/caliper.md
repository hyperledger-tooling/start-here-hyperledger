---
layout: default
title: caliper
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/caliper
---

# caliper <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/caliper){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Hyperledger Caliper v0.5.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.5.0
                </span>
            </td>
            <td>
                # Hyperledger Caliper v0.5.0

# Notable

## New features
✨ Official support for Node 14 and Node 16 for users and contributors
✨Experimental release for a Declaritive Workload Module
✨Support for the new Peer Gateway API introduced in Hyperledger Fabric 2.4

## Bug fixes
🐸 Fix Caliper round hang with unfinished transactions never completing
🐸 Corrections and Improvements to the documentation

## Breaking
💥Caliper no longer supports the 1.0 version of the Fabric Network Configuration format
💥Caliper no longer supports creating channels or deploying chaincode to Hyperledger Fabric
💥Caliper no longer supports Hyperledger Fabric 1.3 or older


# Complete list

## What's Changed
* bump to 0.4.3-unstable by @nklincoln in https://github.com/hyperledger/caliper/pull/1100
* Azure pipelines build by @nklincoln in https://github.com/hyperledger/caliper/pull/1105
* Enable builds for PRs that target master branch by @nklincoln in https://github.com/hyperledger/caliper/pull/1108
* Update contributing guide by @nklincoln in https://github.com/hyperledger/caliper/pull/1109
* publish to npm stage by @nklincoln in https://github.com/hyperledger/caliper/pull/1110
* update conditionals by @nklincoln in https://github.com/hyperledger/caliper/pull/1112
* update pipeline condition by @nklincoln in https://github.com/hyperledger/caliper/pull/1113
* Change build reason for publish by @nklincoln in https://github.com/hyperledger/caliper/pull/1114
* prevent cascade skip by @nklincoln in https://github.com/hyperledger/caliper/pull/1116
* Publish containers by @nklincoln in https://github.com/hyperledger/caliper/pull/1117
* use single publish script by @nklincoln in https://github.com/hyperledger/caliper/pull/1118
* use 0.21.1 axios by @nklincoln in https://github.com/hyperledger/caliper/pull/1119
* Adding changes related to value parameter for payable function in Ethereum. by @nachikettapas in https://github.com/hyperledger/caliper/pull/1122
* Make Mosquitto authentication and authorization explicit for v2 by @aklenik in https://github.com/hyperledger/caliper/pull/1128
* FIX: caliper bind command now compatible with Windows OS by @fransotodev in https://github.com/hyperledger/caliper/pull/1127
* Resolve issue in which only first round would be docker-monitored by @Viserius in https://github.com/hyperledger/caliper/pull/1135
* Added basic value providers in workload module by @bistaastha in https://github.com/hyperledger/caliper/pull/1164
* Added open in Visual Studio Code badge by @Justinjdaniel in https://github.com/hyperledger/caliper/pull/1170
* Update link for security bug handling wiki page by @aklenik in https://github.com/hyperledger/caliper/pull/1171
* Update branch name in Azure CI pipeline configuration by @aklenik in https://github.com/hyperledger/caliper/pull/1172
* Add factory class, formatted string and list element value providers. by @bistaastha in https://github.com/hyperledger/caliper/pull/1168
* Fix Besu integration test by @aklenik in https://github.com/hyperledger/caliper/pull/1174
* Fix Ethereum integration test by @aklenik in https://github.com/hyperledger/caliper/pull/1175
* Fix generator integration test by @aklenik in https://github.com/hyperledger/caliper/pull/1176
* Fix issue where init flow errors when not using mutual TLS by @davidkel in https://github.com/hyperledger/caliper/pull/1183
* Fix CompositeRateController class bug (#1181) by @aklenik in https://github.com/hyperledger/caliper/pull/1184
* Propose myself as a new caliper Maintainer by @davidkel in https://github.com/hyperledger/caliper/pull/1186
* Fix the unit of the interval of default-observer in the log by @justin-themedium in https://github.com/hyperledger/caliper/pull/1193
* Update CONTRIBUTING.md document by @aklenik in https://github.com/hyperledger/caliper/pull/1192
* Add GitHub web forms-based issue templates by @aklenik in https://github.com/hyperledger/caliper/pull/1189
* Value provider integration by @bistaastha in https://github.com/hyperledger/caliper/pull/1194
* address fabric:1.4 sut binding not working in caliper container by @davidkel in https://github.com/hyperledger/caliper/pull/1211
* Docker monitor metrics fixes - cpu and memory usage by @fraVlaca in https://github.com/hyperledger/caliper/pull/1214
* enable support for node 14  by @fraVlaca in https://github.com/hyperledger/caliper/pull/1219
* Node 14 support  by @fraVlaca in https://github.com/hyperledger/caliper/pull/1221
* Add new connector Wallet facade and Wallet facade Fatory on the peer-gateway folder by @fraVlaca in https://github.com/hyperledger/caliper/pull/1227
* Add support for node 16 by @davidkel in https://github.com/hyperledger/caliper/pull/1223
* Reference Discord instead of Rocket Chat by @davidkel in https://github.com/hyperledger/caliper/pull/1228
* Correct timeout defaults by @davidkel in https://github.com/hyperledger/caliper/pull/1230
* Bump version to 0.5.0-unstable by @davidkel in https://github.com/hyperledger/caliper/pull/1239
* Remove the legacy fabric connectors by @davidkel in https://github.com/hyperledger/caliper/pull/1235
* Update bindings to latest fabric sdks and remove old ones by @davidkel in https://github.com/hyperledger/caliper/pull/1244
* ensure endorsetimeout is set on v2 fabric connector by @davidkel in https://github.com/hyperledger/caliper/pull/1246
* add txid to proposal when doing a query by @davidkel in https://github.com/hyperledger/caliper/pull/1247
* Remove the need for gateway-enabled when binding to a fabric 2.2 SUT by @davidkel in https://github.com/hyperledger/caliper/pull/1255
* PeerGateway connector: Added new methods in the ConnectionProfileDefinition by @fraVlaca in https://github.com/hyperledger/caliper/pull/1253
* Improve integration tests by @davidkel in https://github.com/hyperledger/caliper/pull/1259
* improve message to help when file not found by @davidkel in https://github.com/hyperledger/caliper/pull/1262
* rename certain terms in code base by @davidkel in https://github.com/hyperledger/caliper/pull/1280
* Remove CountQueryAsLoad Option by @davidkel in https://github.com/hyperledger/caliper/pull/1276
* Caliper terminates if prometheus is not available by @davidkel in https://github.com/hyperledger/caliper/pull/1288
* Fabric Gateway connector implementation: PeerGateway.js implementation + unit tests by @fraVlaca in https://github.com/hyperledger/caliper/pull/1270
* fix RecordRate rate controller by @davidkel in https://github.com/hyperledger/caliper/pull/1292
* remove latency values if no successful txns in final report by @davidkel in https://github.com/hyperledger/caliper/pull/1290
* Update the usage examples to more appropriate versions by @davidkel in https://github.com/hyperledger/caliper/pull/1297
* Peer Gateway: Added Connector Selector implementation modifications to support the new Peer Gateway Connector by @fraVlaca in https://github.com/hyperledger/caliper/pull/1298
* Fixes for default.yaml in packages/caliper-core/lib/common/config/ and updates for the fabric Channel operations for the v1 fabric connector by @fraVlaca in https://github.com/hyperledger/caliper/pull/1306
* Peer Gateway: Integration tests for the new Peer Gateway connnector ( + update docker compose to use  by @fraVlaca in https://github.com/hyperledger/caliper/pull/1310
* Fixed colors dependency to 1.4.0 by @fraVlaca in https://github.com/hyperledger/caliper/pull/1311
* Change monitor intervals from milliseconds to seconds by @davidkel in https://github.com/hyperledger/caliper/pull/1314
* address worker cleanup when an error occurs by @davidkel in https://github.com/hyperledger/caliper/pull/1315
* Fixed docker monitor to use Dockerode only by @fraVlaca in https://github.com/hyperledger/caliper/pull/1319
* correct interval usage in fabric-tests by @davidkel in https://github.com/hyperledger/caliper/pull/1323
* Fix cli and update dependabot security dependencies by @davidkel in https://github.com/hyperledger/caliper/pull/1324
* Ensure that connector errors finishes caliper transactions by @davidkel in https://github.com/hyperledger/caliper/pull/1328
* disable logging debug to file by @davidkel in https://github.com/hyperledger/caliper/pull/1331
* add peers property support to fabric network config by @davidkel in https://github.com/hyperledger/caliper/pull/1329
* Upgraded node-sdk binding for fabric-v1-lts from 1.4.19 to 1.4.20 by @fraVlaca in https://github.com/hyperledger/caliper/pull/1332
* upgraded node-sdk binding for fabric-v2-lts from 2.2.11 to 2.2.12 by @fraVlaca in https://github.com/hyperledger/caliper/pull/1335
* Changed all 'bit.ly' links with a direct link by @fraVlaca in https://github.com/hyperledger/caliper/pull/1336
* Explicitly bind grpc-js for fabric 2.4 connector by @fraVlaca in https://github.com/hyperledger/caliper/pull/1344
* Peer Gateway Connector Txs Error messsage: added output of err.details array by @fraVlaca in https://github.com/hyperledger/caliper/pull/1345
* Fixes caliper hang of unfinished transactions by @davidkel in https://github.com/hyperledger/caliper/pull/1342
* [Release 0.5.0] Update Changelog by @davidkel in https://github.com/hyperledger/caliper/pull/1350
* [Release 0.5.0] Publish official release by @davidkel in https://github.com/hyperledger/caliper/pull/1349

## New Contributors
* @fransotodev made their first contribution in https://github.com/hyperledger/caliper/pull/1127
* @Viserius made their first contribution in https://github.com/hyperledger/caliper/pull/1135
* @Justinjdaniel made their first contribution in https://github.com/hyperledger/caliper/pull/1170
* @justin-themedium made their first contribution in https://github.com/hyperledger/caliper/pull/1193

**Full Changelog**: https://github.com/hyperledger/caliper/compare/v0.4.2...v0.5.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/caliper/releases/tag/v0.5.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-05-19 15:32:05 +0000 UTC
    </span>
</div>

