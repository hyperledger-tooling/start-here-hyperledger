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
                PR <a href="https://github.com/hyperledger/firefly/pull/281" class=".btn">#281</a>
            </td>
            <td>
                <b>
                    Fix release action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This will prevent duplicate build tasks when creating pre-release versions, as well as `latest` getting set to a pre-release version.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 20:01:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/280" class=".btn">#280</a>
            </td>
            <td>
                <b>
                    pools-by-connector Add connector field to TokenPoolQueryFactory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To support the new [Tokens Page in the UI](https://github.com/hyperledger/firefly-ui/issues/65), filtering that supports getting pools by connector is needed

```GET /namespaces/<namespace>/tokens/pools?connector={connectorName}``` returns all token pools with specified connector
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 15:36:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/278" class=".btn">#278</a>
            </td>
            <td>
                <b>
                    tokens-by-id getTokenPoolByNameOrID() and getTokenTransfersByID()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To support the new [Tokens Page in the UI](https://github.com/hyperledger/firefly-ui/issues/65), an endpoint to get token pools by name or ID and to get token transfers by ID is needed.

```GET /namespaces/<namespace>/tokens/pools/{nameOrID}``` returns all token pools with specified name or ID
```GET /namespaces/<namespace>/tokens/transfers/{transferID}``` returns token transfer with specified ID
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 01:03:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/277" class=".btn">#277</a>
            </td>
            <td>
                <b>
                    introduce FFTime.Time()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 - Converts FFTime -> Time
 - some misc. changes my linter pointed out
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 20:25:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/276" class=".btn">#276</a>
            </td>
            <td>
                <b>
                    Add extra columns to token tables for UI support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Extra columns desired in support of https://github.com/hyperledger/firefly-ui/issues/65
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 18:06:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/275" class=".btn">#275</a>
            </td>
            <td>
                <b>
                    New GET routes for tokens
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reviewed separately on a branch:
* https://github.com/kaleido-io/firefly/pull/33
* https://github.com/kaleido-io/firefly/pull/34
* https://github.com/kaleido-io/firefly/pull/35
* https://github.com/kaleido-io/firefly/pull/36

Squashed together here for upstreaming.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 16:53:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/274" class=".btn">#274</a>
            </td>
            <td>
                <b>
                    Additional E2E coverage for tokens
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ensure that testing covers fungible/non-fungible, sync/async, and with/without
message data.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 16:32:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/273" class=".btn">#273</a>
            </td>
            <td>
                <b>
                    Group token database calls into RunAsGroup wherever possible
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
        Created At 2021-10-20 16:30:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/270" class=".btn">#270</a>
            </td>
            <td>
                <b>
                    Allow nested RunAsGroup calls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If a transaction is already started, it is reused.

This allows code to be reused in a fashion where it may need to start a transaction, or may be called from
within an already-started transaction (useful for operations that span multiple packages, such as the
ongoing work on token transfers with associated messages).

It does introduce a new constraint for database implementations (noted in the database plugin definition).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 14:47:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/268" class=".btn">#268</a>
            </td>
            <td>
                <b>
                    Split asset manager into multiple files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                No code changes - just splitting up files.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 14:18:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/267" class=".btn">#267</a>
            </td>
            <td>
                <b>
                    Adjust version for firefly-tokens-erc1155
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Moving to a pre-release versioning pattern to avoid incrementing version numbers
too frequently.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 14:16:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/266" class=".btn">#266</a>
            </td>
            <td>
                <b>
                    Use firefly_e2e instead of firefly-e2e for container names
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fits with other FireFly naming conventions and makes highlighting in terminal
a bit easier.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 18:22:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/264" class=".btn">#264</a>
            </td>
            <td>
                <b>
                    Do not use tokenIndex in E2E test for fungible tokens
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Pulls in the behavior from https://github.com/hyperledger/firefly-tokens-erc1155/pull/35 and adjusts E2E test to match.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 17:27:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/262" class=".btn">#262</a>
            </td>
            <td>
                <b>
                    Do not allow UUIDs to be used as names
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
        Created At 2021-10-18 19:03:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/261" class=".btn">#261</a>
            </td>
            <td>
                <b>
                    Added more tests to the Fabric plugin for 100% coverage
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
        Created At 2021-10-18 15:51:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/260" class=".btn">#260</a>
            </td>
            <td>
                <b>
                    Move e2e to new routes, and add private/broadcast strong datatype tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                New E2E tests created as part of a recreate for #257, which turned out to be working as designed (due to a quirk of the JSON Schema syntax allowing additional properties by default).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-16 20:46:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/258" class=".btn">#258</a>
            </td>
            <td>
                <b>
                    Fix logic for transfer+message with waitConfirm=true
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Part of #218.

Includes a new MessageSender interface that is used by asset manager, broadcast manager, private messaging,
and sync-async bridge. This allows cleaner tracking of the progress of resolving and sending a message, and
injection of hooks at particular spots in the flow (which is needed here to dispatch the transfer and message in
a specific order).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-15 19:08:33 +0000 UTC
    </div>
</div>

