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
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/86" class=".btn">#86</a>
            </td>
            <td>
                <b>
                    Fix sqlite receipt store test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update one of the sqlite receipt store tests to work with updated
`list_receipts_since` method that now returns an iterator of
Result<TransactionReceipt, ReceiptStoreError> rather than just
TransactionReceipt

Signed-off-by: Isabel Tomb <tomb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-03 17:03:04 +0000 UTC
    </div>
</div>

