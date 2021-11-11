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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3047" class=".btn">#3047</a>
            </td>
            <td>
                <b>
                    fix: Crytpo signature verification using P384 key from JWK import 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since P-384 DER format was using Tink's default signature template which uses SHA512, it was causing keys imported from a JWK to fail.
This change uses a template with SHA384 instead to keep signature/verification consistent in all cases (native kms key vs JWK imported key).


Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 16:54:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3044" class=".btn">#3044</a>
            </td>
            <td>
                <b>
                    feat: Credential Manifest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 04:12:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3042" class=".btn">#3042</a>
            </td>
            <td>
                <b>
                    feat: add issue credential V3 wasm test
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
        Created At 2021-11-08 08:24:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3040" class=".btn">#3040</a>
            </td>
            <td>
                <b>
                    chore: fix bdd test run flag
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
        Created At 2021-11-04 22:01:22 +0000 UTC
    </div>
</div>

