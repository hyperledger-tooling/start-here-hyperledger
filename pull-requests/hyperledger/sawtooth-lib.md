---
layout: default
title: sawtooth-lib
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-lib
---

# sawtooth-lib <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-lib){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/98" class=".btn">#98</a>
            </td>
            <td>
                <b>
                    Stabilize `transaction-receipt-store-lmdb`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Rename the 'transaction-receipt-store-lmdb' feature to 'lmdb' and move
it from experimental to stable.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 19:47:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/97" class=".btn">#97</a>
            </td>
            <td>
                <b>
                    Stabilize `transaction-receipt-store`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Move the 'transaction-receipt-store' feature from experimental to stable.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 17:10:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/96" class=".btn">#96</a>
            </td>
            <td>
                <b>
                    Add a `service_id` to the `DieselReceiptStore`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a `service_id` to the diesel implementation of receipt store. The `service_id` scopes the store to a specific instance of a receipt store. The index field is also updated to longer have a unique constraint, this is because with the addition of the `service_id` index only needs to be unique for a given `service_id`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-24 18:18:30 +0000 UTC
    </div>
</div>

