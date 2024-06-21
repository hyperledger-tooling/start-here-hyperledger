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
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1192" class=".btn">#1192</a>
            </td>
            <td>
                <b>
                    feat: implement ADR Use ZIO Failures and Defects Effectively - Mercury should not throw exceptions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">mercury</span><span class="chip">cloud-agent</span><span class="chip">autoupdate</span>
            </td>
            <td>
                ### Description: 
Improve Mercury API
Methods should not throw exceptions


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
        Created At 2024-06-17 13:06:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1191" class=".btn">#1191</a>
            </td>
            <td>
                <b>
                    ci: auto merge main into the feature branch [skip ci]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci</span>
            </td>
            <td>
                ### Description: 
- auto merge the main branch into the a feature brach when a pull request is labeled with `autoupdate`. The idea of this improvement is to optimize the work of the engineers: engineer shouldn't keep an eye on the PR and press "Update..." button after each successful merge of another PR into the main branch. The bot will do this work for you.


### Checklist: 
- [x] My PR follows the [contribution guidelines](https://github.com/hyperledger/identus-cloud-agent/blob/main/CONTRIBUTING.md) of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [x] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [x] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 09:32:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1190" class=".btn">#1190</a>
            </td>
            <td>
                <b>
                    fix: KeyID from String to Opaque Type and presentation job cleanup 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">shared</span><span class="chip">cloud-agent</span>
            </td>
            <td>
                ### Description: 
making KeyId type safe and general cleanup of unused functions

### Alternatives Considered (optional): 
Link to existing ADR (Architecture Decision Record), if any. If relevant, describe other approaches explored and the selected approach. Documenting why the methods were not selected will create a knowledge base for future reference, helping prevent others from revisiting less optimal ideas.

### Checklist: 
- [ X] My PR follows the [contribution guidelines](https://github.com/hyperledger/identus-cloud-agent/blob/main/CONTRIBUTING.md) of this project
- [ X] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ X] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-17 08:53:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1189" class=".btn">#1189</a>
            </td>
            <td>
                <b>
                    build: make docker image only for the server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">build</span>
            </td>
            <td>
                ### Description: 
- republish the @FabioPinheiro [PR](https://github.com/hyperledger/identus-cloud-agent/pull/900) with DCO to disable the docker image build for the pollux building block

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
        Created At 2024-06-17 08:22:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1188" class=".btn">#1188</a>
            </td>
            <td>
                <b>
                    build: internal dependency updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">build</span>
            </td>
            <td>
                ## About this PR
Updates:

* 📦 [io.iohk.atala.prism.apollo:apollo-jvm](https://github.com/input-output-hk/atala-prism-apollo) from `1.3.4` to `1.3.5`
  + 📜 [GitHub Release Notes](https://github.com/input-output-hk/atala-prism-apollo/releases/tag/v1.3.5) - [Version Diff](https://github.com/input-output-hk/atala-prism-apollo/compare/v1.3.4...v1.3.5)

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
package-lock.json
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
labels: library-update, early-semver-patch, semver-spec-patch, old-version-remains, commit-count:1
</sup>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-16 00:19:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1187" class=".btn">#1187</a>
            </td>
            <td>
                <b>
                    build: sbt and plugins dependency update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## About this PR
Updates:

* 📦 [org.scalameta:scalafmt-core](https://github.com/scalameta/scalafmt) from `3.8.1` to `3.8.2`
  + 📜 [GitHub Release Notes](https://github.com/scalameta/scalafmt/releases/tag/v3.8.2) - [Version Diff](https://github.com/scalameta/scalafmt/compare/v3.8.1...v3.8.2)

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
build.sbt
```
</details>
<details>
<summary>⚙ Adjust future updates</summary>

Add these to your `.scala-steward.conf` file to ignore future updates of these dependencies:
```
updates.ignore = [
  { groupId = "org.scalameta", artifactId = "scalafmt-core" }
]
```
Or, add these to slow down future updates of these dependencies:
```
dependencyOverrides = [
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "org.scalameta", artifactId = "scalafmt-core" }
  }
]
```
</details>

<sup>
labels: library-update, early-semver-patch, semver-spec-patch, old-version-remains, commit-count:n:3
</sup>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-16 00:19:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1186" class=".btn">#1186</a>
            </td>
            <td>
                <b>
                    feat: ATL-6833 integrate ZIO failures and defects in wallet event controller
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">cloud-agent</span>
            </td>
            <td>
                ### Description: 
[ATL-6833](https://input-output.atlassian.net/browse/ATL-6833)

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
        Created At 2024-06-14 15:32:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1185" class=".btn">#1185</a>
            </td>
            <td>
                <b>
                    feat: SDJWT holder key binding
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">cloud-agent</span>
            </td>
            <td>
                ### Description: 
SDJWT
This feature enables the creation of credentials bound to the holder's key.
Verifiers can now use a challenge and domain to verify the holder's binding to the credential.
If a `keyId`  is provided (an optional field) when the holder accepts the offer, the holder's key will be bound to the credential.
If the `keyId` is not provided, holder key binding is not supported.
During verification request if the domain and challenge is requested, the key binding is necessary to support this flow and key bouded to the credential is used 

### Alternatives Considered (optional): 
Link to existing ADR (Architecture Decision Record), if any. If relevant, describe other approaches explored and the selected approach. Documenting why the methods were not selected will create a knowledge base for future reference, helping prevent others from revisiting less optimal ideas.

### Checklist: 
- [X] My PR follows the [contribution guidelines](https://github.com/hyperledger/identus-cloud-agent/blob/main/CONTRIBUTING.md) of this project
- [X] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [X] I have commented my code, particularly in hard-to-understand areas
- [  ] I have made corresponding changes to the documentation
- [  ] I have added tests that prove my fix is effective or that my feature works
- [  ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-14 12:37:11 +0000 UTC
    </div>
</div>

