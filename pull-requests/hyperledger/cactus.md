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
                PR <a href="https://github.com/hyperledger/cactus/pull/1978" class=".btn">#1978</a>
            </td>
            <td>
                <b>
                    feat(odap-plugin): odap crash recovery first implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Addition of retries when making requests
* Addition of timeouts when making requests
* Addition of endpoints for recovery procedure
* Tests with crashes in the first phase of the protocol
* Addition of logging in local SQLite database
* IPFS is now only to store hashes and signatures of the logs and proofs/claims
* Migrate odap-api-call-with-ledger-connector.test from tape to jest
* Addition of rollbacks when counterparty gateway is and is not crashed
* Update README.md with a new protocol image and the description of each test file
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-18 23:20:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1977" class=".btn">#1977</a>
            </td>
            <td>
                <b>
                    test(connector-fabric-socketio): add functional test, bug fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added functional jest test `fabric-socketio-connector.test` that can be run during CI process. It checks evaluate/sending transactions and monitoring for new events. Connector had to be refactored to be testable, tests also discovered some bugs that had to be fixed in order to pass.

### SocketIOApiClient refactors:
- Added option for supplying `validatorKeyValue` instead of `validatorKeyPath`.
- JWT validation function works with key value now (instead of reading the key).
- Validator can now return messages that are not encrypted (it throwed error previously).
- Adjusted unit tests.

### connector-fabric-socketio refactors:
- Connector can be run both as a standalone app and loaded as a module `www.js`. Caller can use exported `startFabricSocketIOConnector` function to run the connector. Configuration must be supplied in file or in env variable like it's done in functional test.
- All cryptographic data (keys, certificates, etc…) can now be supplied as a value (previously it supported only path to a file).
- `sendSignedTransaction` can now be called synchronously (it had wrong response format before).
- Fixed a bug introduced during my last changes in this component, which caused fabric-client session to be disconnected but still reused by follow-up requests. I didn't know that gateway disconnects client it operates on.
- Increased JWT expiration to 15 minutes to prevent constant JWT expiration error (I'm pretty sure 15 minutes is still secure period).
- Minor improvements (logging, formatting, etc…)

### fabric-test-ledger-v1 changes:
- Added `adminCredentials()` to have programatic access to admin credentials on currently used ledger
 (unlikely, but can change in the future).

Depends on: https://github.com/hyperledger/cactus/pull/1975

Closes: https://github.com/hyperledger/cactus/issues/1976

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-15 15:35:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1975" class=".btn">#1975</a>
            </td>
            <td>
                <b>
                    refactor(connector-fabric-socketio): fix strict flag warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                cactus-plugin-ledger-connector-fabric-socketio will compile with global strict flag.

Related issue: #1671

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-15 15:26:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1973" class=".btn">#1973</a>
            </td>
            <td>
                <b>
                    Cross-Site Scripting attack (XSS).
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Unsanitized input from an HTTP parameter flows into send, where it is used to render an HTML page returned to the user. This may result in a Cross-Site Scripting attack (XSS).

Signed-off-by: Bhaskar <dev@bhaskar.email>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-14 05:32:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1972" class=".btn">#1972</a>
            </td>
            <td>
                <b>
                    test: jestify api client routing node to node test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This test file required more refactoring because the `tap` tests were nested, however `jest` doesn't allow nested test cases


File Path: 
packages/cactus-test-api-client/src/test/typescript/integration/api-client-routing-node-to-node.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: Youngone Lee <youngone.lee@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 16:05:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1971" class=".btn">#1971</a>
            </td>
            <td>
                <b>
                    chore(deps): upgrade angular in examples/carbon accounting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1651

Signed-off-by: aldousalvarez <aldousss.alvarez@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 06:51:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1970" class=".btn">#1970</a>
            </td>
            <td>
                <b>
                    docs(readme): add missing inclusive language statement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                Fixes #1969

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 00:41:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1968" class=".btn">#1968</a>
            </td>
            <td>
                <b>
                    test(connector-iroha): tested previously skipped test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                All I did was change from `test.skip` to just `test` and it turns out that the test works just fine. So for I've ran the test 20 times and it has passed every single time. This issue is a "fix" to #1957 ?

Signed-off-by: Youngone Lee <youngone.lee@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 21:45:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1967" class=".btn">#1967</a>
            </td>
            <td>
                <b>
                    ci: remove nodejs v12 exclusion logic from run custom checks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1961

Signed-off-by: Youngone Lee <youngone.lee@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 20:48:42 +0000 UTC
    </div>
</div>

