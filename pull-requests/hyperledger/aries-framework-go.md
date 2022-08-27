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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3345" class=".btn">#3345</a>
            </td>
            <td>
                <b>
                    feat: wallet.Issue supports jwtvc, verifiable.Credential can hold a jwtvc
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
        Created At 2022-08-23 19:13:12 +0000 UTC
    </div>
</div>

