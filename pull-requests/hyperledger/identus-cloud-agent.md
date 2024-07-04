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
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1248" class=".btn">#1248</a>
            </td>
            <td>
                <b>
                    fix: Wallet Management Error Handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">cloud-agent</span>
            </td>
            <td>
                https://input-output.atlassian.net/browse/ATL-6838
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-04 13:49:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1245" class=".btn">#1245</a>
            </td>
            <td>
                <b>
                    [WIP] Epic VDR phase 3 branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description: 
Epic branch for https://input-output.atlassian.net/browse/ATL-6543

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
        Created At 2024-07-02 14:32:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1240" class=".btn">#1240</a>
            </td>
            <td>
                <b>
                    fix: Move InMemory classes to the test moduels
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">connect</span><span class="chip">cloud-agent</span>
            </td>
            <td>
                ### Description: 
Move InMemory classes to the test moduels

### Checklist: 
- [x] My PR follows the [contribution guidelines](https://github.com/hyperledger/identus-cloud-agent/blob/main/CONTRIBUTING.md) of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [x] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-01 14:21:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1239" class=".btn">#1239</a>
            </td>
            <td>
                <b>
                    build: fix wrongly generated TS client models
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">cloud-agent</span>
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
        Created At 2024-07-01 14:01:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1237" class=".btn">#1237</a>
            </td>
            <td>
                <b>
                    ci: tweak JVM memory limit for release job
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">build</span><span class="chip">infra</span><span class="chip">ci</span><span class="chip">cloud-agent</span>
            </td>
            <td>
                ### Description: 

Increase memory limit because release process has been consistenly failing due to high-pressured GC causing weird issue.

![Screenshot_2024-07-01_14-43-53](https://github.com/hyperledger/identus-cloud-agent/assets/108713642/e3b1bfc0-8102-48d0-a667-839965062475)

![Screenshot_2024-07-01_14-43-35](https://github.com/hyperledger/identus-cloud-agent/assets/108713642/55f5723b-64e0-4707-9d1d-5b19320de959)

![Screenshot_2024-07-01_14-42-54](https://github.com/hyperledger/identus-cloud-agent/assets/108713642/0fd68075-4fae-4ef3-af7d-774ac8b4f850)

The release job run is green https://github.com/hyperledger/identus-cloud-agent/actions/runs/9739373037

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
        Created At 2024-07-01 07:45:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1236" class=".btn">#1236</a>
            </td>
            <td>
                <b>
                    fix: move mocks into the test modules
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">build</span><span class="chip">castor</span><span class="chip">connect</span><span class="chip">cloud-agent</span>
            </td>
            <td>
                ### Description: 
Move mocks classes into the test modules


### Checklist: 
- [x] My PR follows the [contribution guidelines](https://github.com/hyperledger/identus-cloud-agent/blob/main/CONTRIBUTING.md) of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [x] I have commented my code, particularly in hard-to-understand areas
- [x] I have made corresponding changes to the documentation
- [x] I have added tests that prove my fix is effective or that my feature works
- [x] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-28 15:57:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1235" class=".btn">#1235</a>
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
        Created At 2024-06-28 07:58:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1234" class=".btn">#1234</a>
            </td>
            <td>
                <b>
                    test: add oid4vci issuer crud scenario
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">cloud-agent</span>
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
        Created At 2024-06-28 07:55:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1233" class=".btn">#1233</a>
            </td>
            <td>
                <b>
                    fix: avoid name and operationId conflict when creating oas client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">cloud-agent</span>
            </td>
            <td>
                ### Description: 

This fix some issues when generating OAS client as it fails some validation. New client release is required for new oid4vci test scenarios.

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
        Created At 2024-06-28 07:54:24 +0000 UTC
    </div>
</div>

