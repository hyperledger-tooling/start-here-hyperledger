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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/307" class=".btn">#307</a>
            </td>
            <td>
                <b>
                    Add tests with json attachment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This was supposed to be part of #302 which was merged prematurely due to missed PM.

Signed-off-by: Miroslav Kovar <miroslavkovar@protonmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 18:26:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/306" class=".btn">#306</a>
            </td>
            <td>
                <b>
                    Use libindy with rusql fix for ios build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">hotfix</span><span class="chip">pre-release</span><span class="chip">update</span>
            </td>
            <td>
                Includes new version of libindy with [this](https://github.com/hyperledger/indy-sdk/pull/2402) changes which fixes a bug present on iOS where thread panics on wallet opening.

In order to successfully build for iOS however, we have to use the `vendored` [feature](https://docs.rs/openssl/0.10.35/openssl/#vendored) for openssl dependency. This, in turn, breaks compilation for the musl C environment on Alpine. Hence, `X86_64_ALPINE_LINUX_MUSL_OPENSSL_NO_VENDOR` environment variable was set as a way to not use the `vendored` flag on Alpine. This is a temporary fix, as the plan is to remove the dependency on openssl completely.

Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
Signed-off-by: Miroslav Kovar <miroslavkovar@protonmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 12:06:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/305" class=".btn">#305</a>
            </td>
            <td>
                <b>
                    Fix bug in encoding new attributes format
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">hotfix</span>
            </td>
            <td>
                Adding new credential data format in #291 introduced a bug - an `"attr_name"` was encoded instead of `attr_name`. This change fixes the issue and covers the case with a unit test.

Signed-off-by: Miroslav Kovar <miroslavkovar@protonmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-22 15:25:22 +0000 UTC
    </div>
</div>

