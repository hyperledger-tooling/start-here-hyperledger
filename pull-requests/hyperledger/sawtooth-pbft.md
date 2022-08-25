---
layout: default
title: sawtooth-pbft
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-pbft
---

# sawtooth-pbft <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-pbft){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-pbft/pull/185" class=".btn">#185</a>
            </td>
            <td>
                <b>
                    Fix derive_partial_eq_without_eq Clippy error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes a clippy error introduced in Rust 1.63

If a type T derives PartialEq and all of its members implement
Eq, then T can always implement Eq. Implementing Eq allows T to be
used in APIs that require Eq types. It also allows structs
containing T to derive Eq themselves.

Signed-off-by: Andrea Gunderson <agunde@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-24 20:07:38 +0000 UTC
    </div>
</div>

