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
                PR <a href="https://github.com/hyperledger/anoncreds-clsignatures-rs/pull/18" class=".btn">#18</a>
            </td>
            <td>
                <b>
                    Tails and accumulator refactoring
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds wrappers around the Accumulator and Tail types instead of exposing PointG2 (no compatiblity change for indy-credx or anoncreds-rs).

Adds utility methods to RevocationRegistry for generating the initial state and a future state with a set of issued indexes, for use in anoncreds-rs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-16 18:03:17 +0000 UTC
    </div>
</div>

