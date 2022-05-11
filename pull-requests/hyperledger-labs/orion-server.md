---
layout: default
title: orion-server
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/orion-server
---

# orion-server <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/orion-server){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/405" class=".btn">#405</a>
            </td>
            <td>
                <b>
                    Fix missing db in operation provenance
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
        Created At 2022-05-11 16:33:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/403" class=".btn">#403</a>
            </td>
            <td>
                <b>
                    Ledger test: path
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-10 15:17:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/402" class=".btn">#402</a>
            </td>
            <td>
                <b>
                    Ledger path from block to itself
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                Support requesting the ledger path from a block to itself.
When start block is zero the server entered to an endless loop.

Signed-off-by: Yoav Tock <tock@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-10 12:15:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/399" class=".btn">#399</a>
            </td>
            <td>
                <b>
                    fix backward link to deleted key in provenance
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                When the key is deleted from the world state in
a one block and the same key is added in the future
block, there should be two links (previous/next) between old deleted
value and the new value. Due to a mistake in the unit-test,
we missed to detect the bug in the production code.

Now with the integration test, we could detect this bug.
To get the last deleted value to construct the next/previous
link with the new value, we need to pass the correct key. The
existing code passes the incorrect key to find the last deleted
key node.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-09 07:27:34 +0000 UTC
    </div>
</div>

