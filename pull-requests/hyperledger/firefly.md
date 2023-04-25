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
                PR <a href="https://github.com/hyperledger/firefly/pull/1291" class=".btn">#1291</a>
            </td>
            <td>
                <b>
                    Use a more optimistic approach when inserting token transfer events, …
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …assuming that they are new and can be inserted without conflict, then handle errors if not
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-24 15:43:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1290" class=".btn">#1290</a>
            </td>
            <td>
                <b>
                    feat: Upgrade to latest ffresty with mTLS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Depends on:
- https://github.com/hyperledger/firefly-common/pull/65
- https://github.com/hyperledger/firefly/pull/1289

Once those are in I'll update this one
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-24 15:18:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1289" class=".btn">#1289</a>
            </td>
            <td>
                <b>
                    chore: remove deprecated config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">migration_consideration</span>
            </td>
            <td>
                - Remove deprecated config for blockchain, tokens, factory, database, dex and shared storaged config
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-24 09:28:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1288" class=".btn">#1288</a>
            </td>
            <td>
                <b>
                    Fix 1287
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1287 

In PR chain with #1280 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-20 18:50:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1286" class=".btn">#1286</a>
            </td>
            <td>
                <b>
                    chore(ci): switch to dedicated Firefly runners
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
        Created At 2023-04-19 00:27:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1285" class=".btn">#1285</a>
            </td>
            <td>
                <b>
                    Enable workflows for release branch
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
        Created At 2023-04-18 22:06:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1284" class=".btn">#1284</a>
            </td>
            <td>
                <b>
                    v1.2: Replace "UpsertBatch" with "InsertOrGetBatch"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When persisting an off-chain batch initially received from data exchange or shared storage, it should always be an insert. If the batch exists, just move on. Otherwise we may accidentally revert a confirmed batch to its previous state if it happens to get redelivered.

Backport of #1208, #1209, and #1204
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-18 19:49:22 +0000 UTC
    </div>
</div>

