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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3382" class=".btn">#3382</a>
            </td>
            <td>
                <b>
                    chore: upgrade to Go 1.19
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Upgrade golang version to 1.19

**Summary**

- Upgrade golang version to 1.19
- Change some unit tests due to changes of `http/client` module of new SDK 1.19
- Change unit tests related to x509 certificate error


Closes #3370
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-23 10:19:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3381" class=".btn">#3381</a>
            </td>
            <td>
                <b>
                    feat: Add validation for domain linkage credential in JWT format for did configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add validation for domain linkage credential in JWT format for did configuration.

Closes #3377

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-22 21:08:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3380" class=".btn">#3380</a>
            </td>
            <td>
                <b>
                    chore: Remove adding "iat" when creating JWT Claim
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently when creating JWT claim from VC we are setting "iat" (IssuedAt). This is not part of spec.

Closes #3379

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-21 18:22:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3378" class=".btn">#3378</a>
            </td>
            <td>
                <b>
                    chore: Remove optional "typ" header (JWS)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently we are setting optional "typ" header.

Closes #3376

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-21 16:41:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3375" class=".btn">#3375</a>
            </td>
            <td>
                <b>
                    feat: parse JWT VCs when resolving credential manifests
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
        Created At 2022-09-20 19:24:25 +0000 UTC
    </div>
</div>

