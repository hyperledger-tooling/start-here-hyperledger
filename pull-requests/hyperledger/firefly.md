---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/893" class=".btn">#893</a>
            </td>
            <td>
                <b>
                    Add sqlite to Docker image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It's helpful to have this handy when debugging database contents.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 16:19:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/892" class=".btn">#892</a>
            </td>
            <td>
                <b>
                    Fix logs from E2E test invocation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Disable parallelization and reduce test timeout to 1m.

This re-enables streaming logs during E2E runs (which is disabled by default when running suites in parallel). No real impact since our test jobs are already divided such that they run 1 suite per job.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 16:18:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/891" class=".btn">#891</a>
            </td>
            <td>
                <b>
                    Custom contract subscriptions now utilize namespaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Now, both ethconnect and fabconnect subscription names contain the namespace name. This means that events will now be delivered only to the callback handler for that namespace, instead of every single callback handler. Older subscriptions will still be delivered to all handlers. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 22:45:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/890" class=".btn">#890</a>
            </td>
            <td>
                <b>
                    Change default contracts to network version 2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also rename the "namespace" parameter to "action" in V2, and handle accordingly.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 18:32:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/889" class=".btn">#889</a>
            </td>
            <td>
                <b>
                    back port of "FAQ and FireFly Tutorial Updates"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                back port of #857 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 01:18:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/887" class=".btn">#887</a>
            </td>
            <td>
                <b>
                    Add E2E tests for gateway mode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 19:46:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/886" class=".btn">#886</a>
            </td>
            <td>
                <b>
                    update token connector versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Alex Shorsher <alex.shorsher@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 19:42:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/885" class=".btn">#885</a>
            </td>
            <td>
                <b>
                    back port of custom URI support for non-fungible tokens
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                back port of https://github.com/hyperledger/firefly/pull/879 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 16:26:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/884" class=".btn">#884</a>
            </td>
            <td>
                <b>
                    Stop orchestrator for ff_system when moving to network V2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Part of [FIR-12](https://github.com/hyperledger/firefly-fir/pull/12)
~~In a chain with #883~~

Background: The legacy `ff_system` namespace is created (ie an orchestrator and managers are initialized) whenever the default namespace is a V1 multiparty network. The `ff_system` namespace is initialized with an exact duplicate of the default namespace config (same plugins, same contract addresses, etc).

With this PR, if the default namespace (and therefore `ff_system`) migrates to V2 rules, the `ff_system` orchestrator will be stopped and removed, along with all its children.

This should allow legacy networks to cleanly migrate to V2 rules and retire `ff_system`. Notable caveat: once the default namespace is on V2, no other V1 namespaces will be supported.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 01:13:35 +0000 UTC
    </div>
</div>

