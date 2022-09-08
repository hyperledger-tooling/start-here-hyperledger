---
layout: default
title: business-partner-agent
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/business-partner-agent
---

# business-partner-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/business-partner-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/823" class=".btn">#823</a>
            </td>
            <td>
                <b>
                    Use same BPA image for all instances in local scenario
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Tim Schlagenhaufer <tim.schlagenhaufer@bosch.io>

Use the same locally built image for both BPAs in the local scenario

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/823"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-08 14:31:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/822" class=".btn">#822</a>
            </td>
            <td>
                <b>
                    Bump actions/checkout from 2 to 3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/checkout](https://github.com/actions/checkout) from 2 to 3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/checkout/releases">actions/checkout's releases</a>.</em></p>
<blockquote>
<h2>v3.0.0</h2>
<ul>
<li>Updated to the node16 runtime by default
<ul>
<li>This requires a minimum <a href="https://github.com/actions/runner/releases/tag/v2.285.0">Actions Runner</a> version of v2.285.0 to run, which is by default available in GHES 3.4 or later.</li>
</ul>
</li>
</ul>
<h2>v2.4.2</h2>
<h2>What's Changed</h2>
<ul>
<li>Add set-safe-directory input to allow customers to take control. (<a href="https://github-redirect.dependabot.com/actions/checkout/issues/770">#770</a>) by <a href="https://github.com/TingluoHuang"><code>@​TingluoHuang</code></a> in <a href="https://github-redirect.dependabot.com/actions/checkout/pull/776">actions/checkout#776</a></li>
<li>Prepare changelog for v2.4.2. by <a href="https://github.com/TingluoHuang"><code>@​TingluoHuang</code></a> in <a href="https://github-redirect.dependabot.com/actions/checkout/pull/778">actions/checkout#778</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/checkout/compare/v2...v2.4.2">https://github.com/actions/checkout/compare/v2...v2.4.2</a></p>
<h2>v2.4.1</h2>
<ul>
<li>Fixed an issue where checkout failed to run in container jobs due to the new git setting <code>safe.directory</code></li>
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
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/actions/checkout/blob/main/CHANGELOG.md">actions/checkout's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<h2>v3.0.2</h2>
<ul>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/770">Add input <code>set-safe-directory</code></a></li>
</ul>
<h2>v3.0.1</h2>
<ul>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/762">Fixed an issue where checkout failed to run in container jobs due to the new git setting <code>safe.directory</code></a></li>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/744">Bumped various npm package versions</a></li>
</ul>
<h2>v3.0.0</h2>
<ul>
<li><a href="https://github-redirect.dependabot.com/actions/checkout/pull/689">Update to node 16</a></li>
</ul>
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
<h2>v2 (beta)</h2>
<ul>
<li>Improved fetch performance</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/checkout/commit/2541b1294d2704b0964813337f33b291d3f8596b"><code>2541b12</code></a> Prepare changelog for v3.0.2. (<a href="https://github-redirect.dependabot.com/actions/checkout/issues/777">#777</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/0ffe6f9c5599e73776da5b7f113e994bc0a76ede"><code>0ffe6f9</code></a> Add set-safe-directory input to allow customers to take control. (<a href="https://github-redirect.dependabot.com/actions/checkout/issues/770">#770</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/dcd71f646680f2efd8db4afa5ad64fdcba30e748"><code>dcd71f6</code></a> Enforce safe directory (<a href="https://github-redirect.dependabot.com/actions/checkout/issues/762">#762</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/add3486cc3b55d4a5e11c8045058cef96538edc7"><code>add3486</code></a> Patch to fix the dependbot alert. (<a href="https://github-redirect.dependabot.com/actions/checkout/issues/744">#744</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/5126516654c75f76bca1de45dd82a3006d8890f9"><code>5126516</code></a> Bump minimist from 1.2.5 to 1.2.6 (<a href="https://github-redirect.dependabot.com/actions/checkout/issues/741">#741</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/d50f8ea76748df49594d9b109b614f3b4db63c71"><code>d50f8ea</code></a> Add v3.0 release information to changelog (<a href="https://github-redirect.dependabot.com/actions/checkout/issues/740">#740</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/2d1c1198e79c30cca5c3957b1e3b65ce95b5356e"><code>2d1c119</code></a> update test workflows to checkout v3 (<a href="https://github-redirect.dependabot.com/actions/checkout/issues/709">#709</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/a12a3943b4bdde767164f792f33f40b04645d846"><code>a12a394</code></a> update readme for v3 (<a href="https://github-redirect.dependabot.com/actions/checkout/issues/708">#708</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/8f9e05e482293f862823fcca12d9eddfb3723131"><code>8f9e05e</code></a> Update to node 16 (<a href="https://github-redirect.dependabot.com/actions/checkout/issues/689">#689</a>)</li>
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

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/822"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-07 13:48:09 +0000 UTC
    </div>
</div>

