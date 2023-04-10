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
                PR <a href="https://github.com/hyperledger/firefly/pull/1265" class=".btn">#1265</a>
            </td>
            <td>
                <b>
                    Allow operations to change between "Failed" and "Succeeded"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1264
Follow-up to #1257

Operations now cannot move from Failed/Succeeded back to Pending, but they can change between Failed and Succeeded.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-07 16:10:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1262" class=".btn">#1262</a>
            </td>
            <td>
                <b>
                    Add route for deleting token pools
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This allows deleting any token pool, regardless of gateway or multiparty mode, along with all associated token transfers, balances, and approvals.

Note that in multiparty mode, if you delete a token pool that was broadcast to the network, you will be voluntarily out of sync with other nodes.

This represents the simplest implementation of (4) from https://github.com/hyperledger/firefly/issues/1220#issuecomment-1496422542, in the context of token pools only.

Note that this does not purge event listeners from the token connector (events will just be ignored). Probably need to find a way to delete them though.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-05 17:00:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1261" class=".btn">#1261</a>
            </td>
            <td>
                <b>
                    Don't publish token pools by default, but allow publishing as a separate action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds a new `publish` boolean query parameter to the `/tokens/pools` creation route, which defaults to "false" and will create the token pool definition locally only. If "true", the definition will be published to the multiparty network.

Adds a new `/tokens/pools/{id}/publish` route for publishing a previously-local definition to the multiparty network as a separate action.

This represents a portion of the behavior defined in 1-2 of https://github.com/hyperledger/firefly/issues/1220#issuecomment-1496422542
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 19:51:18 +0000 UTC
    </div>
</div>

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

