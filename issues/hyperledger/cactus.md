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
                Issue <a href="https://github.com/hyperledger/cactus/issues/1471" class=".btn">1471</a>
            </td>
            <td>
                <b>
                    test(connector-fabric): fix flaky test 2.2.x deploy-cc-from-javascript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">good-first-issue</span><span class="chip">help wanted</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span><span class="chip">Hacktoberfest</span><span class="chip">good-first-issue-400-expert</span><span class="chip">Flaky-Test-Automation</span><span class="chip">Tests</span>
            </td>
            <td>
                **Describe the bug**

We've got a flaky one at:
`packages/cactus-plugin-ledger-connector-fabric/src/test/typescript/integration/fabric-v2-2-x/deploy-cc-from-javascript-source.test.ts`

```sh
2021-10-19T08:07:31.364Z - error: [DiscoveryHandler]: compareProposalResponseResults[undefined] - read/writes result sets do not match index=1
2021-10-19T08:07:31.365Z - error: [Transaction]: Error: No valid responses from any peers. Errors:
    peer=undefined, status=grpc, message=Peer endorsements do not match
[2021-10-19T08:07:31.366Z] ERROR (PluginLedgerConnectorFabric): transact() crashed:  Error: No valid responses from any peers. Errors:
    peer=undefined, status=grpc, message=Peer endorsements do not match
    at newEndorsementError (/home/runner/work/cactus/cactus/packages/cactus-plugin-ledger-connector-fabric/node_modules/fabric-network/src/transaction.ts:69:9)
    at getResponsePayload (/home/runner/work/cactus/cactus/packages/cactus-plugin-ledger-connector-fabric/node_modules/fabric-network/src/transaction.ts:22:17)
    at Transaction.submit (/home/runner/work/cactus/cactus/packages/cactus-plugin-ledger-connector-fabric/node_modules/fabric-network/src/transaction.ts:294:19)
    at processTicksAndRejections (node:internal/process/task_queues:96:5)
    at async PluginLedgerConnectorFabric.transact (/home/runner/work/cactus/cactus/packages/cactus-plugin-ledger-connector-fabric/src/main/typescript/plugin-ledger-connector-fabric.ts:172:75)
    at async RunTransactionEndpointV1.handleRequest (/home/runner/work/cactus/cactus/packages/cactus-plugin-ledger-connector-fabric/src/main/typescript/run-transaction/run-transaction-endpoint-v1.ts:3:1283) {
  responses: [],
  errors: [
    Error: Peer endorsements do not match
        at DiscoveryHandler._endorse (/home/runner/work/cactus/cactus/packages/cactus-plugin-ledger-connector-fabric/node_modules/fabric-network/node_modules/fabric-common/lib/DiscoveryHandler.js:295:14)
        at processTicksAndRejections (node:internal/process/task_queues:96:5)
        at async Endorsement.send (/home/runner/work/cactus/cactus/packages/cactus-plugin-ledger-connector-fabric/node_modules/fabric-network/node_modules/fabric-common/lib/Proposal.js:410:15)
        at async Transaction.submit (/home/runner/work/cactus/cactus/packages/cactus-plugin-ledger-connector-fabric/node_modules/fabric-network/src/transaction.ts:292:28)
        at async PluginLedgerConnectorFabric.transact (/home/runner/work/cactus/cactus/packages/cactus-plugin-ledger-connector-fabric/src/main/typescript/plugin-ledger-connector-fabric.ts:172:75)
        at async RunTransactionEndpointV1.handleRequest (/home/runner/work/cactus/cactus/packages/cactus-plugin-ledger-connector-fabric/src/main/typescript/run-transaction/run-transaction-endpoint-v1.ts:3:1283) {
      endorsements: [Array]
    }
  ]
}
[2021-10-19T08:07:31.416Z] ERROR (run-transaction-endpoint-v1): RunTransactionEndpointV1#handleRequest() failed to serve request Error: PluginLedgerConnectorFabric#transact() Unable to run transaction: No valid responses from any peers. Errors:
    peer=undefined, status=grpc, message=Peer endorsements do not match
    at PluginLedgerConnectorFabric.transact (/home/runner/work/cactus/cactus/packages/cactus-plugin-ledger-connector-fabric/src/main/typescript/plugin-ledger-connector-fabric.ts:173:81)
    at processTicksAndRejections (node:internal/process/task_queues:96:5)
    at async RunTransactionEndpointV1.handleRequest (/home/runner/work/cactus/cactus/packages/cactus-plugin-ledger-connector-fabric/src/main/typescript/run-transaction/run-transaction-endpoint-v1.ts:3:1283)
TypeError [ERR_INVALID_CHAR]: Invalid character in statusMessage
    at new NodeError (node:internal/errors:371:5)
    at ServerResponse.writeHead (node:_http_server:323:11)
    at ServerResponse._implicitHeader (node:_http_server:266:8)
    at write_ (node:_http_outgoing:763:9)
    at ServerResponse.end (node:_http_outgoing:852:5)
    at ServerResponse.send (/home/runner/work/cactus/cactus/node_modules/express/lib/response.js:221:10)
    at ServerResponse.json (/home/runner/work/cactus/cactus/node_modules/express/lib/response.js:267:15)
    at RunTransactionEndpointV1.handleRequest (/home/runner/work/cactus/cactus/packages/cactus-plugin-ledger-connector-fabric/src/main/typescript/run-transaction/run-transaction-endpoint-v1.ts:3:1626)
    at processTicksAndRejections (node:internal/process/task_queues:96:5) {
  code: 'ERR_INVALID_CHAR'
}
    [2021-10-19T08:07:21.099Z] DEBUG (FabricTestLedgerV1): [ghcr.io/hyperledger/cactus-fabric2-all-in-one:2021-09-02--fix-876-supervisord-retries] 'time="2021-10-19T08:07:21.098239687Z" level=info msg="starting signal loop" namespace=moby path=/run/docker/containerd/daemon/io.containerd.runtime.v2.task/moby/ccef22b5fafcb85bc871020341a66c9710f87345eed3c8f29d941dbf86993595 pid=8108\r\n'
    [2021-10-19T08:07:21.100Z] DEBUG (FabricTestLedgerV1): [ghcr.io/hyperledger/cactus-fabric2-all-in-one:2021-09-02--fix-876-supervisord-retries] "2021-10-19 08:07:21,100 DEBG 'dockerd' stderr output:\r\n"
    [2021-10-19T08:07:21.101Z] DEBUG (FabricTestLedgerV1): [ghcr.io/hyperledger/cactus-fabric2-all-in-one:2021-09-02--fix-876-supervisord-retries] 'time="2021-10-19T08:07:21.098239687Z" level=info msg="starting signal loop" namespace=moby path=/run/docker/containerd/daemon/io.containerd.runtime.v2.task/moby/ccef22b5fafcb85bc871020341a66c9710f87345eed3c8f29d941dbf86993595 pid=8108\r\n'
    [2021-10-19T08:07:21.102Z] DEBUG (FabricTestLedgerV1): [ghcr.io/hyperledger/cactus-fabric2-all-in-one:2021-09-02--fix-876-supervisord-retries] '\r\n'
    [2021-10-19T08:07:21.140Z] DEBUG (FabricTestLedgerV1): [ghcr.io/hyperledger/cactus-fabric2-all-in-one:2021-09-02--fix-876-supervisord-retries] 'time="2021-10-19T08:07:21.131972625Z" level=info msg="starting signal loop" namespace=moby path=/run/docker/containerd/daemon/io.containerd.runtime.v2.task/moby/44c89c9cada869351d3b0e667e13e3b5131d1a2d7142fa76c7dc999174ed942e pid=8127\r\n'
    [2021-10-19T08:07:21.140Z] DEBUG (FabricTestLedgerV1): [ghcr.io/hyperledger/cactus-fabric2-all-in-one:2021-09-02--fix-876-supervisord-retries] "2021-10-19 08:07:21,138 DEBG 'dockerd' stderr output:\r\n"
    [2021-10-19T08:07:21.140Z] DEBUG (FabricTestLedgerV1): [ghcr.io/hyperledger/cactus-fabric2-all-in-one:2021-09-02--fix-876-supervisord-retries] 'time="2021-10-19T08:07:21.131972625Z" level=info msg="starting signal loop" namespace=moby path=/run/docker/containerd/daemon/io.containerd.runtime.v2.task/moby/44c89c9cada869351d3b0e667e13e3b5131d1a2d7142fa76c7dc999174ed942e pid=8127\r\n'
    [2021-10-19T08:07:21.140Z] DEBUG (FabricTestLedgerV1): [ghcr.io/hyperledger/cactus-fabric2-all-in-one:2021-09-02--fix-876-supervisord-retries] '\r\n'
    [2021-10-19T08:07:31.047Z] DEBUG (run-transaction-endpoint-v1): POST /api/v1/plugins/@hyperledger/cactus-plugin-ledger-connector-fabric/run-transaction
    [2021-10-19T08:07:31.051Z] DEBUG (PluginLedgerConnectorFabric): discovery={ enabled: true, asLocalhost: true }
    [2021-10-19T08:07:31.051Z] DEBUG (PluginLedgerConnectorFabric): eventHandlerOptions={
      commitTimeout: 300,
      endorseTimeout: 300,
      strategy: [Function: NETWORK_SCOPE_ALLFORTX] {
        [length]: 2,
        [name]: 'NETWORK_SCOPE_ALLFORTX'
      }
    }
    [2021-10-19T08:07:31.244Z] DEBUG (PluginLedgerConnectorFabric): transact() gateway connection established OK
    # test count(4) != plan(null)
    # failed 1 of 4 tests
```

