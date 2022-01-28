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
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/135" class=".btn">#135</a>
            </td>
            <td>
                <b>
                    Add Release Notes for 0.7.3
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
        Created At 2022-01-27 21:14:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/134" class=".btn">#134</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-7: Add a database index on transaction_receipt
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of PR #133 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 20:55:41 +0000 UTC
    </div>
</div>

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
                This change adds an index on the "idx" and "service_id" columns of the transaction_receipt table.  These columns are frequently used for queries.

Use of these columns  has been identified as the source of a performance issue with the query to find the latest `idx` value for a given service id (found at the start of the `AddTxnReceiptsOperation`).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 16:58:55 +0000 UTC
    </div>
</div>

