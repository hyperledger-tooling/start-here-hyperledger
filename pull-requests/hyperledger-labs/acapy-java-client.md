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
                PR <a href="https://github.com/hyperledger-labs/acapy-java-client/pull/16" class=".btn">#16</a>
            </td>
            <td>
                <b>
                    Bump actions/checkout from 2 to 3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [actions/checkout](https://github.com/actions/checkout) from 2 to 3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/checkout/releases">actions/checkout's releases</a>.</em></p>
<blockquote>
<h2>v3.0.0</h2>
<ul>
<li>Update default runtime to node16</li>
</ul>
<h2>v2.4.0</h2>
<ul>
<li>Convert SSH URLs like <code>org-&lt;ORG_ID&gt;@github.com:</code> to <code>https://github.com/</code> - <a href="https://github-redirect.dependabot.com/actions/checkout/pull/621">pr</a></li>
</ul>
<h2>v2.3.5</h2>
<p>Update dependencies</p>
<h2>v2.3.4</h2>
<ul>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/379">Add missing <code>await</code>s</a></li>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/360">Swap to Environment Files</a></li>
</ul>
<h2>v2.3.3</h2>
<ul>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/345">Remove Unneeded commit information from build logs</a></li>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/326">Add Licensed to verify third party dependencies</a></li>
</ul>
<h2>v2.3.2</h2>
<p><a href="https://github-redirect.dependabot.com/actions/checkout/pull/320">Add Third Party License Information to Dist Files</a></p>
<h2>v2.3.1</h2>
<p><a href="https://github-redirect.dependabot.com/actions/checkout/pull/284">Fix default branch resolution for .wiki and when using SSH</a></p>
<h2>v2.3.0</h2>
<p><a href="https://github-redirect.dependabot.com/actions/checkout/pull/278">Fallback to the default branch</a></p>
<h2>v2.2.0</h2>
<p><a href="https://github-redirect.dependabot.com/actions/checkout/pull/258">Fetch all history for all tags and branches when fetch-depth=0</a></p>
<h2>v2.1.1</h2>
<p>Changes to support GHES (<a href="https://github-redirect.dependabot.com/actions/checkout/pull/236">here</a> and <a href="https://github-redirect.dependabot.com/actions/checkout/pull/248">here</a>)</p>
<h2>v2.1.0</h2>
<ul>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/191">Group output</a></li>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/199">Changes to support GHES alpha release</a></li>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/184">Persist core.sshCommand for submodules</a></li>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/163">Add support ssh</a></li>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/179">Convert submodule SSH URL to HTTPS, when not using SSH</a></li>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/157">Add submodule support</a></li>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/144">Follow proxy settings</a></li>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/141">Fix ref for pr closed event when a pr is merged</a></li>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/128">Fix issue checking detached when git less than 2.22</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/actions/checkout/blob/main/CHANGELOG.md">actions/checkout's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<h2>v2.3.1</h2>
<ul>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/284">Fix default branch resolution for .wiki and when using SSH</a></li>
</ul>
<h2>v2.3.0</h2>
<ul>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/278">Fallback to the default branch</a></li>
</ul>
<h2>v2.2.0</h2>
<ul>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/258">Fetch all history for all tags and branches when fetch-depth=0</a></li>
</ul>
<h2>v2.1.1</h2>
<ul>
<li>Changes to support GHES (<a href="https://github-redirect.dependabot.com/actions/checkout/pull/236">here</a> and <a href="https://github-redirect.dependabot.com/actions/checkout/pull/248">here</a>)</li>
</ul>
<h2>v2.1.0</h2>
<ul>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/191">Group output</a></li>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/199">Changes to support GHES alpha release</a></li>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/184">Persist core.sshCommand for submodules</a></li>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/163">Add support ssh</a></li>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/179">Convert submodule SSH URL to HTTPS, when not using SSH</a></li>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/157">Add submodule support</a></li>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/144">Follow proxy settings</a></li>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/141">Fix ref for pr closed event when a pr is merged</a></li>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/128">Fix issue checking detached when git less than 2.22</a></li>
</ul>
<h2>v2.0.0</h2>
<ul>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/108">Do not pass cred on command line</a></li>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/107">Add input persist-credentials</a></li>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/104">Fallback to REST API to download repo</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/checkout/commit/a12a3943b4bdde767164f792f33f40b04645d846"><code>a12a394</code></a> update readme for v3 (<a href="https://github-redirect.dependabot.com/actions/checkout/issues/708">#708</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/8f9e05e482293f862823fcca12d9eddfb3723131"><code>8f9e05e</code></a> Update to node 16 (<a href="https://github-redirect.dependabot.com/actions/checkout/issues/689">#689</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/230611dbd0eb52da1e1f4f7bc8bb0c3a339fc8b7"><code>230611d</code></a> Change secret name for PAT to not start with GITHUB_ (<a href="https://github-redirect.dependabot.com/actions/checkout/issues/623">#623</a>)</li>
<li>See full diff in <a href="https://github.com/actions/checkout/compare/v2...v3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/checkout&package-manager=github_actions&previous-version=2&new-version=3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 14:28:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/acapy-java-client/pull/15" class=".btn">#15</a>
            </td>
            <td>
                <b>
                    minor w3c compatibility fixes
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
        Created At 2022-02-28 11:40:59 +0000 UTC
    </div>
</div>

