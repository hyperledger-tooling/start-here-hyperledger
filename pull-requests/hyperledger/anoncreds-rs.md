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
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/229" class=".btn">#229</a>
            </td>
            <td>
                <b>
                    Update to anoncreds-clsignatures 0.2, update tails access
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This merges some changes to the tails file handling from indy-credx. The tempfile library is not compatible with some filesystems like on Azure (https://github.com/hyperledger/indy-shared-rs/issues/21). This removes that dependency and adds buffering to the IO operations which helps performance.

The tails file path is no longer required for the credential revocation config when issuing, this would require a JS wrapper update as well.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-03 21:03:20 +0000 UTC
    </div>
</div>

