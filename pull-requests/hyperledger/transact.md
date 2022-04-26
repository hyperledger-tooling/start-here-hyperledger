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
                PR <a href="https://github.com/hyperledger/transact/pull/330" class=".btn">#330</a>
            </td>
            <td>
                <b>
                    Backport 0-4: InTransaction Back-end implementations for both Postgres and Sqlite
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of #327 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 18:13:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/329" class=".btn">#329</a>
            </td>
            <td>
                <b>
                    Backport 0-4: Experimental State Traits v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of PR #326 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 15:30:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/328" class=".btn">#328</a>
            </td>
            <td>
                <b>
                    Implement state traits v2 for kv::MerkleState
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change implements the "V2" state trait over the key-value MerkleState implementation.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-22 19:50:09 +0000 UTC
    </div>
</div>

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
                Implements Sql backends that wrap connection references, instead of owning a connection pool.  This requires that the SqlMerkleState for these backends can only implement the state traits v2, as they cannot be sync or send.


 
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

