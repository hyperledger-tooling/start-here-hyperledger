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
                    v0.6.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.6.0
                </span>
            </td>
            <td>
                # [0.6.0](https://github.com/petermetz/cactus/compare/v0.4.1...v0.6.0) (2021-07-19)


### Bug Fixes

* **carbon-accounting:** deleted incorrect plugin aspect ([e30f48a](https://github.com/petermetz/cactus/commit/e30f48abcc8dfcd6fb17ec1ba90c4e742222543f))
* **ci:** dependent issues bot workflow has no job id [#848](https://github.com/petermetz/cactus/issues/848) ([af61202](https://github.com/petermetz/cactus/commit/af61202f73b72efe6df31e5697eedd94f84d417c))
* **cmd-api-server:** config-service example - authorization JSON ([a209fef](https://github.com/petermetz/cactus/commit/a209feffdea47f0992f17a7c0265535614143dfe))
* **cmd-api-server:** drop URI type alt name from self signed TLS cert ([eb5d1df](https://github.com/petermetz/cactus/commit/eb5d1dfaf8523690008c1c1c0aaa0b0efedb2cba))
* **cmd-api-server:** no CLI args causes crash [#794](https://github.com/petermetz/cactus/issues/794) ([a285b96](https://github.com/petermetz/cactus/commit/a285b96785792cd29f450bfc1cc066067c82f558))
* **connector-besu:** network update only if present in keychain ([8ac2444](https://github.com/petermetz/cactus/commit/8ac2444f86f9a1310f045ff0f7e4e78b91635be0))
* **connector-besu:** remove magic strings ([6d9ae53](https://github.com/petermetz/cactus/commit/6d9ae53c64bd4e6c3eb33164bfa5d5507582220b)), closes [#1104](https://github.com/petermetz/cactus/issues/1104)
* **connector-besu:** removed repeated check ([a4cb63b](https://github.com/petermetz/cactus/commit/a4cb63b483d61578dd0d356fc0c9c20d8a2024e0))
* **connector-corda:** container image kotlin compilation fails in model ([a8a4531](https://github.com/petermetz/cactus/commit/a8a4531d379fe16d4c991802525ec573a7e3ede1))
* **connector-corda:** kotlin compilation error due to missing method ([403f135](https://github.com/petermetz/cactus/commit/403f13592734cfdcbbfa3714b76a9557aaa4a8b4))
* **connector-fabric:** export IPluginLedgerConnectorFabricOptions ([ada532e](https://github.com/petermetz/cactus/commit/ada532ef09603727379b6193b175e2834fa803d3))
* **connector-quorum:** web3 Contract type usage ([80c8253](https://github.com/petermetz/cactus/commit/80c82536f6446896a07aab9276f93598266ea5c3))
* **connector-xdai:** add missing hasTransactionFinality ([cc4f3e1](https://github.com/petermetz/cactus/commit/cc4f3e141da9292b8db5b0261a3347b3ba9c0689))
* **connector-xdai:** web3.eth.estimateGas, works considering called solidity method do not throw an exception. So, for method having modifier with access control on msg.sender calling estimateGas without from field throws error.to make it work ,transactionConfig.from = web3SigningCredential.ethAccount before calling estimateGas ([63f5ff6](https://github.com/petermetz/cactus/commit/63f5ff62b20aaf4dfdb5dd48a24dabc3342a0868))
* **deps:** elliptic upgrade to >6.5.3 for CVE-2020-28498 ([d75b9af](https://github.com/petermetz/cactus/commit/d75b9af764241ab2e10914769412201fb040b1ed))
* **example:** fix README and add script to cleanup app data after test ([b07bde4](https://github.com/petermetz/cactus/commit/b07bde41de04e80d913b929e42a55eef5141fd2f))
* **examples:** supply chain backend bundle build RAM [#766](https://github.com/petermetz/cactus/issues/766) ([f5c5d82](https://github.com/petermetz/cactus/commit/f5c5d82ef3ae327f057da94ea12a224f9b4d78c6))
* fixing branch name for code cov badge ([d79d965](https://github.com/petermetz/cactus/commit/d79d96525e2117683e20a8442fd4efbfaf32e55b))
* **github/workflows:** dependent issues job name typo ([0b4e333](https://github.com/petermetz/cactus/commit/0b4e333fe81b12352258159d35e61f0108df1212))
* keychain to registry, uuid dep, add back missing gas req parameter ([4635d81](https://github.com/petermetz/cactus/commit/4635d817a719bcdaa2a3bf1b4aa3b5d8cc1f6961))
* **readthedocs:** updated readthedocs file ([645f47d](https://github.com/petermetz/cactus/commit/645f47de0304f3ade38dfedc056159a613f3f005))
* **test:** eliminate CVE-2020-8203 in besu connector test pkg ([6411933](https://github.com/petermetz/cactus/commit/6411933a167711152165d86a260d5f49d272746d))
* **tools:** ci.sh retry mechanism no longer ignores last failure ([b5e751e](https://github.com/petermetz/cactus/commit/b5e751e405d0c612f71c50fa964600134d25e0c2))
* **tools:** fix a typo of README on iroha-testnet ([1b333cd](https://github.com/petermetz/cactus/commit/1b333cdc8757ec4733ec0189d092ada7c827023d))
* **tools:** use latest fabric bootstrap.sh script for AIO image ([b298b76](https://github.com/petermetz/cactus/commit/b298b76a03382fa2729b89a6066b693e3c072582))
* **typo:** fix typo of bisiness ([142cd56](https://github.com/petermetz/cactus/commit/142cd569c2c681042c592443b57108a127a8b820))
* **Validator,verifier:** delete some minor duplicated files ([9acb8ab](https://github.com/petermetz/cactus/commit/9acb8abfa52f1dc576abb755431cfa85d94b34e6))
* **whitepaper:** build fails on Ubuntu 18 due to glibc 2.29 [#703](https://github.com/petermetz/cactus/issues/703) ([ec22a0f](https://github.com/petermetz/cactus/commit/ec22a0fc94929ae0fe8b44f93ce20f44847ec176))
* **whitepaper:** fix rendering ([d64f3cd](https://github.com/petermetz/cactus/commit/d64f3cd9cc6fd2c3998d139f1872f2c3eaeffc60))


### Features

* add SocketIoConnectionPathV1 constant to OpenAPI specs ([405865d](https://github.com/petermetz/cactus/commit/405865d02e57031c1531431a4a46b96a1b9aff03))
* adding additional info into err logs ([888f85a](https://github.com/petermetz/cactus/commit/888f85a680a330cfc6be98bab3e8aed5d9e9dde2)), closes [#295](https://github.com/petermetz/cactus/issues/295)
* **api-server:** ability to install plugins at runtime [#764](https://github.com/petermetz/cactus/issues/764) ([8dda0f6](https://github.com/petermetz/cactus/commit/8dda0f61937c6e1a85afee0345af44b1bfa09c0a))
* **api-server:** publish API server docker image ([ad7b221](https://github.com/petermetz/cactus/commit/ad7b2211305bcefb044701276a56d5ad09d8468c))
* **atomic-swap-erc20:** implemented plugin and test ([0c9423a](https://github.com/petermetz/cactus/commit/0c9423a2a2cd4675c3c6dec4288190f148cad938))
* besu WatchBlocksV1Endpoint with SocketIO ([d5e1708](https://github.com/petermetz/cactus/commit/d5e1708e84ab5192d07410d5120e144d477ef6ce))
* **besu:** add sequence diagram of run transaction endpoint ([754a11a](https://github.com/petermetz/cactus/commit/754a11a449d9a67dd8d6ebecbeb1b65cefa71b7f)), closes [#755](https://github.com/petermetz/cactus/issues/755)
* **cmd-api-server:** add Socket.IO as transport [#297](https://github.com/petermetz/cactus/issues/297) ([51c586a](https://github.com/petermetz/cactus/commit/51c586aa01bff3e75f0e87be43f0764b30d8222c))
* **cmd-api-server:** container image definition ([eb69fff](https://github.com/petermetz/cactus/commit/eb69fff36fca805c6b96c6db7caadfbed85e8485))
* **cmd-api-server:** user defined type guard isHealthcheckResponse ([16077d4](https://github.com/petermetz/cactus/commit/16077d42ec7edce4999d77cfbca5c02177d15fa6))
* **connector-besu, connector-quorum:** filesystem replaced by keychain ([14d1790](https://github.com/petermetz/cactus/commit/14d17904442723450790644653ff18dda79dfa5e))
* **connector-besu,connector-quorum:** updated ([985f12f](https://github.com/petermetz/cactus/commit/985f12f69c52a139a72aecc9b050e71545a90df8))
* **connector-besu:** add get balance method ([db71c5c](https://github.com/petermetz/cactus/commit/db71c5ce1af09bd1c60b9dbc841ca13c3eb75782))
* **connector-besu:** add get past logs method ([e3fcfa7](https://github.com/petermetz/cactus/commit/e3fcfa7173667b0d3c7a4bd92a6706444e0717b1))
* **connector-besu:** add get past logs method ([c4900e9](https://github.com/petermetz/cactus/commit/c4900e98f753e733e07170cea7003aefcee0dbdd))
* **connector-besu:** add getBalance web service ([50107f6](https://github.com/petermetz/cactus/commit/50107f62cda1e3be688576b9074b9408757e9b49)), closes [#1066](https://github.com/petermetz/cactus/issues/1066)
* **connector-besu:** add getBlock web service [#1065](https://github.com/petermetz/cactus/issues/1065) ([869c48b](https://github.com/petermetz/cactus/commit/869c48ba4d8000b50d1d64a8a0897b50dde21d5d))
* **connector-besu:** add getPastLogs web service ([c037ec5](https://github.com/petermetz/cactus/commit/c037ec55bc07e5314cd2104579b1a882d79f1488)), closes [#1067](https://github.com/petermetz/cactus/issues/1067)
* **connector-besu:** add getTransaction web service ([0ca0769](https://github.com/petermetz/cactus/commit/0ca0769ac4d1c3d43afc553813cf31983e5cb1b1)), closes [#1062](https://github.com/petermetz/cactus/issues/1062) [#1061](https://github.com/petermetz/cactus/issues/1061)
* **connector-besu:** contract deployment with constructor arguments ([48d67a7](https://github.com/petermetz/cactus/commit/48d67a7a7af223337777917a01002426a79f8463)), closes [#810](https://github.com/petermetz/cactus/issues/810)
* **connector-besu:** contractAbi optional parameter ([26cf7c2](https://github.com/petermetz/cactus/commit/26cf7c23919436ca82107b532309b5197ad2e39d))
* **connector-besu:** dockerfile ([7174004](https://github.com/petermetz/cactus/commit/71740048eb97e2855febc96a91a5f64215591187))
* **connector-besu:** getTransaction method ([d470540](https://github.com/petermetz/cactus/commit/d4705403b88023ecd3b7f68223215019053982cd))
* **connector-besu:** replace invokeContractV2 ([ecd62ea](https://github.com/petermetz/cactus/commit/ecd62eac5721514dbcfc401d5f28dfdc58ef8873))
* **connector-fabric:** containerize-fabric ([b53b3a4](https://github.com/petermetz/cactus/commit/b53b3a4c1cb36e7a0f14d405cdecb3c8341f956d))
* **connector-fabric:** contract deployment Fabric 2.x ([139a8ed](https://github.com/petermetz/cactus/commit/139a8ed96d5d547a514839a461abcb7d0e937cb0))
* **connector-fabric:** enrollAdmin() and createCaClient() ([da1cb1b](https://github.com/petermetz/cactus/commit/da1cb1bc3c3751b5d10f98a457ae0ec62b6bdebf))
* **connector-quorum:** contractAbi optional parameter ([c79d763](https://github.com/petermetz/cactus/commit/c79d763e0cb093647209417cfed7a2645283f302))
* **connector-quorum:** support v21.4.1 and Tessera 21.1.1 [#901](https://github.com/petermetz/cactus/issues/901) ([33fdd50](https://github.com/petermetz/cactus/commit/33fdd50e6a9cdeff433a9614c6498fa1c370f50a))
* **connector-xdai:** add interval to pollForTxReceipt ([40be742](https://github.com/petermetz/cactus/commit/40be74234f3bbd059fbc41f61890d25eec1d6ff8))
* **connector-xdai:** add ledger connector plugin for xdai [#852](https://github.com/petermetz/cactus/issues/852) ([99399a3](https://github.com/petermetz/cactus/commit/99399a3bd5020c66d2899aca500a880777b6523d))
* **corda:** prometheus exporter metrics integration ([9f37755](https://github.com/petermetz/cactus/commit/9f3775580381cbdf314c6a75188114315d1844c6)), closes [#535](https://github.com/petermetz/cactus/issues/535)
* **core-api:** add plugin object store interface definition ([4bf8038](https://github.com/petermetz/cactus/commit/4bf8038ea4c0c341cef3a63b59f77c12cec65a46))
* **core-api:** decouple web service install & registration [#771](https://github.com/petermetz/cactus/issues/771) ([b50e148](https://github.com/petermetz/cactus/commit/b50e148f43c0b27138471c972aab391486e761e6))
* **core-api:** hasTransactionFinality() on connector API [#354](https://github.com/petermetz/cactus/issues/354) ([a2d0582](https://github.com/petermetz/cactus/commit/a2d058218780e5e4c81e5f847cc875879a946e3f))
* **core-api:** jwt authorization [#770](https://github.com/petermetz/cactus/issues/770) ([2016750](https://github.com/petermetz/cactus/commit/2016750849b4333bb4dd78897468771f0642a4f5))
* **core-api:** plugin async initializer method ([9678c2e](https://github.com/petermetz/cactus/commit/9678c2e9288a73589e84f9fd254c26aed6a93297))
* **core-api:** plugin interface async initializer ([d40f68b](https://github.com/petermetz/cactus/commit/d40f68bd9eaff498df8514fe7397986b5a2f865d))
* **core:** add plugin registry log level constructor arg ([1652b33](https://github.com/petermetz/cactus/commit/1652b33255c211e87e33ceb3e421cb9fb4182502))
* expose besu test ledger web socket API port ([e198a99](https://github.com/petermetz/cactus/commit/e198a99f5fe7c2ac5c7bc1a8be0f0d29259871a8))
* **fabric-connector:** add private data support ([3f503f9](https://github.com/petermetz/cactus/commit/3f503f9a57bcdb14c3a3045fb516491b4f4879b4))
* **fabric:** add sequence diagram of run transaction endpoint ([155cbab](https://github.com/petermetz/cactus/commit/155cbab3c0358f6c259df8c0f92b788cbdfc6a71)), closes [#756](https://github.com/petermetz/cactus/issues/756)
* **htlc-eth-besu:** implemented plugin + test ([6684557](https://github.com/petermetz/cactus/commit/6684557d5de863fa3e023b4c8afe239ea62143eb))
* incorporating load testing into our CI pipeline ([7125d10](https://github.com/petermetz/cactus/commit/7125d1043091e0443edaa7b63021cd0b96404c4b)), closes [#295](https://github.com/petermetz/cactus/issues/295)
* **iroha-testnet:** Add REJECT check for transactions to setup-iroha-wallet.sh script in iroha-testnet ([cf60ec0](https://github.com/petermetz/cactus/commit/cf60ec0fd3f09762c940765c07265f928294b465))
* **iroha-testnet:** iroha-testnet ([dee1b12](https://github.com/petermetz/cactus/commit/dee1b12f98e70ac24faf69d757db6220be751bc7))
* **keychain-vault:** add the missing endpoint classes [#676](https://github.com/petermetz/cactus/issues/676) ([341cffc](https://github.com/petermetz/cactus/commit/341cffcef72286169a4ceced69414618d5059d0e))
* **plugin-object-store-ipfs:** add IPFS plugin implementation ([6d1de27](https://github.com/petermetz/cactus/commit/6d1de274b45a3fd2cc5120588f9d8594d5d3ace6))
* **readme:** removing enforced 100% code coverage check ([04cacc9](https://github.com/petermetz/cactus/commit/04cacc9502e017a84258cb1cd1c56b66f6f9dd58))
* **test-tooling:** add besu multi-party test ledger ([89f173e](https://github.com/petermetz/cactus/commit/89f173eea9deb15f0c2f6bd94ccefeb453fbeb39))
* **test-tooling:** add besu test ledger log level constructor arg ([60ee32f](https://github.com/petermetz/cactus/commit/60ee32fb0e65e8325194a8798dd8cde093a141d3)), closes [#780](https://github.com/petermetz/cactus/issues/780)
* **test-tooling:** add keycloak container ([f1abb3e](https://github.com/petermetz/cactus/commit/f1abb3e8d2e05aa18008da176753b240528e95e6))
* **test-tooling:** add OpenEthereumTestLedger [#851](https://github.com/petermetz/cactus/issues/851) ([9ca1f68](https://github.com/petermetz/cactus/commit/9ca1f6839749450b4d8887c5af14a888225d645f))
* **test-tooling:** containers#logDiagnostics() utility method ([ed9e125](https://github.com/petermetz/cactus/commit/ed9e125723508827a096293c808dbfac1fdba41c))
* **test-tooling:** go-ipfs test container ([e62b1b0](https://github.com/petermetz/cactus/commit/e62b1b08988463fdccdd88743562081a486285f2))
* **test-tooling:** quorum AIO upgrade to Quorum v21.4.1 [#900](https://github.com/petermetz/cactus/issues/900) ([67af2c4](https://github.com/petermetz/cactus/commit/67af2c466f10800124a3288aa8fcf13cfd05d1f8))
* **test-tooling:** quorum test ledger omit pull parameter ([73f84f7](https://github.com/petermetz/cactus/commit/73f84f7399c30f6cf3e1a0c46e4b9b9ec26dbced))
* **test-tooling:** rust compiler container for wasm builds ([ad7cdc0](https://github.com/petermetz/cactus/commit/ad7cdc07e1f40e2b663577312ed47b1b64e9eafc))
* **tools:** add test-npm-registry contaimer image ([19afe85](https://github.com/petermetz/cactus/commit/19afe851dc9efbc37ab012146e9c41bfc296304a))
* **tools:** docker-compose files for indy corresponding to issue [#866](https://github.com/petermetz/cactus/issues/866) ([599acc0](https://github.com/petermetz/cactus/commit/599acc0d2fe2454c74d4072c3c0646a500765779))
* **tools:** fabric all-in-one 2.x add nodejs to image ([dc09540](https://github.com/petermetz/cactus/commit/dc09540ba96e346e256363cd4cbeecc6d7aacf73))
* **tools:** upgrade go to 1.16.3 in Fabric 1.4.x AIO image ([d28ed6e](https://github.com/petermetz/cactus/commit/d28ed6ef982bec670245360498e204d46f1d2f0c)), closes [#914](https://github.com/petermetz/cactus/issues/914)
* **validator:** indy validator and indy-testnet files ([8eef3fa](https://github.com/petermetz/cactus/commit/8eef3fa46cd178c7991fdcc9053284e6da5ddfd8))


### Performance Improvements

* **cmd-api-server:** shrink API server bundle with type-only imports ([4875fc3](https://github.com/petermetz/cactus/commit/4875fc346bba70ee87d8fe033435035201d48b3e))
* leverage import type syntax to save on bundle size ([11f93a0](https://github.com/petermetz/cactus/commit/11f93a03116d26b64b516dba3c05d97a59afeabc))
* **tools:** fabric 1.x AIO image pre-fetching [#649](https://github.com/petermetz/cactus/issues/649) ([a4722fa](https://github.com/petermetz/cactus/commit/a4722fa1a8a1141bb274d10bc6192f4174c60302))

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cactus/releases/tag/v0.6.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-07-20 02:06:11 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v0.5.0
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
                # [0.5.0](https://github.com/petermetz/cactus/compare/v0.4.1...v0.5.0) (2021-05-19)


### Bug Fixes

* **ci:** dependent issues bot workflow has no job id [#848](https://github.com/petermetz/cactus/issues/848) ([af61202](https://github.com/petermetz/cactus/commit/af61202f73b72efe6df31e5697eedd94f84d417c))
* **cmd-api-server:** no CLI args causes crash [#794](https://github.com/petermetz/cactus/issues/794) ([a285b96](https://github.com/petermetz/cactus/commit/a285b96785792cd29f450bfc1cc066067c82f558))
* **connector-besu:** network update only if present in keychain ([8ac2444](https://github.com/petermetz/cactus/commit/8ac2444f86f9a1310f045ff0f7e4e78b91635be0))
* **connector-fabric:** export IPluginLedgerConnectorFabricOptions ([ada532e](https://github.com/petermetz/cactus/commit/ada532ef09603727379b6193b175e2834fa803d3))
* **connector-quorum:** web3 Contract type usage ([80c8253](https://github.com/petermetz/cactus/commit/80c82536f6446896a07aab9276f93598266ea5c3))
* **connector-xdai:** add missing hasTransactionFinality ([cc4f3e1](https://github.com/petermetz/cactus/commit/cc4f3e141da9292b8db5b0261a3347b3ba9c0689))
* **deps:** elliptic upgrade to >6.5.3 for CVE-2020-28498 ([d75b9af](https://github.com/petermetz/cactus/commit/d75b9af764241ab2e10914769412201fb040b1ed))
* **examples:** supply chain backend bundle build RAM [#766](https://github.com/petermetz/cactus/issues/766) ([f5c5d82](https://github.com/petermetz/cactus/commit/f5c5d82ef3ae327f057da94ea12a224f9b4d78c6))
* **test:** eliminate CVE-2020-8203 in besu connector test pkg ([6411933](https://github.com/petermetz/cactus/commit/6411933a167711152165d86a260d5f49d272746d))
* **tools:** ci.sh retry mechanism no longer ignores last failure ([b5e751e](https://github.com/petermetz/cactus/commit/b5e751e405d0c612f71c50fa964600134d25e0c2))
* **tools:** use latest fabric bootstrap.sh script for AIO image ([b298b76](https://github.com/petermetz/cactus/commit/b298b76a03382fa2729b89a6066b693e3c072582))
* **whitepaper:** build fails on Ubuntu 18 due to glibc 2.29 [#703](https://github.com/petermetz/cactus/issues/703) ([ec22a0f](https://github.com/petermetz/cactus/commit/ec22a0fc94929ae0fe8b44f93ce20f44847ec176))
* **whitepaper:** fix rendering ([d64f3cd](https://github.com/petermetz/cactus/commit/d64f3cd9cc6fd2c3998d139f1872f2c3eaeffc60))
* keychain to registry, uuid dep, add back missing gas req parameter ([4635d81](https://github.com/petermetz/cactus/commit/4635d817a719bcdaa2a3bf1b4aa3b5d8cc1f6961))


### Features

* **api-server:** ability to install plugins at runtime [#764](https://github.com/petermetz/cactus/issues/764) ([8dda0f6](https://github.com/petermetz/cactus/commit/8dda0f61937c6e1a85afee0345af44b1bfa09c0a))
* **besu:** add sequence diagram of run transaction endpoint ([754a11a](https://github.com/petermetz/cactus/commit/754a11a449d9a67dd8d6ebecbeb1b65cefa71b7f)), closes [#755](https://github.com/petermetz/cactus/issues/755)
* **cmd-api-server:** container image definition ([eb69fff](https://github.com/petermetz/cactus/commit/eb69fff36fca805c6b96c6db7caadfbed85e8485))
* **cmd-api-server:** user defined type guard isHealthcheckResponse ([16077d4](https://github.com/petermetz/cactus/commit/16077d42ec7edce4999d77cfbca5c02177d15fa6))
* **connector-besu:** contract deployment with constructor arguments ([48d67a7](https://github.com/petermetz/cactus/commit/48d67a7a7af223337777917a01002426a79f8463)), closes [#810](https://github.com/petermetz/cactus/issues/810)
* **connector-besu:** contractAbi optional parameter ([26cf7c2](https://github.com/petermetz/cactus/commit/26cf7c23919436ca82107b532309b5197ad2e39d))
* **connector-besu:** dockerfile ([7174004](https://github.com/petermetz/cactus/commit/71740048eb97e2855febc96a91a5f64215591187))
* **connector-besu:** replace invokeContractV2 ([ecd62ea](https://github.com/petermetz/cactus/commit/ecd62eac5721514dbcfc401d5f28dfdc58ef8873))
* **connector-besu, connector-quorum:** filesystem replaced by keychain ([14d1790](https://github.com/petermetz/cactus/commit/14d17904442723450790644653ff18dda79dfa5e))
* **connector-besu,connector-quorum:** updated ([985f12f](https://github.com/petermetz/cactus/commit/985f12f69c52a139a72aecc9b050e71545a90df8))
* **connector-fabric:** containerize-fabric ([b53b3a4](https://github.com/petermetz/cactus/commit/b53b3a4c1cb36e7a0f14d405cdecb3c8341f956d))
* **connector-fabric:** contract deployment Fabric 2.x ([139a8ed](https://github.com/petermetz/cactus/commit/139a8ed96d5d547a514839a461abcb7d0e937cb0))
* **connector-fabric:** enrollAdmin() and createCaClient() ([da1cb1b](https://github.com/petermetz/cactus/commit/da1cb1bc3c3751b5d10f98a457ae0ec62b6bdebf))
* **connector-quorum:** contractAbi optional parameter ([c79d763](https://github.com/petermetz/cactus/commit/c79d763e0cb093647209417cfed7a2645283f302))
* **connector-xdai:** add ledger connector plugin for xdai [#852](https://github.com/petermetz/cactus/issues/852) ([99399a3](https://github.com/petermetz/cactus/commit/99399a3bd5020c66d2899aca500a880777b6523d))
* **corda:** prometheus exporter metrics integration ([9f37755](https://github.com/petermetz/cactus/commit/9f3775580381cbdf314c6a75188114315d1844c6)), closes [#535](https://github.com/petermetz/cactus/issues/535)
* **core:** add plugin registry log level constructor arg ([1652b33](https://github.com/petermetz/cactus/commit/1652b33255c211e87e33ceb3e421cb9fb4182502))
* **core-api:** decouple web service install & registration [#771](https://github.com/petermetz/cactus/issues/771) ([b50e148](https://github.com/petermetz/cactus/commit/b50e148f43c0b27138471c972aab391486e761e6))
* **core-api:** hasTransactionFinality() on connector API [#354](https://github.com/petermetz/cactus/issues/354) ([a2d0582](https://github.com/petermetz/cactus/commit/a2d058218780e5e4c81e5f847cc875879a946e3f))
* **test-tooling:** add OpenEthereumTestLedger [#851](https://github.com/petermetz/cactus/issues/851) ([9ca1f68](https://github.com/petermetz/cactus/commit/9ca1f6839749450b4d8887c5af14a888225d645f))
* adding additional info into err logs ([888f85a](https://github.com/petermetz/cactus/commit/888f85a680a330cfc6be98bab3e8aed5d9e9dde2)), closes [#295](https://github.com/petermetz/cactus/issues/295)
* incorporating load testing into our CI pipeline ([7125d10](https://github.com/petermetz/cactus/commit/7125d1043091e0443edaa7b63021cd0b96404c4b)), closes [#295](https://github.com/petermetz/cactus/issues/295)
* **core-api:** jwt authorization [#770](https://github.com/petermetz/cactus/issues/770) ([2016750](https://github.com/petermetz/cactus/commit/2016750849b4333bb4dd78897468771f0642a4f5))
* **fabric:** add sequence diagram of run transaction endpoint ([155cbab](https://github.com/petermetz/cactus/commit/155cbab3c0358f6c259df8c0f92b788cbdfc6a71)), closes [#756](https://github.com/petermetz/cactus/issues/756)
* **test-tooling:** add besu test ledger log level constructor arg ([60ee32f](https://github.com/petermetz/cactus/commit/60ee32fb0e65e8325194a8798dd8cde093a141d3)), closes [#780](https://github.com/petermetz/cactus/issues/780)
* **test-tooling:** add keycloak container ([f1abb3e](https://github.com/petermetz/cactus/commit/f1abb3e8d2e05aa18008da176753b240528e95e6))
* **tools:** add test-npm-registry contaimer image ([19afe85](https://github.com/petermetz/cactus/commit/19afe851dc9efbc37ab012146e9c41bfc296304a))
* **tools:** fabric all-in-one 2.x add nodejs to image ([dc09540](https://github.com/petermetz/cactus/commit/dc09540ba96e346e256363cd4cbeecc6d7aacf73))


### Performance Improvements

* **tools:** fabric 1.x AIO image pre-fetching [#649](https://github.com/petermetz/cactus/issues/649) ([a4722fa](https://github.com/petermetz/cactus/commit/a4722fa1a8a1141bb274d10bc6192f4174c60302))


### BREAKING CHANGES

* 🧨 Behaviour in a cloud environment is currently untested and could impact
CI pipeline time.




            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cactus/releases/tag/v0.5.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-07-13 23:21:02 +0000 UTC
    </span>
</div>

