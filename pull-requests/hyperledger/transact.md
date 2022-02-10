---
layout: default
title: transact
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/transact
---

# transact <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/transact){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/314" class=".btn">#314</a>
            </td>
            <td>
                <b>
                    Cache "large" reads in SqlMerkleState
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change introduces a data cache used to cache the data values for "large" (where "large" is a configurable value) during the "get_leaves" store operation.

This cache mitigates issues when used with large state values and postgres, where the frequent return of large data (for example, when smart contracts are in play) causes a cloud instance to throttle bandwidth.

It is currently available under the experimental feature `"state-merkle-sql-caching"`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 21:52:39 +0000 UTC
    </div>
</div>

