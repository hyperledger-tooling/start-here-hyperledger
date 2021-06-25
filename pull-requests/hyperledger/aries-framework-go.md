---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2848" class=".btn">#2848</a>
            </td>
            <td>
                <b>
                    feat: vcwallet command controller - expire token option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Part of #2433

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-24 20:53:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2847" class=".btn">#2847</a>
            </td>
            <td>
                <b>
                    did:key updates for JsonWebKey2020
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                All the changes applies to the did:key method.

Updated the serialization of the EC keys (P-256, P-384, P-521) to use the compressed format as specified in the multicodec specs.
When creating a did:key with JsonWebKey2020 the caller must pass in a json web key.
When reading a did:key with JsonWebKey2020 then return a did doc with a json web key
When reading a did:key enforce that the did method is "key"
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-24 14:32:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2846" class=".btn">#2846</a>
            </td>
            <td>
                <b>
                    feat: vcwallet - auth capability support for WebKMS & EDV unlock
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Closes #2845

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-24 02:06:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2844" class=".btn">#2844</a>
            </td>
            <td>
                <b>
                    feat: wallet - check profile exists
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Closes #2843

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 16:49:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2842" class=".btn">#2842</a>
            </td>
            <td>
                <b>
                    feat: JSON-LD Context API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andriy Holovko <andriy.holovko@gmail.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-22 16:43:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2841" class=".btn">#2841</a>
            </td>
            <td>
                <b>
                    feat: finalize 1PU draft4 implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">aip 2.0</span><span class="chip">enhancement</span>
            </td>
            <td>
                This change concludes 1PU Draft4 implementation by:
- using AES-CBC+HMAC-SHA content encryption
- make content encryption execute before key wrapping
- pass encrytpion tag to key wrapping
- make epk, apu, apv and alg recipient headers common in ProtectHeaders
- ensures JWE/KW compatibility with ecdh-1pu draft4 example B test vector for both content encryption and full JWE decryption

closes #2816

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-22 01:19:05 +0000 UTC
    </div>
</div>

