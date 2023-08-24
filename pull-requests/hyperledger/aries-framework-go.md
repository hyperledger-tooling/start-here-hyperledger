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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3625" class=".btn">#3625</a>
            </td>
            <td>
                <b>
                    wip: use trustbloc/kms-go instead of kmscrypto component
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
        Created At 2023-08-24 06:06:06 +0000 UTC
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3622" class=".btn">#3622</a>
            </td>
            <td>
                <b>
                    feat: change SignerInitializerOptions KMS type
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
        Created At 2023-08-22 12:17:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3621" class=".btn">#3621</a>
            </td>
            <td>
                <b>
                    feat: change KMS interface for Data Integrity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Change KMS interface for Data Integrity.

**Summary:**
1. Introduced private KMS interface for ecdsa2019 Data integrity suite with only onte method.
2. Made `publicKeyBytesToHandle` function as exported from localkms package and used it in ecdsa2019 Data integrity suite verifier. The reason for it is that method
```
func (l *LocalKMS) PubKeyBytesToHandle(pubKey []byte, kt kmsapi.KeyType, opts ...kmsapi.KeyOpts) (interface{}, error) {
	return publicKeyBytesToHandle(pubKey, kt, opts...)
}
```
does not use receiver and func `PublicKeyBytesToHandle` can be used independently.



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-22 10:37:16 +0000 UTC
    </div>
</div>

