---
layout: default
title: private-data-objects
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/private-data-objects
---

# private-data-objects <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/private-data-objects){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/396" class=".btn">#396</a>
            </td>
            <td>
                <b>
                    consolidate hash and hmac functions & export them to wawaka contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                We started the day with three duplicate implementations of the hash functions in the common crypto library. This removes all but the one in the "correct" place (hash.cpp). 

Adds hash and hmac functions for sha512.

Makes the suite of hash and hmac functions available to wawaka contracts. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-27 18:27:39 +0000 UTC
    </div>
</div>

