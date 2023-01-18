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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3480" class=".btn">#3480</a>
            </td>
            <td>
                <b>
                    chore: Create SD-JWT without signature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add test for creating SD-JWT without signature.

Closes #3479

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-17 21:03:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3477" class=".btn">#3477</a>
            </td>
            <td>
                <b>
                    chore: Rename DisclosureSeparator to CombinedFormatSeparator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Clean-up task:

- rename DisclosureSeparator to CombinedFormatSeparator
- move issuer Payload struct from common to issuer package

Closes #3476

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-16 18:12:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3475" class=".btn">#3475</a>
            </td>
            <td>
                <b>
                    feat: SD-JWT Verifier: Verify Holder Binding
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If Holder Binding is required, verify that the Holder Binding JWT is signed by the Holder and valid.

Closes #3471

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-13 21:47:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3473" class=".btn">#3473</a>
            </td>
            <td>
                <b>
                    feat: SD-JWT Holder: Add Holder Binding
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Holder MAY add an optional JWT to prove Holder Binding to the Verifier. Nonce and aud claims are included to show that the proof is intended for the Verifier.

Closes #3470

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-11 22:55:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3472" class=".btn">#3472</a>
            </td>
            <td>
                <b>
                    feat: SD-JWT Issuer: Add Holder Public Key Claim (JWK)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If the Issuer wants to enable Holder Binding, it MAY include a public key associated with the Holder, or a reference thereto.

We use confirmation "cnf" claim to include raw public key by value in SD-JWT.

In this first iteration of "cnf" claim we will use "jwk" confirmation method and include public key information in JWK format. Other confirmation methods such as "jwe", "kid" and "jku" may be implemented at later time (if required).

Closes #3469 

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-11 18:57:46 +0000 UTC
    </div>
</div>

