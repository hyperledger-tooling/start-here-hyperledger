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
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/129" class=".btn">#129</a>
            </td>
            <td>
                <b>
                    Update receipt store function to filter on `service_id`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Update the `count_txn_receipts` function to filter on the optional service ID when one is set.
- Update the multiple service ID receipt store test to call `count_txn_receipts` and ensure it returns the correct number of receipts.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-29 23:49:27 +0000 UTC
    </div>
</div>

