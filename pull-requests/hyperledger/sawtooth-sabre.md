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
                PR <a href="https://github.com/hyperledger/sawtooth-sabre/pull/168" class=".btn">#168</a>
            </td>
            <td>
                <b>
                    Fix mistune doc build error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-15 16:55:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-sabre/pull/167" class=".btn">#167</a>
            </td>
            <td>
                <b>
                    Switch simple logger to use UTC timestamps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates simple logger to be configured with UTC timestamps. Local timestamps require a compiler flag, unsound_local_offset, which is required by a transient dependency.  The time crate (the transient
dependency in question) describes this flag as untested, and it fails in certain environments, such as CI.

See https://time-rs.github.io/internal-api/time/index.html#feature-flags for more information

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-15 15:19:20 +0000 UTC
    </div>
</div>

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

