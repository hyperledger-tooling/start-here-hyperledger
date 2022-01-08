---
layout: default
title: fabric-sdk-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-java
---

# fabric-sdk-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/184" class=".btn">#184</a>
            </td>
            <td>
                <b>
                    Bump protobuf-java from 3.19.1 to 3.19.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">java</span>
            </td>
            <td>
                Bumps [protobuf-java](https://github.com/protocolbuffers/protobuf) from 3.19.1 to 3.19.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/protocolbuffers/protobuf/releases">protobuf-java's releases</a>.</em></p>
<blockquote>
<h2>Protocol Buffers v3.19.2</h2>
<h1>Python</h1>
<ul>
<li>Fix missing Windows wheel for Python 3.10 on PyPI</li>
</ul>
<h1>Java</h1>
<ul>
<li>Improve performance characteristics of UnknownFieldSet parsing (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/9371">#9371</a>)</li>
<li>This release addresses a <a href="https://github.com/protocolbuffers/protobuf/security/advisories/GHSA-wrvw-hg22-4m67">Security Advisory for Java users</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/cb46755e6405e083b45481f5ea4754b180705529"><code>cb46755</code></a> Tweak wording of CHANGES.txt</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/eb94f17a8b8babc4851fb9bb27f9fb1919fe9cfc"><code>eb94f17</code></a> Update protobuf version</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/ea9a01a0f5c259e9597c199e447d99eaab19930b"><code>ea9a01a</code></a> Update CHANGES.txt for 3.19.2 release</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/9638a5e5315bf73f5e7148c16181676372321892"><code>9638a5e</code></a> Improve performance of parsing unknown fields in Java (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/9371">#9371</a>)</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/0e02f95b876c40ecb04a76e729dd3f0d9185431e"><code>0e02f95</code></a> Fix Ruby release build by pinning rake-compiler-dock version (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/9372">#9372</a>)</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/9057466a7aea0b927f3bf7ab125355be3317d4a0"><code>9057466</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/9336">#9336</a> from acozzette/merge-3.18.x</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/9227f60f85701be60f5a0585a27d0e881ebc84b0"><code>9227f60</code></a> Merge branch '3.18.x' into merge-3.18.x</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/1fe07f9ce2e98ca66a403b989d78a060f3153d5b"><code>1fe07f9</code></a> Cherry-pick fix from <a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/9311">#9311</a> into 3.18.x (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/9320">#9320</a>)</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/cb1f49ae73cf26dd61368f8bd1297e11c62a5f03"><code>cb1f49a</code></a> Cherry-pick Python 3.10 fix to 3.19.x (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/9323">#9323</a>)</li>
<li><a href="https://github.com/protocolbuffers/protobuf/commit/bb5094881c6a496a458cb5d1c939ac4d0e822964"><code>bb50948</code></a> Update python 3.10 install MD5 Sum (<a href="https://github-redirect.dependabot.com/protocolbuffers/protobuf/issues/9322">#9322</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/protocolbuffers/protobuf/compare/v3.19.1...v3.19.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=com.google.protobuf:protobuf-java&package-manager=maven&previous-version=3.19.1&new-version=3.19.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-sdk-java/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-07 22:32:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/183" class=".btn">#183</a>
            </td>
            <td>
                <b>
                    Release v1.4.15
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-04 15:02:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/182" class=".btn">#182</a>
            </td>
            <td>
                <b>
                    Release v2.2.11
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-04 13:56:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/181" class=".btn">#181</a>
            </td>
            <td>
                <b>
                    Update dependencies (release-1.4)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Includes a fix to another security vulnerability (CVE-2021-44832) in Log4j.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-04 13:30:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/180" class=".btn">#180</a>
            </td>
            <td>
                <b>
                    Update dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cherry-pick of 74293f0f9a9198ba634893cf416da27087f4500d from main branch.

Includes a fix to another security vulnerability (CVE-2021-44832) in Log4j.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-04 12:53:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/179" class=".btn">#179</a>
            </td>
            <td>
                <b>
                    Update dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Includes a fix to another security vulnerability (CVE-2021-44832) in Log4j.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-04 10:40:29 +0000 UTC
    </div>
</div>

