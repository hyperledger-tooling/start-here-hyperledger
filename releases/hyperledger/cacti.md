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
                    v2.0.0-rc.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v2.0.0-rc.2
                </span>
            </td>
            <td>
                # [2.0.0-rc.2](https://github.com/hyperledger/cacti/compare/v2.0.0-rc.1...v2.0.0-rc.2) (2024-07-03)

### Bug Fixes

* **cmd-api-server:** shutdown hook was not waiting for promises ([d14bf02](https://github.com/hyperledger/cacti/commit/d14bf02aed215eeecdba258bb48a330da3fc2c36))
* **cmd-api-server:** stop changing LoggerProvider log level ([6ef514c](https://github.com/hyperledger/cacti/commit/6ef514cc01eda2640ed144bdd4750dbcb1e35e27))
* **deps:** fix batch of missing production dependencies v2.0.0-rc.1 ([51d64ee](https://github.com/hyperledger/cacti/commit/51d64eead473d928086eb53adf0850c3b43cbda9)), closes [#3344](https://github.com/hyperledger/cacti/issues/3344)
* **go-sdk:** use protos v1 api for fabric-protos-go unmarshal ([8896518](https://github.com/hyperledger/cacti/commit/88965187de69076420237a93548a9e5fdd7f0e74))
* **plugin-persistence-ethereum:** make created_at TIMESTAMPTZ in schema ([08925ff](https://github.com/hyperledger/cacti/commit/08925ffc8815d9613a69204a74c85d168f8a8305)), closes [#3373](https://github.com/hyperledger/cacti/issues/3373)

### Features

* **cactus-example-tcs-huawei:** remove deprecated sample app ([45fadcd](https://github.com/hyperledger/cacti/commit/45fadcd089bb59cf5f604110030a5e7eba5d67b2)), closes [#3155](https://github.com/hyperledger/cacti/issues/3155) [#3157](https://github.com/hyperledger/cacti/issues/3157)
* **connector-besu:** expose API client and OpenAPI code for web builds ([199c1f0](https://github.com/hyperledger/cacti/commit/199c1f05c282d15ba2ded9e7a69253483fbac2ec))
* **connector-corda:** add initial set of JvmObject factory functions ([d9d5904](https://github.com/hyperledger/cacti/commit/d9d590450af6d231c5e38046bffd6d08786c29f4))
* **connector-corda:** add JSON classname->JVM class object deserialize ([0508f14](https://github.com/hyperledger/cacti/commit/0508f14c64e452f8f89881db363cd00b3c8c255c))
* **fabric-driver:** added weaver fabric driver as cacti plugin package ([36b8470](https://github.com/hyperledger/cacti/commit/36b8470f8a159bcb16c5ef62074aee2ff99758eb))
* **ledger-browser:** refactor eth dashboard page ([c69fb4c](https://github.com/hyperledger/cacti/commit/c69fb4c5982669d335870218c617ff847fbe1db9)), closes [#3207](https://github.com/hyperledger/cacti/issues/3207)
* **ledger-browser:** refactor eth tokens page into accounts page ([0b0c22c](https://github.com/hyperledger/cacti/commit/0b0c22cd39fb67e809595ceb23fb8b3c2a0f1da0)), closes [#3237](https://github.com/hyperledger/cacti/issues/3237)
* **ledger-browser:** refactor routing, improve UI ([3fcc7a1](https://github.com/hyperledger/cacti/commit/3fcc7a1215435341db927ec211af598a0a298d44))
* **ledger-browser:** use react query in eth app ([4d3fb7e](https://github.com/hyperledger/cacti/commit/4d3fb7e25d78804ffda498e9cdd4600bf0a50f0c)), closes [#3203](https://github.com/hyperledger/cacti/issues/3203)

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/v2.0.0-rc.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-04 15:17:41 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0-rc.2 - GO Fabric Weaver SDK - Jul 04, 2024
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    weaver/sdks/fabric/go-sdk/v2.0.0-rc.2
                </span>
            </td>
            <td>
                - Go Module: `github.com/hyperledger/cacti/weaver/sdks/fabric/go-sdk`
- Release: v2.0.0-rc.2
- Readme: [Here](https://github.com/hyperledger/cacti/blob/weaver/sdks/fabric/go-sdk/v2.0.0-rc.2/weaver/sdks/fabric/go-sdk/README.md).
- Source: [Here](https://github.com/hyperledger/cacti/blob/weaver/sdks/fabric/go-sdk/v2.0.0-rc.2/weaver/sdks/fabric/go-sdk)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/weaver/sdks/fabric/go-sdk/v2.0.0-rc.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-03 22:47:17 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0-rc.2 - GO Fabric Utils Library for Interoperation - Jul 04, 2024
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    weaver/core/network/fabric-interop-cc/libs/utils/v2.0.0-rc.2
                </span>
            </td>
            <td>
                - Go Module: `github.com/hyperledger/cacti/weaver/core/network/fabric-interop-cc/libs/utils`
- Release: v2.0.0-rc.2
- Readme: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/libs/utils/v2.0.0-rc.2/weaver/core/network/fabric-interop-cc/libs/utils/README.md).
- Source: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/libs/utils/v2.0.0-rc.2/weaver/core/network/fabric-interop-cc/libs/utils)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/weaver/core/network/fabric-interop-cc/libs/utils/v2.0.0-rc.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-03 22:47:17 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0-rc.2 - GO Fabric Library for Asset Exchange - Jul 04, 2024
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    weaver/core/network/fabric-interop-cc/libs/assetexchange/v2.0.0-rc.2
                </span>
            </td>
            <td>
                - Go Module: `github.com/hyperledger/cacti/weaver/core/network/fabric-interop-cc/libs/assetexchange`
- Release: v2.0.0-rc.2
- Readme: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/libs/assetexchange/v2.0.0-rc.2/weaver/core/network/fabric-interop-cc/libs/assetexchange/README.md).
- Source: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/libs/assetexchange/v2.0.0-rc.2/weaver/core/network/fabric-interop-cc/libs/assetexchange)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/weaver/core/network/fabric-interop-cc/libs/assetexchange/v2.0.0-rc.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-03 22:47:17 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0-rc.2 - GO Fabric Asset Management Interface - Jul 04, 2024
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt/v2.0.0-rc.2
                </span>
            </td>
            <td>
                - Go Module: `github.com/hyperledger/cacti/weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt`
- Release: v2.0.0-rc.2
- Readme: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt/v2.0.0-rc.2/weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt/README.md).
- Source: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt/v2.0.0-rc.2/weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/weaver/core/network/fabric-interop-cc/interfaces/asset-mgmt/v2.0.0-rc.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-03 22:47:17 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0-rc.2 - GO Fabric Interop Chaincode - Jul 04, 2024
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    weaver/core/network/fabric-interop-cc/contracts/interop/v2.0.0-rc.2
                </span>
            </td>
            <td>
                - Go Module: `github.com/hyperledger/cacti/weaver/core/network/fabric-interop-cc/contracts/interop`
- Release: v2.0.0-rc.2
- Readme: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/contracts/interop/v2.0.0-rc.2/weaver/core/network/fabric-interop-cc/contracts/interop/README.md).
- Source: [Here](https://github.com/hyperledger/cacti/blob/weaver/core/network/fabric-interop-cc/contracts/interop/v2.0.0-rc.2/weaver/core/network/fabric-interop-cc/contracts/interop)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/weaver/core/network/fabric-interop-cc/contracts/interop/v2.0.0-rc.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-03 22:47:17 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.0.0-rc.2 - GO Weaver Protos - Jul 04, 2024
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    weaver/common/protos-go/v2.0.0-rc.2
                </span>
            </td>
            <td>
                - Go Module: `github.com/hyperledger/cacti/weaver/common/protos-go`
- Release: v2.0.0-rc.2
- Readme: [Here](https://github.com/hyperledger/cacti/blob/weaver/common/protos-go/v2.0.0-rc.2/weaver/common/protos-go/README.md).
- Source: [Here](https://github.com/hyperledger/cacti/blob/weaver/common/protos-go/v2.0.0-rc.2/weaver/common/protos-go)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cacti/releases/tag/weaver/common/protos-go/v2.0.0-rc.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-03 22:47:17 +0000 UTC
    </span>
</div>

