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
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/76" class=".btn">#76</a>
            </td>
            <td>
                <b>
                    Add LMDB `ReceiptStore` implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add the LMDB implementation of `ReceiptStore`. This includes `LmdbReceiptStoreIter`, an iterator which loads transaction receipts from an lmdb receipt store instance, this iterator is used in the `list_receipts_since` method.

Tests for all methods are included.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-28 23:55:42 +0000 UTC
    </div>
</div>

