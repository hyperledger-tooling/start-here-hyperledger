---
layout: default
title: anoncreds-rs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/anoncreds-rs
---

# anoncreds-rs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/anoncreds-rs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/291" class=".btn">#291</a>
            </td>
            <td>
                <b>
                    Reworked w3c credentials and presentations to use DataIntegrityProof  instead of custom AnonCreds context
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update W3C Credential to match the design: https://github.com/hyperledger/anoncreds-spec/issues/192

I also included changes from the following PRs as their changes significantly intersected with the current one: 
* Drop encoding - https://github.com/hyperledger/anoncreds-rs/pull/284
* Drop mapping - https://github.com/hyperledger/anoncreds-rs/pull/274

Regarding vc format `1.1`/`2.0:` I added an option parameter `version` to `anoncreds_process_w3c_credential`, `anoncreds_credential_to_w3c`, and `anoncreds_create_w3c_presentation` functions defining what vc format to return.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-20 06:16:52 +0000 UTC
    </div>
</div>

