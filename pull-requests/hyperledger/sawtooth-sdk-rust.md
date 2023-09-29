---
layout: default
title: sawtooth-sdk-rust
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-sdk-rust
---

# sawtooth-sdk-rust <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-sdk-rust){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-sdk-rust/pull/88" class=".btn">#88</a>
            </td>
            <td>
                <b>
                    Fix clippy::single_range_in_vec_init lint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is almost always incorrect, as it will result in a Vec that has only one element. Almost always, the programmer intended for it to include all elements in the range or for the end of the range to be the length instead.

This means our correlations ids are not 16 characters long like we want. This fixes that issue.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-29 14:34:39 +0000 UTC
    </div>
</div>

