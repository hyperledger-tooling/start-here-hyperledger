---
layout: default
title: anoncreds-clsignatures-rs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/anoncreds-clsignatures-rs
---

# anoncreds-clsignatures-rs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/anoncreds-clsignatures-rs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-clsignatures-rs/pull/24" class=".btn">#24</a>
            </td>
            <td>
                <b>
                    Ensure revocation index is in range
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For the issuer, this ensures that `rev_idx` is in range, to avoid issuing invalid credentials. Previously this could issue an invalid credential with the index `0`, or panic due to an overflow for values greater than `max_cred_num`.

For the prover, this checks that the revocation index is not zero when processing a credential (`max_cred_num` is not available here without changing the API).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-05 22:31:28 +0000 UTC
    </div>
</div>

