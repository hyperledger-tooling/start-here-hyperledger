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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3362" class=".btn">#3362</a>
            </td>
            <td>
                <b>
                    test: add JWTVC coverage to wallet VC bdd tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also fixes an issue with pEx JWTVC constraint filtering.

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-02 19:27:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3360" class=".btn">#3360</a>
            </td>
            <td>
                <b>
                    feat: Change Credential Fulfillment name to Credential Response
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Derek Trider <Derek.Trider@securekey.com>

closes #3358 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 18:48:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3357" class=".btn">#3357</a>
            </td>
            <td>
                <b>
                    JSON LD Contexts in JWT VCs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Mykhailo Sizov <mykhailo.sizov@securekey.com>

**Title:**
JSON LD Contexts in JWT VCs

**Description:**
Solves: https://github.com/hyperledger/aries-framework-go/issues/3351

**Summary:**

Added extra option to `ValidateJSONLD` function called `WithStrictContextURIPosition` that sets strict validation of URI position within context property. The index of uri in underlying slice represents the position of given URI in parsed context array.
Also, added this option as a default to `*verifiable.Credential.validateJSONLD(.... docjsonld.WithStrictContextURIPosition(baseContext))` function in order to make base context URI required.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 14:51:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3355" class=".btn">#3355</a>
            </td>
            <td>
                <b>
                    feat: BDD tests for legacy connection protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
BDD tests for legacy-connection protocol

**Summary:**

- Add BDD test feature for case with mediator. 
- Enable to add recipient keys while creating did:peer doc with legacy service type.
-  Make a few refactoring

Closes #3301 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 07:10:04 +0000 UTC
    </div>
</div>

