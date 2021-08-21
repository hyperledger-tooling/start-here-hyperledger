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
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/80" class=".btn">#80</a>
            </td>
            <td>
                <b>
                    Fix SQLite receipt store indexing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously the way that the index value was being assigned to the transaction receipt entry when adding new transaction receipts to the store did not guarantee uniqueness. This PR updates that process to retrieve the index of the most recently added transaction receipt and increment it by one to get the index of each new transaction receipt being added to the database.

This PR also adds a uniqueness constraint to the idx field of the `transaction_receipt` table.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-20 21:45:39 +0000 UTC
    </div>
</div>

