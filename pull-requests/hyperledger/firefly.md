---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1398" class=".btn">#1398</a>
            </td>
            <td>
                <b>
                    Do not expect to retrieve local org during definition handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-candidate</span>
            </td>
            <td>
                Only the org DID is needed for this check - no need to actually look up the org from the database. At this point the message author has already been verified, so a database lookup here is just extra unnecessary processing (and can lead to infinite retries if it fails).

Fixes #1397
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-05 18:47:02 +0000 UTC
    </div>
</div>

