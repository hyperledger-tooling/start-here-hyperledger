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
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/83" class=".btn">#83</a>
            </td>
            <td>
                <b>
                    Add release notes for 0.6.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Isabel Tomb <tomb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-26 15:14:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/82" class=".btn">#82</a>
            </td>
            <td>
                <b>
                    SQLite/PostgreSQL receipt store stabilization changes
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

