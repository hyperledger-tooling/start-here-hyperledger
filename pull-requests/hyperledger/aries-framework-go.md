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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3627" class=".btn">#3627</a>
            </td>
            <td>
                <b>
                    fix: data-integrity ecdsa2019 signer uses common signer interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-28 13:49:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3626" class=".btn">#3626</a>
            </td>
            <td>
                <b>
                    feat: DI - change verifier interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changed Data Integrity verifier interface.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-25 08:43:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3624" class=".btn">#3624</a>
            </td>
            <td>
                <b>
                    feat: added data integrity jsonld context
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Added data integrity JSON-LD context

**Description:**
Because of the missed DI JSON LD context (and disabled strict validation), Aries on issuance stage generated invalid `canonicalProofConfig` considering only `type` field.
Example:
```
_:c14n0 <http://www.w3.org/1999/02/22-rdf-syntax-ns#type> <DataIntegrityProof> .
```
Verification part was successful because Aries considered same `type` field. And because of that, Unit tests did not catch the typo that on verification stage field `created` was empty.

According to [Spec](https://www.w3.org/TR/vc-di-ecdsa/#base-proof-configuration-ecdsa-sd-2023), another fields must be also included in `canonicalProofConfig`.

After this PR, Aries generates the following `canonicalProofConfig`:
```
_:c14n0 <http://purl.org/dc/terms/created> "2023-08-23T16:57:33+03:00"^^<http://www.w3.org/2001/XMLSchema#dateTime> .
_:c14n0 <http://www.w3.org/1999/02/22-rdf-syntax-ns#type> <https://w3id.org/security#DataIntegrityProof> .
_:c14n0 <https://w3id.org/security#cryptosuite> "ecdsa-2019" .
_:c14n0 <https://w3id.org/security#proofPurpose> <https://w3id.org/security#assertionMethod> .
_:c14n0 <https://w3id.org/security#verificationMethod> <did:foo:bar#key-1> .
```



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-23 13:58:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3623" class=".btn">#3623</a>
            </td>
            <td>
                <b>
                    feat: create DI options aliases
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Follow up PR for https://github.com/hyperledger/aries-framework-go/pull/3621
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-22 14:04:39 +0000 UTC
    </div>
</div>

