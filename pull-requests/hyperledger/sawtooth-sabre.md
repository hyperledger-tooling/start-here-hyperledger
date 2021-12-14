---
layout: default
title: sawtooth-sabre
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-sabre
---

# sawtooth-sabre <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-sabre){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-sabre/pull/166" class=".btn">#166</a>
            </td>
            <td>
                <b>
                    Replace rust-crypto with sha2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The `"rust-crypto"` dependency was only being used for the Sha512 hashing capability. This can easily be replaced with the `"sha2"` library.  This library benefits from a number of things:

* It's maintained - rust-crypto hasn't been updated for 5 years
* It's a smaller, single-purpose library - lower compile times
* It's wasm-friendly - no need for target-specific dependencies
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-14 16:08:01 +0000 UTC
    </div>
</div>

