---
layout: default
title: identus-edge-agent-sdk-ts
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/identus-edge-agent-sdk-ts
---

# identus-edge-agent-sdk-ts <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/identus-edge-agent-sdk-ts){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v6.0.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v6.0.0
                </span>
            </td>
            <td>
                ## What's Changed
* chore: add required md files by @essbante-io in https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/212


* docs: improve main readme as per feedback we got from community in https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/227
* feat: Backup and Restore https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/215
* feat: Implement sd+jwt for issuance and verification flows with cloud agent in  https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/228
* feat: add sdk jwt revocation verification in https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/231
* docs: backup and sd-jwt  in https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/230
* fix: Message properties body, createdTime, expiresTimePlus in https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/232
* fix: create custom class to verify bitstring position more precisely in https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/234
* fix: add missing files in package to clean rxdb vulnerabilities to fix e2e  in https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/233
* fix: using rust dependency for jwe in https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/235
* fix: e2e issues fix in https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/236
* fix: jwe rust library for backup encryption not including the node wa… in ttps://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/237
* test: enable multi sdk actors  in ttps://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/238
* fix: attachment encoding fallback base64 + base64url by default in https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/239
* test: add backup e2e scenarios in https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/242
* fix(Castor): createPrismDID and resolveDID key id conflicts  in https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/243
* fix: attachment descriptor parameters in https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/240
* fix: add e2e tests for jwt revocation, sdk verification for jwt and anoncreds  in https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/244
* fix: moving to hyperledger namespace in https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/245
* fix: escape the `<->` sequence to fix the build error in the identus-… in https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/248
* chore: use identus apollo in https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/247
* fix: releasing to HL in  https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/253
* fix: remove typo in release pipeline in https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/254
* fix: generate docs after releasing as we cannot access a package that…  in https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/255

BREAKING CHANGE:

- Pollux instance now requires to have Apollo first constructor parameter (used internally)
- Deprecated internal function processJWTCredential, processAnoncredsCredential and extractCredentialFormatFromMessage. Internally, in order to process any type of credential offer just call pollux.processCredentialOffer instead. In order to extract the credentialFormat from a DIDComm message if available, use message.credentialFormat (will return known CredentialType or unknown) In order to extract the payload of whatever DIDComm message, use message.payload which will decode it into the right object instance
- JWT class now needs apollo and castor in constructor as they now instantiate from JWTCore (used internally)
Derivable Private key is not deriving using the derivationPath as a string not the DerivationPath class (used internally)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/identus-edge-agent-sdk-ts/releases/tag/v6.0.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-20 10:51:24 +0000 UTC
    </span>
</div>

