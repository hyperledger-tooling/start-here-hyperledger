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
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1138" class=".btn">#1138</a>
            </td>
            <td>
                <b>
                    fix: Schema Error Handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">cloud-agent</span>
            </td>
            <td>
                https://input-output.atlassian.net/browse/ATL-6828
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-04 19:56:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1135" class=".btn">#1135</a>
            </td>
            <td>
                <b>
                    style: remove unused imports
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">cloud-agent</span>
            </td>
            <td>
                ### Description: 
Remove unused imports

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
        Created At 2024-06-03 14:18:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1134" class=".btn">#1134</a>
            </td>
            <td>
                <b>
                    style: remove deprecated Scala syntax
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">build</span><span class="chip">shared</span><span class="chip">mercury</span><span class="chip">castor</span><span class="chip">connect</span><span class="chip">cloud-agent</span>
            </td>
            <td>
                ### Description: 
this Scala syntax is deprecated and we are not able to upgrade the Scala version until stop using this  syntax


### Checklist: 
- [ ] My PR follows the [contribution guidelines](https://github.com/hyperledger/identus-cloud-agent/blob/main/CONTRIBUTING.md) of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [x] I have added tests that prove my fix is effective or that my feature works
- [x] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-03 12:00:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1133" class=".btn">#1133</a>
            </td>
            <td>
                <b>
                    feat: improve ZIO failures and defects in credential definition
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">cloud-agent</span>
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
        Created At 2024-06-03 11:53:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1132" class=".btn">#1132</a>
            </td>
            <td>
                <b>
                    fix: Add expiration time for cloud-agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">cloud-agent</span>
            </td>
            <td>
                ### Description: 
This PR allows the expiration time for the Agent (Role Issuer) to be configurable.
The expiration time for SD JWT credentials can also be set when the Issuer makes a credential offer, including other claims in the exp field.
If the exp field is present, its value takes precedence over the configurable value.
The value in the exp field must be specified in Unix epoch seconds.
For more details, refer to [RFC 7519](https://datatracker.ietf.org/doc/html/rfc7519#page-9).

 "claims": {
       ......
        "exp" : 1618244393 
    }


### Checklist: 
- [x] My PR follows the [contribution guidelines](https://github.com/hyperledger/identus-cloud-agent/blob/main/CONTRIBUTING.md) of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [x] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-03 11:30:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1131" class=".btn">#1131</a>
            </td>
            <td>
                <b>
                    fix: make oidc local script work
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
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
        Created At 2024-06-03 11:14:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1130" class=".btn">#1130</a>
            </td>
            <td>
                <b>
                    feat: improve OpenAPI's PresentProof to make more consistent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">cloud-agent</span>
            </td>
            <td>
                ### Description: 
Improve OpenAPI's PresentProof to make more consistent and add missing examples

Current is like https://staging-docs.atalaprism.io/agent-api/#tag/Present-Proof/operation/getAllPresentation

ATL-6373

![2024-06-03-11_59_42](https://github.com/hyperledger/identus-cloud-agent/assets/4622245/e28ebd9f-86fe-4b7b-bdb4-dc3709c663f2)
![2024-06-03-11_59_37](https://github.com/hyperledger/identus-cloud-agent/assets/4622245/fdd37bb7-0cd6-4628-b748-8fc6ae8712d3)
![2024-06-03-11_59_51](https://github.com/hyperledger/identus-cloud-agent/assets/4622245/0bfe6883-81c1-4304-9e09-e4406928dd40)

On the last image the output should look like json

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
        Created At 2024-06-03 11:05:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1129" class=".btn">#1129</a>
            </td>
            <td>
                <b>
                    fix: Changing .chart.name reference, adding name override
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">infra</span>
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
        Created At 2024-06-03 10:12:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1128" class=".btn">#1128</a>
            </td>
            <td>
                <b>
                    docs(agent): Regenerate PNG images from updated PUML files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">docs</span>
            </td>
            <td>
                ### Description: 
ATL-7050: Regenerate PNG images from updated PUML files

### Checklist: 
- [x] My PR follows the [contribution guidelines](https://github.com/hyperledger/identus-cloud-agent/blob/main/CONTRIBUTING.md) of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [x] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-03 08:32:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1127" class=".btn">#1127</a>
            </td>
            <td>
                <b>
                    feat: add support for EcdsaSecp256k1Signature2019Proof and fix pk encoding for EddsaJcs2022Proof
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">build</span><span class="chip">shared</span><span class="chip">cloud-agent</span>
            </td>
            <td>
                ### Description: 
DO NOT MERGE THIS YET
### Alternatives Considered (optional): 

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
        Created At 2024-06-02 01:17:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1126" class=".btn">#1126</a>
            </td>
            <td>
                <b>
                    build: internal dependency updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">build</span><span class="chip">shared</span><span class="chip">cloud-agent</span>
            </td>
            <td>
                ## About this PR
Updates:

* 📦 [io.iohk.atala.prism.apollo:apollo-jvm](https://github.com/input-output-hk/atala-prism-apollo) from `1.2.16` to `1.3.4`
  + 📜 [GitHub Release Notes](https://github.com/input-output-hk/atala-prism-apollo/releases/tag/v1.3.4) - [Version Diff](https://github.com/input-output-hk/atala-prism-apollo/compare/v1.2.16...v1.3.4)

## Usage
✅ **Please merge!**

I'll automatically update this PR to resolve conflicts as long as you don't change it yourself.

If you have any feedback, just mention me in the comments below.

Configure Scala Steward for your repository with a [`.scala-steward.conf`](https://github.com/scala-steward-org/scala-steward/blob/767fcfecbfd53c507152f6cf15c846176bae561d/docs/repo-specific-configuration.md) file.

_Have a fantastic day writing Scala!_

<details>
<summary>🔍 Files still referring to the old version numbers</summary>

The following files still refer to the old version numbers.
You might want to review and update them manually.
```
DEPENDENCIES.md
```
</details>
<details>
<summary>⚙ Adjust future updates</summary>

Add these to your `.scala-steward.conf` file to ignore future updates of these dependencies:
```
updates.ignore = [
  { groupId = "io.iohk.atala.prism.apollo", artifactId = "apollo-jvm" }
]
```
Or, add these to slow down future updates of these dependencies:
```
dependencyOverrides = [
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "io.iohk.atala.prism.apollo", artifactId = "apollo-jvm" }
  }
]
```
</details>

<sup>
labels: library-update, early-semver-minor, semver-spec-minor, old-version-remains, commit-count:1
</sup>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-02 00:18:18 +0000 UTC
    </div>
</div>