**To Reproduce**

Keep running the test and eventually you'll see it.

**Expected behavior**

Tests are stable, not flaky.

**Logs/Stack traces**

The CI logs from the GHA runner as of this morning:
[logs_10074.zip](https://github.com/hyperledger/cactus/files/7393247/logs_10074.zip)

**Cloud provider or hardware configuration:**

GHA runner

**Operating system name, version, build:**

Ubuntu 20.04

**Hyperledger Cactus release version or commit (git rev-parse --short HEAD):**

1.0.0-rc.1

**Hyperledger Cactus Plugins/Connectors Used**

Fabric

**Additional context**

I'll send a separate PR that skips this test to avoid flakiness in the meantime.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 22:42:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/cactus/issues/1469" class=".btn">1469</a>
            </td>
            <td>
                <b>
                    test(connector-corda): fix flaky v4.8 test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">good-first-issue</span><span class="chip">help wanted</span><span class="chip">Corda</span><span class="chip">Developer_Experience</span><span class="chip">Hacktoberfest</span><span class="chip">good-first-issue-400-expert</span><span class="chip">Flaky-Test-Automation</span><span class="chip">Tests</span>
            </td>
            <td>
                **Describe the bug**

We've got a flaky one at:
packages/cactus-plugin-ledger-connector-corda/src/test/typescript/integration/deploy-cordapp-jars-to-nodes-v4.8.test.ts

One of the corda nodes within the container occasionally don't boot up (hangs and then the test waits for an hour before giving up).

**To Reproduce**

Keep running the test and eventually you'll see it.

**Expected behavior**

Tests are stable, not flaky.

**Logs/Stack traces**

The CI logs from the GHA runner as of this morning:
[logs_10155.zip](https://github.com/hyperledger/cactus/files/7392356/logs_10155.zip)

**Cloud provider or hardware configuration:**

GHA runner

**Operating system name, version, build:**

Ubuntu 20.04

**Hyperledger Cactus release version or commit (git rev-parse --short HEAD):**

1.0.0-rc.1

**Hyperledger Cactus Plugins/Connectors Used**

Corda

**Additional context**

I'll send a separate PR that skips this test to avoid flakiness in the meantime.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 19:33:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/cactus/issues/1461" class=".btn">1461</a>
            </td>
            <td>
                <b>
                    fix(key-converter): Files needs to migrated from Tape to Jest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">good-first-issue</span><span class="chip">help wanted</span><span class="chip">Nice-to-Have</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span><span class="chip">Hacktoberfest</span><span class="chip">good-first-issue-400-expert</span>
            </td>
            <td>
                **Describe the bug**

Test file, key-converter, has multiple methods that are being skipped. 

**Expected behavior**

The test file should be able to run without it's methods having to be skipped.

**File Path:** packages/cactus-common/src/test/typescript/unit/key-converter.test.ts

**After Correction**
Migrate file from Tape to Jest.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-18 15:33:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/cactus/issues/1386" class=".btn">1386</a>
            </td>
            <td>
                <b>
                    test(connector-besu): fix missing multi-party all-in-one ledger image caching
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">good-first-issue</span><span class="chip">help wanted</span><span class="chip">Nice-to-Have</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span><span class="chip">Performance</span><span class="chip">Hacktoberfest</span><span class="chip">good-first-issue-400-expert</span>
            </td>
            <td>
                > This is marked as a good first issue because mostly you just need to be experienced in containerization, not necessarily the core of the Cactus code nor distributed ledgers. Do bear in mind that it is level 400 though so it's not exactly easy unless you have significant experience with containers.

**Describe the bug**

The  multi-party all-in-one ledger image for Besu tests does not cache the images it downloads from DockerHub, meaning that every time the tests run it pulls all the images again and this has been leading to rate limiting errors that make the CI flaky (once again)

**To Reproduce**

Run a lot of tests for a lot of PRs all at once and in a few hours you will have exhausted the DockerHub rate limit and all the tests will start failing for the next 6-12 hours until the rate limit cools off.

**Expected behavior**

Tests are stable, DockerHub rate limits are not at risk of being hit at any time regardless of how many tests we run in parallel. 

Either the AIO besu multi-party image caches a set of pinned versions of all the images it uses (e.g. fetches from dockerhub) at image **build** time so that by the time the CI pulls up the container for the tests, it only needs to download the one big image from ghcr.io instead of dockerhub (the former does not have rate limits - yet)

Relevant Dockerfile:
`tools/docker/besu-multi-party-all-in-one/Dockerfile`

**Logs/Stack traces**

N/A

**Screenshots**

N/A

**Cloud provider or hardware configuration:**

GH managed action runners

**Operating system name, version, build:**

Ubuntu 20.04

**Hyperledger Cactus release version or commit (git rev-parse --short HEAD):**

0.9.0 / 0.10.0

**Hyperledger Cactus Plugins/Connectors Used**

Besu

**Additional context**

The AIO besu multi-party image caches a set of pinned versions of all the images it uses

Relevant Dockerfile:
`tools/docker/besu-multi-party-all-in-one/Dockerfile`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 00:52:43 +0000 UTC
    </div>
</div>

