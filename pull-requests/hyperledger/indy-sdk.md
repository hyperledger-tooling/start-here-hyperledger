---
layout: default
title: indy-sdk
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-sdk
---

# indy-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2594" class=".btn">#2594</a>
            </td>
            <td>
                <b>
                    fix: ignore credential not satisfying predicate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `fn _get_requested_credentials` throws an error even though the prover has a valid credential satisfying predicate. Let's say the prover has the following credential.

- cred1: have attribute `value=ANYTHING_BUT_NOT_A_NUMBER`
- cred2: have attribute `value=3`

and proof request with predicate
- value < 5

Ideally, `_get_requested_credentials` should return `[cred2]` in this case, but the function will throw an error. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-06 10:33:06 +0000 UTC
    </div>
</div>

