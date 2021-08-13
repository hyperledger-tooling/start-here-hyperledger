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
                PR <a href="https://github.com/hyperledger/grid/pull/900" class=".btn">#900</a>
            </td>
            <td>
                <b>
                    Add action stubs for Purchase Order smart contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds unimplemented functions for the Purchase Order
smart contract's transaction handler actions. Also, this adds the
handling in the `apply` function to determine a payload's action.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-12 19:30:20 +0000 UTC
    </div>
</div>

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

