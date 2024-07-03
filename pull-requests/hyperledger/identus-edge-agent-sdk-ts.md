---
layout: default
title: identus-edge-agent-sdk-ts
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/identus-edge-agent-sdk-ts
---

# identus-edge-agent-sdk-ts <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/identus-edge-agent-sdk-ts){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/243" class=".btn">#243</a>
            </td>
            <td>
                <b>
                    fix(Castor): createPrismDID and resolveDID key id conflicts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description: 
Multiple fixes around did resolution:

Bug1: Resolving a PrismDID was overwriting the key ids with our own value
  fix: src/castor/resolver/LongFormPrismDIDResolver.ts line 124
    use the `key.id` instead of generating our own with `getUsageId`

Bug2: Creating a PrismDID with multiple `issuing keys` only encodes one, as the key ids conflict.
  fix: src/castor/Castor.ts line 146
    create the `id` from both the `usage` and the `index`

Bug3: JWT verify required the encoded verification methods to be in order with the signing key first, otherwise would fail
  fix: attempt verification with all verification methods, as no way of determining which was used


### Checklist: 
- [ ] My PR follows the [contribution guidelines](https://github.com/input-output-hk/atala-prism-wallet-sdk-ts/blob/master/CONTRIBUTING.md) of this project
- [ ] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-03 11:26:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/242" class=".btn">#242</a>
            </td>
            <td>
                <b>
                    test: add backup e2e scenarios
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description: 
Tests ATL-6609

### Checklist: 
- [x] My PR follows the [contribution guidelines](https://github.com/input-output-hk/atala-prism-wallet-sdk-ts/blob/master/CONTRIBUTING.md) of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [x] I have commented my code, particularly in hard-to-understand areas
- [x] I have made corresponding changes to the documentation
- [x] I have added tests that prove my fix is effective or that my feature works
- [x] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-02 22:50:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/240" class=".btn">#240</a>
            </td>
            <td>
                <b>
                    fix: attachment descriptor parameters
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description: 
While debugging the repeated message from Mediator we found out the cause of it. This PR fixes this long time issue.

Unit tests:
<img width="571" alt="image" src="https://github.com/input-output-hk/atala-prism-wallet-sdk-ts/assets/101114634/aa47c904-bada-4e41-85f9-c8af6999dbf2">

Integration tests:
<img width="599" alt="image" src="https://github.com/input-output-hk/atala-prism-wallet-sdk-ts/assets/101114634/69abb696-3c8b-4c4e-9714-913a0171f824">


### Checklist: 
- [x] My PR follows the [contribution guidelines](https://github.com/input-output-hk/atala-prism-wallet-sdk-ts/blob/master/CONTRIBUTING.md) of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [x] I have commented my code, particularly in hard-to-understand areas
- [x] I have made corresponding changes to the documentation
- [x] I have added tests that prove my fix is effective or that my feature works
- [x] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-28 21:30:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/239" class=".btn">#239</a>
            </td>
            <td>
                <b>
                    fix: attachment encoding fallback base64 + base64url by default
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

### Description: 
Adding base64 and base64url fallback in didcomm attachment extract fn's. earlier we were using Buffer which was able to handle cases where we get base64url and we should be getting base64.

### Checklist: 
- [ ] My PR follows the [contribution guidelines](https://github.com/input-output-hk/atala-prism-wallet-sdk-ts/blob/master/CONTRIBUTING.md) of this project
- [ ] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-28 14:20:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/238" class=".btn">#238</a>
            </td>
            <td>
                <b>
                    test: enable multi sdk actors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description: 
Enables multiple sdk actors for e2e test

### Checklist: 
- [x] My PR follows the [contribution guidelines](https://github.com/input-output-hk/atala-prism-wallet-sdk-ts/blob/master/CONTRIBUTING.md) of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [x] I have commented my code, particularly in hard-to-understand areas
- [x] I have made corresponding changes to the documentation
- [x] I have added tests that prove my fix is effective or that my feature works
- [x] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-27 16:57:55 +0000 UTC
    </div>
</div>

