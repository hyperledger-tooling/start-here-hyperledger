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
                PR <a href="https://github.com/hyperledger/firefly/pull/1318" class=".btn">#1318</a>
            </td>
            <td>
                <b>
                    First draft of changes for unset handler
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There is probably more work to be done here, but this is what I started on to fix the bug https://github.com/hyperledger/firefly/issues/1317
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-24 15:31:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1316" class=".btn">#1316</a>
            </td>
            <td>
                <b>
                    Derive batch signing key from messages in the batch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-candidate</span>
            </td>
            <td>
                Follow-up to #1313
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-24 04:17:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1315" class=".btn">#1315</a>
            </td>
            <td>
                <b>
                    feat: background start for connector plugins
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
        Created At 2023-05-23 16:55:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1314" class=".btn">#1314</a>
            </td>
            <td>
                <b>
                    Update firefly-common v1.2.11 and firefly-signer v1.1.8
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
        Created At 2023-05-22 19:18:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1313" class=".btn">#1313</a>
            </td>
            <td>
                <b>
                    Do not allow a batch to contain messages from different signing keys
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-candidate</span>
            </td>
            <td>
                This reverts #1175 and allows a single batch processor to process messages from the same identity but different keys. Instead, it adds a new fix to immediately seal and dispatch the current batch if a new message is picked up that has a different signing key than the current in-flight batch assembly.

This will ensure that only one batch processor is allocating nonces for a given context, _and_ that each batch contains only messages signed by a single key. May come at the expense of a slight performance decrease in edge cases that use a variety of signing keys for a single identity, but this is acceptable overall.

Fixes #1311
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-22 16:47:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1309" class=".btn">#1309</a>
            </td>
            <td>
                <b>
                    Confirm group init messages during dispatch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It is not possible for a group init message to fail at this phase. If it fails, it must fail earlier. If it makes it to dispatch, it should flow through to confirm.

Fixes #1308
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-18 19:08:22 +0000 UTC
    </div>
</div>

