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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3374" class=".btn">#3374</a>
            </td>
            <td>
                <b>
                    fix: Docker warning when using frapsoft/openssl on arm64 system
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolved a warning from Docker that would get printed when running the generate-test-keys Makefile target on an arm64 system. The warning from Docker alerts you that the image for frapsoft/openssl is for amd64, which doesn't match the system you're on (when using an arm64-based OS). To resolve the warning, you have to either use an image that matches the system architecture, or explicitly state the platform using the --platform flag. In this case, there is only an amd64 version of frapsoft/openssl, so I added the explicit flag to resolve the warning. I also added a TODO for us to find an arm64 alternative in the future (although the amd64 version of frapsoft/openssl does seem to work fine on arm64 Mac OS currently, presumably due to Apple's Rosetta translation layer or some other emulation layer).

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-15 20:44:38 +0000 UTC
    </div>
</div>

