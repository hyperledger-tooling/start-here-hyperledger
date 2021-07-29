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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/75" class=".btn">#75</a>
            </td>
            <td>
                <b>
                    Add `ReceiptStore` trait
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR moves the existing receipt module to a directory named receipt and adds a `ReceiptStore` trait and corresponding error module to receipt::store. The store module is behind the experimental feature "transaction-receipt-store".
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 18:56:20 +0000 UTC
    </div>
</div>

