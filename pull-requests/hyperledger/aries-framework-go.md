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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3324" class=".btn">#3324</a>
            </td>
            <td>
                <b>
                    fix: vc subject marshal
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
        Created At 2022-08-10 16:10:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3322" class=".btn">#3322</a>
            </td>
            <td>
                <b>
                    fix: JWS algorithm for signature suite 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Firas Qutishat <firas.qutishat@securekey.com>

closes #1589
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 09:59:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3320" class=".btn">#3320</a>
            </td>
            <td>
                <b>
                    feat: allow mediator GetConnections APIs to filter by didcomm version.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #3321 

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-08 23:40:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3319" class=".btn">#3319</a>
            </td>
            <td>
                <b>
                    fix: presentation with empty credential fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change fixes how a presentation is marshalled with empty credential field which wrongly outputs:
'"verifiableCredential": null'

This change skips this field if the presentation Credential field is empty

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-08 19:12:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3318" class=".btn">#3318</a>
            </td>
            <td>
                <b>
                    Add RemoveCredentialByName to aries.js
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Function was available in the core but was missing from the JavaScript
wrapper.

Signed-off-by: Boran Car <boran.car@gmail.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-08 16:44:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3316" class=".btn">#3316</a>
            </td>
            <td>
                <b>
                    fix: small change in schema format for clearness
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changed `mediatype` -> `contentMediaType`
and `encoding` -> `contentEncoding` in schema for better clearness in credential manifests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-05 19:50:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3315" class=".btn">#3315</a>
            </td>
            <td>
                <b>
                    feat: Add jwt-vc test suites supporting AFGO
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Mykhailo Sizov <mykhailo.sizov@securekey.com>

**Title:**
Add jwt-vc test suites supporting AFGO

**Description:**
https://github.com/hyperledger/aries-framework-go/issues/3288

**Summary:**
Added signer and verifier based on private/public key type.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-04 13:37:41 +0000 UTC
    </div>
</div>

