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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3303" class=".btn">#3303</a>
            </td>
            <td>
                <b>
                    feat: mediator supports didcomm v1/v2 per-connection
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
        Created At 2022-07-26 19:02:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3296" class=".btn">#3296</a>
            </td>
            <td>
                <b>
                    test: interop jwt vc ecdsa
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Part of #3289 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-25 12:10:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3295" class=".btn">#3295</a>
            </td>
            <td>
                <b>
                    feat: Connection protocol (RFC-0160) DIDCommV1 implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
[Connection](https://github.com/hyperledger/aries-rfcs/tree/main/features/0160-connection-protocol#0160-connection-protocol) protocol (RFC-0160) DIDCommV1 implementation

**Summary:**

- On this PR only part related to protocol package is implemented (client part is not implemented yet)
- Also package called as `didconnection` because `connection` name is already used


closes https://github.com/hyperledger/aries-framework-go/issues/3299
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-25 11:38:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3294" class=".btn">#3294</a>
            </td>
            <td>
                <b>
                    feat: implement did-core JSON-LD `@context` representation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Chris Abernethy <brownoxford@gmail.com>

**Title:**
Implement did-core JSON-LD `@context` representation

**Description:**
Current implementation assumes `@context` can only be `[]string`, but did-core v1 defines `@context` for DID documents in JSON-LD representation to be either a string or a list containing maps and/or strings.

**Summary:**
* Created `type Context {}interface` to represent did document contexts with appropriate comment for IDE integration.
* Modified `did.parseContext` to add parsing of `string` and `[]interface{}` context representations.
* Added `LookupContextString` helper to search for context string through entire context (used by `requiresLegacyHandling`)
* Added `LookupSchemaFromContext` helper to peek first string in context. Replaces direct references to `context[0]`
* Modified existing tests to account for new context format
* Added tests for new helper functions
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-22 20:35:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3293" class=".btn">#3293</a>
            </td>
            <td>
                <b>
                    fix: bdd test ci
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
        Created At 2022-07-22 19:21:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3291" class=".btn">#3291</a>
            </td>
            <td>
                <b>
                    feat: allow custom GNAP header signer in vcwallet command
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
        Created At 2022-07-22 19:10:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3286" class=".btn">#3286</a>
            </td>
            <td>
                <b>
                    test: interop jwt VCs tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds tests to ensure AFGO does support JWT VC parsing/verificaition by adding interop tests using VCs from external sources.
Also part of this change: expose JWT needed jose verifiers and signers for external use.

closes #3279

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-21 15:16:53 +0000 UTC
    </div>
</div>

