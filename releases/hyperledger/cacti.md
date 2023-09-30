---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0-alpha.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v2.0.0-alpha.2
                </span>
            </td>
            <td>
                
All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

# [2.0.0-alpha.2](https://github.com/hyperledger/cacti/compare/v2.0.0-alpha.1...v2.0.0-alpha.2) (2023-09-27)

### Bug Fixes

* **besu:** testnet web3 version fixed to 1.10.0 ([334612d](https://github.com/hyperledger/cacti/commit/334612d251c56811a844b3308dc1561dcd6fc460))
* **cactus-core-api:** address CVE-2021-38192 - GHSA-x4qm-mcjq-v2gf ([ff1afa5](https://github.com/hyperledger/cacti/commit/ff1afa5a6195399753c22f45837bbbf4ea27fe3c)), closes [#2612](https://github.com/hyperledger/cacti/issues/2612)
* **cactus-validator-socketio-indy:** upgrade pyjwt to 2.4.0 ([59f9f91](https://github.com/hyperledger/cacti/commit/59f9f916f2f931de3a9b83ea38070814db5875f9)), closes [#2614](https://github.com/hyperledger/cacti/issues/2614)
* **cmd-api-server:** fix CVE-2023-36665 protobufjs Prototype Pollution vuln ([7bb3957](https://github.com/hyperledger/cacti/commit/7bb39576080592919bea0ac89646b32105e1748e)), closes [#2682](https://github.com/hyperledger/cacti/issues/2682)
* **connector-fabric:** runTransactionV1 Open API validation crash ([516dd49](https://github.com/hyperledger/cacti/commit/516dd49fd443fc2d50b003104301b8060327b35a))
* ejs critical vulnerability CVE-2022-29078 ([2813b75](https://github.com/hyperledger/cacti/commit/2813b75bf5eebb7505ec05817c584324b3b6b149))
* **indy-validator:** fix package dependencies ([a28641a](https://github.com/hyperledger/cacti/commit/a28641ae47bd686af76d85ac22bcc84548211c59)), closes [#2596](https://github.com/hyperledger/cacti/issues/2596)
* **plugin-odap-hermes:** fix duplicate enum values of OdapMessageType ([292d287](https://github.com/hyperledger/cacti/commit/292d2876abdc8eedfe9b51ed70ed0bc32db63e48)), closes [#2553](https://github.com/hyperledger/cacti/issues/2553)
* **security:** crash in HeaderParser in dicer ([77fb559](https://github.com/hyperledger/cacti/commit/77fb559532448aae45cfe704da2637119bf93c27))
* **security:** the CVE-2022-2421 - upgrade socket.io-parser to >=4.2.1 ([9172172](https://github.com/hyperledger/cacti/commit/917217227a3fa53a00429f047cd6318862e6ab8d)), closes [#2229](https://github.com/hyperledger/cacti/issues/2229) [#2228](https://github.com/hyperledger/cacti/issues/2228)
* **security:** upgrade fabric 2.x deps to 2.2.18 ([36988a5](https://github.com/hyperledger/cacti/commit/36988a5edbf9856a1bcc960a3b9afe443536733e)), closes [#2610](https://github.com/hyperledger/cacti/issues/2610)
* **security:** vulnerabilities found in cactus-whitepaper ([c56334d](https://github.com/hyperledger/cacti/commit/c56334dd75e58e52a345fdafcbbe943ca6664aa4)), closes [#2038](https://github.com/hyperledger/cacti/issues/2038)
* **tessera:** updated tessera version error in quorum-all-in-one [#2411](https://github.com/hyperledger/cacti/issues/2411) ([759f305](https://github.com/hyperledger/cacti/commit/759f3055deba739cee426b089b30f29c0d0fca6c)), closes [#2240](https://github.com/hyperledger/cacti/issues/2240) [#2274](https://github.com/hyperledger/cacti/issues/2274)
* use common conventions: tsconfig.json, package.json ([50f5c02](https://github.com/hyperledger/cacti/commit/50f5c02190ba28b77492c09e81f5d5ba6578e862)), closes [#2216](https://github.com/hyperledger/cacti/issues/2216)
* **vscode/devcontainer:** unexpected exit stdout /etc/passwd ([eb0134b](https://github.com/hyperledger/cacti/commit/eb0134b3486e21014e926c43ba8cd3823c340c12)), closes [#2404](https://github.com/hyperledger/cacti/issues/2404)
* **weaver-corda:** throw error correctly in responder flows ([b888a5e](https://github.com/hyperledger/cacti/commit/b888a5e25aa54fa0a371a05524409b9bbbc2ce5d))
* **webpack:** fix broken bundling - cannot find webpack.config.js ([794f0b4](https://github.com/hyperledger/cacti/commit/794f0b4db6f352849b2d012c5034f0ed8d1903af))

### Code Refactoring

* **cmd-api-server:** clean up configuration parameters [#720](https://github.com/hyperledger/cacti/issues/720) ([b8e8388](https://github.com/hyperledger/cacti/commit/b8e8388306b6708c7d3156e005b1ee9693b35a22))

### Features

* **besu-test-ledger:** send funds to already created address ([3a58508](https://github.com/hyperledger/cacti/commit/3a585085b4510d9755e1d70314187293cbe51222)), closes [#2250](https://github.com/hyperledger/cacti/issues/2250)
* **cacti-cmd-gui-app:** add GUI to visualize Fabric, Ethereum blocks ([15d9e9d](https://github.com/hyperledger/cacti/commit/15d9e9dcdc072ac0f6be2bf5146102b1328faaaf))
* **cactus-common:** add createRuntimeErrorWithCause() & newRex() ([b3a508c](https://github.com/hyperledger/cacti/commit/b3a508c9a080e00a5e39ffa352a38e785b8cea9c)), closes [#1702](https://github.com/hyperledger/cacti/issues/1702)
* **cactus-core:** add GetOpenApiSpecV1EndpointBase<S, P> class ([6d68292](https://github.com/hyperledger/cacti/commit/6d68292f5bd88854f1d625631ce4c70f4151a02f))
* **cactus-plugin-ledger-connector-cdl-socketio:** add new connector plugin ([aee28fe](https://github.com/hyperledger/cacti/commit/aee28fee8ac6f386c8b95560f085daf2ec4965f8)), closes [#2455](https://github.com/hyperledger/cacti/issues/2455)
* **cactus-plugin-ledger-connector-ethereum:** add new connector plugin ([f8a2131](https://github.com/hyperledger/cacti/commit/f8a2131e9fc0ea05c1c1c8863489a43a74f019ae)), closes [#2534](https://github.com/hyperledger/cacti/issues/2534)
* **cbdc-bridging-app:** implementation of CBDC bridging example ([ca1b3be](https://github.com/hyperledger/cacti/commit/ca1b3be87bcc3242790647a71be8eb5db3dcd931)), closes [#2205](https://github.com/hyperledger/cacti/issues/2205)
* **cmd-api-server:** add GetOpenApiSpecV1Endpoint (HTTP GET) ([aeebbd4](https://github.com/hyperledger/cacti/commit/aeebbd4d86cb62f8d1d53fded65ae40eb5e27910))
* **connector-besu:** add GetOpenApiSpecV1Endpoint (HTTP GET) ([76744f0](https://github.com/hyperledger/cacti/commit/76744f0f7b6629959f59939de0fea0f71ff7a5f0))
* **connector-iroha2:** update to the new LTS image as of 28.07.2023 ([ccdaa12](https://github.com/hyperledger/cacti/commit/ccdaa1254cb4d46cc6a0af2c0472f3838603123f))
* **connector-quorum:** add WebsocketProvider options to quorum LP ([b7ad571](https://github.com/hyperledger/cacti/commit/b7ad571e77c6b9e2abb2b5ab8ecd7ffb93172747))
* **connector-tcs-huawei:** add initial version ([d8d538d](https://github.com/hyperledger/cacti/commit/d8d538d42692ddf01ef24327cb31bd8e6cd48c01))
* corda asset transfer test workflow added and bug fixes ([4b5ee09](https://github.com/hyperledger/cacti/commit/4b5ee095b07f7c6a4290cfb85280d825672ce394))
* **fabric-test-ledger:** add support to enrolling users in different Orgs ([b910681](https://github.com/hyperledger/cacti/commit/b9106810db11a2af19c8c06d6be39d2648f96fba)), closes [#2248](https://github.com/hyperledger/cacti/issues/2248)
* **geth-all-in-one:** add ethereum test image and helper class ([fb4231f](https://github.com/hyperledger/cacti/commit/fb4231f3e8ddc2b7c4aadddf62dac759b7a62d44)), closes [#2577](https://github.com/hyperledger/cacti/issues/2577)
* **openapi:** upgrade to 6.3.0 phase1 ([a094614](https://github.com/hyperledger/cacti/commit/a094614877d6043a6e3e8c0b3e95203eed7d6203)), closes [#2298](https://github.com/hyperledger/cacti/issues/2298)
* **plugin-htlc-eth-besu:** add private HTLCs and forge build & test ([aade510](https://github.com/hyperledger/cacti/commit/aade510c5fc13199006466aecd8235130d6ec353))
* **plugin-persistence-fabric:** add new fabric persistence plugin ([47a64ee](https://github.com/hyperledger/cacti/commit/47a64ee17446db8102e2ca95f16b26f8778175a4)), closes [#2259](https://github.com/hyperledger/cacti/issues/2259) [#2265](https://github.com/hyperledger/cacti/issues/2265)
* **quorum-connector:** add script for checking connection status ([d306d21](https://github.com/hyperledger/cacti/commit/d306d211ebaa30b700dce4277c09531ba88d7952)), closes [#2309](https://github.com/hyperledger/cacti/issues/2309)
* **quorum:** private transaction support ([3c944d6](https://github.com/hyperledger/cacti/commit/3c944d601d5824eaf3cc6a9a8af1f8a6e5fe6db3))
* **weaver-corda:** support array of remote views, consequent user flow call ([a8e5d54](https://github.com/hyperledger/cacti/commit/a8e5d5425b2db21d2a72282729c61b1073c000a6))
* **weaver/common:** add data view protocol buffer spec & RFCs for Besu ([97f17e0](https://github.com/hyperledger/cacti/commit/97f17e0deb86621d818c5ac7b3f30595fe82fe03))
* **weaver:** added multiple participants support for data sharing in corda ([4e81b92](https://github.com/hyperledger/cacti/commit/4e81b929ea4996b345616e6a579dccdedc295de3))

### BREAKING CHANGES

* **cmd-api-server:** Removed the `keyPairPem` parameter from the API server
configuration.
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/v2.0.0-alpha.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-09-29 20:40:47 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0-alpha.2 - GO Fabric Weaver SDK - Sep 29, 2023
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    weaver/sdks/fabric/go-sdk/v2.0.0-alpha.2
                </span>
            </td>
            <td>
                - Go Module: `github.com/hyperledger/cacti/weaver/sdks/fabric/go-sdk`
- Release: v2.0.0-alpha.2
- Readme: [Here](https://github.com/hyperledger/cacti/blob/weaver/sdks/fabric/go-sdk/v2.0.0-alpha.2/weaver/sdks/fabric/go-sdk/README.md).
- Source: [Here](https://github.com/hyperledger/cacti/blob/weaver/sdks/fabric/go-sdk/v2.0.0-alpha.2/weaver/sdks/fabric/go-sdk)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/weaver/sdks/fabric/go-sdk/v2.0.0-alpha.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-09-29 16:57:53 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0-alpha.2 - GO Fabric Utils Library for Interoperation - Sep 29, 2023
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    weaver/core/network/fabric-interop-cc/libs/utils/v2.0.0-alpha.2
                </span>
            </td>
            <td>
                - Go Module: `github.com/hyperledger/cacti/weaver/core/network/fabric-interop-cc/libs/utils`
- Release: v2.0.0-alpha.2
- Readme: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/libs/utils/v2.0.0-alpha.2/weaver/core/network/fabric-interop-cc/libs/utils/README.md).
- Source: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/libs/utils/v2.0.0-alpha.2/weaver/core/network/fabric-interop-cc/libs/utils)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/weaver/core/network/fabric-interop-cc/libs/utils/v2.0.0-alpha.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-09-29 16:57:53 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0-alpha.2 - GO Fabric Library for Asset Exchange - Sep 29, 2023
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    weaver/core/network/fabric-interop-cc/libs/assetexchange/v2.0.0-alpha.2
                </span>
            </td>
            <td>
                - Go Module: `github.com/hyperledger/cacti/weaver/core/network/fabric-interop-cc/libs/assetexchange`
- Release: v2.0.0-alpha.2
- Readme: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/libs/assetexchange/v2.0.0-alpha.2/weaver/core/network/fabric-interop-cc/libs/assetexchange/README.md).
- Source: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/libs/assetexchange/v2.0.0-alpha.2/weaver/core/network/fabric-interop-cc/libs/assetexchange)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/weaver/core/network/fabric-interop-cc/libs/assetexchange/v2.0.0-alpha.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-09-29 16:57:53 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0-alpha.2 - GO Fabric Asset Management Interface - Sep 29, 2023
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt/v2.0.0-alpha.2
                </span>
            </td>
            <td>
                - Go Module: `github.com/hyperledger/cacti/weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt`
- Release: v2.0.0-alpha.2
- Readme: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt/v2.0.0-alpha.2/weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt/README.md).
- Source: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt/v2.0.0-alpha.2/weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt/v2.0.0-alpha.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-09-29 16:57:53 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0-alpha.2 - GO Fabric Interop Chaincode - Sep 29, 2023
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    weaver/core/network/fabric-interop-cc/contracts/interop/v2.0.0-alpha.2
                </span>
            </td>
            <td>
                - Go Module: `github.com/hyperledger/cacti/weaver/core/network/fabric-interop-cc/contracts/interop`
- Release: v2.0.0-alpha.2
- Readme: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/contracts/interop/v2.0.0-alpha.2/weaver/core/network/fabric-interop-cc/contracts/interop/README.md).
- Source: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/contracts/interop/v2.0.0-alpha.2/weaver/core/network/fabric-interop-cc/contracts/interop)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/weaver/core/network/fabric-interop-cc/contracts/interop/v2.0.0-alpha.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-09-29 16:57:53 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0-alpha.2 - GO Weaver Protos - Sep 29, 2023
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    weaver/common/protos-go/v2.0.0-alpha.2
                </span>
            </td>
            <td>
                - Go Module: `github.com/hyperledger/cacti/weaver/common/protos-go`
- Release: v2.0.0-alpha.2
- Readme: [Here](https://github.com/hyperledger/cacti/blob/weaver/common/protos-go/v2.0.0-alpha.2/weaver/common/protos-go/README.md).
- Source: [Here](https://github.com/hyperledger/cacti/blob/weaver/common/protos-go/v2.0.0-alpha.2/weaver/common/protos-go)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/weaver/common/protos-go/v2.0.0-alpha.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-09-29 16:57:53 +0000 UTC
    </span>
</div>

