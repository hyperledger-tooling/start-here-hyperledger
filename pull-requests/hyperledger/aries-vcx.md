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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/331" class=".btn">#331</a>
            </td>
            <td>
                <b>
                    WIP: Download messages via a connection handle as u32
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">wrappers</span>
            </td>
            <td>
                The Java wrapper currently stores handles as `int` datatypes, which are converted back to `u32` when calling Rust FFI. However, the signature of `vcx_v2_messages_download` takes a list of handles as string. When passed the handles represented as `int`s through the Java API, the function fails. To enable safe message downloads from Java wrappers, this PR exposes a function which takes a single connection handle instead of a string. See #330 .

Signed-off-by: Miroslav Kovar <miroslavkovar@protonmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-09 14:41:23 +0000 UTC
    </div>
</div>

