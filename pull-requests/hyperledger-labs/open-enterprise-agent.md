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
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/937" class=".btn">#937</a>
            </td>
            <td>
                <b>
                    fix(pollux): Undo edit migration for revocation status lists
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span>
            </td>
            <td>
                ### Description: 

This PR undoes the edit of the migration that was introduced in https://github.com/hyperledger-labs/open-enterprise-agent/pull/934,  and instead creates a new migration that archives the same state in the DB. Essentially after introducing this change the state of the database will be the same as previously, but with this change, we are not editing migration that was already applied in the SIT environment, which will make the deployment easier.

P.S The tables that the second migration is editing (which were created by the first migration) will be empty 100%, so there is no need to worry about retaining data in this case.

### Alternatives Considered (optional): 
Alternatively, we can either clean the database on prod and re-run the migrations, or edit the table manually because migration V16 won't run again on prod, since it has already been applied.

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
        Created At 2024-03-19 23:18:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/936" class=".btn">#936</a>
            </td>
            <td>
                <b>
                    fix: align keycloak version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">build</span><span class="chip">infra</span>
            </td>
            <td>
                ### Description: 
Upgrade keycloak version to `23.0.7` to prepare for oidc4vc keycloak plugin. The newest version is `24.0.1`, but it is relatively new and requires migration of some code. (to upgrade after the OIDCVC plugin is merged) 

### Alternatives Considered (optional): 
Link to existing ADR (Architecture Decision Record), if any. If relevant, describe other approaches explored and the selected approach. Documenting why the methods were not selected will create a knowledge base for future reference, helping prevent others from revisiting less optimal ideas.

### Checklist: 
- [x] My PR follows the [contribution guidelines](https://github.com/hyperledger-labs/open-enterprise-agent/blob/main/CONTRIBUTING.md) of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [x] I have added tests that prove my fix is effective or that my feature works
- [x] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-19 09:47:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/935" class=".btn">#935</a>
            </td>
            <td>
                <b>
                    feat: credential offer endpoint and keycloak plugin wip
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">prism-agent</span><span class="chip">build</span><span class="chip">infra</span>
            </td>
            <td>
                ### Description: 
Summarize the changes you're submitting in a few sentences, including Jira ticket ATL-xxxx if applicable.
Link to any discussion, related issues and bug reports to give the context to help the reviewer understand the PR.

### Alternatives Considered (optional): 
Link to existing ADR (Architecture Decision Record), if any. If relevant, describe other approaches explored and the selected approach. Documenting why the methods were not selected will create a knowledge base for future reference, helping prevent others from revisiting less optimal ideas.

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
        Created At 2024-03-19 04:50:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/934" class=".btn">#934</a>
            </td>
            <td>
                <b>
                    feat: add revocation for JWT credentials
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">prism-agent</span><span class="chip">build</span><span class="chip">infra</span><span class="chip">ci</span><span class="chip">shared</span><span class="chip">mercury</span>
            </td>
            <td>
                ### Description: 

Epic: [ATL-4095](https://input-output.atlassian.net/browse/ATL-4095)
This PR (epic) adds all the functionality required to enable JWT revocation. This PR contains files that have been added via other feature PRs that have been reviewed separately.

Content of this PR was copied over from https://github.com/hyperledger-labs/open-enterprise-agent/pull/795

### Checklist: 
- [x] My PR follows the [contribution guidelines](https://github.com/hyperledger-labs/open-enterprise-agent/blob/main/CONTRIBUTING.md) of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [x] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [x] I have added tests that prove my fix is effective or that my feature works
- [x] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-18 17:52:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/931" class=".btn">#931</a>
            </td>
            <td>
                <b>
                    docs: add missing vault env from docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">docs</span>
            </td>
            <td>
                ### Description: 
Summarize the changes you're submitting in a few sentences, including Jira ticket ATL-xxxx if applicable.
Link to any discussion, related issues and bug reports to give the context to help the reviewer understand the PR.

### Alternatives Considered (optional): 
Link to existing ADR (Architecture Decision Record), if any. If relevant, describe other approaches explored and the selected approach. Documenting why the methods were not selected will create a knowledge base for future reference, helping prevent others from revisiting less optimal ideas.

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
        Created At 2024-03-18 05:13:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/929" class=".btn">#929</a>
            </td>
            <td>
                <b>
                    build(deps): bump follow-redirects from 1.15.2 to 1.15.6 in /prism-agent/client/generator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">prism-agent</span><span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [follow-redirects](https://github.com/follow-redirects/follow-redirects) from 1.15.2 to 1.15.6.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/35a517c5861d79dc8bff7db8626013d20b711b06"><code>35a517c</code></a> Release version 1.15.6 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/c4f847f85176991f95ab9c88af63b1294de8649b"><code>c4f847f</code></a> Drop Proxy-Authorization across hosts.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/8526b4a1b2ab3a2e4044299377df623a661caa76"><code>8526b4a</code></a> Use GitHub for disclosure.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/b1677ce00110ee50dc5da576751d39b281fc4944"><code>b1677ce</code></a> Release version 1.15.5 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/d8914f7982403ea096b39bd594a00ee9d3b7e224"><code>d8914f7</code></a> Preserve fragment in responseUrl.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/65858205e59f1e23c9bf173348a7a7cbb8ac47f5"><code>6585820</code></a> Release version 1.15.4 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/7a6567e16dfa9ad18a70bfe91784c28653fbf19d"><code>7a6567e</code></a> Disallow bracketed hostnames.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/05629af696588b90d64e738bc2e809a97a5f92fc"><code>05629af</code></a> Prefer native URL instead of deprecated url.parse.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/1cba8e85fa73f563a439fe460cf028688e4358df"><code>1cba8e8</code></a> Prefer native URL instead of legacy url.resolve.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/72bc2a4229bc18dc9fbd57c60579713e6264cb92"><code>72bc2a4</code></a> Simplify _processResponse error handling.</li>
<li>Additional commits viewable in <a href="https://github.com/follow-redirects/follow-redirects/compare/v1.15.2...v1.15.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=follow-redirects&package-manager=npm_and_yarn&previous-version=1.15.2&new-version=1.15.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

Dependabot will resolve any conflicts with this PR as long as you don't alter it yourself. You can also trigger a rebase manually by commenting `@dependabot rebase`.

[//]: # (dependabot-automerge-start)
[//]: # (dependabot-automerge-end)

---

<details>
<summary>Dependabot commands and options</summary>
<br />

You can trigger Dependabot actions by commenting on this PR:
- `@dependabot rebase` will rebase this PR
- `@dependabot recreate` will recreate this PR, overwriting any edits that have been made to it
- `@dependabot merge` will merge this PR after your CI passes on it
- `@dependabot squash and merge` will squash and merge this PR after your CI passes on it
- `@dependabot cancel merge` will cancel a previously requested merge and block automerging
- `@dependabot reopen` will reopen this PR if it is closed
- `@dependabot close` will close this PR and stop Dependabot recreating it. You can achieve the same result by closing it manually
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/open-enterprise-agent/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-16 14:29:03 +0000 UTC
    </div>
</div>

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
add performance metrics to revocation status list sync job

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

