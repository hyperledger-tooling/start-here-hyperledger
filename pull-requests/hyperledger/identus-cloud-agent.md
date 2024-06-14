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
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1159" class=".btn">#1159</a>
            </td>
            <td>
                <b>
                    build: protobuf dependency update
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

* 📦 [com.thesamet.scalapb:compilerplugin](https://github.com/scalapb/ScalaPB) from `0.11.15` to `0.11.17`
  + 📜 [GitHub Release Notes](https://github.com/scalapb/ScalaPB/releases/tag/v0.11.17) - [Changelog](https://github.com/scalapb/ScalaPB/blob/master/CHANGELOG.md) - [Version Diff](https://github.com/scalapb/ScalaPB/compare/v0.11.15...v0.11.17)
* 📦 [com.thesamet.scalapb:scalapb-runtime-grpc](https://github.com/scalapb/ScalaPB) from `0.11.15` to `0.11.17`
  + 📜 [GitHub Release Notes](https://github.com/scalapb/ScalaPB/releases/tag/v0.11.17) - [Changelog](https://github.com/scalapb/ScalaPB/blob/master/CHANGELOG.md) - [Version Diff](https://github.com/scalapb/ScalaPB/compare/v0.11.15...v0.11.17)

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
  { groupId = "com.thesamet.scalapb", artifactId = "compilerplugin" },
  { groupId = "com.thesamet.scalapb", artifactId = "scalapb-runtime-grpc" }
]
```
Or, add these to slow down future updates of these dependencies:
```
dependencyOverrides = [
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "com.thesamet.scalapb", artifactId = "compilerplugin" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "com.thesamet.scalapb", artifactId = "scalapb-runtime-grpc" }
  }
]
```
</details>

<sup>
labels: library-update, early-semver-minor, semver-spec-patch, version-scheme:early-semver, old-version-remains, commit-count:1
</sup>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-09 00:19:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1158" class=".btn">#1158</a>
            </td>
            <td>
                <b>
                    fix: Update the Holder to send the presentation only, No claims to disclose is needed separately 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">cloud-agent</span>
            </td>
            <td>
                ### Description: 
This change allows the Holder to make a presentation without sending the claims to be disclosed separately. As a result, the DIDComm attachment will only contain the presentation
https://input-output.atlassian.net/browse/ATL-7240
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
        Created At 2024-06-07 13:49:40 +0000 UTC
    </div>
</div>

