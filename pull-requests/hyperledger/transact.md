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
                PR <a href="https://github.com/hyperledger/transact/pull/327" class=".btn">#327</a>
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
                This change requires a number of changes on trait constraits, removing many Sync, Send and Clone constraints, but does require a new trait, split out from Read, to cover a Read implementation that is sync and send. This is necessary, as the ContextManager requires Sync/Send Read impls.

(Replaces PR #325)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-22 16:05:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/326" class=".btn">#326</a>
            </td>
            <td>
                <b>
                    Experimental state traits v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds the initial implementation of traits defined in the [RFC for State Traits v2](https://github.com/hyperledger/transact-rfcs/pull/12)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-21 16:53:33 +0000 UTC
    </div>
</div>

