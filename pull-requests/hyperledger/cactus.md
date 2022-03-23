---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1944" class=".btn">#1944</a>
            </td>
            <td>
                <b>
                    fix(deps): force minimist >=1.2.6 for CVE-2021-44906
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Security</span><span class="chip">P1</span>
            </td>
            <td>
                Ensures that yarn will only install 1.2.6 or newer versions for
minimist.

The proper fix would be to have the dependencies issue releases
which upgrade their own (transitive) dependencies of minimist
so that we don't have to explicitly force it here, but at the time
of this writing these upgrades in our direct dependencies are just
not available yet.

Fixes #1943

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 04:54:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1942" class=".btn">#1942</a>
            </td>
            <td>
                <b>
                    replaced rocketchat with discord
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Replaced the old rocketchat link with the new discord link
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-22 19:09:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1940" class=".btn">#1940</a>
            </td>
            <td>
                <b>
                    feat(keychain-aws-sm): bootstrap readme.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Commit to be reviewed

feat(keychain-aws-sm): bootstrap readme.md

	Primary Changes
	-----------------------
	1. Updated the README.md located at packages/cactus-plugin-keychain-aws-sm/README.md
	2. The aws secret manager plugin now includes the prometheus metrics exporter integration
	3. OpenApi spec now has api endpoint for getting the prometheus metrics

Fixes #968

Signed-off-by: jagpreetsinghsasan <jagpreet.singh.sasan@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-22 10:19:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1938" class=".btn">#1938</a>
            </td>
            <td>
                <b>
                    feat(plugin-odap): addition of client endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implementation of client endpoints in ODAP plugin.

The changes can be summarized as follows:
- Implementation of client endpoints
- Adapted and added more tests (now divided into unit and integration tests)
- Addition of more checks regarding the validity of the messages received on the server side

closes #1939

Signed-off-by: André Augusto <andre.augusto@tecnico.ulisboa.pt>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-20 23:38:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1936" class=".btn">#1936</a>
            </td>
            <td>
                <b>
                    fix: resolve some CodeQL warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix CodeQL warnings:
- Reflected cross-site scripting
- Exception text reinterpreted as HTML

In following files:
- `examples/cactus-check-connection-ethereum-validator/check-ethereum-validator.ts`
- `examples/discounted-cartrade/trades.ts`
- `examples/electricity-trade/electricity-trade.ts`
- `examples/test-run-transaction/test-run-transaction.ts`
- `packages/cactus-cmd-socketio-server/src/main/typescript/routing-interface/routes/index.ts`

Also, sample apps in `example/` did not build after last socketio upgrade, had to upgrade typescript to make them build again.

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 15:35:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1934" class=".btn">#1934</a>
            </td>
            <td>
                <b>
                    docs(plugin-object-store-ipfs): added README.md description
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span>
            </td>
            <td>
                Added some instructions for the usage of the package `plugin-object-store-ipfs` in the README.md.

Signed-off-by: André Augusto <andre.augusto@tecnico.ulisboa.pt>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 02:29:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1933" class=".btn">#1933</a>
            </td>
            <td>
                <b>
                    feat(quorum-connector): implement validator interface on go-quorum-connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                - Add three new endpoints to quorum ledger connector achieve legacy verifier compatibility.
  - `InvokeRawWeb3EthContractEndpoint` can be used to form any call to deployed contract.
  - `InvokeRawWeb3EthMethodEndpoint` can be used to call any web3.eth function. Both are marked as low-level functions, should be used only when there's no designated endpoint for given functionality yet.
  - `WatchBlocksV1Endpoint` can be used to monitor new block headers / data from the ledger. Type of the output is determined from input option flag.
- Extend `QuorumApiClient` to support Verifier interface, that is: block monitoring, and sending sync/async requests. Sending requests is marked as deprecated, because user can use direct REST calls from generated ApiClient, nevertheless this API was requested by one of the teams.
- Added functional tests for two new, request based endpoints.
- Moved verifier-besu integration test to besu-test package.
- Added verifier-quorum integration test, it supplements direct endpoint tests and provides a reference for API usage.
- Added support for `QuorumApiClient` in Verifier.

Closes: https://github.com/hyperledger/cactus/issues/1604
Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

### Notes
- I can't make CodeQL to cooperate, it reports dynamic call errors, even though I explicitly check if methods are defined on a contract / object (also assert they type is a function). Tried different methods to make the scanner notice it but did not succeed. Please double check and mark as false positive if possible.

Depends on https://github.com/hyperledger/cactus/pull/1928
Depends on https://github.com/hyperledger/cactus/pull/1926
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 19:08:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1931" class=".btn">#1931</a>
            </td>
            <td>
                <b>
                    chore(release): publish v1.0.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">dependencies</span>
            </td>
            <td>
                The current 1.0.0 release is undergoing a being security audited by a
third-party security audit company at the time of this writing. and the
process will take about 6 to 8 weeks to complete, but we are planning
to keep the 1.0.0 API stability in place as dictated by the semantic
versioning rules.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com> 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 09:34:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1930" class=".btn">#1930</a>
            </td>
            <td>
                <b>
                    ci: add fuzzer tests for our APIs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">API_Server</span><span class="chip">Security</span><span class="chip">P1</span>
            </td>
            <td>
                Fixes #495

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 06:22:37 +0000 UTC
    </div>
</div>

