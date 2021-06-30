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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/313" class=".btn">#313</a>
            </td>
            <td>
                <b>
                    Update version of libc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 17:01:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/312" class=".btn">#312</a>
            </td>
            <td>
                <b>
                    Remove unncesessary deps from agency client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslavkovar@protonmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 10:37:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/310" class=".btn">#310</a>
            </td>
            <td>
                <b>
                    Try to fix occasionally failing integration test.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci</span><span class="chip">hotfix</span><span class="chip">tests</span>
            </td>
            <td>
                The test `test_create_credential_works_twice` occasionally fails in CI - never run into this issue locally. The CI failure of this test is such that the second of creating the same credential definition passes, while it's expected to fail. I think the reason is  that probably on the second attempt, the created credential definition is not yet fully propagated through the pool, and so it appears like the credential definition doesn't exist yet. 
This PR add timeout into the test between first and second attempt to create the same cred. definition.

Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 08:10:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/309" class=".btn">#309</a>
            </td>
            <td>
                <b>
                    Ci/crate publishing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci</span>
            </td>
            <td>
                - Add CI jobs to locally overwrite version in crate.toml files for `libvcx` and `agency_client` crates and subsequently publish them on crates.io
- If CI is running for release, crates are published only if tests pass
- If CI is running non-release, crates are published as soon as possible
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-28 13:38:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/308" class=".btn">#308</a>
            </td>
            <td>
                <b>
                    Release 0.19.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslavkovar@protonmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-28 12:30:34 +0000 UTC
    </div>
</div>

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

