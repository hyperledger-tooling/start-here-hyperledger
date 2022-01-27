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
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/133" class=".btn">#133</a>
            </td>
            <td>
                <b>
                    Add a database index on transaction_receipt
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds an index on the `"idx"` column of the `transaction_receipt` table.  This column is frequently used for queries.  It has also been identified as the source of a performance issue with the query to find the latest `idx` value for a given service id (found at the start of the `AddTxnReceiptsOperation`).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 16:58:55 +0000 UTC
    </div>
</div>

