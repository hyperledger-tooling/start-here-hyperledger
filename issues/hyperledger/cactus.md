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

