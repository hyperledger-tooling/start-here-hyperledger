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
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/203" class=".btn">#203</a>
            </td>
            <td>
                <b>
                    change import path to hyperledger-labs/orion-server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: senthil <cendhu@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-13 17:50:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/202" class=".btn">#202</a>
            </td>
            <td>
                <b>
                    Release transactions with error from PendingTxs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">replication</span>
            </td>
            <td>
                - Add a ReleaseWithError method to PendingTxs queue
- Add a link to PendindTxs queue to block-creator & block-replicator
- Functinality of block-creator & block-replicator in later commits

Signed-off-by: Yoav Tock <tock@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 07:37:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/197" class=".btn">#197</a>
            </td>
            <td>
                <b>
                    test flake in TestBlockReplicator_Submit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">replication</span>
            </td>
            <td>
                Address the test flake in TestBlockReplicator_Submit/normal_flow:_blocked_submit
as described in issue #195

Signed-off-by: Yoav Tock <tock@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-10 12:43:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/194" class=".btn">#194</a>
            </td>
            <td>
                <b>
                    maintain order between -ve and +ve number
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">query support</span>
            </td>
            <td>
                This commits make the -ve number appear first
in the order before the +ve number. Further,
the value order is preserved too (i.e., -1000
appear before -100 and -90 appears before 10,
and so on)

Signed-off-by: senthil <cendhu@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 12:48:54 +0000 UTC
    </div>
</div>

