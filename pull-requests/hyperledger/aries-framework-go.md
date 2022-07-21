---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3285" class=".btn">#3285</a>
            </td>
            <td>
                <b>
                    chore(deps): bump terser from 4.8.0 to 4.8.1 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [terser](https://github.com/terser/terser) from 4.8.0 to 4.8.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/terser/terser/blob/master/CHANGELOG.md">terser's changelog</a>.</em></p>
<blockquote>
<h2>v4.8.1 (backport)</h2>
<ul>
<li>Security fix for RegExps that should not be evaluated (regexp DDOS)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/terser/terser/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=terser&package-manager=npm_and_yarn&previous-version=4.8.0&new-version=4.8.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-go/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 20:50:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3284" class=".btn">#3284</a>
            </td>
            <td>
                <b>
                    feat: Size computation for allocation may overflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Performing calculations involving the size of potentially large strings or slices can result in an overflow (for signed integer types) or a wraparound (for unsigned types). An overflow causes the result of the calculation to become negative, while a wraparound results in a small (positive) number.

This can cause further issues. If, for example, the result is then used in an allocation, it will cause a runtime panic if it is negative, and allocate an unexpectedly small buffer otherwise.

Signed-off-by: Bhaskar <ram@hacker.ind.in>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 16:13:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3283" class=".btn">#3283</a>
            </td>
            <td>
                <b>
                    chore(deps): bump actions/upload-artifact from 2 to 3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/upload-artifact](https://github.com/actions/upload-artifact) from 2 to 3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/upload-artifact/releases">actions/upload-artifact's releases</a>.</em></p>
<blockquote>
<h2>v3.0.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Update default runtime to node16 (<a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/293">#293</a>)</li>
<li>Update package-lock.json file version to 2 (<a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/302">#302</a>)</li>
</ul>
<h3>Breaking Changes</h3>
<p>With the update to Node 16, all scripts will now be run with Node 16 rather than Node 12.</p>
<h2>v2.3.1</h2>
<p>Fix for empty fails on Windows failing on upload <a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/281">#281</a></p>
<h2>v2.3.0 Upload Artifact</h2>
<ul>
<li>Optimizations for faster uploads of larger files that are already compressed</li>
<li>Significantly improved logging when there are chunked uploads</li>
<li>Clarifications in logs around the upload size and prohibited characters that aren't allowed in the artifact name or any uploaded files</li>
<li>Various other small bugfixes &amp; optimizations</li>
</ul>
<h2>v2.2.4</h2>
<ul>
<li>Retry on HTTP 500 responses from the service</li>
</ul>
<h2>v2.2.3</h2>
<ul>
<li>Fixes for proxy related issues</li>
</ul>
<h2>v2.2.2</h2>
<ul>
<li>Improved retryability and error handling</li>
</ul>
<h2>v2.2.1</h2>
<ul>
<li>Update used actions/core package to the latest version</li>
</ul>
<h2>v2.2.0</h2>
<ul>
<li>Support for artifact retention</li>
</ul>
<h2>v2.1.4</h2>
<ul>
<li>Add Third Party License Information</li>
</ul>
<h2>v2.1.3</h2>
<ul>
<li>Use updated version of the <code>@action/artifact</code> NPM package</li>
</ul>
<h2>v2.1.2</h2>
<ul>
<li>Increase upload chunk size from 4MB to 8MB</li>
<li>Detect case insensitive file uploads</li>
</ul>
<h2>v2.1.1</h2>
<ul>
<li>Fix for certain symlinks not correctly being identified as directories before starting uploads</li>
</ul>
<h2>v2.1.0</h2>
<ul>
<li>Support for uploading artifacts with multiple paths</li>
<li>Support for using exclude paths</li>
<li>Updates to dependencies</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/upload-artifact/commit/3cea5372237819ed00197afe530f5a7ea3e805c8"><code>3cea537</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/327">#327</a> from actions/robherley/artifact-1.1.0</li>
<li><a href="https://github.com/actions/upload-artifact/commit/849aa7758a428ee22be38de371b49c8bd57c4b9d"><code>849aa77</code></a> nvm use 12 &amp; npm run release</li>
<li><a href="https://github.com/actions/upload-artifact/commit/4d3986961d0423ba9a593efb490a2960eb65f43b"><code>4d39869</code></a> recompile with correct ncc version</li>
<li><a href="https://github.com/actions/upload-artifact/commit/2e0d362ec5cf81e334dda822c49c96dcd4b7df2c"><code>2e0d362</code></a> bump <code>@​actions/artifact</code> to 1.1.0</li>
<li><a href="https://github.com/actions/upload-artifact/commit/09a5d6a283da3e7c9f3253a5d4cdab2347712a66"><code>09a5d6a</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/320">#320</a> from actions/dependabot/npm_and_yarn/ansi-regex-4.1.1</li>
<li><a href="https://github.com/actions/upload-artifact/commit/189315d9106f43a2a8eb60836608bb96b1f69d77"><code>189315d</code></a> Bump ansi-regex from 4.1.0 to 4.1.1</li>
<li><a href="https://github.com/actions/upload-artifact/commit/d159c2d80bf32e77611286e4d71bfe6d15208d88"><code>d159c2d</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/297">#297</a> from actions/dependabot/npm_and_yarn/ajv-6.12.6</li>
<li><a href="https://github.com/actions/upload-artifact/commit/c26a7ba4b5dbaecea906fec3b7d2c0c86f1ccaba"><code>c26a7ba</code></a> Bump ajv from 6.11.0 to 6.12.6</li>
<li><a href="https://github.com/actions/upload-artifact/commit/6ed6c729229a623bcb1fdd75903dc6e436b3d0a7"><code>6ed6c72</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/303">#303</a> from actions/dependabot/npm_and_yarn/yargs-parser-13.1.2</li>
<li><a href="https://github.com/actions/upload-artifact/commit/2aeee267b2cb1f938c861a763b9770ee6e921dc3"><code>2aeee26</code></a> Bump yargs-parser from 13.1.1 to 13.1.2</li>
<li>Additional commits viewable in <a href="https://github.com/actions/upload-artifact/compare/v2...v3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/upload-artifact&package-manager=github_actions&previous-version=2&new-version=3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-07-19 14:53:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3282" class=".btn">#3282</a>
            </td>
            <td>
                <b>
                    chore(deps): bump actions/checkout from 2 to 3
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
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-19 04:33:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3278" class=".btn">#3278</a>
            </td>
            <td>
                <b>
                    chore(deps): bump actions/setup-node from 2.4.0 to 3.4.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/setup-node](https://github.com/actions/setup-node) from 2.4.0 to 3.4.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/setup-node/releases">actions/setup-node's releases</a>.</em></p>
<blockquote>
<h2>Fix pnpm output and node-version  output issues</h2>
<p>In scope of this release we fixed bugs related to the pnpm 7.5.1 output issue from <code>pnpm store path</code> <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/545">actions/setup-node#545</a>. Moreover we fixed the issue with falling on node-version output <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/540">actions/setup-node#540</a>.</p>
<h2>Add support for asdf format and update actions/cache version to 3.0.0</h2>
<p>In scope of this release we updated <code>actions/cache</code> package as the new version contains fixes for <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/526">caching error handling</a>. Moreover, we added support for asdf format as Node.js version file <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/373">actions/setup-node#373</a>. Besides, we introduced new output <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/534">node-version</a> and added <code>npm-shrinkwrap.json</code> to dependency file patterns: <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/439">actions/setup-node#439</a></p>
<h2>Add support for lts/-n aliases</h2>
<p>In scope of this release we added support for <code>lts/-n</code> aliases, improve logic for <code>current</code>, <code>latest</code> and <code>node</code> aliases to handle them from <code>toolcache</code>, update <code>ncc</code> package.</p>
<h3>Support of lts/-n aliases</h3>
<ul>
<li>Related pull request: <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/481">actions/setup-node#481</a></li>
<li>Related issue: <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/26">actions/setup-node#26</a></li>
</ul>
<pre lang="yaml"><code>steps:
- uses: actions/checkout@v3
- uses: actions/setup-node@v3
  with:
    node-version: lts/-1
- run: npm ci
- run: npm test
</code></pre>
<h3>Minor improvements</h3>
<ul>
<li>Update zeit/ncc to vercel/ncc: <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/476">actions/setup-node#476</a></li>
<li>Get latest version from cache if exists: <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/496">actions/setup-node#496</a></li>
</ul>
<h2>Add current, node, latest aliases</h2>
<p>In scope of this release we added new aliases to install the latest Node.js version. <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/483">actions/setup-node#483</a></p>
<pre lang="yml"><code>steps:
- uses: actions/checkout@v3
- uses: actions/setup-node@v3
  with:
    node-version: current
- run: npm ci
- run: npm test
</code></pre>
<h2>Update actions/cache version to 2.0.2</h2>
<p>In scope of this release we updated <code>actions/cache</code> package as the new version contains fixes related to GHES 3.5 (<a href="https://github-redirect.dependabot.com/actions/setup-node/pull/460">actions/setup-node#460</a>)</p>
<h2>Add caching support on GHES 3.5</h2>
<p>In scope of this release we added <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/452">support for caching from GHES 3.5</a> and fixed download issue for files &gt; 2GB during restore. Besides, we updated <code>actions/cache</code> dependency to 2.0.0 version.</p>
<h2>v3.0.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/setup-node/commit/2fddd8803e2f5c9604345a0b591c3020ee971a93"><code>2fddd88</code></a> fixing pnpm output issue (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/545">#545</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/ad8542ca5eddfadd434c12500073d0cfe51ca1c7"><code>ad8542c</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/540">#540</a> from dmitry-shibanov/fix-error-node-version</li>
<li><a href="https://github.com/actions/setup-node/commit/3d11add77113802f5dc907ae13379fa7ffdcd839"><code>3d11add</code></a> remove unused import</li>
<li><a href="https://github.com/actions/setup-node/commit/072a2e3b100f5d9394c602616700b044ce5e72f8"><code>072a2e3</code></a> add trim and silent true</li>
<li><a href="https://github.com/actions/setup-node/commit/28ad38fe0624edc69ffde19aa0a6b8be0573641f"><code>28ad38f</code></a> add try catch</li>
<li><a href="https://github.com/actions/setup-node/commit/48de4c13f6f686eebe0d350838793fffd4421b26"><code>48de4c1</code></a> change to streams</li>
<li><a href="https://github.com/actions/setup-node/commit/aab7cc882a63a6e74f0d36e92552d03d190d4e7e"><code>aab7cc8</code></a> add silent</li>
<li><a href="https://github.com/actions/setup-node/commit/5b949b50c3461bbcd5a540b150c368278160234a"><code>5b949b5</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/373">#373</a> from ganta/add-support-for-asdf-format-as-node-versio...</li>
<li><a href="https://github.com/actions/setup-node/commit/09ba51f18e18a3756fea1f54d09c6745c064491d"><code>09ba51f</code></a> README.md: Encourage testing on current Node.js (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/533">#533</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/b3ca1ac971f58028968bf4f3199547ade2bb277d"><code>b3ca1ac</code></a> Support npm-shrinkwrap.json out-of-the-box (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/439">#439</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/actions/setup-node/compare/v2.4.0...v3.4.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/setup-node&package-manager=github_actions&previous-version=2.4.0&new-version=3.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-07-15 08:16:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3277" class=".btn">#3277</a>
            </td>
            <td>
                <b>
                    feat: add did document support for alsoKnownAs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Chris Abernethy <brownoxford@gmail.com>

**Title:**
Add `alsoKnownAs` support to DID document

**Description:**
Implement support for `alsoKnownAs` DID document element [as described in DID Core v1](https://www.w3.org/TR/did-core/#dfn-alsoknownas)

**Summary:**
Add `AlsoKnownAs` element to `did.Doc` and populate value in `did.ParseDocument()`
Add `AlsoKnownAs` element to `did.rawDoc` and populate value in `did.Doc.JSONBytes()`
Add `did.populateRawAlsoKnownAs()` helper function to convert `alsoKnownAs` from `[]string` to `[]interface{}`
Add `alsoKnownAs` to schemas used for DID Schema Validation


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-14 16:44:41 +0000 UTC
    </div>
</div>

