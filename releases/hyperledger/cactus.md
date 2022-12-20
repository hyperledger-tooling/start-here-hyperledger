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
                    v1.1.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.1.3
                </span>
            </td>
            <td>
                # Change Log

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

## [1.1.3](https://github.com/hyperledger/cactus/compare/v1.1.2...v1.1.3) (2022-12-08)

### Bug Fixes

* **build:** sync-ts-config script needs import assertion of type json ([aa936ec](https://github.com/hyperledger/cactus/commit/aa936ec9e2c7b905c737c7721854c8b6bc305709)), closes [#2163](https://github.com/hyperledger/cactus/issues/2163)
* **connector-iroha:** fix review comments and smaller issues ([b2742e8](https://github.com/hyperledger/cactus/commit/b2742e8f6512f9804c6b4a943947b5bbe90785f0)), closes [PR#2048](https://github.com/PR/issues/2048)
* **odap-plugin:** fixes [#2198](https://github.com/hyperledger/cactus/issues/2198) - two gateways are using the same database ([9da24a0](https://github.com/hyperledger/cactus/commit/9da24a0ecd5e8682cbd6e6edbc349149b5d69d00))
* **plugin-ledger-connector-iroha:** running dockerfile locally ([f5faaab](https://github.com/hyperledger/cactus/commit/f5faaab75cecf22f588f0cdcb502952652fee058)), closes [#1874](https://github.com/hyperledger/cactus/issues/1874)
* **security:** vulnerabilities found in test-npm-registry ([4bbe012](https://github.com/hyperledger/cactus/commit/4bbe012d3db1f8264b19a2c822b45c72f46cb32c)), closes [#2061](https://github.com/hyperledger/cactus/issues/2061)
* **test-tooling:** substrate test ledger fails if WS_PORT not specified ([c668c41](https://github.com/hyperledger/cactus/commit/c668c41dcb4294530978e98349cd9158026d37e7)), closes [#2213](https://github.com/hyperledger/cactus/issues/2213)

### Features

* **cmd-socketio-server:** support multiple BLP in single server ([0f67085](https://github.com/hyperledger/cactus/commit/0f670855b0fa0fd33f71bf5a1814fb6fcac2c7b6)), closes [#2102](https://github.com/hyperledger/cactus/issues/2102) [#2030](https://github.com/hyperledger/cactus/issues/2030)
* **connector-iroha:** update-iroha-js ([74929b1](https://github.com/hyperledger/cactus/commit/74929b17869731adb67930429780cb5d33346d4a))
* **fabric-socketio-connector:** sending transactions signed on the client-side ([0b34ca3](https://github.com/hyperledger/cactus/commit/0b34ca3d35a39826c05cc047e480d377c1c52bef))
* **iroha2-ledger:** add Iroha V2 test ledger image and setup class ([6ff6aac](https://github.com/hyperledger/cactus/commit/6ff6aac7fff4669fca873ef40ae6b0818e70b5ec)), closes [#2138](https://github.com/hyperledger/cactus/issues/2138)
* monitoring, sync and async requests ([47da608](https://github.com/hyperledger/cactus/commit/47da608d378f5d48ca78b3d388b1c67da4c7aaf3)), closes [#1941](https://github.com/hyperledger/cactus/issues/1941)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cactus/releases/tag/v1.1.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-12-08 04:50:13 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v1.1.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.1.2
                </span>
            </td>
            <td>
                # Change Log

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

## [1.1.2](https://github.com/hyperledger/cactus/compare/v1.1.1...v1.1.2) (2022-11-11)

**Note:** Version bump only for package @hyperledger/cactus
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cactus/releases/tag/v1.1.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-11-11 17:40:35 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v1.1.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.1.1
                </span>
            </td>
            <td>
                # Change Log

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

## [1.1.1](https://github.com/hyperledger/cactus/compare/v1.1.0...v1.1.1) (2022-11-03)

### Bug Fixes

* **plugin-keychain-vault:** hyper upgrade ([3062343](https://github.com/hyperledger/cactus/commit/3062343d47a492d6a15f7189a72e6ab3bb6a52f2)), closes [#2120](https://github.com/hyperledger/cactus/issues/2120)
* **security:** vulnerabilities found in besu-all-in-one [#2055](https://github.com/hyperledger/cactus/issues/2055) ([2ce098f](https://github.com/hyperledger/cactus/commit/2ce098f490c0e20c7f5d00a81e8fced1ec81341c))
* **tools:** ghcr-quorum-multi-party-all-in-one pip install ([5809fd8](https://github.com/hyperledger/cactus/commit/5809fd8fac06638220bbe12df4f3ff82d02ef0eb)), closes [#2183](https://github.com/hyperledger/cactus/issues/2183)

### Features

* **cbdc-bridging-app:** refactor ODAP plugin implementation ([6975fef](https://github.com/hyperledger/cactus/commit/6975fefd4994cc9c6dd7d649dc2d6400646a59ae))
* **connector-iroha:** add dynamic request params ([a1f908f](https://github.com/hyperledger/cactus/commit/a1f908f4c27b652a15896c9847aee97cc6ea11fd))

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cactus/releases/tag/v1.1.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-11-04 00:16:24 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v1.1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.1.0
                </span>
            </td>
            <td>
                # Change Log

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

# [1.1.0](https://github.com/hyperledger/cactus/compare/v1.0.0...v1.1.0) (2022-10-17)

### Bug Fixes

* **api-server:** allow no authorization on socketio endpoints ([bf51960](https://github.com/hyperledger/cactus/commit/bf519608f39666e15cafd507c6defcfe956145a8)), closes [#1925](https://github.com/hyperledger/cactus/issues/1925)
* **cactus-example-discounted-asset-trade:** enable ([12e972e](https://github.com/hyperledger/cactus/commit/12e972e9cac63fd03a0ba3c7c8a29dc9ca544b9d)), closes [#2145](https://github.com/hyperledger/cactus/issues/2145)
* **cactus-example-electricity-trade:** enable tsconfig strict flag an… ([f7e726c](https://github.com/hyperledger/cactus/commit/f7e726c2720ed21bc4a582f6c4f345d0b2c65af7)), closes [#2144](https://github.com/hyperledger/cactus/issues/2144)
* **cactus-verifier-client:** update supported ledgers in readme ([84f3bae](https://github.com/hyperledger/cactus/commit/84f3bae982167d2d8c55ab44579f99dc5ee09c9f))
* custom-checks script from package.json does not work [#1809](https://github.com/hyperledger/cactus/issues/1809) ([dba3331](https://github.com/hyperledger/cactus/commit/dba33313c280ebf52117e18d2200c9abbfd4e694))
* **deps:** force minimist >=1.2.6 for CVE-2021-44906 ([b96806a](https://github.com/hyperledger/cactus/commit/b96806a0f30021eb39c47f7d9f54de8a16c5fb75)), closes [#1943](https://github.com/hyperledger/cactus/issues/1943)
* remove skip to pass test case ([99cb9a7](https://github.com/hyperledger/cactus/commit/99cb9a7fb22f112f32de333756f32ac13e588a54)), closes [#1957](https://github.com/hyperledger/cactus/issues/1957)
* resolve some CodeQL warnings ([824f5c8](https://github.com/hyperledger/cactus/commit/824f5c80ce5efbd9765699fdd635ab1d7f29cea2))
* **security:** address CVE-2017-16138 Fixes: [#1776](https://github.com/hyperledger/cactus/issues/1776) ([9f1d013](https://github.com/hyperledger/cactus/commit/9f1d01320cacf859bfd2e03426f85fb234f52dd8))
* **security:** address CVE-2021-23337 ([eccef40](https://github.com/hyperledger/cactus/commit/eccef405e5d6b33f3eebbb541eb07111c70301ed)), closes [#1778](https://github.com/hyperledger/cactus/issues/1778)
* **security:** address CVE-2021-23358 ([ed71f42](https://github.com/hyperledger/cactus/commit/ed71f42aca1683dd2fd6f762fbc6cd19b4c3c253)), closes [#1775](https://github.com/hyperledger/cactus/issues/1775)
* **security:** address CVE-2022-29244, CVE-2021-39135 ([7309f2a](https://github.com/hyperledger/cactus/commit/7309f2a8dc07d20fbffc9a2562f11e3140c8d79d)), closes [#2136](https://github.com/hyperledger/cactus/issues/2136)
* **security:** close DDoS vulnerability in eth tx consistenty strategy ([64b61a7](https://github.com/hyperledger/cactus/commit/64b61a742a885f0027543bc620b5db08b5444669)), closes [#2001](https://github.com/hyperledger/cactus/issues/2001)
* **security:** ensure node-forge > 1.3.0 for CVE-2022-24772 ([38fe287](https://github.com/hyperledger/cactus/commit/38fe287b958204d92a0353e369511120e38c625c)), closes [#1947](https://github.com/hyperledger/cactus/issues/1947)
* **security:** mitigate Cross-Site Scripting attack (XSS) ([2cb68c3](https://github.com/hyperledger/cactus/commit/2cb68c3e9899691b1e0abeb6993c37c97a61dcdb))

### Code Refactoring

* **examples:** include sample apps in monorepo build ([51ac163](https://github.com/hyperledger/cactus/commit/51ac1630f53ca3ac881341c7f8847b6ae581b220))

### Features

* add jwt authorization to supply chain example ([a4f07f6](https://github.com/hyperledger/cactus/commit/a4f07f6b1ea5b6cdd0397662cfbd9bb205a28bbe)), closes [#1579](https://github.com/hyperledger/cactus/issues/1579)
* **connector-fabric:** add GetBlock operation to fabric connectors ([00572ed](https://github.com/hyperledger/cactus/commit/00572edfafb82420f93570129e7e233a521f82e7)), closes [#2124](https://github.com/hyperledger/cactus/issues/2124)
* **connector-iroha:** sending transactions signed on the client-side ([da94cd6](https://github.com/hyperledger/cactus/commit/da94cd6b4fc5a364761716374ec7f6e7021bc76b))
* **corda4:** implement monitoring of state changes ([865ec2f](https://github.com/hyperledger/cactus/commit/865ec2f097df73e4907d812b18c2acf25e7896b1)), closes [#1610](https://github.com/hyperledger/cactus/issues/1610)
* **keychain-aws-sm:** bootstrap readme.md ([060f351](https://github.com/hyperledger/cactus/commit/060f3514a3dfaf19dab52345c0f0d2f80b12149c)), closes [#968](https://github.com/hyperledger/cactus/issues/968)
* **keychain-azure-kv:** complete request handler and endpoints ([932df10](https://github.com/hyperledger/cactus/commit/932df106734ec63146d1dc97d8db9c54d26086c6)), closes [#1010](https://github.com/hyperledger/cactus/issues/1010) [#1349](https://github.com/hyperledger/cactus/issues/1349)
* **odap-plugin:** addition of client endpoints ([cfa8db6](https://github.com/hyperledger/cactus/commit/cfa8db6c96e314bcefd6958b9823c4e0a5cf9620))
* **odap-plugin:** backup gateway implementation ([61da528](https://github.com/hyperledger/cactus/commit/61da5289cefe55527bf6ef3cd6204b6ae7002ce1))
* **odap-plugin:** odap crash recovery first implementation ([2e94ef8](https://github.com/hyperledger/cactus/commit/2e94ef8d3b34449c7b4d48e37d81245851477a3e))
* **quorum-connector:** implement validator interface on go-quorum-connector ([8d36bea](https://github.com/hyperledger/cactus/commit/8d36bea5146a544a2cb4615ec7291a1b425e568f)), closes [#1604](https://github.com/hyperledger/cactus/issues/1604)
* **sawtooth-ledger:** add single sawtooth test ledger image ([cd4c746](https://github.com/hyperledger/cactus/commit/cd4c7460f6e005ce56a0d79edea6f609756bf9d5)), closes [#2108](https://github.com/hyperledger/cactus/issues/2108) [#2030](https://github.com/hyperledger/cactus/issues/2030)
* **secret:** remove Validator/Verifier secret keys from repository ([59b4af4](https://github.com/hyperledger/cactus/commit/59b4af44835e2babafe398040a280ed23e9b490e))
* **socketio-server:** cross site scripting attack ([a5303ed](https://github.com/hyperledger/cactus/commit/a5303ed3a161477313646fc1f24220e53a20f7a4))
* **substrate-aio:** add ws-port argument ([fbb9859](https://github.com/hyperledger/cactus/commit/fbb9859584bdd5daf88424f3571ee4204a1e6ee3))

### BREAKING CHANGES

* **examples:** building discounted-asset-trade app (or any future app that use indy validator)
                 requires Indy SDK to be installed on the build machine.

Closes: 2029

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cactus/releases/tag/v1.1.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-10-19 04:32:13 +0000 UTC
    </span>
</div>

