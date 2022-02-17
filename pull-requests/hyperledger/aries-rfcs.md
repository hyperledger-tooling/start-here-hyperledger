---
layout: default
title: aries-rfcs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-rfcs
---

# aries-rfcs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-rfcs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/721" class=".btn">#721</a>
            </td>
            <td>
                <b>
                    feature: revocation notification v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds revocation notification v2 as discussed in Aries WG calls 2022/01/19, 2022/02/16, and in #705. 
The primary changes from the v1 protocol are adding a field to identify the format of revocation and adjusting `thread_id` to be `credential_id` to communicate the credential identifier of the revoked credential instead of the thread of the issue-credential-v2 exchange (as this exchange may include multiple credentials being issued in the same thread and the thread_id may not be held onto by all holders).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-16 19:24:02 +0000 UTC
    </div>
</div>

