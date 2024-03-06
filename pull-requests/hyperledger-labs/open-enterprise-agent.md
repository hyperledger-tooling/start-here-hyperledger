---
layout: default
title: open-enterprise-agent
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/open-enterprise-agent
---

# open-enterprise-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/open-enterprise-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/920" class=".btn">#920</a>
            </td>
            <td>
                <b>
                    feat: Fix Update Schema and CredentialDef on Receive Credential
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">prism-agent</span>
            </td>
            <td>
                ### Description: 
https://input-output.atlassian.net/browse/ATL-6665

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-05 18:05:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/919" class=".btn">#919</a>
            </td>
            <td>
                <b>
                    fix(prism-agent): add validation for endpoint url
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">prism-agent</span>
            </td>
            <td>
                ### Description: 
https://github.com/hyperledger-labs/open-enterprise-agent/issues/859 

### Checklist: 
- [X] My PR follows the contribution guidelines of this project
- [X] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [] I have commented my code, particularly in hard-to-understand areas
- [] I have made corresponding changes to the documentation
- [] I have added tests that prove my fix is effective or that my feature works
- [X] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-05 14:48:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/918" class=".btn">#918</a>
            </td>
            <td>
                <b>
                    fix: allow configurable path convention for vault secrets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">prism-agent</span><span class="chip">docs</span>
            </td>
            <td>
                ### Description: 
Support config `VAULT_USE_SEMANTIC_PATH=false` to opt-out from using meaningful secret path for a fixed-length secret path. The path hierarchy is cut-off at certain depth and replaced by sha256 hash of path relative to the cut-off. The original path is stored in `semanticPath` key of the secret `custom_metadata` 

Fixes https://github.com/hyperledger-labs/open-enterprise-agent/issues/908

### Checklist: 
- [x] My PR follows the contribution guidelines of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [x] I have commented my code, particularly in hard-to-understand areas
- [x] I have made corresponding changes to the documentation
- [x] I have added tests that prove my fix is effective or that my feature works
- [x] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-05 09:51:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/917" class=".btn">#917</a>
            </td>
            <td>
                <b>
                    feat(pollux): check verification status on presentation verification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">prism-agent</span><span class="chip">build</span><span class="chip">shared</span>
            </td>
            <td>
                ### Description: 

Check credential revocation status within present proof flow if status is available, and fail it if one of the credentials is revoked

### Alternatives Considered (optional): 
Link to existing ADR (Architecture Decision Record), if any. If relevant, describe other approaches explored and the selected approach. Documenting why the methods were not selected will create a knowledge base for future reference, helping prevent others from revisiting less optimal ideas.

### Checklist: 
- [x] My PR follows the contribution guidelines of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [x] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [x] I have added tests that prove my fix is effective or that my feature works
- [x] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-04 14:02:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/915" class=".btn">#915</a>
            </td>
            <td>
                <b>
                    fix: integration test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description: 
Fixes Integration test by fixing breaking changes introduce VerificationPolicy api

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-01 16:57:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/914" class=".btn">#914</a>
            </td>
            <td>
                <b>
                    feat(agent): make the connection pool size configurable, fixes #913
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">prism-agent</span>
            </td>
            <td>
                ### Description: 
Make the Postgresql connection pool size configurable and reduce the default number from 8 to 4

### Checklist: 
- [x] My PR follows the contribution guidelines of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [x] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [x] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-01 12:32:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/912" class=".btn">#912</a>
            </td>
            <td>
                <b>
                    docs(prism-agent): 895 update the pr template
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">prism-agent</span><span class="chip">build</span><span class="chip">infra</span><span class="chip">ci</span>
            </td>
            <td>
                ### Description: 
Take the feedback from the team into account to merge context into description to make clearer and simpler the PR.
Remove the spaces in the checklist so it appears as a cross (x) instead of a dot (.).

### Checklist: 
- [x] My PR follows the contribution guidelines of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [] I have commented my code, particularly in hard-to-understand areas
- [] I have made corresponding changes to the documentation
- [] I have added tests that prove my fix is effective or that my feature works
- [x] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-29 12:33:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/910" class=".btn">#910</a>
            </td>
            <td>
                <b>
                    docs: update multi-tenancy.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">docs</span>
            </td>
            <td>
                Fixed environment variable name to enable default entity and wallet.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-28 22:55:30 +0000 UTC
    </div>
</div>

