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
                    v2.0.0-rc.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v2.0.0-rc.1
                </span>
            </td>
            <td>
                All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

# [2.0.0-rc.1](https://github.com/hyperledger/cacti/compare/v2.0.0-alpha.2...v2.0.0-rc.1) (2024-06-14)

### Bug Fixes

* **cactus-common:** coerceUnknownToError() now uses HTML sanitize ([d70488a](https://github.com/hyperledger/cacti/commit/d70488a82e9c1d6958ac3ab0368f3c3bfca378c6))
* **cactus-example-cbdc-bridging-backend:** add missing CRPC port config option ([84c0733](https://github.com/hyperledger/cacti/commit/84c0733db93e6b2cd91050c48641562130f3ea0b))
* **cmd-api-server:** add runtime type validation to HTTP verbs pulled from OAS ([b0ff599](https://github.com/hyperledger/cacti/commit/b0ff599b2c32b83d7d45c41ef215372044ccda23)), closes [#2751](https://github.com/hyperledger/cacti/issues/2751) [#2751](https://github.com/hyperledger/cacti/issues/2751) [#2751](https://github.com/hyperledger/cacti/issues/2751) [#2754](https://github.com/hyperledger/cacti/issues/2754)
* **cmd-api-server:** address CVE-2022-25881 ([81da333](https://github.com/hyperledger/cacti/commit/81da3334d8e638f85e398dd228bcef836a278230)), closes [#2862](https://github.com/hyperledger/cacti/issues/2862)
* **cmd-api-server:** fix CVE-2023-36665 protobufjs try 2 ([4e8b553](https://github.com/hyperledger/cacti/commit/4e8b5534d6a86c856768c0b47af794d66304f90d)), closes [#2682](https://github.com/hyperledger/cacti/issues/2682)
* **cmd-api-server:** healthcheck broken due to missing wget binary ([8f1ca3f](https://github.com/hyperledger/cacti/commit/8f1ca3fcce9fedaedd4ceafbb51d8e8cd41cc50e)), closes [#2894](https://github.com/hyperledger/cacti/issues/2894)
* **connector-besu:** error handling of DeployContractSolidityBytecodeEndpoint ([89d9b93](https://github.com/hyperledger/cacti/commit/89d9b93b7380477c10d8da78fcd259c95b495fa9)), closes [#2868](https://github.com/hyperledger/cacti/issues/2868)
* **connector-besu:** toBuffer only supports 0x-prefixed hex ([1d00e32](https://github.com/hyperledger/cacti/commit/1d00e32ed0f76b1d9081a7cea55ad41c956ec25b))
* **connector-corda:** contract deployment SSH reconnect race condition ([0af2eb1](https://github.com/hyperledger/cacti/commit/0af2eb13235d4dda5dfe92912be48722caea09b1))
* **connector-fabric:** address CVEs: CVE-2022-21190, CVE-2021-3918 ([11e775d](https://github.com/hyperledger/cacti/commit/11e775d6e6611d0b054cd18cca620969cb947dd8)), closes [#2864](https://github.com/hyperledger/cacti/issues/2864)
* **connector-quorum/ethereum:** strengthen contract parameter validation ([779bb7e](https://github.com/hyperledger/cacti/commit/779bb7e24b06352bad64c96eab3b24c0961d1381)), closes [#2760](https://github.com/hyperledger/cacti/issues/2760)
* **corda-simple-app:** use correct bond asset flows and contracts for bond asset exchange ([caa2b3a](https://github.com/hyperledger/cacti/commit/caa2b3a50ab7928942e72341ebc7e5511e3054f7))
* **deps:** bulk add missing dependencies - 2023-11-02 ([8addb01](https://github.com/hyperledger/cacti/commit/8addb018b6d124d54d9d948bbaeba6ea33b67153)), closes [#2857](https://github.com/hyperledger/cacti/issues/2857)
* GHSA-8qv2-5vq6-g2g7 webpki CPU denial of service in certificate path ([e24458f](https://github.com/hyperledger/cacti/commit/e24458f0541d7000ea915d97668831723744baea))
* **indy-vdr-nodejs:** update dependency version ([f81b46b](https://github.com/hyperledger/cacti/commit/f81b46bce5ca0880e6bf6b51be2233e2616759a5))
* **ledger-browser:** fix vulnerability CVE-2022-37601 ([55c7d3d](https://github.com/hyperledger/cacti/commit/55c7d3d8054af35eb903ee903a91b8f23b905998))
* **persistence-fabric:** hide not critical API ([793f94f](https://github.com/hyperledger/cacti/commit/793f94ffefe483bd2a08ad7afb30fac7aa029007))
* **plugin-htlc-coordinator-besu:** add missing HSTS header ([dff34e8](https://github.com/hyperledger/cacti/commit/dff34e8f26f94a391b8b926057cbd6346bc0b3f8))
* **plugin-keychain-vault:** fix CVE-2024-0553 in vault server image ([1eacf7e](https://github.com/hyperledger/cacti/commit/1eacf7e2a33349de794d486a47cc6bd62d93311a))
* **security:** address CVE-2021-3749 - axios >=0.22.0 ([61fc700](https://github.com/hyperledger/cacti/commit/61fc7001b1dd0849ab1d9bcab08e2475c695adae))
* **security:** mitigate CVE-2024-21505 ([f48994f](https://github.com/hyperledger/cacti/commit/f48994fe0e3736909103a844eb59cb7f3cfed247))
* **security:** remediate qs vulnerability CVE-2022-24999 ([536b6b1](https://github.com/hyperledger/cacti/commit/536b6b1b7ab9014ebcd6b162e1a467e78b52afdd))
* **weaver-asset-transfer:** return proper error messages for pledge status and claim status ([f8f6bcb](https://github.com/hyperledger/cacti/commit/f8f6bcb67733dd57b2ecde94922cff24342b7589))
* **weaver-fabric-node-sdk:** made AES key length configurable in ECIES functions ([e679801](https://github.com/hyperledger/cacti/commit/e67980141d2fb2e54ef8408e36dbab55b7195905))
* **weaver-go-cli:** updated Weaver Fabric Go CLI module to ensure local compilation ([1668cf4](https://github.com/hyperledger/cacti/commit/1668cf4104a3a653bb17ebc04d86d72b9b22547f))
* **weaver-go-sdk:** corrected membership API function signatures ([083ea4f](https://github.com/hyperledger/cacti/commit/083ea4f4464691fc967a897bf267daaeea216343))
* **weaver-go-sdk:** revert fabric-protos-go-apiv2 dep to fabric-protos-go ([6994e5b](https://github.com/hyperledger/cacti/commit/6994e5b7a43b4f3e06535babb17edd466c4d4abc))
* **weaver-membership-functions:** reverted earlier buggy change affecting identity mgmt ([faf90dd](https://github.com/hyperledger/cacti/commit/faf90ddbe9c061cd6261d642842ab12ae4be3c48))
* **weaver-packages:** removing unnecessary package-lock.json file ([f3e53e4](https://github.com/hyperledger/cacti/commit/f3e53e4625d6667a59b55647d026c59431c32d85))
* **weaver-satp:** bug and configuration fixes in relays and Fabric drivers for sample SATP implementation ([9f77871](https://github.com/hyperledger/cacti/commit/9f77871419712bacc623dd9fbbe40f6016f0a94f))
* **weaver:** improper exception handling ([a33f30c](https://github.com/hyperledger/cacti/commit/a33f30c07cb7b952581c2401da60a25170b23d1c)), closes [#2767](https://github.com/hyperledger/cacti/issues/2767)
* **weaver:** upgraded Corda dependencies to overcome Log4j vulnerability ([76f0c68](https://github.com/hyperledger/cacti/commit/76f0c680bcf74d0d78e02e95ab6c9268d15d82d2))
* **weaver:** usage of weak PRNG issue ([fa17b52](https://github.com/hyperledger/cacti/commit/fa17b52d641345a6ffc3ff6b0845be75202dc945)), closes [#2765](https://github.com/hyperledger/cacti/issues/2765)

### Features

* **actionlint:** fix the errors produced by the ActionLint tool ([e6d5d88](https://github.com/hyperledger/cacti/commit/e6d5d88fd33b2078035447bc0e452f3d862e0e68))
* **bungee-hermes:** new plugin bungee-hermes ([ecf52ec](https://github.com/hyperledger/cacti/commit/ecf52ecce310d626ea96a53c2d41dcb797510c4d))
* **bungee-hermes:** process & merge views ([231a5e5](https://github.com/hyperledger/cacti/commit/231a5e532bcb8219986dd7f5c8fa4d66cef99f34))
* **bungee-hermes:** viewProof & ethereum strategy ([22f389f](https://github.com/hyperledger/cacti/commit/22f389fc311490e5f3959b4f80e7f4caf4ac5804))
* **cactus-core-api:** add ISendRequestResultV1<T> for Fujitsu verifier ([483de38](https://github.com/hyperledger/cacti/commit/483de3838017961656c0fb850934988ae0c63c91))
* **cactus-core:** add ConnectRPC service interface and type guard ([9e83087](https://github.com/hyperledger/cacti/commit/9e830874dfed51a805566a5bedc62e3d43fc234f))
* **cactus-core:** add handleRestEndpointException utility to public API ([bf9dfe8](https://github.com/hyperledger/cacti/commit/bf9dfe882f78f7fc88ee52d86d62b7e851716b79))
* **cactus-example-discounted-asset-trade:** use openapi ethereum connector ([dcaf9fe](https://github.com/hyperledger/cacti/commit/dcaf9fe5de5b830975f3d308f140eff32d3cb79d)), closes [#2645](https://github.com/hyperledger/cacti/issues/2645)
* **cactus-example-discounted-asset-trade:** use openapi sawtooth connector ([86d6b38](https://github.com/hyperledger/cacti/commit/86d6b38e213a5304799beab48bdd46a8fc0cc0c3)), closes [#2825](https://github.com/hyperledger/cacti/issues/2825)
* **cactus-example-electricity-trade:** use openapi ethereum connector ([9e66850](https://github.com/hyperledger/cacti/commit/9e66850438c97883a8999c3def36e807bfbb1a76))
* **cactus-plugin-ledger-connector-aries:** add new connector plugin ([afef5ae](https://github.com/hyperledger/cacti/commit/afef5ae3e2f36bf7f25928ee75f82bc4800b3172)), closes [#2946](https://github.com/hyperledger/cacti/issues/2946)
* **cactus-plugin-ledger-connector-cdl-socketio:** separate endpoint for subscription key ([b1048af](https://github.com/hyperledger/cacti/commit/b1048af272e7f33fae3c68dc854d40f9be7a4e84))
* **cactus-plugin-ledger-connector-cdl-socketio:** support subscription key auth ([a04fc5b](https://github.com/hyperledger/cacti/commit/a04fc5b2593a27d5c0f9311a1ad2f83f727e2e70))
* **cactus-plugin-ledger-connector-cdl:** add new connector plugin ([6efd8de](https://github.com/hyperledger/cacti/commit/6efd8de9ff5bb8d6b894147e5c6e49aed2fa8ae4))
* **cactus-plugin-ledger-connector-ethereum:** add json-rpc proxy ([ed04201](https://github.com/hyperledger/cacti/commit/ed04201671bdb614549e995b3d88cc2cae218e56))
* **cactus-plugin-ledger-connector-ethereum:** add signing utils ([84c5b34](https://github.com/hyperledger/cacti/commit/84c5b34afa73b4f906e413c4d5dd3ff46a1dd7a8))
* **cactus-plugin-ledger-connector-ethereum:** add stress test ([55fa26e](https://github.com/hyperledger/cacti/commit/55fa26ef41d405b26da02b099418da5fa281c78f)), closes [#2631](https://github.com/hyperledger/cacti/issues/2631)
* **cactus-plugin-ledger-connector-ethereum:** refactor connector API ([cda279f](https://github.com/hyperledger/cacti/commit/cda279fb0009a4d5756c461024ad88f525bfe946)), closes [#2630](https://github.com/hyperledger/cacti/issues/2630)
* **cactus-plugin-ledger-connector-ethereum:** support London fork gas prices ([80a89dd](https://github.com/hyperledger/cacti/commit/80a89dd95d51bdc604392dbe96ab27d233b116a4)), closes [#2581](https://github.com/hyperledger/cacti/issues/2581)
* **cactus-plugin-ledger-connector-ethereum:** update web3js to 4.X ([55f82c9](https://github.com/hyperledger/cacti/commit/55f82c9568b3e875de4f3ceb89a828f8b23d65be)), closes [#2580](https://github.com/hyperledger/cacti/issues/2580) [#2535](https://github.com/hyperledger/cacti/issues/2535) [#2578](https://github.com/hyperledger/cacti/issues/2578)
* **cactus-plugin-ledger-connector-fabric-socketio:** remove fabric-socketio connector ([704e201](https://github.com/hyperledger/cacti/commit/704e201d6bd6bf7a38f0de7da60723118e18cea7)), closes [#2644](https://github.com/hyperledger/cacti/issues/2644)
* **cactus-plugin-ledger-connector-fabric:** support delegated (offline) signatures ([e2812f4](https://github.com/hyperledger/cacti/commit/e2812f4abce00a1918b8d13a6cfff382289ff998)), closes [#2598](https://github.com/hyperledger/cacti/issues/2598)
* **cactus-plugin-ledger-connector-iroha:** remove deprecated iroha connector ([fa27fde](https://github.com/hyperledger/cacti/commit/fa27fde9a28f83ff29964693be656dc107046517)), closes [#3159](https://github.com/hyperledger/cacti/issues/3159) [#3155](https://github.com/hyperledger/cacti/issues/3155)
* **cactus-plugin-ledger-connector-sawtooth:** add new connector plugin ([e379504](https://github.com/hyperledger/cacti/commit/e37950403636a3fbc378fc7462b886294e6c7923))
* **cactus-plugin-persistence-ethereum:** use openapi ethereum connector ([b8f9b79](https://github.com/hyperledger/cacti/commit/b8f9b79daa7a97cbd75325eba00c7458bfed5ce5)), closes [#2631](https://github.com/hyperledger/cacti/issues/2631)
* **cbdc-bridging:** add frontend code for the CBDC example ([5ad0ebf](https://github.com/hyperledger/cacti/commit/5ad0ebffe9de0eabbdfabb8ce8fa5c426519ee33))
* **cmd-api-server:** add ConnectRPC auto-registration for plugins ([c569460](https://github.com/hyperledger/cacti/commit/c569460b099469184a7953ffc0f806ddf3facb38))
* **cmd-api-server:** add gRPC plugin auto-registration support ([5762dad](https://github.com/hyperledger/cacti/commit/5762dadfe108c6c73251d5b474961e4888941b90))
* **common:** add express http verb method name string literal type ([8f048ea](https://github.com/hyperledger/cacti/commit/8f048ea72750595016eea4e40fd57291001cff95))
* **common:** add isGrpcStatusObjectWithCode user-defined type guard ([941dbad](https://github.com/hyperledger/cacti/commit/941dbad8fa5950b754dde97b02cc4c0ac0e9e0bb))
* **connector-besu:** add continuous benchmarking with JMeter ([379d41d](https://github.com/hyperledger/cacti/commit/379d41dd4b2cc994801c85f1fa16ea854f0301f7))
* **connector-besu:** add gRPC support for operations ([ab676d2](https://github.com/hyperledger/cacti/commit/ab676d23e1781aa17b5f2c61cb7dec643443bded)), closes [#3173](https://github.com/hyperledger/cacti/issues/3173)
* **connector-fabric:** drop support for Fabric v1.x ([ec8123c](https://github.com/hyperledger/cacti/commit/ec8123cf954b09ba8cb213c7332dfe82224c351f))
* **connector-polkadot:** add connector pkg, openapi specs, test suite ([6a476a0](https://github.com/hyperledger/cacti/commit/6a476a0f1143380d2fd6bf81c68b0842c13c6ae2))
* **core-api:** add IPluginGrpcService type & user-defined type guard ([e87e577](https://github.com/hyperledger/cacti/commit/e87e57791024824bb19830c66b9f3d2eaed6d629))
* **core:** add configureExpressAppBase() utility function ([383f852](https://github.com/hyperledger/cacti/commit/383f8528d88989b44c9763fc883c3d9ac74da21e))
* **ethereum-connector:** support block monitoring with http only connection ([f4373a9](https://github.com/hyperledger/cacti/commit/f4373a90020cbc8bfbc16da6c32babe627e7d4ae))
* **indy-sdk:** replace indy SDK with AFJ ([3291dcc](https://github.com/hyperledger/cacti/commit/3291dcc57e9e4eb04e0b9abab4134e1a5e2b0bbf)), closes [#2859](https://github.com/hyperledger/cacti/issues/2859) [#2860](https://github.com/hyperledger/cacti/issues/2860)
* **indy-test-ledger:** add helper class for indy ledger ([8c746c3](https://github.com/hyperledger/cacti/commit/8c746c331564e76e8619c5c6987cd9380ce4a13f)), closes [#2861](https://github.com/hyperledger/cacti/issues/2861)
* **plugin-keychain-memory:** add ConnectRPC support ([c5fecf6](https://github.com/hyperledger/cacti/commit/c5fecf6802efba0c982db1adc4a98b785c9cb8e0)), closes [#3183](https://github.com/hyperledger/cacti/issues/3183)
* **plugin-keychain-memory:** add observability via RxJS ReplaySubjects ([9b41377](https://github.com/hyperledger/cacti/commit/9b41377c3885cf12be3c0f49bd2745200b0d07d3))
* **plugin-keychain-memory:** add REST API endpoint implementations ([c7a8fa5](https://github.com/hyperledger/cacti/commit/c7a8fa5e3e33b3c6a1464d9762a66337176e6cdd))
* **plugin-satp-hermes:** replace IPFS dependency in SATP package ([3bb7157](https://github.com/hyperledger/cacti/commit/3bb7157b8c910c31aa3fe125ecfb3437c2bef5bb)), closes [#2984](https://github.com/hyperledger/cacti/issues/2984) [#3006](https://github.com/hyperledger/cacti/issues/3006)
* **satp:** sample implementation of SATP standard using relays ([c23197c](https://github.com/hyperledger/cacti/commit/c23197c314885b99146b52c3cd0e056439193d6e))
* **supabase-all-in-one:** update versions, use skopeo ([eeb34f9](https://github.com/hyperledger/cacti/commit/eeb34f9515bf6a7a85c1b2343b94075c4ee0a505)), closes [#3099](https://github.com/hyperledger/cacti/issues/3099)
* **test-tooling:** add Stellar test ledger ([58fa94e](https://github.com/hyperledger/cacti/commit/58fa94e194f7716934e717a0e3075773ebd31b4c)), closes [#3239](https://github.com/hyperledger/cacti/issues/3239)
* **weaver-go:** upgraded Weaver Fabric Go SDK with membership functions ([43cce8e](https://github.com/hyperledger/cacti/commit/43cce8e3778a574514d2759c282a7f0108be86b5))
* **weaver:** add build script and fix minor issues ([6d4fd00](https://github.com/hyperledger/cacti/commit/6d4fd00d457d3a72017a7cd8d4a9cf3fb4d5f37e))

### Performance Improvements

* **cmd-api-server:** add demonstration of continuous benchmarking ([0804bab](https://github.com/hyperledger/cacti/commit/0804bab4c9b43f2e22be6d77be127415a9a0532f))

### BREAKING CHANGES

* **connector-fabric:** The Open API specification that has the enums for
ledger versions will no longer have an option for Fabric v1.x
This means that in the core-api package the LedgerType enum has changes
which means that code that depends on that enum value will need to be
updated.

Fabric v1.x has had unmaintained dependencies associated with it such as
the native grpc package that stopped receiving security updates years ago
and therefore it's dangerous to have around.

There are also some issues with Fabric v1.x that make the AIO image flaky
which also makes the relevant tests flaky due to which we couldn't run
the v1.x Fabric tests on the CI for a while now anyway.

In order to reduce the CI resource usage and our own maintenance burden
I suggest that we get rid of the Fabric v1.x support meaning that we can
eliminate the AIO image build and some code complexity from the test ledger
code as well.

In addition some old fixtures can be removed that the tests were using.
Overall a net-positive as deleting code without losing functionality (that
we care about) is always a plus.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/v2.0.0-rc.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-06-18 16:24:11 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0-rc.1 - GO Fabric Utils Library for Interoperation - Jun 18, 2024
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    weaver/core/network/fabric-interop-cc/libs/utils/v2.0.0-rc.1
                </span>
            </td>
            <td>
                - Go Module: `github.com/hyperledger/cacti/weaver/core/network/fabric-interop-cc/libs/utils`
- Release: v2.0.0-rc.1
- Readme: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/libs/utils/v2.0.0-rc.1/weaver/core/network/fabric-interop-cc/libs/utils/README.md).
- Source: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/libs/utils/v2.0.0-rc.1/weaver/core/network/fabric-interop-cc/libs/utils)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/weaver/core/network/fabric-interop-cc/libs/utils/v2.0.0-rc.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-06-18 16:19:03 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0-rc.1 - GO Fabric Library for Asset Exchange - Jun 18, 2024
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    weaver/core/network/fabric-interop-cc/libs/assetexchange/v2.0.0-rc.1
                </span>
            </td>
            <td>
                - Go Module: `github.com/hyperledger/cacti/weaver/core/network/fabric-interop-cc/libs/assetexchange`
- Release: v2.0.0-rc.1
- Readme: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/libs/assetexchange/v2.0.0-rc.1/weaver/core/network/fabric-interop-cc/libs/assetexchange/README.md).
- Source: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/libs/assetexchange/v2.0.0-rc.1/weaver/core/network/fabric-interop-cc/libs/assetexchange)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/weaver/core/network/fabric-interop-cc/libs/assetexchange/v2.0.0-rc.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-06-18 16:19:03 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0-rc.1 - GO Fabric Asset Management Interface - Jun 18, 2024
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt/v2.0.0-rc.1
                </span>
            </td>
            <td>
                - Go Module: `github.com/hyperledger/cacti/weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt`
- Release: v2.0.0-rc.1
- Readme: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt/v2.0.0-rc.1/weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt/README.md).
- Source: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt/v2.0.0-rc.1/weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt/v2.0.0-rc.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-06-18 16:19:03 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0-rc.1 - GO Fabric Interop Chaincode - Jun 18, 2024
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    weaver/core/network/fabric-interop-cc/contracts/interop/v2.0.0-rc.1
                </span>
            </td>
            <td>
                - Go Module: `github.com/hyperledger/cacti/weaver/core/network/fabric-interop-cc/contracts/interop`
- Release: v2.0.0-rc.1
- Readme: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/contracts/interop/v2.0.0-rc.1/weaver/core/network/fabric-interop-cc/contracts/interop/README.md).
- Source: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/contracts/interop/v2.0.0-rc.1/weaver/core/network/fabric-interop-cc/contracts/interop)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/weaver/core/network/fabric-interop-cc/contracts/interop/v2.0.0-rc.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-06-18 16:19:03 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0-rc.1 - GO Weaver Protos - Jun 18, 2024
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    weaver/common/protos-go/v2.0.0-rc.1
                </span>
            </td>
            <td>
                - Go Module: `github.com/hyperledger/cacti/weaver/common/protos-go`
- Release: v2.0.0-rc.1
- Readme: [Here](https://github.com/hyperledger/cacti/blob/weaver/common/protos-go/v2.0.0-rc.1/weaver/common/protos-go/README.md).
- Source: [Here](https://github.com/hyperledger/cacti/blob/weaver/common/protos-go/v2.0.0-rc.1/weaver/common/protos-go)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/weaver/common/protos-go/v2.0.0-rc.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-06-18 16:19:03 +0000 UTC
    </span>
</div>

