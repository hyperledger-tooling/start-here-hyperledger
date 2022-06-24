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
                PR <a href="https://github.com/hyperledger/cactus/pull/2098" class=".btn">#2098</a>
            </td>
            <td>
                <b>
                    fix: part 2 of lint warnings resolved for batch 7/26 #1356 : Commit to be reviewed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Solved remaining lint warnings issue:  style: 2021-09-20 linter warnings batch 7 / 26 #1356
Part one of the solution submitted in #2087
Changes made:
- Fixed lint warnings associated with  non-any type in getAllMethodNames and getAllFieldNames
- Fixes lint errors associated with unexpected any for private-public keypairs
Signed-off-by: Akanksha Dixit <akanksha.dixit12@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-24 11:10:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2096" class=".btn">#2096</a>
            </td>
            <td>
                <b>
                    test: fix CI - chunk up Jest tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The test runners used within ./tools/ci.sh are now configurable
through environment variables. For example this works in
the yaml files for GH action workflows:

    env:
      JEST_TEST_PATTERN:
     "packages\/cactus-common\/src\/test\/typescript\/(unit|integration|benchmark)\/.*\/*.test.ts"
      JEST_TEST_RUNNER_DISABLED: false
      TAPE_TEST_RUNNER_DISABLED: true

Fixes #2090

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 20:39:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2095" class=".btn">#2095</a>
            </td>
            <td>
                <b>
                    fix: compile errors in the electricity-trade example
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fix allows the cactus repository to configure without errors when `npm run configure` is run in the cactus root directory
It enables various examples like the electricity-trade to work
Signed-off-by: Jande Vincent [janvinsha@gmail.com](url) 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 16:41:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2089" class=".btn">#2089</a>
            </td>
            <td>
                <b>
                    chore(connector-go-eth): upgrade web3.js to recent version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                - Upgrade web3 package used by go-ethereum-socketio connector from "0.20.7" to "1.7.3"
- Major cleanup and refactor of go-ethereum-socketio logic,
  without affecting the current functionalities.
- Add safety checking of method called in web3Eth and contract functions.
  Add tests to check if it works.
- Add websocket eth RPC support and some helper functions in openethereum-test-ledger.
- Expose WS RPC in geth-testnet, use this port in sample apps
  (required to monitor new blocks in updated web3.js)
- Change raw use of sendRawTransaction to sendSignedTransaction in sample apps
  in order to conform to new web3.js version.
- Add safeStringifyException to cactus-common that can be used by validators
  to sanitize response errors.
- Refactor socketio-based validators to use safeStringifyException.
- Adjust connector README files.

Closes #2088

Depends on #2053

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

------------

Please review only the last commit, the rest are dependencies that should be merged in separate PRs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-21 12:15:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2087" class=".btn">#2087</a>
            </td>
            <td>
                <b>
                    fix: Lint Warnings resolved for batch 7/26 #1356 : Commit to be reviewed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix: batch 7/26 of lint warning fixes #1356(fixed 5 warnings, partial solution): 

Changes made:
- Fixed lint warnings associated with any-type for truthyness and nonBlankString checking
- Fixed lint warnings associated with Unexpected any, edited type-aliases in logger
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 09:37:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2086" class=".btn">#2086</a>
            </td>
            <td>
                <b>
                    refactor(cmd-api-server): clean up configuration parameters gitguardi…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …an scanner test

test

Signed-off-by: ruzell22 <ruzell.vince.aquino@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 06:31:30 +0000 UTC
    </div>
</div>

