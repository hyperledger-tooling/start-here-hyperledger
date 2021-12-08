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
                    v1.0.0-rc.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.0.0-rc.3
                </span>
            </td>
            <td>
                # Change Log

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

# [1.0.0-rc.3](https://github.com/hyperledger/cactus/compare/v1.0.0-rc.2...v1.0.0-rc.3) (2021-12-07)


### Bug Fixes

* added a dummy package ([e1e8aee](https://github.com/hyperledger/cactus/commit/e1e8aee692dd0055e4f2b772590ad7386008c500)), closes [#1210](https://github.com/hyperledger/cactus/issues/1210)
* **cmd-api-server:** build occasionally broken - protoc-gen-ts [#1563](https://github.com/hyperledger/cactus/issues/1563) ([c2ecba5](https://github.com/hyperledger/cactus/commit/c2ecba54396d5e72b28d9ad538460d3bde2ca6d0))
* **cmd-api-server:** cockpit off by default [#1239](https://github.com/hyperledger/cactus/issues/1239) ([10344b5](https://github.com/hyperledger/cactus/commit/10344b574013209f1cb96e37a01d0d79e629be1f))
* **connector-corda:** add script to remove files before generate them ([58d1ce9](https://github.com/hyperledger/cactus/commit/58d1ce9d5fb176c1e3b9a55e1a4e6cd9c673f682)), closes [#1559](https://github.com/hyperledger/cactus/issues/1559)
* **connector-fabric:** chain code deployment fails >1 scp concurrency ([71c9063](https://github.com/hyperledger/cactus/commit/71c9063a70d3ea77264d631272e792d339ffb1e3)), closes [#1570](https://github.com/hyperledger/cactus/issues/1570)
* **connector-quorum:** transaction with different credentials [#1098](https://github.com/hyperledger/cactus/issues/1098) ([af6c240](https://github.com/hyperledger/cactus/commit/af6c24045f3696b3a64d64182afbd610c6409b17))
* **deps:** sibling package dependencies keychain-memory 0.6.0 [#1532](https://github.com/hyperledger/cactus/issues/1532) ([d01d72d](https://github.com/hyperledger/cactus/commit/d01d72d36200d47acac89f7ab90f6ddc96afba6f))
* endpoints implementation in corda plugin ([21a22b5](https://github.com/hyperledger/cactus/commit/21a22b574fb2e08c8c69106a6b3ecf1cb252c654)), closes [#1346](https://github.com/hyperledger/cactus/issues/1346)
* fixes 1445 and implementing correct interface types ([9022064](https://github.com/hyperledger/cactus/commit/9022064e245a92f71d2d303d77bfdaf64d1b1678)), closes [#1445](https://github.com/hyperledger/cactus/issues/1445)
* openapi validation for corda server endpoints ([21fc5ba](https://github.com/hyperledger/cactus/commit/21fc5ba874e0d1974a7e9524aff5103bb8af4b53))
* openapi validation for keychain-aws-sm plugin ([b270d28](https://github.com/hyperledger/cactus/commit/b270d2891d88149caa3de66096e727e82df0233e)), closes [#847](https://github.com/hyperledger/cactus/issues/847)
* **security:** remedy CVE-2021-3749 ([b33aa90](https://github.com/hyperledger/cactus/commit/b33aa904cfa3794357c77b24f464d41a325f1d80)), closes [#1569](https://github.com/hyperledger/cactus/issues/1569)
* **security:** upgrade fabric-common to 2.2.10 or later ([45c4a69](https://github.com/hyperledger/cactus/commit/45c4a69fb86964bc4e7018c31c5914a0063c7638)), closes [#1600](https://github.com/hyperledger/cactus/issues/1600)
* **supply-chain-app:** enable cockpit in supply-chain ([4a65b96](https://github.com/hyperledger/cactus/commit/4a65b96cfd83564343ec548c715946480ce228ea)), closes [#1622](https://github.com/hyperledger/cactus/issues/1622)
* **tools:** fix the names of scripts on README ([93360e1](https://github.com/hyperledger/cactus/commit/93360e12fa0e8af1d8c9fe73a3ebf955bc069201))


### Features

* **core-api:** add weaver protocol buffer definitions [#1523](https://github.com/hyperledger/cactus/issues/1523) ([851c071](https://github.com/hyperledger/cactus/commit/851c071e13e2ed3748a9c52ae9d02fb85d235c9a))
* **docs:** upated maintainers list ([b5c94dc](https://github.com/hyperledger/cactus/commit/b5c94dc744c48040b5cadd49b8903534ba5998d1))
* **example:** make cartrade support more environments ([e7e0402](https://github.com/hyperledger/cactus/commit/e7e04026059b7c1dfd1c5bd8c65f052651464966))
* **odap:** first implemenation for odap plugin and endpoints ([51bf753](https://github.com/hyperledger/cactus/commit/51bf753d421cdd255c178036fe901eb9c1c04130))
* **test-tooling:** embed couch-db image in the faio ([95d956d](https://github.com/hyperledger/cactus/commit/95d956d9bbfb15b15b043a753f07cbf876c33707))
* **test-tooling:** env injenction for Besu, Fabric, Quorum AIOs ([bb0352d](https://github.com/hyperledger/cactus/commit/bb0352dad85a1acbb4fc4b34026f39f289cfa9c0)), closes [#1580](https://github.com/hyperledger/cactus/issues/1580)
* **test-tooling:** faio features and improvements ([794e8b8](https://github.com/hyperledger/cactus/commit/794e8b89aba5a7bc6144343607893bca64affda1))


            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cactus/releases/tag/v1.0.0-rc.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-12-08 02:47:18 +0000 UTC
    </span>
</div>

