---
layout: default
title: grid
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/grid
---

# grid <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/grid){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/899" class=".btn">#899</a>
            </td>
            <td>
                <b>
                    Fix typos in PO workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes several typos in the PO workflow.rs file.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-12 17:02:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/898" class=".btn">#898</a>
            </td>
            <td>
                <b>
                    Add 0.2.2 release notes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Darian Plumb <dplumb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-09 17:31:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/897" class=".btn">#897</a>
            </td>
            <td>
                <b>
                    Refactor SDE transaction handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the SDE to properly run database operations in a transaction. To facilitate this, two new `StoreFactory` traits were introduced, `TransactionalStoreFactory` and `InContextStoreFactory`, that expose this functionality in the daemon. These traits allow for the creation of a `StoreFactory` that can be used to initialize a transaction, get various Grid stores, and then run DB operations all within a transaction on a single Connection. Previously, there was no guarantee that operations were run within the same transaction as each operation got a Connection from a ConnectionPool individually.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-06 19:43:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/896" class=".btn">#896</a>
            </td>
            <td>
                <b>
                    BACKPORT 0.2: Avoid duplicate events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of #894
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-06 14:16:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/895" class=".btn">#895</a>
            </td>
            <td>
                <b>
                    Add API docs to protocol module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds rustdoc comments to the protocol code for each smart contract.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-05 18:52:26 +0000 UTC
    </div>
</div>

