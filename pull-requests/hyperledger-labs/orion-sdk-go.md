---
layout: default
title: orion-sdk-go
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/orion-sdk-go
---

# orion-sdk-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/orion-sdk-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-sdk-go/pull/71" class=".btn">#71</a>
            </td>
            <td>
                <b>
                    Allow external TxID on data tx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Allow external TxIDs on data tx (for now)
- check the characters of external TxID
- the internal commonTxContext augmented with variadic config function parameter
- config function WithTxID

This forms the basis for future options to be given to the TxContext of other types as well.

Signed-off-by: Yoav Tock <tock@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-25 09:34:38 +0000 UTC
    </div>
</div>

