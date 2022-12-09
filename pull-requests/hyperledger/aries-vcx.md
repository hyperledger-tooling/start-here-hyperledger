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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/691" class=".btn">#691</a>
            </td>
            <td>
                <b>
                    689 support didkey aries rfc 0360
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">feature</span>
            </td>
            <td>
                function _ed25519_public_key_to_did_key was created, which transforms a naked did into a did:key
and the did_key_to_public_key function returns if did:key, just your key
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-08 20:45:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/688" class=".btn">#688</a>
            </td>
            <td>
                <b>
                    Release 0.50.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pre-release</span>
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-05 09:35:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/687" class=".btn">#687</a>
            </td>
            <td>
                <b>
                    Release 0.49.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pre-release</span>
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-04 18:13:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/686" class=".btn">#686</a>
            </td>
            <td>
                <b>
                    Fix legacy wrapper ios release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pre-release</span>
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-04 16:01:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/684" class=".btn">#684</a>
            </td>
            <td>
                <b>
                    Replace failure crate with thiserror
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span><span class="chip">agents</span><span class="chip">dependencies</span>
            </td>
            <td>
                Replaces the dependency on outdated `failure` crate with the dependency on `thiserror` in `messages`, `aries-vcx-agent`, `aries-vcx` and `libvcx`. Although our entire approach to logging needs to be reconsidered, removing a dependency on an unmaintained crate is likely not a step in the wrong direction.

It seems that we have to temporarily give up backtrace in libvcx errors stored in `CURRENT_ERROR_C_JSON` until `error_generic_member_access` is [stabilized](https://github.com/rust-lang/rust/issues/99301) since `thiserror` makes use of [unstable](https://doc.rust-lang.org/std/error/trait.Error.html#method.provide) `provide()` method to the error type in order to capture and share `std::backtrace::Backtrace`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-02 21:57:10 +0000 UTC
    </div>
</div>

