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
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1271" class=".btn">#1271</a>
            </td>
            <td>
                <b>
                    fix: changed IO to UIO as as underline repository doesn't throw error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">cloud-agent</span>
            </td>
            <td>
                ### Description: 
PresentationRepository update updateAfterFail doesn't throw error, Chnaged IO to UIO


### Checklist: 
- [ ] My PR follows the [contribution guidelines](https://github.com/hyperledger/identus-cloud-agent/blob/main/CONTRIBUTING.md) of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-22 10:53:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1270" class=".btn">#1270</a>
            </td>
            <td>
                <b>
                    fix: rename folder from atala to identus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">shared</span>
            </td>
            <td>
                ### Description: 
Rename the folder from atala to identus

### Checklist: 
- [x] My PR follows the [contribution guidelines](https://github.com/hyperledger/identus-cloud-agent/blob/main/CONTRIBUTING.md) of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-22 08:54:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1269" class=".btn">#1269</a>
            </td>
            <td>
                <b>
                    ci: do not use default token for autoupdate CI job [skip ci]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci</span>
            </td>
            <td>
                ### Description: 

Any PR with `autoupdate` label gets the merge from `main` by the default `GITHUB_TOKEN` [will not trigger another workflow](https://docs.github.com/en/actions/using-workflows/triggering-a-workflow#triggering-a-workflow-from-a-workflow).

However, this requires `IDENTUS_CI` to have these permissions

![Screenshot_2024-07-19_16-32-21](https://github.com/user-attachments/assets/fb362e1c-0e8c-48d6-b24b-67623f42a532)


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
        Created At 2024-07-19 09:33:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1267" class=".btn">#1267</a>
            </td>
            <td>
                <b>
                    feat: add implementation for DID url resolver
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">shared</span>
            </td>
            <td>
                ### Description: 
Add DID url resolver

### Alternatives Considered (optional): 
Link to existing ADR (Architecture Decision Record), if any. If relevant, describe other approaches explored and the selected approach. Documenting why the methods were not selected will create a knowledge base for future reference, helping prevent others from revisiting less optimal ideas.

### Checklist: 
- [x] My PR follows the [contribution guidelines](https://github.com/hyperledger/identus-cloud-agent/blob/main/CONTRIBUTING.md) of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [x] I have added tests that prove my fix is effective or that my feature works
- [ ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-18 20:45:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1266" class=".btn">#1266</a>
            </td>
            <td>
                <b>
                    style: apply linters automatic fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">docs</span>
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-16 12:19:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1265" class=".btn">#1265</a>
            </td>
            <td>
                <b>
                    docs: oid4vci example and docs [skip ci]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">docs</span><span class="chip">autoupdate</span>
            </td>
            <td>
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
        Created At 2024-07-16 10:38:08 +0000 UTC
    </div>
</div>

