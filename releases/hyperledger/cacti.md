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
                    v2.0.0-rc.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v2.0.0-rc.3
                </span>
            </td>
            <td>
                # [2.0.0-rc.3](https://github.com/hyperledger/cacti/compare/v2.0.0-rc.2...v2.0.0-rc.3) (2024-07-21)

### Bug Fixes

* address CVE-2022-24434, GHSA-wm7h-9275-46v2 caused by dicer ([6ff8111](https://github.com/hyperledger/cacti/commit/6ff8111c2534f71a5f623433eba59a610d84f4eb))
* **ci:** deprecationWarning in yarn_custom_checks ([96a3865](https://github.com/hyperledger/cacti/commit/96a3865ce5404e0fd3bf5a6471eb5a653e579d33))
* **cmd-api-server:** use ncc bundle in container image - CVE-2024-29415 ([9eefa66](https://github.com/hyperledger/cacti/commit/9eefa66446a193c7ca164c876f8ed6d5cc56549b))
* **connector-fabric:** decode blocks in getTransactionReceiptByTxID() ([1bdc35d](https://github.com/hyperledger/cacti/commit/1bdc35d5c9d49315e2b8b32c90c66b322d866bf9))
* **connector-polkadot:** use dynamic import calls for ESM dependencies ([76adf12](https://github.com/hyperledger/cacti/commit/76adf12afa40829226b4698f2d4394bd6fbe3aba)), closes [#3077](https://github.com/hyperledger/cacti/issues/3077)
* the CVEs of braces nth-check vite webpack-dev-middleware - 2024-07 ([4253d3f](https://github.com/hyperledger/cacti/commit/4253d3f75aef3e3e7849c56182ddd67e56f89fb3))

### Build System

* bump uuid@10.0.0 fs-extra@11.2.0 @bufbuild/protobuf@1.10.0 ([9970352](https://github.com/hyperledger/cacti/commit/997035216694fe335215b8a3586488ac8c12447f))

### Code Refactoring

* retire connector plugin specific container images, fix docs ([24b5888](https://github.com/hyperledger/cacti/commit/24b5888247d134ea417fc0e83dccc9826b4075f3))

### Features

* **besu:** remove hard dependency on keychain ([f5b60b4](https://github.com/hyperledger/cacti/commit/f5b60b4d25acc7a4bc53f3b9b87433b18a5d9153)), closes [#963](https://github.com/hyperledger/cacti/issues/963)
* **bungee-hermes:** ability to use connectors without instanciating APIs ([6a71ddf](https://github.com/hyperledger/cacti/commit/6a71ddfb5568d1fc11818e225782713bfaddc6d5))
* **connector-corda:** add vaultQueryV1 REST API operation + endpoint ([d2bf145](https://github.com/hyperledger/cacti/commit/d2bf1458ce2f1342fe330d9118aae7fc2fdd3312))
* **connector-corda:** support JVM 17 Cordapps ([1994128](https://github.com/hyperledger/cacti/commit/19941280469a3f66cb678525a4088f86b9cacee3))
* **fabric-connector:** add getChainInfo, improve getBlock output ([8c030ae](https://github.com/hyperledger/cacti/commit/8c030ae9e739a28ff0900f7af27ec0fbbb4b7ff9))
* **persistence-fabric:** rewrite the plugin ([c867a9f](https://github.com/hyperledger/cacti/commit/c867a9f5ef084e4e6d7c6f5a641d1dd13f9ce233)), closes [#3298](https://github.com/hyperledger/cacti/issues/3298)

### Performance Improvements

* **ci:** only publish artifacts on git version tags of main ([66e3139](https://github.com/hyperledger/cacti/commit/66e3139505c5bb3cd2e2aee86cd635d76d17374e))

### BREAKING CHANGES

* Container images are being deleted here and will also
get deleted from GHCR. Though the public APIs of the Typescript code
do not change, still, some parts of the documentation will become invalid
until we update it to match the changes here.
I invested a large amount of effort into doing this documentation update
as part of this change but it is very likely that I've missed a few spots
and therefore it is best to mark this as a breaking change in my opinion
to call attention to the fact that we still have ways to go with updating
the documentation around these container images.

1. Deleted all the container images that were just wrappers around the
cmd-api-server container image installing their own npm package from
the registry.
The reason for this is that they ended up just being maintenance burden
since we can achieve the exact same things just by re-using the API server's
container image directly.
2. This way we don't have to deal with CVEs in 10x container images when
it's really just the one container image that we use as the base that needs
to deal with them anyway.
3. I also spent quite a bit of effort in this change to update the README.md
files of the packages where previously we had plugin specific container images
defined so that the README.md files have the tutorials that are more up to
date compared to how they were (most of them had the tutorials completely
broken for a long while which was causing a lot of difficulties to the
newcomers who were trying to work with the packages).
4. The reason why they got so out of date traces back to the undue maintenance
burden of keeping separate images for each connector plugin. We hope that
with this simplification we can keep the documentation continuously up to
date since it will require less time do so.
5. Also deleted the ci.yaml container building jobs which were relevant to
the scope of this change so that we also save on CI resources, another
long-running project that's been in need of some attention from the maintainers.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
* Renamed classes to fix typos in their name: `PluginFactoryPersistanceFabric`
This is being done in this pull request because for some reason (that I still don't understand)
the spell checker started failing on these only in the context of this pull request.
The typos were present on the main branch already somehow having passed spellchecking earlier
and every other time since then.

And also
- prom-clien@15.1.3
- del-cli@5.1.0
- cspell@8.10.4
- del-cli@5.1.0

Quality of life improvements and also hoping to get rid of a few of the
vulnerable dependency versions we have in the codebase according to
dependabot.

More similar changes are coming in with further upgrades but I want to
avoid making bigger changes in one go so that it's easier to hunt down
bugs later if something only gets discovered after we've merged a bunch
of these.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
* **fabric-connector:** It accepts `type` instead of `skipDecode` flag.
- Move common block formatting logic to `cacti-block-formatters.ts`.
- Add tests for new features. Move test common to quering `qscc` to single file
  to increase CI speed.

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/v2.0.0-rc.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-24 15:30:43 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0-rc.3 - GO Fabric Weaver SDK - Jul 24, 2024
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    weaver/sdks/fabric/go-sdk/v2.0.0-rc.3
                </span>
            </td>
            <td>
                - Go Module: `github.com/hyperledger/cacti/weaver/sdks/fabric/go-sdk`
- Release: v2.0.0-rc.3
- Readme: [Here](https://github.com/hyperledger/cacti/blob/weaver/sdks/fabric/go-sdk/v2.0.0-rc.3/weaver/sdks/fabric/go-sdk/README.md).
- Source: [Here](https://github.com/hyperledger/cacti/blob/weaver/sdks/fabric/go-sdk/v2.0.0-rc.3/weaver/sdks/fabric/go-sdk)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/weaver/sdks/fabric/go-sdk/v2.0.0-rc.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-24 12:17:00 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0-rc.3 - GO Fabric Utils Library for Interoperation - Jul 24, 2024
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    weaver/core/network/fabric-interop-cc/libs/utils/v2.0.0-rc.3
                </span>
            </td>
            <td>
                - Go Module: `github.com/hyperledger/cacti/weaver/core/network/fabric-interop-cc/libs/utils`
- Release: v2.0.0-rc.3
- Readme: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/libs/utils/v2.0.0-rc.3/weaver/core/network/fabric-interop-cc/libs/utils/README.md).
- Source: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/libs/utils/v2.0.0-rc.3/weaver/core/network/fabric-interop-cc/libs/utils)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/weaver/core/network/fabric-interop-cc/libs/utils/v2.0.0-rc.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-24 12:17:00 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0-rc.3 - GO Fabric Library for Asset Exchange - Jul 24, 2024
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    weaver/core/network/fabric-interop-cc/libs/assetexchange/v2.0.0-rc.3
                </span>
            </td>
            <td>
                - Go Module: `github.com/hyperledger/cacti/weaver/core/network/fabric-interop-cc/libs/assetexchange`
- Release: v2.0.0-rc.3
- Readme: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/libs/assetexchange/v2.0.0-rc.3/weaver/core/network/fabric-interop-cc/libs/assetexchange/README.md).
- Source: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/libs/assetexchange/v2.0.0-rc.3/weaver/core/network/fabric-interop-cc/libs/assetexchange)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/weaver/core/network/fabric-interop-cc/libs/assetexchange/v2.0.0-rc.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-24 12:17:00 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0-rc.3 - GO Fabric Asset Management Interface - Jul 24, 2024
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt/v2.0.0-rc.3
                </span>
            </td>
            <td>
                - Go Module: `github.com/hyperledger/cacti/weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt`
- Release: v2.0.0-rc.3
- Readme: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt/v2.0.0-rc.3/weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt/README.md).
- Source: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt/v2.0.0-rc.3/weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt/v2.0.0-rc.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-24 12:17:00 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0-rc.3 - GO Fabric Interop Chaincode - Jul 24, 2024
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    weaver/core/network/fabric-interop-cc/contracts/interop/v2.0.0-rc.3
                </span>
            </td>
            <td>
                - Go Module: `github.com/hyperledger/cacti/weaver/core/network/fabric-interop-cc/contracts/interop`
- Release: v2.0.0-rc.3
- Readme: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/contracts/interop/v2.0.0-rc.3/weaver/core/network/fabric-interop-cc/contracts/interop/README.md).
- Source: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/contracts/interop/v2.0.0-rc.3/weaver/core/network/fabric-interop-cc/contracts/interop)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/weaver/core/network/fabric-interop-cc/contracts/interop/v2.0.0-rc.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-24 12:17:00 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0-rc.3 - GO Weaver Protos - Jul 24, 2024
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    weaver/common/protos-go/v2.0.0-rc.3
                </span>
            </td>
            <td>
                - Go Module: `github.com/hyperledger/cacti/weaver/common/protos-go`
- Release: v2.0.0-rc.3
- Readme: [Here](https://github.com/hyperledger/cacti/blob/weaver/common/protos-go/v2.0.0-rc.3/weaver/common/protos-go/README.md).
- Source: [Here](https://github.com/hyperledger/cacti/blob/weaver/common/protos-go/v2.0.0-rc.3/weaver/common/protos-go)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/weaver/common/protos-go/v2.0.0-rc.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-24 12:17:00 +0000 UTC
    </span>
</div>

