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
                PR <a href="https://github.com/hyperledger/firefly/pull/1260" class=".btn">#1260</a>
            </td>
            <td>
                <b>
                    Update CLI to v1.2.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See https://github.com/hyperledger/firefly-cli/releases/tag/v1.2.1

This will fix the failing integration test which relies on a new Fabric flag: https://github.com/hyperledger/firefly/actions/runs/4602562209/jobs/8131661028
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 15:41:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1259" class=".btn">#1259</a>
            </td>
            <td>
                <b>
                    Fix coverage gaps from new operation update logic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Address missing coverage from #1257
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 15:39:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1258" class=".btn">#1258</a>
            </td>
            <td>
                <b>
                    Update Swagger UI used in the docs site
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We had a previous PR to update this library in the product itself https://github.com/hyperledger/firefly-common/pull/44 but the published docs site still used the old Swagger UI package. The previous version was susceptible to URL injection attacks so this PR fixes that.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 14:30:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1257" class=".btn">#1257</a>
            </td>
            <td>
                <b>
                    Do not update operations once they enter succeeded/failed state
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1256
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 20:58:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1254" class=".btn">#1254</a>
            </td>
            <td>
                <b>
                    fixing broken test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                doesn't look like these changes are related to the single-line change. Therefore, I raised it as a separate PR. @nguyer 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 10:03:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1253" class=".btn">#1253</a>
            </td>
            <td>
                <b>
                    fixing broken link for polygon testnet json-rpc endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                the existing link is no longer available. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-31 16:49:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1251" class=".btn">#1251</a>
            </td>
            <td>
                <b>
                    Check message on-chain consistency before initializing context
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This prevents inserting a group from a malformed "group init" message.

Possible/partial fix for https://github.com/hyperledger/firefly/issues/1247
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-31 12:45:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1249" class=".btn">#1249</a>
            </td>
            <td>
                <b>
                    Add support for evmconnect's "execution reverted" error code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When querying network version, look for the unique error codes returned by either ethconnect or evmconnect.

Partial fix for #1245
Depends on https://github.com/hyperledger/firefly-evmconnect/pull/67
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 18:49:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1248" class=".btn">#1248</a>
            </td>
            <td>
                <b>
                    Always send "group init" message with a registered signing key
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Private messages can be sent and signed by any arbitrary key if desired, but "group init" messages (which can be auto-triggered by a private message) must be signed by a registered key.

Possible/partial fix for #1247
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 17:51:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1246" class=".btn">#1246</a>
            </td>
            <td>
                <b>
                    Actually start the legacy "ff_system" namespace when needed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Partial fix for #1245

Somewhere in the refactoring of namespace manager, it looks like we ended up in a situation where we _initialize_ but do not _start_ the legacy "ff_system" namespace.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 16:54:00 +0000 UTC
    </div>
</div>

