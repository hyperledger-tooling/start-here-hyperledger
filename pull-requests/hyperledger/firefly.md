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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/948" class=".btn">#948</a>
            </td>
            <td>
                <b>
                    Store full details of EVMConnect/EthConnect updates for Token ops
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/72 for additional detail.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 03:37:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/947" class=".btn">#947</a>
            </td>
            <td>
                <b>
                    Replace namespace.remotename with namespace.multiparty.networkname
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a proposed rename for discussion.

Currently a namespace can have a `name` and a `remoteName` - `name` is how it's known locally (on APIs and most database objects), while `remoteName` is how it's written into objects that transmit the namespace in a multi-party system (specifically messages, batches, and groups on dataexchange, and the BatchPin method of the V1 blockchain contract).

Since the thing we've called `remoteName` is entirely specific to multiparty networks, it could be renamed to `multiparty.networkNamespace`, which seems more accurate. It would still default to the value of the local namespace `name` if unset.

Counterpoints:
- These fields will continue to show as `localNamespace` and `namespace` on messages and groups when queried (and the latter can't easily be modified due to the way hashes are computed).
- Tokens plugins have a similar `name` and `remoteName` (one is stored locally and one is sent in messages), so this would be a departure from that terminology.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 00:10:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/946" class=".btn">#946</a>
            </td>
            <td>
                <b>
                    Add deprecation warning for old node config
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
        Created At 2022-08-10 00:00:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/945" class=".btn">#945</a>
            </td>
            <td>
                <b>
                    Remove unneeded sleep from txcommon test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #618
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-09 20:04:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/942" class=".btn">#942</a>
            </td>
            <td>
                <b>
                    Advertise full node name (with suffix) to DX
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Depends on https://github.com/hyperledger/firefly-dataexchange-https/pull/67
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-08 20:38:59 +0000 UTC
    </div>
</div>

