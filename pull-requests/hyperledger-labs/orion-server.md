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
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/469" class=".btn">#469</a>
            </td>
            <td>
                <b>
                    Remove redundant lock
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Using locks causes a long hold of the `transactionProcessor` lock, which is the single contention point of the TX processing.
It can be avoided because the `blockReplicator` uses its own lock and by making `pendingTxs` lock-free.

Signed-off-by: Liran Funaro <liran.funaro@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-24 13:53:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/467" class=".btn">#467</a>
            </td>
            <td>
                <b>
                    Access control on writing user records - restrictive
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: May Rosenbaum <mayro1595@gmail.com> #456 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-22 11:49:19 +0000 UTC
    </div>
</div>

