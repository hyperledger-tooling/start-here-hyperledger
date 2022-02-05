---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/cactus/issues/1567" class=".btn">1567</a>
            </td>
            <td>
                <b>
                    ci: enable caching of container image builds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">good-first-issue</span><span class="chip">help wanted</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span><span class="chip">Hacktoberfest</span><span class="chip">good-first-issue-400-expert</span><span class="chip">Flaky-Test-Automation</span><span class="chip">Tests</span><span class="chip">P3</span>
            </td>
            <td>
                ### Description

As a maintainer I want to make the CI faster and less wasteful so that it's easier to work with it and uses less energy in an attempt to save the planet.

Therefore the CI should check before building images if they were built already, e.g. some kind of shared cache among different executions would be nice because the way it is now, likely 95% of our image builds are producing the same SHAs from scratch every single time which is wasteful and slower than it should be and especially annoying when we get a flaky build fail even though it was passing several times before.

### Acceptance Criteria
1. Given an image SHA, it only ever gets built once on the CI
2. Applies to all of the image builds that we are doing as part of the `build-containers` CI job (10+ images IIRC)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 22:37:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/cactus/issues/1528" class=".btn">1528</a>
            </td>
            <td>
                <b>
                    test: stabilize cactus-plugin-htlc-eth-besu-erc20 openapi validation - refundV1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">good-first-issue</span><span class="chip">help wanted</span><span class="chip">Nice-to-Have</span><span class="chip">Besu</span><span class="chip">Security</span><span class="chip">Hacktoberfest</span><span class="chip">good-first-issue-400-expert</span><span class="chip">Flaky-Test-Automation</span><span class="chip">Tests</span><span class="chip">P4</span>
            </td>
            <td>
                **Describe the bug**

This test appears to be flaky:
`packages/cactus-test-plugin-htlc-eth-besu-erc20/src/test/typescript/integration/plugin-htlc-eth-besu-erc20/openapi/openapi-validation.test.ts:443:17`

**To Reproduce**

Run the CI enough times to see it happen.

**Expected behavior**

A clear and concise description of what you expected to happen.

**Logs/Stack traces**

