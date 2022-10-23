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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3413" class=".btn">#3413</a>
            </td>
            <td>
                <b>
                    feat: Update Tink version, protobuf type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updated the Tink version and our methods to use the newer protobuf type that it uses.

Reason for this change: the existing version of Tink makes use of a very large int in one particular place in the code, and this very large int prevents the gomobile tool from successfully generating Android bindings. This meant that aries-framework-go packages that used Tink could not be used in any code that you may want to generate Android bindings for. The updated version of Tink does not have that check anymore, which resolves the issue.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-21 21:46:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3412" class=".btn">#3412</a>
            </td>
            <td>
                <b>
                    chore: add issuedAt claim to jwt
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Firas Qutishat <firas.qutishat@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-21 15:34:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3411" class=".btn">#3411</a>
            </td>
            <td>
                <b>
                    feat: support secp256k1 curve in KMS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds secp256k1 keys support in the kms for the IEEE-P1363 format only.
DER format is not supported because the x509 package does not support this curve.
The framework does support the creation of an secp256k1 key with DER format, however storing it in the KMS is not supported.

closes #3410

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-21 13:41:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3409" class=".btn">#3409</a>
            </td>
            <td>
                <b>
                    fix: parse generic ServicePoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Firas Qutishat <firas.qutishat@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-20 08:02:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3405" class=".btn">#3405</a>
            </td>
            <td>
                <b>
                    chore: handle PathNested in presexch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Firas Qutishat <firas.qutishat@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-17 18:36:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3403" class=".btn">#3403</a>
            </td>
            <td>
                <b>
                    fix: get DID uri from kid if exists
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Firas Qutishat <firas.qutishat@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-17 11:12:35 +0000 UTC
    </div>
</div>

