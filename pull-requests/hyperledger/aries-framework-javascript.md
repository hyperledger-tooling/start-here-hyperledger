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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1471" class=".btn">#1471</a>
            </td>
            <td>
                <b>
                    chore: improve ed25519 context url checks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We got some errors for a did document that didn't conform, but they weren't very helpful (hiding the actual error).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 14:49:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1470" class=".btn">#1470</a>
            </td>
            <td>
                <b>
                    feat: Split AFJ demo for two cases: Main and DidCommV2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Started work on splitting the Alice/Faber demo into smaller cases. Using this we can add demos for various optional modules.

- `Main` - general demo of issuing credentials and presenting the proof
- `DidComm V2` - demo reflecting supported didcomm v2 protocols


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 08:42:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1469" class=".btn">#1469</a>
            </td>
            <td>
                <b>
                    chore: add shared package as peer dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                this should hopefully help a bit with the version mismatches we've encountered with the shared comonents. By making it a peer dep it will be installed by the nodejs / react-native package and thus always be in sync
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-24 20:38:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1468" class=".btn">#1468</a>
            </td>
            <td>
                <b>
                    feat(w3cCredentials)!: add jwt vc support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds support for JWT VCs in addition to the already supported JSON-LD VCs. 

It became a bigger PR than anticipated, mainly because I moved some files around and made some changes to e.g. how verification methods are handled so they can be used without JSON-LD as well.

The PR has extracted the JSON-LD specific functionality from the `W3cCredentialService` into a new `W3cJsonLdCredentialService`, and we've got a new `W3cJwtCredentialService`. The general w3c credential service exposes a generic api to work with both, while the specific classes implement the logic. Records are only handled through the general w3c credential service. The idea is that users will mostly use the W3cCredentialService, and not the underlying imlementations, that is more to split up logic based on format.

The API has changed to now require a format when signing credentials / presentations:

```ts
w3cCredentialService.signCredential({
  format: 'jwt_vc',
  credential: /* the credential */,
  alg: 'ES256'
})
```

For the verification the API has also changed to support a more rich API. This rich API has been fully implemented for JWT VCs, but could not be fully supported for JSON-LD library due to the way errors are thrown in that library (see #1466, this will be addressed in a follow up pr).

The idea for the results is that now everything is handled by a custom validation object that has the following structure. The specific validations differ a bit between a VC and VP, but the idea is the same.

```ts
{
  isValid: true,
  validations: {
    // credential has no credentialStatus, so always valid
    credentialStatus: {
      isValid: true,
    },
    // This both validates whether the credential matches the
    // data model, as well as whether the credential is expired etc..
    dataModel: {
      isValid: true,
    },
    // This validates whether the signature is valid
    signature: {
      isValid: true,
    },
    // This validates whether the issuer is also the signer of the credential
    issuerIsSigner: {
      isValid: true,
    },
  },
};
```

For now, for JSON-LD verifications the result looks like this. This means the same data is available before this PR (the VC.js structure was followed), but a bit more nested. Over time we want to remove the use of vc.js and use the same structure as above for both credential formats. This allows for fine grained control over what you want to validate. 

```ts
{
  isValid: true,
  validations: {
    vcJs: {
      isValid: true,
      // results from the VC.JS library
      results: []
     }
  }
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-24 10:28:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1467" class=".btn">#1467</a>
            </td>
            <td>
                <b>
                    feat: openid4vci draft 11 support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                draft PR to update the openid4vci-client implementation to support Draft 11 of the openid4vci specification.

Currently there are some issues with the authorized code flow. Mainly the query parameters are not formatted correctly which should be fixed in the library we are using.

edit: fix for the authorization parameter issue: https://github.com/Sphereon-Opensource/OID4VCI/pull/50

Everything passes now (with my local build of the OIDC4VC library) so we just have to wait for an alpha release or stable.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-24 09:46:30 +0000 UTC
    </div>
</div>

