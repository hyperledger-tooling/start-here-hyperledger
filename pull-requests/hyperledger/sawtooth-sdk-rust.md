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
                PR <a href="https://github.com/hyperledger/sawtooth-sdk-rust/pull/79" class=".btn">#79</a>
            </td>
            <td>
                <b>
                    Fix "needless_late_init" Clippy lint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This lint was introduced in 1.59v of Rust

Checks for late initializations that can be replaced by
a let statement with an initializer.

Assigning in the let statement is less repetitive.

Signed-off-by: Andrea Gunderson <agunde@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-03 21:59:26 +0000 UTC
    </div>
</div>

