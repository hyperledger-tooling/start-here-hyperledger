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
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/327" class=".btn">#327</a>
            </td>
            <td>
                <b>
                    fix(rn): update libanoncreds headers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I was updating my react-native app to last credo alpha (which uses anoncreds-rs 0.2.0) and wasn't able to build in any OS due to a type error. It seems that the libanoncreds.h header wasn't updated after the changes in https://github.com/hyperledger/anoncreds-rs/pull/320.

I've regenerated the file using `cbindgen` and noticed several changes (like comments and some methods that were missing), so I guess it has been modified manually lately.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-15 22:03:29 +0000 UTC
    </div>
</div>

