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
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/928" class=".btn">#928</a>
            </td>
            <td>
                <b>
                    refactor(prism-agent): add metrics to status list background job
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">prism-agent</span><span class="chip">mercury</span>
            </td>
            <td>
                ### Description: 
Summarize the changes you're submitting in a few sentences, including Jira ticket ATL-xxxx if applicable.
Link to any discussion, related issues and bug reports to give the context to help the reviewer understand the PR.

### Alternatives Considered (optional): 
Link to existing ADR (Architecture Decision Record), if any. If relevant, describe other approaches explored and the selected approach. Documenting why the methods were not selected will create a knowledge base for future reference, helping prevent others from revisiting less optimal ideas.

### Checklist: 
- [x] My PR follows the [contribution guidelines](https://github.com/hyperledger-labs/open-enterprise-agent/blob/main/CONTRIBUTING.md) of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [x] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-15 23:52:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/927" class=".btn">#927</a>
            </td>
            <td>
                <b>
                    feat(connect): ATL-6599 Use ZIO Failures and Defects effectively + RFC-9457 in connect
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">prism-agent</span><span class="chip">shared</span><span class="chip">connect</span>
            </td>
            <td>
                ### Description: 
[ATL-6599](https://input-output.atlassian.net/browse/ATL-6599) Implement the following error-handling ADRs for **Connect**:
 - [Use ZIO Failures and Defects Effectively](https://staging-docs.atalaprism.io/adrs/adr/20240116-use-zio-failures-and-defects-effectively/)
 - [Use RFC 9457 for REST API Error Reporting](https://docs.google.com/document/d/1oD4iNTu7jVt2fwrRMB_BfqVXVE3ReL3nIybs8QGMAZI/edit#heading=h.8emnqnl3zhxs)

### Checklist: 
- [] My PR follows the [contribution guidelines](https://github.com/hyperledger-labs/open-enterprise-agent/blob/main/CONTRIBUTING.md) of this project
- [] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [] I have commented my code, particularly in hard-to-understand areas
- [] I have made corresponding changes to the documentation
- [] I have added tests that prove my fix is effective or that my feature works
- [] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-15 18:50:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/926" class=".btn">#926</a>
            </td>
            <td>
                <b>
                    test: fix revocation new variable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">prism-agent</span><span class="chip">infra</span><span class="chip">ci</span>
            </td>
            <td>
                ### Description: 
- Fixes integration tests caused due new hard coded variable
- Bounds default value for `statusListRegistry.publicEndpointUrl` variable to `AGENT_HTTP_PORT`

### Checklist: 
- [ ] My PR follows the [contribution guidelines](https://github.com/hyperledger-labs/open-enterprise-agent/blob/main/CONTRIBUTING.md) of this project
- [ ] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-15 13:07:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/925" class=".btn">#925</a>
            </td>
            <td>
                <b>
                    docs: update code owners
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci</span>
            </td>
            <td>
                ### Description: 
- Code owners: the content editor will be automatically added to any PR related to markdown files
- Code owners: update to the current team
- Pull request template: add the link to the contributing guideline
- Issue template: update an old link

### Checklist: 
- [x] My PR follows the contribution guidelines of this project
- [] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [x] I have commented my code, particularly in hard-to-understand areas
- [x] I have made corresponding changes to the documentation
- [] I have added tests that prove my fix is effective or that my feature works
- [x] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-14 10:42:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/924" class=".btn">#924</a>
            </td>
            <td>
                <b>
                    test: enhancements + vault token test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description: 
Updated integration tests
- Vault token scenario added
- Added gradle tasks for each config available
  - e.g. `./gradlew test_basic`
- Updated ktlint + format (many files changes due that)
 
### Alternatives Considered (optional): 
Link to existing ADR (Architecture Decision Record), if any. If relevant, describe other approaches explored and the selected approach. Documenting why the methods were not selected will create a knowledge base for future reference, helping prevent others from revisiting less optimal ideas.

### Checklist: 
- [ ] My PR follows the contribution guidelines of this project
- [ ] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-11 14:23:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/923" class=".btn">#923</a>
            </td>
            <td>
                <b>
                    fix: add Anoncreds Integration Test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description: 
https://input-output.atlassian.net/browse/ATL-6027

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-11 12:57:13 +0000 UTC
    </div>
</div>

