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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3244" class=".btn">#3244</a>
            </td>
            <td>
                <b>
                    feat: add support of multibase encoding for proofValue.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Volodymyr Kubiv <volodymyr.kubiv@euristiq.com>

**Title:**
Add support of multibase encoding for proofValue.

**Description:**
https://github.com/hyperledger/aries-framework-go/issues/3228

**Summary:**

Add support of multibase encoding for proofValue and update unit tests to reflect this change.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-18 11:56:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3243" class=".btn">#3243</a>
            </td>
            <td>
                <b>
                    chore(deps): bump actions/setup-node from 2.4.0 to 3.2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/setup-node](https://github.com/actions/setup-node) from 2.4.0 to 3.2.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/setup-node/releases">actions/setup-node's releases</a>.</em></p>
<blockquote>
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
<p>In scope of this release we changed version of the runtime Node.js for the setup-node action and updated package-lock.json file to  v2.</p>
<h3>Breaking Changes</h3>
<ul>
<li>With the update to Node 16 in <a href="https://github-redirect.dependabot.com/actions/setup-node/pull/414">actions/setup-node#414</a>, all scripts will now be run with Node 16 rather than Node 12.</li>
<li>We removed deprecated <code>version</code> input (<a href="https://github-redirect.dependabot.com/actions/setup-node/pull/424">actions/setup-node#424</a>). Please use <code>node-version</code> input instead.</li>
</ul>
<h2>Fix logic of error handling for npm warning and uncaught exception</h2>
<p>In scope of this release we fix logic of error handling related to caching (<a href="https://github-redirect.dependabot.com/actions/setup-node/pull/358">actions/setup-node#358</a>) and (<a href="https://github-redirect.dependabot.com/actions/setup-node/pull/359">actions/setup-node#359</a>).</p>
<p>In the previous behaviour we relied on <code>stderr</code> output to throw error. The warning messages from package managers can be written to the stderr's output. For now the action will throw an error only if exit code differs from zero. Besides, we add logic to сatch and log unhandled exceptions.</p>
<h2>Adding Node.js version file support</h2>
<p>In scope of this release we add the <code>node-version-file</code> input and update <code>actions/cache</code> dependency to the latest version.</p>
<h2>Adding Node.js version file support</h2>
<p>The new input (<code>node-version-file</code>) provides functionality to specify the path to the file containing Node.js's version with such behaviour:</p>
<ul>
<li>If the file does not exist the action will throw an error.</li>
<li>If you specify both <code>node-version</code> and <code>node-version-file</code> inputs, the action will use value from the <code>node-version</code> input and throw the following warning: <code>Both node-version and node-version-file inputs are specified, only node-version will be used</code>.</li>
<li>For now the action does not support all of the variety of values for Node.js version files. The action can handle values according to the <a href="https://github.com/actions/setup-node#supported-version-syntax">documentation</a> and values with <code>v</code> prefix (<code>v14</code>)</li>
</ul>
<pre lang="yaml"><code>steps:
  - uses: actions/checkout@v2
  - name: Setup node from node version file
    uses: actions/setup-node@v2
    with:
      node-version-file: '.nvmrc'
  - run: npm install
  - run: npm test
</code></pre>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/setup-node/commit/17f8bd926464a1afa4c6a11669539e9c1ba77048"><code>17f8bd9</code></a> Expand current syntax to support aliases for latest version (current/latest/n...</li>
<li><a href="https://github.com/actions/setup-node/commit/b067f78ed37e8b6503efbf8c2b320b7f1e48369a"><code>b067f78</code></a> Use CI friendly commands in documentation (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/326">#326</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/0bd06765ef0b51db720effb3b27b09a604b36300"><code>0bd0676</code></a> Improve advanced usage docs (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/472">#472</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/25184c4485a7b08d05f0d0a07d714e3611e40d38"><code>25184c4</code></a> Update README.md (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/475">#475</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/337fdf2194d3e87cdd26672305866d19d404fcd3"><code>337fdf2</code></a> fix broken link in readme (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/473">#473</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/86bf502a33df3d7ca5daace2b5d63c9877c85c28"><code>86bf502</code></a> extend documentation on <code>scope</code> parameter (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/470">#470</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/146c4d84a51256d5571b40011b76c0c6f7dfd981"><code>146c4d8</code></a> improve caching documentation (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/468">#468</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/56337c425554a6be30cdef71bf441f15be286854"><code>56337c4</code></a> Updated <code>@​actions/cache</code> (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/460">#460</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/76d3665dc084409ba9e6c467009338cf86e9dd5f"><code>76d3665</code></a> Convert CONDUCT to CODE_OF_CONDUCT.md (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/391">#391</a>)</li>
<li><a href="https://github.com/actions/setup-node/commit/5b52f097d36d4b0b2f94ed6de710023fbb8b2236"><code>5b52f09</code></a> Bump <code>actions/checkout@v3</code> within advanced usage examples documentation (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/456">#456</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/actions/setup-node/compare/v2.4.0...v3.2.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/setup-node&package-manager=github_actions&previous-version=2.4.0&new-version=3.2.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-05-17 08:17:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3242" class=".btn">#3242</a>
            </td>
            <td>
                <b>
                    feat: Add multi-tag support to mem DB
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The mem DB now supports queries with multiple tags using the '&&' operator.

Signed-off-by: Bob Stasyszyn <Bob.Stasyszyn@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-16 14:49:23 +0000 UTC
    </div>
</div>

