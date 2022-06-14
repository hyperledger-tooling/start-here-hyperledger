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
                PR <a href="https://github.com/hyperledger/transact/pull/362" class=".btn">#362</a>
            </td>
            <td>
                <b>
                    Add remove_pruned_entries to in-txn variants
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds the remove_pruned_entries function to the InTransaction- variants of SqlMerklState.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-13 18:24:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/361" class=".btn">#361</a>
            </td>
            <td>
                <b>
                    Add release notes for 0.4.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Schwarz <pschwarz@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-13 16:50:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/360" class=".btn">#360</a>
            </td>
            <td>
                <b>
                    Backport 0-4: Clean Pruned Elements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of #356 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-10 20:44:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/359" class=".btn">#359</a>
            </td>
            <td>
                <b>
                    Backport 0-4: Remove use of immediate_transaction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of #358 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-09 20:50:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/358" class=".btn">#358</a>
            </td>
            <td>
                <b>
                    Remove use of immediate_transaction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change removes the use of immediate_transaction for sqlite operations, as this function does not interact well within existing transactions.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 20:45:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/357" class=".btn">#357</a>
            </td>
            <td>
                <b>
                    Backport 0-4: Remove parent state root reference
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of #355 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 14:20:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/356" class=".btn">#356</a>
            </td>
            <td>
                <b>
                    Clean pruned elements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 14:18:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/355" class=".btn">#355</a>
            </td>
            <td>
                <b>
                    Remove parent state root reference
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change fixes an issue during state pruning in SQLite where the parent_state_root for change logs was not being unlinked. This causes a foreign key constraint violation when cleaning up pruned items.

The postgres implementation already has this unlinking code.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-07 17:38:46 +0000 UTC
    </div>
</div>

