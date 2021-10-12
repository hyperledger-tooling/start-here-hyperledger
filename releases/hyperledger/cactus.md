---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v1.0.0-rc1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.0.0-rc.1
                </span>
            </td>
            <td>
                # Change Log

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

# [1.0.0-rc.1](https://github.com/hyperledger/cactus/compare/v0.10.0...v1.0.0-rc.1) (2021-10-11)


### Bug Fixes

* **cmd-api-server:** enable version selection in plugins ([b982777](https://github.com/hyperledger/cactus/commit/b9827772fa6694381716686759f85f96b915662e)), closes [#839](https://github.com/hyperledger/cactus/issues/839) [#840](https://github.com/hyperledger/cactus/issues/840)
* **cmd-socker-server:** delete unnecessary files on cmd-socker-server ([20e15cd](https://github.com/hyperledger/cactus/commit/20e15cd257628fe392818e14728851304a76c7cb))
* **core-api:** modifications in openapi specs ([96c8b82](https://github.com/hyperledger/cactus/commit/96c8b82a642fdf106178ecdc47ff1f12fff229d1))
* openapi tests for besu, htlc-eth-besu and htlc-eth-besu-erc20 ([b9170e9](https://github.com/hyperledger/cactus/commit/b9170e929492f3305a420c75c7d12d06b288e0ab)), closes [#1291](https://github.com/hyperledger/cactus/issues/1291) [#847](https://github.com/hyperledger/cactus/issues/847)
* openapi validation test for fabric plugin ([01a5eb4](https://github.com/hyperledger/cactus/commit/01a5eb423abcc54aed8e2b4973251961e7849f76)), closes [#1295](https://github.com/hyperledger/cactus/issues/1295) [#847](https://github.com/hyperledger/cactus/issues/847)
* openapi validation test for iroha plugin ([6deed6d](https://github.com/hyperledger/cactus/commit/6deed6d3f070982061e33a11064ffb8d4e752f37)), closes [#1331](https://github.com/hyperledger/cactus/issues/1331) [#847](https://github.com/hyperledger/cactus/issues/847)
* **plugin-ledger-connector-quorum:** no keychain endpoints ([15cf65c](https://github.com/hyperledger/cactus/commit/15cf65cea6a779d12542b4ccc2e4940e7ac12039))
* **tools:** add docker network on tools/docker/sawtooth ledger ([8a0d182](https://github.com/hyperledger/cactus/commit/8a0d182e6badb3a6f10e40811390693e92628d1d))
* **tools:** fix the wallet config of fabcar chaincode on tools/docker/fabric ledger ([7ab0c44](https://github.com/hyperledger/cactus/commit/7ab0c44b488f441b31a8ef5dedd9ba9d2358ad78))
* **webpack:** prod build chokes on upgraded ssh2 binaries [#1405](https://github.com/hyperledger/cactus/issues/1405) ([18979fb](https://github.com/hyperledger/cactus/commit/18979fb33880d8ca30e2fda01fb3d598deb839f9))


### Features

* **besu-test-ledger:** added omitPull parameter to besu test ledger ([336a024](https://github.com/hyperledger/cactus/commit/336a0242e20b075736b1b008a478e65b4db3af8b))
* **cmd-server-socket:** add a communication test to open-api validators ([c1fe6a0](https://github.com/hyperledger/cactus/commit/c1fe6a0e0b6b84442adf2641393b8f744e76ab34))
* **cmd-server-socket:** add validator-registry setting ([1d1ce21](https://github.com/hyperledger/cactus/commit/1d1ce21a10244fc1b5a8a267d85a3f2beffc981e))
* **connector-go-ethereum:** add the docker environment ([2583cc7](https://github.com/hyperledger/cactus/commit/2583cc7ff7428a427454e7dd9211a129942e50d4))
* **connector-iroha-socket:** add sendAsyncRequest feature on connector ([6bad29b](https://github.com/hyperledger/cactus/commit/6bad29bddfb2a4ef3b98d7c8c4d41efad974bb56))
* **connector-quorum:** containerize plugin ([d016678](https://github.com/hyperledger/cactus/commit/d0166780215802c2e5bb6e895448ac687de0383c))
* **connector-sawtooth:** add the docker environment of Validator on connector-sawtooth-socketio ([7a57ea4](https://github.com/hyperledger/cactus/commit/7a57ea4adeb84bdf00bf32472ceac68fd43dc52d))
* **fabric-connector:** add transact receipt ([c6d1b7a](https://github.com/hyperledger/cactus/commit/c6d1b7a180025f84f055bf537b5263eb44b2511f))
* **keychain-aws-sm:** complete request handler and endpoint ([e6099b8](https://github.com/hyperledger/cactus/commit/e6099b86152a35ac7a21aecc02824410c05eac88)), closes [#967](https://github.com/hyperledger/cactus/issues/967) [#1349](https://github.com/hyperledger/cactus/issues/1349)
* **keychain-google-sm:** complete request handler and endpoints ([9c7bab5](https://github.com/hyperledger/cactus/commit/9c7bab5b06c7081421bcbfa1ae6aa8a3577a917e)), closes [#1097](https://github.com/hyperledger/cactus/issues/1097) [#1349](https://github.com/hyperledger/cactus/issues/1349)
* **tools:** substrate test ledger ([1a5edea](https://github.com/hyperledger/cactus/commit/1a5edeae834bc275252e588379f214324977a3ff))


            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cactus/releases/tag/v1.0.0-rc.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-10-12 00:28:53 +0000 UTC
    </span>
</div>

