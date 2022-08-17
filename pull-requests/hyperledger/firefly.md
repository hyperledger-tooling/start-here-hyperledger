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
                PR <a href="https://github.com/hyperledger/firefly/pull/971" class=".btn">#971</a>
            </td>
            <td>
                <b>
                    Fix group race condition, optimize transaction cache
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Insert local group only after inserting groupinit message.
This ensures no other threads pick up on the group before the
message is sequenced.

Update transaction cache after initial insert.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 17:53:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/970" class=".btn">#970</a>
            </td>
            <td>
                <b>
                    Update to firefly-signer v0.9.15
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 15:51:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/969" class=".btn">#969</a>
            </td>
            <td>
                <b>
                    Update to firefly-signer v0.9.13
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 15:07:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/967" class=".btn">#967</a>
            </td>
            <td>
                <b>
                    Performance improvements for batch lookups
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ensure batch ID queries match the current indexes (to avoid sequential scan), and improve the caching in aggregator when processing a group of pins.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 04:15:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/966" class=".btn">#966</a>
            </td>
            <td>
                <b>
                    Add tutorial for Polygon testnet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Rendered preview is currently available at: https://nguyer.github.io/firefly/head/tutorials/chains/polygon_testnet.html
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-15 20:59:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/965" class=".btn">#965</a>
            </td>
            <td>
                <b>
                    bump ui to 1.1 alpha 3
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
        Created At 2022-08-15 19:41:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/963" class=".btn">#963</a>
            </td>
            <td>
                <b>
                    Update to latest dependencies ready for V1.1 alpha.3
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
        Created At 2022-08-15 16:42:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/961" class=".btn">#961</a>
            </td>
            <td>
                <b>
                    Update readme for local dev set up
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixed an error and added link in the core readme to link to component dev readme

Signed-off-by: Chengxuan Xing <chengxuan.xing@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-12 11:26:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/960" class=".btn">#960</a>
            </td>
            <td>
                <b>
                    Changes to support E2E tests with confirmations, where requests might be slow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Biggest change is to the HTTP Server to allow requests longer than 15s to complete without the client getting an EOF.

See https://github.com/hyperledger/firefly-common/pull/31
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-11 20:28:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/958" class=".btn">#958</a>
            </td>
            <td>
                <b>
                    Update Ruby deps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For https://github.com/hyperledger/firefly/security/dependabot/19
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-11 16:23:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/956" class=".btn">#956</a>
            </td>
            <td>
                <b>
                    Messages that fail validation should be rejected
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There was some confusion between "message is invalid" and "message could not yet
be dispatched" in the event aggregator. This attempts to separate those two
situations, as the former should be an immediate rejection.

Fixes #952
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-11 15:06:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/955" class=".btn">#955</a>
            </td>
            <td>
                <b>
                    Properly match operation updates to the plugin that generated them
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
        Created At 2022-08-10 20:57:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/953" class=".btn">#953</a>
            </td>
            <td>
                <b>
                    Distinguish "message not available" from "message missing data"
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
        Created At 2022-08-10 18:12:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/950" class=".btn">#950</a>
            </td>
            <td>
                <b>
                    fixing the example firefly core command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update the example command to match the latest folder structure.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 13:37:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/949" class=".btn">#949</a>
            </td>
            <td>
                <b>
                    Add BLOCKCHAIN_CONNECTOR env var and add evmconnect to manifest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Broadhurst <peter.broadhurst@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 13:29:02 +0000 UTC
    </div>
</div>

