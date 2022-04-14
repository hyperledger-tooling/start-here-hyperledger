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
                PR <a href="https://github.com/hyperledger/transact/pull/325" class=".btn">#325</a>
            </td>
            <td>
                <b>
                    InTransaction Back-end implementations for both Postgres and Sqlite 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change requires a number of changes on trait constraits, removing many Sync, Send and Clone constraints, but does require a new trait, split out from Read, to cover a Read implementation that is sync and send.  This is necessary, as the ContextManager requires Sync/Send Read impls.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 22:30:39 +0000 UTC
    </div>
</div>

