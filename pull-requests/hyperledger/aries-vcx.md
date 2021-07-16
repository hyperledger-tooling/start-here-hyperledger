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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/318" class=".btn">#318</a>
            </td>
            <td>
                <b>
                    Release 0.20.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">changelog-excluded</span>
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslavkovar@protonmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 13:20:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/317" class=".btn">#317</a>
            </td>
            <td>
                <b>
                    Replace openssl by crates num-bigint, sha2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span>
            </td>
            <td>
                OpenSSL in libvcx is increasing build complexity and has occasionally produced build issues on some platforms.
However there's only 2 use cases for OpenSSL - big numbers and sha256. These problems has been implemented in pure Rust already.
Big numbers and sha hashing is used for encoding credential attributes and is being tested by following tests:
```
    aries::handlers::issuance::issuer::utils::tests::test_encode_empty_field
    aries::handlers::issuance::issuer::utils::tests::test_encode_with_aries_format_several_attributes_success
    aries::handlers::issuance::issuer::utils::tests::test_encode_with_mixed_format_several_attributes_success
    aries::handlers::issuance::issuer::utils::tests::test_encode_with_new_format_one_attribute_success
    aries::handlers::issuance::issuer::utils::tests::test_encode_with_new_format_several_attributes_success
    aries::handlers::issuance::issuer::utils::tests::test_encode_with_one_attribute_success
    aries::handlers::issuance::issuer::utils::tests::test_encode_with_several_attributes_success
    utils::openssl::test::test_encoding
 ```

Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-12 12:21:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/316" class=".btn">#316</a>
            </td>
            <td>
                <b>
                    Install cargo via rustup in alpine image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci</span><span class="chip">hotfix</span>
            </td>
            <td>
                Cargo has been installed via apk until now, limiting us with regards to the toolchain version we used to compile our images. Via rustup, we have more freedom to choose the toolchain version.

Signed-off-by: Miroslav Kovar <miroslavkovar@protonmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-12 10:39:43 +0000 UTC
    </div>
</div>

