---
layout: default
title: agora-glass_pumpkin
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/agora-glass_pumpkin
---

# agora-glass_pumpkin <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/agora-glass_pumpkin){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/agora-glass_pumpkin/pull/24" class=".btn">#24</a>
            </td>
            <td>
                <b>
                    Faster safe prime generation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This update aligns the safe prime generation more with the recommendations in https://eprint.iacr.org/2003/186, particularly in eliminating candidates for `q` that are congruent to `(r-1)/2` for the small primes that are checked.

On my system the time to generate a 256-bit safe prime is reduced by 90-95% (to about 25ms on average) and seems competitive with OpenSSL. Unit tests in anoncreds-clsignatures can run in a few minutes.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-24 17:02:23 +0000 UTC
    </div>
</div>

