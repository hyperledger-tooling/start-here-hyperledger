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
                PR <a href="https://github.com/hyperledger/cactus/pull/1649" class=".btn">#1649</a>
            </td>
            <td>
                <b>
                    fix(config-service): faulty shutdownHook definition in the Config-Schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In the config-service of the api-server the configuration value for
"shutdownHook" is not getting applied due to an issue in the reducer of
the newExampleConfigEnv(). The reducer is not populating the
shutdownHook configuration based on a faulty Config-Schema definition
for the shutdownHook where "arg" and "env" are missing.

Closes: #1648
Signed-off-by: Michael Courtin <michael.courtin@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 13:50:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1643" class=".btn">#1643</a>
            </td>
            <td>
                <b>
                    fix(plugin-odap-hermes): remove extraneous dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                1. Removed a lot of extraneous dependencies and
2. Changed the license to Apache-2.0 from ISC

Fixes #1641

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 19:05:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1640" class=".btn">#1640</a>
            </td>
            <td>
                <b>
                    fix(security): upgrade web3 to upgrade elliptic > 6.5.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Security</span><span class="chip">P1</span>
            </td>
            <td>
                Upgrade the web3 packages in besu connector and the hermes ODAP plugin
to eliminate some of the security vulnerabilities that were reported by the
robots.

Fixes #1639

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 18:49:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1638" class=".btn">#1638</a>
            </td>
            <td>
                <b>
                    refactor(connector-fabric): deprecate chain code compiler
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">Fabric</span>
            </td>
            <td>
                Removed the chain code compiler and its related pieces of code/docs.

Also updated the Fabric connector plugin's README file to be much more
up to date.

Fixes #1131

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 05:33:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1630" class=".btn">#1630</a>
            </td>
            <td>
                <b>
                    chore(release): publish v1.0.0-rc.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">Security</span>
            </td>
            <td>
                Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-07 01:13:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1629" class=".btn">#1629</a>
            </td>
            <td>
                <b>
                    test: ethereum BLP with connectivity check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add BLP that checks connectivity between ethereum ledger and connector

Closes: #1628
Signed-off-by: stepniowskip <piotr.stepniowski@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-06 13:56:26 +0000 UTC
    </div>
</div>

