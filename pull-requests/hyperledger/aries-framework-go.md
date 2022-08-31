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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3353" class=".btn">#3353</a>
            </td>
            <td>
                <b>
                    feat: Add BDD test for legacy-connection protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Add BDD test for legacy-connection protocol

**Summary:**

- Add BDD test for legacy-connection protocol. Edge to edge case is fully implemented. Case through mediator is implemented partially (Only steps are added. Need to add .feature file to run test)
- Make a few refactoring

Related to #3301 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-29 11:08:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3352" class=".btn">#3352</a>
            </td>
            <td>
                <b>
                    Clean up connections after websocket close
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Clean up connections after WebSocket close

**Description:**
Make sure we clean up connections by just going through the map and
cleaning all the verkeys that match the connection. This is a suboptimal
solution, but a connection close is not something happening often.

Fixes https://github.com/hyperledger/aries-framework-go/issues/3349


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-26 22:46:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3350" class=".btn">#3350</a>
            </td>
            <td>
                <b>
                    feat: wallet Prove supports creating JWT presentations.
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
        Created At 2022-08-26 18:03:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3347" class=".btn">#3347</a>
            </td>
            <td>
                <b>
                    feat: support multi-format VC in presentation exchange
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #3348

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 20:22:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3346" class=".btn">#3346</a>
            </td>
            <td>
                <b>
                    test: BDD tests for universal wallet JSON-LD support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Mykhailo Sizov <mykhailo.sizov@securekey.com>

**Title:**
Support for JSON-LD in universal wallet implementation.

**Description:**
Solves: https://github.com/hyperledger/aries-framework-go/issues/3344

**Summary:**
Added BDD tests for universal wallet JSON-LD support.

Included the next actions:
- Sign JSON-LD Credential - Add it to wallet - get from wallet - verify Credential.
- Get JSON-LD Credential (without proof) - Call wallet.Issue() - get signed credential back - verify credential.
- Use signed credentials from previous steps - call wallet.Prove() - get presentation back - verify presentation.
- Add all the credentials from previous steps to holder's wallet - call wallet.Add(json-ld Credential) - wallet.Query() - get query result as json-ld presentation. (Included `wallet.QueryByExample` and `wallet.PresentationExchange` query types).
- Call wallet.GetAll() credential - get json-ld credentials back - check expected amount.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-24 09:53:26 +0000 UTC
    </div>
</div>

