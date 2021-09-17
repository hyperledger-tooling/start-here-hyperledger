---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/348" class=".btn">#348</a>
            </td>
            <td>
                <b>
                    Expose thread id
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">wrappers</span><span class="chip">breaking</span>
            </td>
            <td>
                Expose getters of thread ids of message threads associated with the corresponding connection, proof, disclosed proof, credential or issuer credential.

New methods:
* `vcx_connection_get_thread_id`
* `vcx_credential_get_thread_id`
* `vcx_disclosed_proof_get_thread_id`
* `vcx_issuer_credential_get_thread_id`
* `vcx_proof_get_thread_id`

Signed-off-by: Miroslav Kovar <miroslavkovar@protonmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 19:24:51 +0000 UTC
    </div>
</div>

