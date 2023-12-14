---
layout: default
title: acapy-java-client
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/acapy-java-client
---

# acapy-java-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/acapy-java-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/acapy-java-client/pull/93" class=".btn">#93</a>
            </td>
            <td>
                <b>
                    Bump github/codeql-action from 2 to 3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [github/codeql-action](https://github.com/github/codeql-action) from 2 to 3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/github/codeql-action/releases">github/codeql-action's releases</a>.</em></p>
<blockquote>
<h2>CodeQL Bundle v2.15.4</h2>
<p>Bundles CodeQL CLI v2.15.4</p>
<ul>
<li>(<a href="https://github.com/github/codeql-cli-binaries/blob/HEAD/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql-cli-binaries/releases/tag/v2.15.4">release</a>)</li>
</ul>
<p>Includes the following CodeQL language packs from <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4"><code>github/codeql@codeql-cli/v2.15.4</code></a>:</p>
<ul>
<li><code>codeql/cpp-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/cpp/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/cpp/ql/src">source</a>)</li>
<li><code>codeql/cpp-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/cpp/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/cpp/ql/lib">source</a>)</li>
<li><code>codeql/csharp-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/csharp/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/csharp/ql/src">source</a>)</li>
<li><code>codeql/csharp-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/csharp/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/csharp/ql/lib">source</a>)</li>
<li><code>codeql/go-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/go/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/go/ql/src">source</a>)</li>
<li><code>codeql/go-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/go/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/go/ql/lib">source</a>)</li>
<li><code>codeql/java-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/java/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/java/ql/src">source</a>)</li>
<li><code>codeql/java-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/java/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/java/ql/lib">source</a>)</li>
<li><code>codeql/javascript-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/javascript/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/javascript/ql/src">source</a>)</li>
<li><code>codeql/javascript-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/javascript/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/javascript/ql/lib">source</a>)</li>
<li><code>codeql/python-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/python/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/python/ql/src">source</a>)</li>
<li><code>codeql/python-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/python/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/python/ql/lib">source</a>)</li>
<li><code>codeql/ruby-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/ruby/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/ruby/ql/src">source</a>)</li>
<li><code>codeql/ruby-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/ruby/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/ruby/ql/lib">source</a>)</li>
<li><code>codeql/swift-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/swift/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/swift/ql/src">source</a>)</li>
<li><code>codeql/swift-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/swift/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.4/swift/ql/lib">source</a>)</li>
</ul>
<h2>CodeQL Bundle</h2>
<p>Bundles CodeQL CLI v2.15.3</p>
<ul>
<li>(<a href="https://github.com/github/codeql-cli-binaries/blob/HEAD/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql-cli-binaries/releases/tag/v2.15.3">release</a>)</li>
</ul>
<p>Includes the following CodeQL language packs from <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3"><code>github/codeql@codeql-cli/v2.15.3</code></a>:</p>
<ul>
<li><code>codeql/cpp-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/cpp/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/cpp/ql/src">source</a>)</li>
<li><code>codeql/cpp-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/cpp/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/cpp/ql/lib">source</a>)</li>
<li><code>codeql/csharp-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/csharp/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/csharp/ql/src">source</a>)</li>
<li><code>codeql/csharp-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/csharp/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/csharp/ql/lib">source</a>)</li>
<li><code>codeql/go-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/go/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/go/ql/src">source</a>)</li>
<li><code>codeql/go-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/go/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/go/ql/lib">source</a>)</li>
<li><code>codeql/java-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/java/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/java/ql/src">source</a>)</li>
<li><code>codeql/java-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/java/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/java/ql/lib">source</a>)</li>
<li><code>codeql/javascript-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/javascript/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/javascript/ql/src">source</a>)</li>
<li><code>codeql/javascript-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/javascript/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/javascript/ql/lib">source</a>)</li>
<li><code>codeql/python-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/python/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/python/ql/src">source</a>)</li>
<li><code>codeql/python-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/python/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/python/ql/lib">source</a>)</li>
<li><code>codeql/ruby-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/ruby/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/ruby/ql/src">source</a>)</li>
<li><code>codeql/ruby-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/ruby/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/ruby/ql/lib">source</a>)</li>
<li><code>codeql/swift-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/swift/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/swift/ql/src">source</a>)</li>
<li><code>codeql/swift-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/swift/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.3/swift/ql/lib">source</a>)</li>
</ul>
<h2>CodeQL Bundle</h2>
<p>Bundles CodeQL CLI v2.15.2</p>
<ul>
<li>(<a href="https://github.com/github/codeql-cli-binaries/blob/HEAD/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql-cli-binaries/releases/tag/v2.15.2">release</a>)</li>
</ul>
<p>Includes the following CodeQL language packs from <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.2"><code>github/codeql@codeql-cli/v2.15.2</code></a>:</p>
<ul>
<li><code>codeql/cpp-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.2/cpp/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.15.2/cpp/ql/src">source</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/github/codeql-action/blob/main/CHANGELOG.md">github/codeql-action's changelog</a>.</em></p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/github/codeql-action/commit/3a9f6a89e06fb331ce22481637d19617501a5b7f"><code>3a9f6a8</code></a> update javascript files</li>
<li><a href="https://github.com/github/codeql-action/commit/cc4fead714532424ab15b501a01d18c7f34d17e2"><code>cc4fead</code></a> update version in various hardcoded locations</li>
<li><a href="https://github.com/github/codeql-action/commit/183559cea87c163bb01e99e0a15fd5500b23307f"><code>183559c</code></a> Merge branch 'main' into update-bundle/codeql-bundle-v2.15.4</li>
<li><a href="https://github.com/github/codeql-action/commit/5b52b36d41451ee775917788e3bf225d7c1ceab3"><code>5b52b36</code></a> reintroduce PR check that confirm action can be still be compiled on node16</li>
<li><a href="https://github.com/github/codeql-action/commit/5b19bef41e08b00f3d8f48219f46b1866a4f940d"><code>5b19bef</code></a> change to node20 for all actions</li>
<li><a href="https://github.com/github/codeql-action/commit/f2d0c2e7ae58b70f81b81bf4c8b5c7a81fb2a5d6"><code>f2d0c2e</code></a> upgrade node type definitions</li>
<li><a href="https://github.com/github/codeql-action/commit/d651fbc494fab13836ab76ffcfc8ce08c7c98d78"><code>d651fbc</code></a> change to node20 for all actions</li>
<li><a href="https://github.com/github/codeql-action/commit/382a50a0284c0de445104889a9d6003acb4b3c1d"><code>382a50a</code></a> Merge pull request <a href="https://redirect.github.com/github/codeql-action/issues/2021">#2021</a> from github/mergeback/v2.22.9-to-main-c0d1daa7</li>
<li><a href="https://github.com/github/codeql-action/commit/458b4226ad8e38f90ff6a4ad1e18ab2593e7e3dc"><code>458b422</code></a> Update checked-in dependencies</li>
<li><a href="https://github.com/github/codeql-action/commit/5e0f9dbc48f564b68392e465dcdacd74eab63e25"><code>5e0f9db</code></a> Update changelog and version after v2.22.9</li>
<li>See full diff in <a href="https://github.com/github/codeql-action/compare/v2...v3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github/codeql-action&package-manager=github_actions&previous-version=2&new-version=3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-14 14:28:10 +0000 UTC
    </div>
</div>

