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
                PR <a href="https://github.com/hyperledger/cactus/pull/2113" class=".btn">#2113</a>
            </td>
            <td>
                <b>
                    test(cactus): remove flaky tests from main CI execution
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Remove flaky tests from main CI execution.
- Add separate TAP and jest configuration for running only flaky tests.
- Add test:*:flaky scripts in the main package.json
- Add new step to github CI script to run flaky tests as optional (i.e. don't fail if flaky test fails)

Closes: #2112

Related: #2104
Related: #1626
Related: #2019
Related: #1625
Related: #1543
Related: #1598
Related: #1528
Related: #1521
Related: #1495
Related: #1485
Related: #1473
Related: #1471
Related: #1469
Related: #1150

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-04 15:38:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2111" class=".btn">#2111</a>
            </td>
            <td>
                <b>
                    test(connector-sawtooth-socketio): add functional test, bug fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add functional test of all functions from sawtooth-socketio validator.
- Refactor sawtooth validator to allow importing as a module, to simplify the functional test.
- Add stopMonitor to terminate tests easily.
- Allow multiple clients to monitor for blocks.
- Fix parsing of URL from config so that it doesn't depend on trailing slash anymore.

Closes: https://github.com/hyperledger/cactus/issues/2107

Depends on: https://github.com/hyperledger/cactus/pull/2109
Depends on: https://github.com/hyperledger/cactus/pull/2110
Depends on: https://github.com/hyperledger/cactus/pull/2047

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 18:41:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2110" class=".btn">#2110</a>
            </td>
            <td>
                <b>
                    feat(sawtooth-ledger): add single sawtooth test ledger image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                feat(sawtooth-ledger): add single sawtooth test ledger image

- Enclose starting sawtooth ledger into single container that will fetch and run the entire setup.
- Remove reduntant files, update the readme.
- Add SawtoothTestLedger class to simplify setting the test ledger in jest tests.
- Refactor electricity-trade to generate usage without sawtooth shell patching.
- Refactor electricity-trade to use new sawtooth ledger container and wait until it's healthy.

Closes: https://github.com/hyperledger/cactus/issues/2108

Depends on: https://github.com/hyperledger/cactus/pull/2030

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 18:27:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2109" class=".btn">#2109</a>
            </td>
            <td>
                <b>
                    refactor(connector-sawtooth-socketio): fix strict flag warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                cactus-plugin-ledger-connector-sawtooth-socketio will compile with global strict flag.

Related issue: #1671

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 18:26:24 +0000 UTC
    </div>
</div>

