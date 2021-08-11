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
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/79" class=".btn">#79</a>
            </td>
            <td>
                <b>
                    Add PostgreSQL `ReceiptStore`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a DieselReceiptStore implementation of ReceiptStore. It also expands the migrations module to handle postgres migrations and adds the necessary postgres migrations for the receipt store tables.

The postgres receipt store and migrations are behind the experimental feature "postgres".
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 22:13:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/78" class=".btn">#78</a>
            </td>
            <td>
                <b>
                    Add sqlite `ReceiptStore`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a `DieselReceiptStore` implementation of `ReceiptStore`.  This PR also adds a necessary migrations module for running sqlite migrations.

The `DieselReceiptStore` includes 12 tests that test sqlite migrations as well as all the methods in the ReceiptStore implementation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-06 19:26:48 +0000 UTC
    </div>
</div>