Log archive of CI run (see Node 16 execution for error, Node 14 succeeded): [https://app.zenhub.com/files/216610150/ea67dae7-1d9a-4b99-8428-1ed0b1bee3ef/download](https://app.zenhub.com/files/216610150/ea67dae7-1d9a-4b99-8428-1ed0b1bee3ef/download)

Short Excerpt:

```sh
2021-11-09T18:05:59.9147459Z     # Test cactus-plugin-htlc-eth-besu-erc20 openapi validation - refundV1 - without bad request error
2021-11-09T18:05:59.9149431Z     ok 21 result is truthy OK
2021-11-09T18:06:07.2152565Z [2021-11-09T18:06:07.213Z] ERROR (RefundEndpoint): RefundEndpoint#handleRequest() failed to serve request Error: Transaction has been reverted by the EVM:
2021-11-09T18:06:07.2153975Z {
2021-11-09T18:06:07.2155444Z   "blockHash": "0x6d1b09fbc78b79b85277f464ddce84d9d756b13bb0af4214d20725e23eb76c91",
2021-11-09T18:06:07.2156523Z   "blockNumber": 17,
2021-11-09T18:06:07.2157020Z   "contractAddress": null,
2021-11-09T18:06:07.2157794Z   "cumulativeGasUsed": 24728,
2021-11-09T18:06:07.2158734Z   "from": "0x90f8bf6a479f320ead074411a4b0e7944ea8c9c1",
2021-11-09T18:06:07.2159435Z   "gasUsed": 24728,
2021-11-09T18:06:07.2159888Z   "logs": [],
2021-11-09T18:06:07.2161202Z   "logsBloom": "0x00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000",
2021-11-09T18:06:07.2163113Z   "status": false,
2021-11-09T18:06:07.2163887Z   "to": "0xe78a0f7e598cc8b0bb87894b0f60dd2a88d6a8ab",
2021-11-09T18:06:07.2165182Z   "transactionHash": "0xef941d252d9907ea7d10217db363266d9e646b3a25d385ee229e34f53433549b",
2021-11-09T18:06:07.2166249Z   "transactionIndex": 0,
2021-11-09T18:06:07.2167533Z   "revertReason": "0x08c379a00000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000000c494e56414c49445f54494d450000000000000000000000000000000000000000"
2021-11-09T18:06:07.2168580Z }
2021-11-09T18:06:07.2170210Z     at Object.TransactionError (/home/runner/work/cactus/cactus/node_modules/web3-eth/node_modules/web3-core-helpers/lib/errors.js:87:21)
2021-11-09T18:06:07.2173452Z     at Object.TransactionRevertedWithoutReasonError (/home/runner/work/cactus/cactus/node_modules/web3-eth/node_modules/web3-core-helpers/lib/errors.js:98:21)
2021-11-09T18:06:07.2175471Z     at /home/runner/work/cactus/cactus/node_modules/web3-eth/node_modules/web3-core-method/lib/index.js:393:57
2021-11-09T18:06:07.2176571Z     at processTicksAndRejections (node:internal/process/task_queues:96:5) {
2021-11-09T18:06:07.2177535Z   receipt: {
2021-11-09T18:06:07.2178795Z     blockHash: '0x6d1b09fbc78b79b85277f464ddce84d9d756b13bb0af4214d20725e23eb76c91',
2021-11-09T18:06:07.2179765Z     blockNumber: 17,
2021-11-09T18:06:07.2180633Z     contractAddress: null,
2021-11-09T18:06:07.2181192Z     cumulativeGasUsed: 24728,
2021-11-09T18:06:07.2182121Z     from: '0x90f8bf6a479f320ead074411a4b0e7944ea8c9c1',
2021-11-09T18:06:07.2182829Z     gasUsed: 24728,
2021-11-09T18:06:07.2183276Z     logs: [],
2021-11-09T18:06:07.2185253Z     logsBloom: '0x00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000',
2021-11-09T18:06:07.2186288Z     status: false,
2021-11-09T18:06:07.2187230Z     to: '0xe78a0f7e598cc8b0bb87894b0f60dd2a88d6a8ab',
2021-11-09T18:06:07.2188651Z     transactionHash: '0xef941d252d9907ea7d10217db363266d9e646b3a25d385ee229e34f53433549b',
2021-11-09T18:06:07.2699663Z     transactionIndex: 0,
2021-11-09T18:06:07.2702276Z     revertReason: '0x08c379a00000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000000c494e56414c49445f54494d450000000000000000000000000000000000000000'
2021-11-09T18:06:07.2703396Z   }
2021-11-09T18:06:07.2703868Z }
2021-11-09T18:06:07.2854324Z     not ok 22 Error: Request failed with status code 400
2021-11-09T18:06:07.2901234Z       ---
2021-11-09T18:06:07.2902485Z         operator: error
2021-11-09T18:06:07.2904059Z         at: bound (/home/runner/work/cactus/cactus/node_modules/tape-promise/node_modules/onetime/index.js:30:12)
2021-11-09T18:06:07.2905098Z         stack: |-
2021-11-09T18:06:07.2905747Z           Error: Request failed with status code 400
2021-11-09T18:06:07.2906732Z               at createError (/home/runner/work/cactus/cactus/node_modules/axios/lib/core/createError.js:16:15)
2021-11-09T18:06:07.2907823Z               at settle (/home/runner/work/cactus/cactus/node_modules/axios/lib/core/settle.js:17:12)
2021-11-09T18:06:07.2909261Z               at /home/runner/work/cactus/cactus/node_modules/axios-cookiejar-support/lib/interceptors/response.js:83:25
2021-11-09T18:06:07.2910272Z               at new Promise (<anonymous>)
2021-11-09T18:06:07.2925417Z               at responseInterceptor (/home/runner/work/cactus/cactus/node_modules/axios-cookiejar-support/lib/interceptors/response.js:82:9)
2021-11-09T18:06:07.2927356Z               at /home/runner/work/cactus/cactus/node_modules/axios-cookiejar-support/lib/index.js:130:67
2021-11-09T18:06:07.2928992Z               at processTicksAndRejections (node:internal/process/task_queues:96:5)
2021-11-09T18:06:07.2931313Z               at async /home/runner/work/cactus/cactus/packages/cactus-test-plugin-htlc-eth-besu-erc20/src/test/typescript/integration/plugin-htlc-eth-besu-erc20/openapi/openapi-validation.test.ts:443:17
2021-11-09T18:06:07.2933249Z       ...
2021-11-09T18:06:07.3162026Z     # Test cactus-plugin-htlc-eth-besu-erc20 openapi validation - refundV1 - not sending all required parameters
2021-11-09T18:06:07.3165184Z     Bail out! Error: Request failed with status code 400
2021-11-09T18:06:07.3335551Z Bail out! Error: Request failed with status code 400
```

**Cloud provider or hardware configuration:**

GHA CI runner

**Operating system name, version, build:**

Ubuntu 20.04

**Hyperledger Cactus release version or commit (git rev-parse --short HEAD):**

1.0.0-rc.2

**Hyperledger Cactus Plugins/Connectors Used**

Besu/HTLC ERC 20

**Additional context**

This flake was noticed while the CI ran against the main branch after a PR merge.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 00:18:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/cactus/issues/1495" class=".btn">1495</a>
            </td>
            <td>
                <b>
                    test: fix flake in install-basic-plugin-ledger-connector-fabric-0-7-0.test.ts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">good-first-issue</span><span class="chip">help wanted</span><span class="chip">API_Server</span><span class="chip">Nice-to-Have</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span><span class="chip">Hacktoberfest</span><span class="chip">good-first-issue-400-expert</span><span class="chip">Flaky-Test-Automation</span><span class="chip">Tests</span>
            </td>
            <td>
                **Describe the bug**

The test fails in the CI environment intermittently:
`packages/cactus-cmd-api-server/src/test/typescript/unit/plugins/install-basic-plugin-ledger-connector-fabric-0-7-0.test.ts`

**To Reproduce**

Run the CI enough times to make it fail.

**Expected behavior**

Test is stable/consistent in it's outcome.

**Logs/Stack traces**

Complete log archives of the full CI run:  [logs_10454.zip](https://github.com/hyperledger/cactus/files/7464078/logs_10454.zip)

Relevant snippet:

```sh
# Subtest: packages/cactus-cmd-api-server/src/test/typescript/unit/plugins/install-basic-plugin-ledger-connector-fabric-0-7-0.test.ts
    # can install plugin-ledger-connector-fabric
    Warning: configuration param 'type' not declared in the schema
    [2021-11-02T18:03:33.486Z] INFO (config-service): Configuration validation OK.
    [2021-11-02T18:03:33.503Z] DEBUG (api-server): pluginsPath: '/home/runner/work/cactus/cactus/.tmp/test/cmd-api-server/runtime-plugin-imports_test/43a396a5-f016-4be5-85ef-21ab165e6a69'
    [2021-11-02T18:03:33.504Z] INFO (api-server): Setting tls.DEFAULT_MAX_VERSION to TLSv1.3...
    [2021-11-02T18:03:33.505Z] INFO (api-server): wwwRoot: packages/cactus-cmd-api-server/node_modules/@hyperledger/cactus-cockpit/www/
    [2021-11-02T18:03:33.505Z] INFO (api-server): resolvedWwwRoot: /home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/node_modules/@hyperledger/cactus-cockpit/www
    [2021-11-02T18:03:33.505Z] INFO (api-server): resolvedIndexHtml: /home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/node_modules/@hyperledger/cactus-cockpit/www/index.html
    [2021-11-02T18:03:33.510Z] INFO (api-server): Cactus Cockpit net.AddressInfo { address: '127.0.0.1', family: 'IPv4', port: 42967 }
    [2021-11-02T18:03:33.512Z] INFO (api-server): getOrInitPluginRegistry() initializing a new one...
    [2021-11-02T18:03:33.512Z] INFO (api-server): Instantiated empty registry, invoking plugin factories...
    [2021-11-02T18:03:33.512Z] INFO (api-server): Creating plugin from package: @hyperledger/cactus-plugin-ledger-connector-fabric {
      instanceId: '410cf847-dd52-4b2f-90ff-9c36277ab46e',
      logLevel: 'TRACE',
      connectionProfile: {},
      peerBinary: 'peer'
    }
    [2021-11-02T18:03:33.515Z] DEBUG (api-server): @hyperledger/cactus-plugin-ledger-connector-fabric plugin package dir: '/home/runner/work/cactus/cactus/.tmp/test/cmd-api-server/runtime-plugin-imports_test/43a396a5-f016-4be5-85ef-21ab165e6a69/410cf847-dd52-4b2f-90ff-9c36277ab46e'
    [2021-11-02T18:03:33.515Z] DEBUG (api-server): Installing @hyperledger/cactus-plugin-ledger-connector-fabric for plugin import {
      packageName: '@hyperledger/cactus-plugin-ledger-connector-fabric',
      type: 'org.hyperledger.cactus.plugin_import_type.LOCAL',
      options: {
        instanceId: '410cf847-dd52-4b2f-90ff-9c36277ab46e',
        logLevel: 'TRACE',
        connectionProfile: {},
        peerBinary: 'peer'
      }
    }
npm ERR! code ETARGET
npm ERR! notarget No matching version found for @hyperledger/cactus-common@1.0.0-rc.2.
npm ERR! notarget In most cases you or one of your dependencies are requesting
npm ERR! notarget a package version that doesn't exist.

npm ERR! A complete log of this run can be found in:
npm ERR!     /home/runner/.npm/_logs/2021-11-02T18_04_24_139Z-debug.log
[2021-11-02T18:04:24.182Z] ERROR (api-server): Failed to start ApiServer: RuntimeError: ApiServer#installPluginPackage() plugin install fail: @hyperledger/cactus-plugin-ledger-connector-fabric
    at ApiServer.installPluginPackage (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:14:406)
    at processTicksAndRejections (internal/process/task_queues.js:95:5)
    at async ApiServer.instantiatePlugin (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:8:2659)
    at async ApiServer.initPluginRegistry (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:8:2073)
    at async ApiServer.getOrInitPluginRegistry (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:8:1240)
    at async ApiServer.startApiServer (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:4:21)
    at async ApiServer.start (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:3:5740)
    at async /home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/test/typescript/unit/plugins/install-basic-plugin-ledger-connector-fabric-0-7-0.test.ts:63:3
[2021-11-02T18:04:24.182Z] ERROR (api-server): Attempting shutdown...
    [2021-11-02T18:04:24.182Z] INFO (api-server): Shutting down API server ...
    [2021-11-02T18:04:24.183Z] INFO (api-server): getOrInitPluginRegistry() initializing a new one...
    [2021-11-02T18:04:24.183Z] INFO (api-server): Instantiated empty registry, invoking plugin factories...
    [2021-11-02T18:04:24.183Z] INFO (api-server): Creating plugin from package: @hyperledger/cactus-plugin-ledger-connector-fabric {
      instanceId: '410cf847-dd52-4b2f-90ff-9c36277ab46e',
      logLevel: 'TRACE',
      connectionProfile: {},
      peerBinary: 'peer'
    }
    [2021-11-02T18:04:24.186Z] DEBUG (api-server): @hyperledger/cactus-plugin-ledger-connector-fabric plugin package dir: '/home/runner/work/cactus/cactus/.tmp/test/cmd-api-server/runtime-plugin-imports_test/43a396a5-f016-4be5-85ef-21ab165e6a69/410cf847-dd52-4b2f-90ff-9c36277ab46e'
    [2021-11-02T18:04:24.186Z] DEBUG (api-server): Installing @hyperledger/cactus-plugin-ledger-connector-fabric for plugin import {
      packageName: '@hyperledger/cactus-plugin-ledger-connector-fabric',
      type: 'org.hyperledger.cactus.plugin_import_type.LOCAL',
      options: {
        instanceId: '410cf847-dd52-4b2f-90ff-9c36277ab46e',
        logLevel: 'TRACE',
        connectionProfile: {},
        peerBinary: 'peer'
      }
    }
npm ERR! code ETARGET
npm ERR! notarget No matching version found for @hyperledger/cactus-common@1.0.0-rc.2.
npm ERR! notarget In most cases you or one of your dependencies are requesting
npm ERR! notarget a package version that doesn't exist.

npm ERR! A complete log of this run can be found in:
npm ERR!     /home/runner/.npm/_logs/2021-11-02T18_04_26_792Z-debug.log
[2021-11-02T18:04:26.817Z] ERROR (api-server): API server failed to shut itself down, will ignore this because we were already crashing anyway... r [RuntimeError]: ApiServer#installPluginPackage() plugin install fail: @hyperledger/cactus-plugin-ledger-connector-fabric
    at ApiServer.installPluginPackage (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:14:406)
    at processTicksAndRejections (internal/process/task_queues.js:95:5)
    at async ApiServer.instantiatePlugin (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:8:2659)
    at async ApiServer.initPluginRegistry (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:8:2073)
    at async ApiServer.getOrInitPluginRegistry (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:8:1240)
    at async ApiServer.shutdown (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:14:652)
    at async ApiServer.start (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:3:7220)
    at async /home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/test/typescript/unit/plugins/install-basic-plugin-ledger-connector-fabric-0-7-0.test.ts:63:3 {
  cause: Error: Command failed with exit code 1: npm install @hyperledger/cactus-plugin-ledger-connector-fabric --production --audit=false --progress=false --fund=false --prefix=/home/runner/work/cactus/cactus/.tmp/test/cmd-api-server/runtime-plugin-imports_test/43a396a5-f016-4be5-85ef-21ab165e6a69/410cf847-dd52-4b2f-90ff-9c36277ab46e
      at makeError (/home/runner/work/cactus/cactus/node_modules/lmify/node_modules/execa/lib/error.js:59:11)
      at handlePromise (/home/runner/work/cactus/cactus/node_modules/lmify/node_modules/execa/index.js:114:26)
      at processTicksAndRejections (internal/process/task_queues.js:95:5)
      at async ApiServer.installPluginPackage (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:13:203)
      at async ApiServer.instantiatePlugin (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:8:2659)
      at async ApiServer.initPluginRegistry (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:8:2073)
      at async ApiServer.getOrInitPluginRegistry (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:8:1240)
      at async ApiServer.shutdown (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:14:652)
      at async ApiServer.start (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:3:7220)
      at async /home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/test/typescript/unit/plugins/install-basic-plugin-ledger-connector-fabric-0-7-0.test.ts:63:3 {
    shortMessage: 'Command failed with exit code 1: npm install @hyperledger/cactus-plugin-ledger-connector-fabric --production --audit=false --progress=false --fund=false --prefix=/home/runner/work/cactus/cactus/.tmp/test/cmd-api-server/runtime-plugin-imports_test/43a396a5-f016-4be5-85ef-21ab165e6a69/410cf847-dd52-4b2f-90ff-9c36277ab46e',
    command: 'npm install @hyperledger/cactus-plugin-ledger-connector-fabric --production --audit=false --progress=false --fund=false --prefix=/home/runner/work/cactus/cactus/.tmp/test/cmd-api-server/runtime-plugin-imports_test/43a396a5-f016-4be5-85ef-21ab165e6a69/410cf847-dd52-4b2f-90ff-9c36277ab46e',
    exitCode: 1,
    signal: undefined,
    signalDescription: undefined,
    stdout: undefined,
    stderr: undefined,
    failed: true,
    timedOut: false,
    isCanceled: false,
    killed: false
  }
}
    not ok 1 started API server dynamic imports OK
      ---
        operator: throws
        expected: |-
          undefined
        actual: |-
          [Error: Failed to start ApiServer: RuntimeError: ApiServer#installPluginPackage() plugin install fail: @hyperledger/cactus-plugin-ledger-connector-fabric
        at ApiServer.installPluginPackage (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:14:406)
        at processTicksAndRejections (internal/process/task_queues.js:95:5)
        at async ApiServer.instantiatePlugin (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:8:2659)
        at async ApiServer.initPluginRegistry (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:8:2073)
        at async ApiServer.getOrInitPluginRegistry (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:8:1240)
        at async ApiServer.startApiServer (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:4:21)
        at async ApiServer.start (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:3:5740)
        at async /home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/test/typescript/unit/plugins/install-basic-plugin-ledger-connector-fabric-0-7-0.test.ts:63:3]
        at: <anonymous> (/home/runner/work/cactus/cactus/node_modules/tape-promise/index.compiled.js:56:12)
        stack: |-
          Error: Failed to start ApiServer: RuntimeError: ApiServer#installPluginPackage() plugin install fail: @hyperledger/cactus-plugin-ledger-connector-fabric
              at ApiServer.installPluginPackage (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:14:406)
              at processTicksAndRejections (internal/process/task_queues.js:95:5)
              at async ApiServer.instantiatePlugin (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:8:2659)
              at async ApiServer.initPluginRegistry (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:8:2073)
              at async ApiServer.getOrInitPluginRegistry (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:8:1240)
              at async ApiServer.startApiServer (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:4:21)
              at async ApiServer.start (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:3:5740)
              at async /home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/test/typescript/unit/plugins/install-basic-plugin-ledger-connector-fabric-0-7-0.test.ts:63:3
              at ApiServer.start (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:3:7435)
              at processTicksAndRejections (internal/process/task_queues.js:95:5)
              at async /home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/test/typescript/unit/plugins/install-basic-plugin-ledger-connector-fabric-0-7-0.test.ts:63:3
      ...
    Bail out! started API server dynamic imports OK
Bail out! started API server dynamic imports OK
```

**Screenshots**

Nope.

**Cloud provider or hardware configuration:**

GHA CI runner

**Operating system name, version, build:**

Ubuntu 20.04

**Hyperledger Cactus release version or commit (git rev-parse --short HEAD):**

rc2

**Hyperledger Cactus Plugins/Connectors Used**

N/A

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 21:35:16 +0000 UTC
    </div>
</div>

