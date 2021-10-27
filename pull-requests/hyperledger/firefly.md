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

