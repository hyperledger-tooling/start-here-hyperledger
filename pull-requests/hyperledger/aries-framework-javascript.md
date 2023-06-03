---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1475" class=".btn">#1475</a>
            </td>
            <td>
                <b>
                    chore(release): v0.4.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci-test</span>
            </td>
            <td>
                Release version 0.4.0
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-01 12:10:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1474" class=".btn">#1474</a>
            </td>
            <td>
                <b>
                    feat: support for openid4vci draft 11
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
        Created At 2023-05-31 09:29:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1472" class=".btn">#1472</a>
            </td>
            <td>
                <b>
                    feat(openid4vc): jwt format and more crypto
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds support for receiving JWT credentials in the openid4vc client, and also extends support for supported proof of possession JWA signature algorithms. 

To be able to support multiple signature algs, I had to remove the `kid` parameter, as the crypto that will be used, and the did methods the issuer supports has a big impact of the `kid` that will be selected.

For this, a new `proofOfPossessionVerificationMethodResolver` function MUST be supplied when requesting a credential through the openi4vc-client in AFJ, that is called whenever a verification method id (kid) must be determined for a to be created proof of possesion. The callback takes the following options, which should give the caller enough  information to determine the verification method:

```ts
export interface ProofOfPossessionVerificationMethodResolverOptions {
  /**
   * The credential format that will be requested from the issuer.
   * E.g. `jwt_vc` or `ldp_vc`.
   */
  credentialFormat: SupportedCredentialFormats

  /**
   * The JWA Signature Algorithm that will be used in the proof of possession.
   * This is based on the `allowedProofOfPossessionSignatureAlgorithms` passed
   * to the request credential method, and the supported signature algorithms.
   */
  proofOfPossessionSignatureAlgorithm: JwaSignatureAlgorithm

  /**
   * This is a list of verification methods types that are supported
   * for creating the proof of possession signature. The returned
   * verification method type must be of one of these types.
   */
  supportedVerificationMethods: string[]

  /**
   * The key type that will be used to create the proof of possession signature.
   * This is related to the verification method and the signature algorithm, and
   * is added for convenience.
   */
  keyType: KeyType

  /**
   * The credential type that will be requested from the issuer. This is
   * based on the credential types that are included the credential offer.
   */
  credentialType: string

  /**
   * Whether the issuer supports the `did` cryptographic binding method,
   * indicating they support all did methods. In most cases, they do not
   * support all did methods, and it means we have to make an assumption
   * about the did methods they support.
   *
   * If this value is `false`, the `supportedDidMethods` property will
   * contain a list of supported did methods.
   */
  supportsAllDidMethods: boolean

  /**
   * A list of supported did methods. This is only used if the `supportsAllDidMethods`
   * property is `false`. When this array is populated, the returned verification method
   * MUST be based on one of these did methods.
   *
   * The did methods are returned in the format `did:<method>`, e.g. `did:web`.
   */
  supportedDidMethods: string[]
}
```

It adds a bit of complexity for the caller, but there's simply no way for AFJ to know which did method or key we should use in a proof of possession, as that's heavily reliant on business logic. And passing it upfront also doesn't work, as the caller is missing important information. 

The crypto that can be used for the proof of possesion is based on what is supported by the wallet and the registered JSON-LD signatuer suites. So if we were to add new key types / JWA siganture algortihms or signature suites, the openid4vc client wouldn't have to be changed at all.

You can limit which algs and credential formats you want to allow, so those aren't considered as option when the issuer supports them through the `allowedCredentialFormats` and `allowedProofOfPossessionSignatureAlgorithms` properties. (e.g. I only want to receive `jwt_vc` credentials with `ES256` alg, even if my wallet and the issuer both support `Ed25519Signature2018`. We may want to also add a property for `allowedDidMethods` so we won't consider an option if your specific did method, or all did methods arern't supported by the issuer.

~~Dependant on #1468~~
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-29 10:57:47 +0000 UTC
    </div>
</div>

