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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3514" class=".btn">#3514</a>
            </td>
            <td>
                <b>
                    fix: prexexch - contains check on filter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-03 22:39:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3513" class=".btn">#3513</a>
            </td>
            <td>
                <b>
                    chore: Add audience option to issuer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Included:
- resolve merge conflict in unit-tests between Filip's id PR and add SD-JWT to presexch PR
- add audience option to issuer
- remove irrelevant to-do(s)
- remove one integration test (was replaced by NewFromVC)
- add sha-384 to integration tests

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-03 21:21:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3512" class=".btn">#3512</a>
            </td>
            <td>
                <b>
                    feat: creating SD-JWT from VC will leave subject ID as regular field
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                instead of turning subject ID into an SD field.

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-02 20:30:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3511" class=".btn">#3511</a>
            </td>
            <td>
                <b>
                    fix: ParseCredential handles SD-JWT VCs with _sd_alg in subject
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-31 20:10:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3510" class=".btn">#3510</a>
            </td>
            <td>
                <b>
                    feat: ParseCredential recognizes if SD-JWT VC is issuance or presentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                without needing the caller to specify.

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-31 16:31:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3509" class=".btn">#3509</a>
            </td>
            <td>
                <b>
                    feat: Add support for SD-JWT in presentation exchange
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add support for SD-JWT in presentation exchange

Closes #3508

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-31 15:11:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3507" class=".btn">#3507</a>
            </td>
            <td>
                <b>
                    chore: decode presentation credential in SD JWT format
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Mykhailo Sizov <mykhailo.sizov@securekey.com>


**Title:**
Fix decoding presentation credential in SD JWT combined format for presentation.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-31 12:38:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3506" class=".btn">#3506</a>
            </td>
            <td>
                <b>
                    feat: Credential.MarshalJSON now marshals all SD-JWT disclosures
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-30 21:02:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3504" class=".btn">#3504</a>
            </td>
            <td>
                <b>
                    fix: allow SD-JWT parsing when sd alg is in cred subject
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-30 15:40:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3503" class=".btn">#3503</a>
            </td>
            <td>
                <b>
                    chore: Additional hash algorithms; check for _sd claim
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add SHA-384 and SHA-512 algorithms to SHA-256.
Also, check for _sd claim in claims before creating SD-JWT.

Closes #3502

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-30 15:25:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3501" class=".btn">#3501</a>
            </td>
            <td>
                <b>
                    chore: make JWT alg name method exportable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Mykhailo Sizov <mykhailo.sizov@securekey.com>


**Title:**
Make JWSAlgorithm.Name() method exportable

**Summary:**
To be able to create JWS signer from external packages and avoid code duplication, I made  JWSAlgorithm.Name() method as exportable
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-30 14:09:26 +0000 UTC
    </div>
</div>

