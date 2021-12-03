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
                PR <a href="https://github.com/hyperledger/cactus/pull/1623" class=".btn">#1623</a>
            </td>
            <td>
                <b>
                    fix(supply-chain-app): enable cockpit in supply-chain
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #1622

Signed-off-by: Elena Izaguirre <e.izaguirre.equiza@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-03 11:57:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1621" class=".btn">#1621</a>
            </td>
            <td>
                <b>
                    fix: shutdown hook configuration is using wrong config key
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In the api-server constructor the evaluation for the activation /
deactivation of the shutdown hook is based on the wrong configuration
property so that it always is falling back to the default value and
pre-configured value is not taken.

Closes: #1619
Signed-off-by: Michael Courtin <michael.courtin@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-03 11:13:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1618" class=".btn">#1618</a>
            </td>
            <td>
                <b>
                    test: jestify transfer-commence test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-plugin-odap-hermes/src/test/typescript/integration/odap/transfer-commence.test.ts

This is a PARTIAL resolution to #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 21:30:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1617" class=".btn">#1617</a>
            </td>
            <td>
                <b>
                    test: jestify transfer-complete test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-plugin-odap-hermes/src/test/typescript/
integration/odap/transfer-complete.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana awadhana0825@gmail.com
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 21:22:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1616" class=".btn">#1616</a>
            </td>
            <td>
                <b>
                    test: jestify transfer-initiation test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-plugin-odap-hermes/src/test/typescript/integration/odap/transfer-initiation.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 21:09:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1615" class=".btn">#1615</a>
            </td>
            <td>
                <b>
                    feat(connector-xdai): remove hard dependency on keychain
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #1162 

Signed-off-by: Elena Izaguirre <e.izaguirre.equiza@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 09:36:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1614" class=".btn">#1614</a>
            </td>
            <td>
                <b>
                    chore(deps): upgrade jose to v4.x
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Commit to be reviewed
-----
chore(deps): upgrade jose to 4.x
	
	Primary Change
	-------------
	1. Upgraded Jose version from 1.x to 4.1.0
	2. Upgraded code and test cases to incorporate the same

Resolves #1231

Signed-off-by: jagpreetsinghsasan <jagpreet.singh.sasan@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 07:10:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1601" class=".btn">#1601</a>
            </td>
            <td>
                <b>
                    fix(security): upgrade fabric-common to 2.2.10 or later
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Security</span><span class="chip">P1</span>
            </td>
            <td>
                In the fabric connector I had to upgrade to a newer snapshot
version because we need the fresh typings from there.

Fixes #1600

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-30 01:32:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1599" class=".btn">#1599</a>
            </td>
            <td>
                <b>
                    test: skip flaky deploy-cordapp-jars-to-nodes-v4.8-express
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">Corda</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span><span class="chip">Flaky-Test-Automation</span><span class="chip">Tests</span>
            </td>
            <td>
                Related to #1598 but does not fix it.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-30 00:30:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1597" class=".btn">#1597</a>
            </td>
            <td>
                <b>
                    refactor(cmd-socketio-server): circular dependency fix and minor fixes for verifier tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix circular dependency between routing-interface and VerifierFactory,
add default validator config used by ValidatorAuthentication, type fixes
in Verifier, format some files according to standard.

Closes: #1596
Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-29 21:11:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1595" class=".btn">#1595</a>
            </td>
            <td>
                <b>
                    test: jestify plugin-registry test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Tests</span>
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-core/src/test/typescript/unit/plugin-registry.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-29 13:53:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1594" class=".btn">#1594</a>
            </td>
            <td>
                <b>
                    test: jestify run transaction endpoint test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Tests</span>
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-plugin-ledger-connector-fabric/src/test/typescript/
integration/fabric-v2-2-x/run-transaction-endpoint-v1.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-29 13:48:16 +0000 UTC
    </div>
</div>

