---
layout: default
title: identus-cloud-agent
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/identus-cloud-agent
---

# identus-cloud-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/identus-cloud-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1149" class=".btn">#1149</a>
            </td>
            <td>
                <b>
                    docs: updating the hdkey ADR  [skip ci] 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">docs</span>
            </td>
            <td>
                
### Description: 
Updating the ADR to reflect the recent changes in bip32 derivation. 

Mainly, secp256k1 stays the same.
We introduce now HDKeys for Ed25519, those will be using  different bip32 implementation.

The ADR changes are to reflect this but no more changes have been done to the derivationPath specification.

Requires no cloud agent changes as that is already implemented.

### Checklist: 
- [ ] My PR follows the [contribution guidelines](https://github.com/hyperledger/identus-cloud-agent/blob/main/CONTRIBUTING.md) of this project
- [ ] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-06 11:16:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1148" class=".btn">#1148</a>
            </td>
            <td>
                <b>
                    feat: authentication for oid4vci credential and nonce endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">cloud-agent</span>
            </td>
            <td>
                ### Description: 

- Keycloak plugin add access token when getting nonce from the agent
- oid4vci nonce endpoint has authenticator based on `issuer_state`
- oid4vci credential endpoint has authenticator based on `issuer_id`
- Add authorization server `client_id` and `client_secret` option when creating `CredentialIssuer`
- `ExtendedErrorResponse` has correct `Schema`, `Encoder`, and `Decoder`

### Alternatives Considered (optional): 
Link to existing ADR (Architecture Decision Record), if any. If relevant, describe other approaches explored and the selected approach. Documenting why the methods were not selected will create a knowledge base for future reference, helping prevent others from revisiting less optimal ideas.

### Checklist: 
- [ ] My PR follows the [contribution guidelines](https://github.com/hyperledger/identus-cloud-agent/blob/main/CONTRIBUTING.md) of this project
- [ ] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-06 07:43:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1147" class=".btn">#1147</a>
            </td>
            <td>
                <b>
                    ci: revert custom DCO check action [skip ci]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci</span>
            </td>
            <td>
                This reverts commit 7257afc697a09a713ce89954e1256320c46865ea.

### Description: 
Summarize the changes you're submitting in a few sentences, including Jira ticket ATL-xxxx if applicable.
Link to any discussion, related issues and bug reports to give the context to help the reviewer understand the PR.

### Alternatives Considered (optional): 
Link to existing ADR (Architecture Decision Record), if any. If relevant, describe other approaches explored and the selected approach. Documenting why the methods were not selected will create a knowledge base for future reference, helping prevent others from revisiting less optimal ideas.

### Checklist: 
- [ ] My PR follows the [contribution guidelines](https://github.com/hyperledger/identus-cloud-agent/blob/main/CONTRIBUTING.md) of this project
- [ ] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-06 05:37:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1146" class=".btn">#1146</a>
            </td>
            <td>
                <b>
                    style: apply linters automatic fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-05 22:34:55 +0000 UTC
    </div>
</div>

