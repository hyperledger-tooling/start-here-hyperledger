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
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/82" class=".btn">#82</a>
            </td>
            <td>
                <b>
                    Fix error message in diesel models
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix an error message in the `from_sql` method for `StateChangeTypeModel`. The method was copy pasted and the error message was not properly updated.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-24 17:07:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/81" class=".btn">#81</a>
            </td>
            <td>
                <b>
                    Modify receipt store `list_receipts_since`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Modify the receipt store `list_receipts_since` method to return an iterator with type `Result<TransactionReceipt, ReceiptStoreError>` rather than just `TransactionReceipt` to cover the cases where an implementation may fail on later records in the iteration.

This PR updates the method signature in the trait as well as the LMDB, SQLite and PostgreSQL implementations.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-24 16:44:17 +0000 UTC
    </div>
</div>

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

