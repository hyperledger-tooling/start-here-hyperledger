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
                PR <a href="https://github.com/hyperledger/firefly/pull/1312" class=".btn">#1312</a>
            </td>
            <td>
                <b>
                    fix: bug with init config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Draft PR where I would appreciate some pointers on my approach!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-22 16:47:09 +0000 UTC
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1305" class=".btn">#1305</a>
            </td>
            <td>
                <b>
                    Replace token pool "confirmed" state with "active" bool
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">migration_consideration</span>
            </td>
            <td>
                Token pool states were originally given similar names to message states, but this has ended up being confusing (because the token pool creation flow also includes a message, but the token pool states have no relation to the identically named message states).

Old terminology:
When pool definition message is "confirmed", pool is created as "pending"
When pool gets "activated" by the connector, pool is moved to "confirmed"

New proposed terminology:
When pool definition message is "confirmed", pool is created as "not active"
When pool gets "activated" by the connector, pool is moved to "active"

My hope is that the new terminology is easier to follow, since it does not overlap with messaging states and more clearly denotes the action of "activating" a token pool. Also with #1261 in the works (which means a pool may get activated first and then _later_ be published by a broadcast message), I think it's better to separate the token pool and message terminology.

This is technically a breaking API change, although I'm not aware of any significant usefulness of the "state" field to
external applications (it's primarily an internal tracking field). The related _event_ called "token_pool_confirmed" will
remain unchanged - it's still consistent with other definitions like datatypes, identities, etc, and I think it's still
appropriate.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-17 01:36:06 +0000 UTC
    </div>
</div>

