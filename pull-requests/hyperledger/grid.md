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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/894" class=".btn">#894</a>
            </td>
            <td>
                <b>
                    Avoid duplicate events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR introduces an EventProcessors struct to manages that event processors are only created once per circuit/service instance.

It also introduces a work-around for an issue with database transaction creation while handling commit events. It serializes the events received from event processors into a channel and handle the events serially.  This fix ensures that duplicate events won't result in duplicate entries in the DB.  This second commit may be rolled back when a proper fix for transactions is introduced.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-04 20:35:14 +0000 UTC
    </div>
</div>

