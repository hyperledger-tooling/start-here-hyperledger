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
                    v1.0.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.0.0
                </span>
            </td>
            <td>
                ---
As part of the continual effort to mitigate risks, the current 1.0.0 release is undergoing a a third-party security audit at the time of this writing. The process will take about 6 to 8 weeks to complete, but we are planning to keep the 1.0.0 API stability in place as dictated by the semantic versioning rules.
---

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

# [1.0.0](https://github.com/hyperledger/cactus/compare/v1.0.0-rc.3...v1.0.0) (2022-03-16)


### Bug Fixes

* 1852: slow breakpoints ([ff02ba1](https://github.com/hyperledger/cactus/commit/ff02ba19d6a28ca194db7eb7fe57ad01a2c0d38c)), closes [#1852](https://github.com/hyperledger/cactus/issues/1852)
* add optional auth token to api-client and consortium-manual ([c2feebf](https://github.com/hyperledger/cactus/commit/c2feebfec56f13d68c2ea1ec3a34ce67394d0720)), closes [#1579](https://github.com/hyperledger/cactus/issues/1579)
* **cmd-api-server:** add express static rate limiting ([190cf12](https://github.com/hyperledger/cactus/commit/190cf12f16345e06fbb6d1ccb428ad0ad8958a3e)), closes [#1840](https://github.com/hyperledger/cactus/issues/1840)
* **cmd-api-server:** disable validateKeyPairMatch ([7deaa22](https://github.com/hyperledger/cactus/commit/7deaa229ca0cdb4ef31fcc033ef08128fcb9e5b1))
* **cmd-api-server:** upgrade socket.io - CVE-2022-21676 ([8e1c69e](https://github.com/hyperledger/cactus/commit/8e1c69e7b8ab5e4ccc31a0ec183a9777ccc22cdc)), closes [#1914](https://github.com/hyperledger/cactus/issues/1914)
* config-service validator throws warnings ([877dcab](https://github.com/hyperledger/cactus/commit/877dcabc82dbc583f0d7e05813ce375c85b66f83))
* **connector-besu/quorum/xdai:** unvalidated dynamic method call ([bdc1aba](https://github.com/hyperledger/cactus/commit/bdc1aba982cc2ec1a74b0458c98ceeacc7acb9e7)), closes [#1911](https://github.com/hyperledger/cactus/issues/1911)
* **connector-fabric:** uncontrolled data used in path expression ([ef0981d](https://github.com/hyperledger/cactus/commit/ef0981d300d03fc5e5b1806f5e7355d0745700ce)), closes [#1909](https://github.com/hyperledger/cactus/issues/1909)
* **deps:** ensure glob-parent is above 5.1.2 - CVE-2020-28469 ([23ded0f](https://github.com/hyperledger/cactus/commit/23ded0f7095559796525bbebc45ae39e65306855)), closes [#1916](https://github.com/hyperledger/cactus/issues/1916)
* fix faulty shutdownHook definition in the Config-Schema ([fbae2da](https://github.com/hyperledger/cactus/commit/fbae2da4071ebbf40cc1941a1d2261b8b06fe8f0)), closes [#1648](https://github.com/hyperledger/cactus/issues/1648)
* **plugin-ledger-connector-fabric-socketio:** upgrade Fabric due to jsrsasign ([a9ecb19](https://github.com/hyperledger/cactus/commit/a9ecb192cb32661c5bdd9ea684f35a90c7948f6a)), closes [#1754](https://github.com/hyperledger/cactus/issues/1754) [#1799](https://github.com/hyperledger/cactus/issues/1799)
* **plugin-odap-hermes:** remove extraneous dependencies ([87af023](https://github.com/hyperledger/cactus/commit/87af02305be25cdb8afb7e1b7a2464bf36791b6e)), closes [#1641](https://github.com/hyperledger/cactus/issues/1641)
* remove jade dependencies ([f4ce09e](https://github.com/hyperledger/cactus/commit/f4ce09e8c07949aa08e4bfd404e4468e6c3544a8)), closes [#1662](https://github.com/hyperledger/cactus/issues/1662)
* reset script from package.json does not work [#1656](https://github.com/hyperledger/cactus/issues/1656) ([c74e002](https://github.com/hyperledger/cactus/commit/c74e002a636994bd1b864fa0bde495bfc5026f9f))
* **security:** address CVE-2019-5413 ([212b770](https://github.com/hyperledger/cactus/commit/212b770c705c279dcc766b7230d7519ed9a98748)), closes [#1777](https://github.com/hyperledger/cactus/issues/1777)
* **security:** address CVE-2021-23358 - TEMPORARY fix ([2fdee4f](https://github.com/hyperledger/cactus/commit/2fdee4fc4326bfb4821ba9c6ad750fa8ae6af3e6)), closes [#1775](https://github.com/hyperledger/cactus/issues/1775)
* **security:** ensure ansi-html > 0.0.8 - CVE-2021-23424 ([e3e2d1c](https://github.com/hyperledger/cactus/commit/e3e2d1cf3e5637212f56f278091e6eee77fbc9b2)), closes [#1920](https://github.com/hyperledger/cactus/issues/1920)
* **security:** force lodash > 4.17.20 - CVE-2020-8203 ([08ace66](https://github.com/hyperledger/cactus/commit/08ace6676cb5be5fa8a9d35e5e159d85eff7735f)), closes [#1918](https://github.com/hyperledger/cactus/issues/1918)
* **security:** upgrade to yarn > 1.22.0 - CVE-2019-10773, CVE-2020-8131 ([43d591d](https://github.com/hyperledger/cactus/commit/43d591d2eff576cb581a2a92d98edf7f4f6ecf13)), closes [#1922](https://github.com/hyperledger/cactus/issues/1922)
* **security:** upgrade web3 to upgrade elliptic > 6.5.4 ([5513848](https://github.com/hyperledger/cactus/commit/55138483e43dd840a6c3822d1ff8f2f7ce8c35e8)), closes [#1639](https://github.com/hyperledger/cactus/issues/1639)
* set apiServerOptions.configFile="" ([5c5a1e1](https://github.com/hyperledger/cactus/commit/5c5a1e16ad92a882b9e99f5413411b4cc7793be6)), closes [#1619](https://github.com/hyperledger/cactus/issues/1619)
* shutdown hook configuration is using wrong config key ([e760e04](https://github.com/hyperledger/cactus/commit/e760e04a9ba946b45b65c68455eedcc2694f8fae)), closes [#1619](https://github.com/hyperledger/cactus/issues/1619)


### Features

* **cactus-api-client:** add support for plain socketio validators in api-server and api-client ([634b10e](https://github.com/hyperledger/cactus/commit/634b10e5eaf82df08b04c11c3af5b109ede5b942)), closes [#1602](https://github.com/hyperledger/cactus/issues/1602) [#1602](https://github.com/hyperledger/cactus/issues/1602)
* **cactus-api-client:** common verifier-factory ([2f70a64](https://github.com/hyperledger/cactus/commit/2f70a6473f30446859427335f2d3602bddca636d)), closes [#1878](https://github.com/hyperledger/cactus/issues/1878)
* **connector-corda:** enable Flow Database Access CorDapp ([60dfe1a](https://github.com/hyperledger/cactus/commit/60dfe1a772d06436132f79bf3e89589e181a783e)), closes [#1493](https://github.com/hyperledger/cactus/issues/1493)
* **connector-corda:** read privateKey from filesystem ([e7e39fd](https://github.com/hyperledger/cactus/commit/e7e39fd5f7ef2d6ec49b4ebebde35875bbf1df44)), closes [#789](https://github.com/hyperledger/cactus/issues/789)
* **connector-xdai:** remove hard dependency on keychain ([da793c5](https://github.com/hyperledger/cactus/commit/da793c568260fd70b80f855833bc60c116099a65)), closes [#1162](https://github.com/hyperledger/cactus/issues/1162)
* **core-api:** add weaver protobuf codegen  [#1556](https://github.com/hyperledger/cactus/issues/1556) ([b5b68a7](https://github.com/hyperledger/cactus/commit/b5b68a76e256555ef362dceaa834d8bbcdcfff06))



            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cactus/releases/tag/v1.0.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-03-16 22:31:01 +0000 UTC
    </span>
</div>

