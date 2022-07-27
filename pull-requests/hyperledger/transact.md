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
                PR <a href="https://github.com/hyperledger/transact/pull/369" class=".btn">#369</a>
            </td>
            <td>
                <b>
                    Backport 0-4: fix midpoint pruning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of #368 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-21 21:44:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/368" class=".btn">#368</a>
            </td>
            <td>
                <b>
                    Fix midpoint pruning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the changelog after pruning by taking into account pruning occurring in the middle of a chain of state roots.  The changelog is updated such that the parent and successor nodes are properly re-linked with the removal of the intermediate node.  It also limits the pruning of changelog additions to those candidates that were deleted.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-21 16:17:56 +0000 UTC
    </div>
</div>

