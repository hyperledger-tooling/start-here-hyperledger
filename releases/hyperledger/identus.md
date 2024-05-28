---
layout: default
title: identus
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/identus
---

# identus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/identus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Identus v2.12
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v2.12
                </span>
            </td>
            <td>
                April, 2024 release of Identus

*Note: Atala PRISM is renamed as Identus from now on. Ongoing renaming is impacting all the repositories and is planned to be completed by the next release.*
- *Open Enterprise Agent --> Cloud Agent*
- *PRISM Mediator --> Mediator*
- *Wallet SDK Typescript/Swift/KMM --> Edge Agent SDK Typescript/Swift/KMM*

## Components

### Platform

* [Cloud Agent v1.33.0](https://github.com/hyperledger-labs/open-enterprise-agent/releases/tag/cloud-agent-v1.33.0)
* [PRISM Node v2.2.1](https://github.com/input-output-hk/atala-prism/releases/tag/v2.2.1)
* [Mediator v0.14.2](https://github.com/input-output-hk/atala-prism-mediator/releases/tag/prism-mediator-v0.14.2)

### SDKs

* [Apollo Crypto Library v1.2.14](https://github.com/input-output-hk/atala-prism-apollo/releases/tag/v1.2.14)
* [Edge Agent SDK Swift v6.0.0](https://github.com/input-output-hk/atala-prism-wallet-sdk-swift/releases/tag/6.0.0)
* [Edge Agent SDK TypeScript v5.1.0](https://github.com/input-output-hk/atala-prism-wallet-sdk-ts/releases/tag/v5.1.0)
* [Edge Agent SDK KMM v3.0.0](https://github.com/input-output-hk/atala-prism-wallet-sdk-kmm/releases/tag/v3.0.0)

### Documentation

* [Documentation Portal v1.92.0](https://github.com/input-output-hk/atala-prism-docs/releases/tag/v1.92.0)

## Changelog

**Updated components:**

| Component             | From    | To        |
| --------------------- | ------- | --------- |
| Documentation Portal  | v1.85.1 | v1.92.0   |
| Cloud Agent           | v1.31.0 | v1.33.0   |
| Mediator              | v0.14.1 | v0.14.2   |
| PRISM Node            | v2.2.1  | no change |
| Edge Agent SDK KMM    | v3.0.0  | no change |
| Edge Agent SDK TypeScript | v5.0.0  | v5.1.0    |
| Edge Agent SDK Swift      | v5.0.0  | v6.0.0    |
| Apollo Crypto Library | v1.2.12 | v1.2.14   |


### Cloud Agent
#### New features
- First iteration of renaming PRISM Agent to Cloud Agent within Identus project
- Use ZIO Failures and Defects effectively + RFC-9457 in connect
- Verification API for Verifiable Credentials
- Support Ed25519 and X25519 key type of managed DID via curve parameter when managing DID using REST interface

#### Bug fixes 
- Check purpose of the keys and fix the fact that issuers DID without purpose `assertionMethod` can issue VC and API does not fail although logs show failure under the hood
- Add shared-crypto module and apollo wrapper for other key types
- Use Apollo for secp256k1 in shared-crypto
- Add missing `PresentationVerificationFailed` status
- Expose pg_admin port on the localhost interface only
- Remove prism-crypto dependency
- Update Open-api-spec and Generator script to use new Identus naming

### Mediator
#### New features
- Set the field `live_delivery` in the [status message](https://didcomm.org/messagepickup/3.0/status)
#### Bug fixes 
- Update some libraries dependencies versions

### Documentation Portal
- Update the Agent API to Cloud Agent v1.33.0 version

### Edge Agent SDK Typescript
#### Breaking changes
- JWTVerifiable Credential: `fromJWT` has been replaced by `fromJWS`.
- Agent Credentials: This class' constructor has changed and it is now requiring an instance of Mercury and DID higher functions.
*Most implementations will not be affected by this breaking change but could be in more advanced implementations*.
- Presentation Request: The type field in the constructor now needs to be called with enum AttachmentFormats instead of CredentialType, making a clear gap between didcomm message format types and credential types.

#### New features
- Updating Anoncreds to IO fork
- Implementing JWT Credential revocation notification
- Add coveralls
- Implementing [Diff presentation exchange protocol v2.0](https://identity.foundation/presentation-exchange/spec/v2.0.0) for SDK to SDK OOB verification. This introduced breaking change.
- Renaming instances of `PRISM Agent` to `Identus`; `Wallet SDK` to `Edge Agent`. Basically, `PRISM` reference will be replaced.

#### Bug fixes 
- `ConnectionManager` emit Messages
- `Agent.createNewPrismDID` was not returning unique DIDs on consecutive calls
- Database cannot be created twice with the same name which crashes demos
- Disabling Mediator live mode by default
- Add compliant dates not in ms, but in seconds


### Edge Agent SDK KMM
- *NOTE:* There are no change on SDK for this release
- Zero-knowledge proof presentation still *NOT* working, [issue](https://github.com/input-output-hk/atala-prism-wallet-sdk-kmm/issues/146)


### Edge Agent SDK Swift
#### Breaking changes
- ProofTypes was replaced by ClaimFilter
#### New features
- Add JWT and Anoncreds verification
- It adds a new utility method to Castor to retrieve all public keys from a DID

#### Bug fixes 
- PRISM DID resolution now correctly resolves all public keys

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/identus/releases/tag/v2.12" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-04-26 05:42:32 +0000 UTC
    </span>
</div>

