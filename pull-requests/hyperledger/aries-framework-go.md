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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2852" class=".btn">#2852</a>
            </td>
            <td>
                <b>
                    added test cases for nist curves for did:key and fingerprint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: david.stark <david.stark@securekey.com>

Added test cases to cover the changes to did:key NIST curve implementation from previous pull request.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-28 18:30:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2851" class=".btn">#2851</a>
            </td>
            <td>
                <b>
                    feat: enable ecdh-1pu draft4 JWE decryption test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">aip 2.0</span><span class="chip">enhancement</span>
            </td>
            <td>
                This change enables the commented out test for full compatibility with ECDH-1PU draft4 Appendix B example.

It also includes the following changes:
* fixes CBC+HMAC keys extracted from the ECDH cek. The keys were inversed.
* moved recipients' kids list from AAD to APV (recipients) protectedHeader
* use originalProtectedHeaders if populated instead of protectedHeader when building authData. To avoid marshal/unmarshal calls from changing the json order.
* ECDH-1PU messages with multi-recipients can now read the sender kid (skid) from APU if skid wass empty since it's an optional header.

closes #2850

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-26 00:40:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2849" class=".btn">#2849</a>
            </td>
            <td>
                <b>
                    fix: wallet - incorrect crypto for EDV with WebKMS profiles
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
        Created At 2021-06-25 21:03:39 +0000 UTC
    </div>
</div>

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

