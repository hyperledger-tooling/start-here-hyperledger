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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2887" class=".btn">#2887</a>
            </td>
            <td>
                <b>
                    chore(deps): bump actions/setup-node from 2.2.0 to 2.3.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/setup-node](https://github.com/actions/setup-node) from 2.2.0 to 2.3.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/setup-node/releases">actions/setup-node's releases</a>.</em></p>
<blockquote>
<h2>Support caching pnpm dependencies</h2>
<p>This release introduces dependency caching support for the <code>pnpm</code> package manager (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/278">#278</a>).</p>
<p><strong>Caching pnpm dependencies:</strong></p>
<pre lang="yaml"><code># This workflow uses actions that are not certified by GitHub.
# They are provided by a third-party and are governed by
# separate terms of service, privacy policy, and support
# documentation.
<p>steps:</p>
<ul>
<li>uses: actions/checkout@v2</li>
<li>uses: pnpm/action-setup@646cdf48217256a3d0b80361c5a50727664284f2
with:
version: 6.10.0</li>
<li>uses: actions/setup-node@v2
with:
node-version: '14'
cache: 'pnpm'</li>
<li>run: pnpm install</li>
<li>run: pnpm test
</code></pre></li>
</ul>
<p><strong>NOTE</strong>: pnpm caching support requires pnpm version &gt;= 6.10.0</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/setup-node/commit/aa759c6c94d3800c55b8601f21ba4b2371704cb7"><code>aa759c6</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/278">#278</a> from jacobwgillespie/cache-pnpm</li>
<li><a href="https://github.com/actions/setup-node/commit/0ae03de2b799ae88b378c51b87476d242b3d8ef0"><code>0ae03de</code></a> Reorder to npm, yarn, pnpm</li>
<li><a href="https://github.com/actions/setup-node/commit/4bc87b8e10a7f0f76173ad410d874a0b1f984af0"><code>4bc87b8</code></a> Bump e2e tests to 6.10.0</li>
<li><a href="https://github.com/actions/setup-node/commit/b96348a4e97e0510304e475e5cec7a7a05518c5d"><code>b96348a</code></a> Remove unused imports</li>
<li><a href="https://github.com/actions/setup-node/commit/3af302a4f220de9ff48cd21cc1ab8e9c54382600"><code>3af302a</code></a> Switch to pnpm store path command</li>
<li><a href="https://github.com/actions/setup-node/commit/f452812b440ff2d1b0ee9d300a037464407004e5"><code>f452812</code></a> Unmock fs.existsSync after tests</li>
<li><a href="https://github.com/actions/setup-node/commit/e93556ca6645851a427f77742aeb1b22a95b4700"><code>e93556c</code></a> Mock fs.existsSync in tests</li>
<li><a href="https://github.com/actions/setup-node/commit/0453e516eb2a16fb262fa8f9db51405c7089b869"><code>0453e51</code></a> Regenerate compiled files</li>
<li><a href="https://github.com/actions/setup-node/commit/399982b36805ac9d772a419dc9f95fb5a8eb5c55"><code>399982b</code></a> Move existence check to cache-save</li>
<li><a href="https://github.com/actions/setup-node/commit/d278e78bddf957771f319214444100b4032fb7aa"><code>d278e78</code></a> Add logic to check that cache folder exists</li>
<li>Additional commits viewable in <a href="https://github.com/actions/setup-node/compare/v2.2.0...v2.3.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/setup-node&package-manager=github_actions&previous-version=2.2.0&new-version=2.3.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-07-21 08:18:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2886" class=".btn">#2886</a>
            </td>
            <td>
                <b>
                    chore(deps): bump codecov/codecov-action from 1.5.2 to 2.0.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [codecov/codecov-action](https://github.com/codecov/codecov-action) from 1.5.2 to 2.0.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/codecov/codecov-action/releases">codecov/codecov-action's releases</a>.</em></p>
<blockquote>
<h2>v2.0.1</h2>
<h3>Fixes</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/424">#424</a> fix: Issue in building all deep dependencies</li>
</ul>
<h2>v2.0.0</h2>
<p>On February 1, 2022, the <code>v1</code> uploader will be full sunset and no longer function. This is due
to the deprecation of the underlying bash uploader. This version uses the new <a href="https://github.com/codecov/uploader">uploader</a>.</p>
<p>The <code>v2</code> Action downloads, verifies, and runs the Codecov binary.</p>
<h3>Breaking Changes</h3>
<ul>
<li>Multiple fields have not been transferred from the bash uploader or have been deprecated. Notably
many of the <code>functionalities</code> and <code>gcov_</code> arguments have been removed. Please check the documentation
for the full list.</li>
</ul>
<h3>Features</h3>
<ul>
<li><code>dry-run</code> argument allows Codecov flow without uploading reports to Codecov</li>
<li>(Enterprise only) <code>slug</code> allows specifying the repository slug manually</li>
<li>(Enterprise only) <code>url</code> allows changing the upload host</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/codecov/codecov-action/blob/master/CHANGELOG.md">codecov/codecov-action's changelog</a>.</em></p>
<blockquote>
<h2>2.0.1</h2>
<h3>Fixes</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/424">#424</a> fix: Issue in building all deep dependencies</li>
</ul>
<h2>2.0.0</h2>
<p>On February 1, 2022, the <code>v1</code> uploader will be full sunset and no longer function. This is due
to the deprecation of the underlying bash uploader. This version uses the new <a href="https://github.com/codecov/uploader">uploader</a>.</p>
<p>The <code>v2</code> Action downloads, verifies, and runs the Codecov binary.</p>
<h3>Breaking Changes</h3>
<ul>
<li>Multiple fields have not been transferred from the bash uploader or have been deprecated. Notably
many of the <code>functionalities</code> and <code>gcov_</code> arguments have been removed. Please check the documentation
for the full list.</li>
</ul>
<h3>Features</h3>
<ul>
<li><code>dry-run</code> argument allows Codecov flow without uploading reports to Codecov</li>
<li>(Enterprise only) <code>slug</code> allows specifying the repository slug manually</li>
<li>(Enterprise only) <code>url</code> allows changing the upload host</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/codecov/codecov-action/commit/c585afe366f940d214dc09df2664c06d7fe07052"><code>c585afe</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/424">#424</a> from codecov/2.0.1-fix-deps</li>
<li><a href="https://github.com/codecov/codecov-action/commit/852cffb35272a9ac5682698829e6c01196b1f8ff"><code>852cffb</code></a> Remove dist/coverage</li>
<li><a href="https://github.com/codecov/codecov-action/commit/d910efb490cda059c2dc38ad33440fb2cbc1714a"><code>d910efb</code></a> Update CHANGELOG</li>
<li><a href="https://github.com/codecov/codecov-action/commit/439c1e508e4c29bd3921d5f6b25df65ccf129116"><code>439c1e5</code></a> Remove coverage folder</li>
<li><a href="https://github.com/codecov/codecov-action/commit/fc5d663f82feaca9160fcd69124d34600b850ef4"><code>fc5d663</code></a> fix: Hack to force asn1.js</li>
<li><a href="https://github.com/codecov/codecov-action/commit/5c832aefb841723472591f9f78e7496f24ea1ccb"><code>5c832ae</code></a> Force the dep</li>
<li><a href="https://github.com/codecov/codecov-action/commit/71fa76a9e49ffc8dcdc9545c8e23e82a7a7c0479"><code>71fa76a</code></a> fix: Add job to test no deps</li>
<li><a href="https://github.com/codecov/codecov-action/commit/672fbdc6af8916f554ec00c5faeb098326538439"><code>672fbdc</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/421">#421</a> from codecov/dependabot/npm_and_yarn/types/node-16.3.3</li>
<li><a href="https://github.com/codecov/codecov-action/commit/1691a31d132c8eb63bb0a11dfd1c25fa7941b3db"><code>1691a31</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/422">#422</a> from codecov/dependabot/npm_and_yarn/vercel/ncc-0.29.0</li>
<li><a href="https://github.com/codecov/codecov-action/commit/ad2b0032e0d254a4141103dc3a727b8d00f807a0"><code>ad2b003</code></a> fix: Add deep deps</li>
<li>Additional commits viewable in <a href="https://github.com/codecov/codecov-action/compare/v1.5.2...v2.0.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=codecov/codecov-action&package-manager=github_actions&previous-version=1.5.2&new-version=2.0.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-07-20 08:12:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2885" class=".btn">#2885</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.45.1 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.45.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
<h2>v5.45.1</h2>
<h1>Bugfixes</h1>
<ul>
<li>temporary revert import assertions because parser changes break the word <code>assert</code> in other places</li>
<li><code>import(/* webpackPrefetch: true */ ...)</code> no longer breaks library output</li>
<li>DataURL tries to avoid re-encoding</li>
<li>fix problems with DataURL encoding in some cases</li>
</ul>
<h2>v5.45.0</h2>
<h1>Features</h1>
<ul>
<li>add support to import assertions</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>SourceMaps will now also be added to <code>.cjs</code> output files</li>
<li>fix non-system externals in a system library</li>
</ul>
<h1>Performance</h1>
<ul>
<li>avoid copying timestamps from the watcher to the compiler</li>
</ul>
<h1>Contributing</h1>
<ul>
<li>update to jest 27</li>
</ul>
<h2>v5.44.0</h2>
<h1>Features</h1>
<ul>
<li>add support for <code>output.module</code> + <code>optimization.runtimeChunk</code></li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>fix inline externals with dash in type</li>
</ul>
<h2>v5.43.0</h2>
<h1>Features</h1>
<ul>
<li>support <code>runtime: false</code> in entry description to disable runtime chunk</li>
<li>support <code>runtime</code> option in ModuleFederationPlugin and ContainerPlugin</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>fix <code>&quot;module&quot;</code> externals when concatenated</li>
</ul>
<h1>Performance</h1>
<ul>
<li>serialize JSON data as buffer and parse on demand for performance and to avoid performance warning</li>
</ul>
<h2>v5.42.1</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/7102df3bb52a33529ff5db4fdf34484d2a359a49"><code>7102df3</code></a> 5.45.1</li>
<li><a href="https://github.com/webpack/webpack/commit/e15752ce9f61ff38fa1e3a6ce245cacc2fa5560b"><code>e15752c</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13431">#13431</a> from Shinyaigeek/fix/overwritten_webpack__exports_o...</li>
<li><a href="https://github.com/webpack/webpack/commit/396757192460e9a4e7d9e8c4c558fb1389bc1932"><code>3967571</code></a> Merge branch 'main' into fix/overwritten_webpack__exports_onChunksLoaded</li>
<li><a href="https://github.com/webpack/webpack/commit/e5570ab5230e98e1030d696e84465b5f533fdae9"><code>e5570ab</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13807">#13807</a> from webpack/issue-1342-from-css-loader</li>
<li><a href="https://github.com/webpack/webpack/commit/61946b7c46584821e6947ea35e00adbc2a02a8d2"><code>61946b7</code></a> Revert &quot;Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/12278">#12278</a> from xtuc/sven/import-assertions&quot;</li>
<li><a href="https://github.com/webpack/webpack/commit/daa40670fc3d15952eb572c5561fe027736b762f"><code>daa4067</code></a> keep original encoding when transforming data url to data url</li>
<li><a href="https://github.com/webpack/webpack/commit/c469adc2651437d9c115a41389ff7e3794416733"><code>c469adc</code></a> fix handling of onChunksLoaded with prefetching</li>
<li><a href="https://github.com/webpack/webpack/commit/3b65860614a10b7ac1209e0a947d4693c84537f2"><code>3b65860</code></a> Chore: add test case for issue 12993</li>
<li><a href="https://github.com/webpack/webpack/commit/1d8f9fd4d0783bfd790333881c7cd69e2180fa17"><code>1d8f9fd</code></a> Fix: overwritten <strong>webpack_exports</strong> on onChunksLoaded</li>
<li><a href="https://github.com/webpack/webpack/commit/db52c58a4fb037ece22be6365f56c11bc78fb426"><code>db52c58</code></a> 5.45.0</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.45.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.45.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-07-19 08:15:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2884" class=".btn">#2884</a>
            </td>
            <td>
                <b>
                    fix: Checks API error (webkms)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrii Soluk <isoluchok@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-16 13:56:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2882" class=".btn">#2882</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack-merge from 4.2.2 to 5.8.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack-merge](https://github.com/survivejs/webpack-merge) from 4.2.2 to 5.8.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/survivejs/webpack-merge/blob/develop/CHANGELOG.md">webpack-merge's changelog</a>.</em></p>
<blockquote>
<h2>5.8.0 / 2021-06-07</h2>
<ul>
<li>Docs - Update <code>env</code> example to be webpack 5 compatible. <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/177">#177</a>, <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/180">#180</a></li>
<li>Feat - Support strings as rules for TypeScript, not just enums. <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/179">#179</a>, <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/185">#185</a></li>
</ul>
<h2>5.7.3 / 2020-12-22</h2>
<ul>
<li>Fix - Don't merge strings with objects in <code>mergeWithRules</code>. <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/172">#172</a></li>
</ul>
<h2>5.7.2 / 2020-12-16</h2>
<ul>
<li>Fix - If there's no match when using <code>merge</code> operation with <code>mergeWithRules</code>, use default merge behavior as a fallback. <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/167">#167</a></li>
</ul>
<h2>5.7.1 / 2020-12-16</h2>
<ul>
<li>Fix - Fix a merge failure for <code>mergeWithRules</code> when non-array matches are merged. <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/166">#166</a></li>
</ul>
<h2>5.7.0 / 2020-12-12</h2>
<ul>
<li>Feat - Throw a <code>TypeError</code> if trying to use <code>mergeWithRules</code> with invalid configuration types for <code>append</code>/<code>prepend</code>/<code>merge</code> operations.</li>
</ul>
<h2>5.6.1 / 2020-12-11</h2>
<ul>
<li>Fix - Drop extraneous logging.</li>
</ul>
<h2>5.6.0 / 2020-12-11</h2>
<ul>
<li>Feat - Support <code>merge</code> (<code>CustomizeRule.Merge</code>) for objects at <code>mergeWithRules</code>. This is useful for merging loader options for example. <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/163">#163</a></li>
</ul>
<h2>5.5.0 / 2020-12-10</h2>
<ul>
<li>Feat - Allow <code>mergeWithRules</code> to merge based on rules without a match. <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/151">#151</a> <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/159">#159</a></li>
</ul>
<h2>5.4.1 / 2020-12-08</h2>
<ul>
<li>Fix - Allow <code>mergeUnique</code> to work with arbitrary order. <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/161">#161</a></li>
</ul>
<h2>5.4.0 / 2020-10-30</h2>
<ul>
<li>Fix - Fall back correctly in <code>mergeWithRules</code> for cases that aren't matched. <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/157">#157</a> <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/158">#158</a></li>
<li>Fix - Don't throw if using <code>mergeWithRules</code> without a rule <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/151">#151</a></li>
<li>Feat - Throw if <code>undefined</code> is passed to <code>merge</code> as a structure to merge</li>
</ul>
<h2>5.3.0 / 2020-10-30</h2>
<ul>
<li>Fix - Expose <code>Configuration</code> type through a generic to TypeScript to support both webpack 4 and 5 <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/141">#141</a> <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/154">#154</a></li>
</ul>
<p>In case you use webpack 4, please change your typing as instructed in the readme as the default type is loose but non-breaking.</p>
<h2>5.2.0 / 2020-10-07</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/survivejs/webpack-merge/commit/7a99833bd9faecd30bbcaeec8a9a10f6bab1d300"><code>7a99833</code></a> 5.8.0</li>
<li><a href="https://github.com/survivejs/webpack-merge/commit/df2b5cf6b28cc8f184dc53ec7a5622a44a7a8080"><code>df2b5cf</code></a> chore: Update changelog</li>
<li><a href="https://github.com/survivejs/webpack-merge/commit/5cb501e60481fb74f38595479c246f7d99d115c2"><code>5cb501e</code></a> feat: Support rules as strings (<a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/185">#185</a>)</li>
<li><a href="https://github.com/survivejs/webpack-merge/commit/72b52ced453ed642cd90de445bcfc4d8e338a412"><code>72b52ce</code></a> chore: Update changelog</li>
<li><a href="https://github.com/survivejs/webpack-merge/commit/afe55817106a61af03c9a25d03e06fab2de7c231"><code>afe5581</code></a> docs: update  example code of Limitations (<a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/180">#180</a>)</li>
<li><a href="https://github.com/survivejs/webpack-merge/commit/1062b06cfbbc2c9f5e7f9f21ab9d2cf0c6851296"><code>1062b06</code></a> chore: Update dependencies</li>
<li><a href="https://github.com/survivejs/webpack-merge/commit/3da07b210cda525ed0b124153d6472c23c88b2f2"><code>3da07b2</code></a> chore(deps): bump y18n from 4.0.0 to 4.0.1 (<a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/178">#178</a>)</li>
<li><a href="https://github.com/survivejs/webpack-merge/commit/53bac19aebff060116fd3b16a581e4bf06c7ac1e"><code>53bac19</code></a> chore(deps): bump lodash from 4.17.20 to 4.17.21 (<a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/181">#181</a>)</li>
<li><a href="https://github.com/survivejs/webpack-merge/commit/936ed0321bee2a2239abfe62f05d201dd46267b0"><code>936ed03</code></a> chore(deps): bump hosted-git-info from 2.8.8 to 2.8.9 (<a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/182">#182</a>)</li>
<li><a href="https://github.com/survivejs/webpack-merge/commit/d70de5320c94037ae2892bf9d76e5bafbfcf49bc"><code>d70de53</code></a> chore(deps): bump browserslist from 4.14.5 to 4.16.6 (<a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/183">#183</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/survivejs/webpack-merge/compare/v4.2.2...v5.8.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack-merge&package-manager=npm_and_yarn&previous-version=4.2.2&new-version=5.8.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-07-15 08:18:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2881" class=".btn">#2881</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack-cli from 3.3.10 to 4.7.2 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack-cli](https://github.com/webpack/webpack-cli) from 3.3.10 to 4.7.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack-cli/releases">webpack-cli's releases</a>.</em></p>
<blockquote>
<h2>v4.7.2</h2>
<h2><a href="https://github.com/webpack/webpack-cli/compare/webpack-cli@4.7.1...webpack-cli@4.7.2">4.7.2</a> (2021-06-07)</h2>
<p><strong>Note:</strong> Version bump only for package webpack-cli</p>
<h2>v4.7.1</h2>
<h2><a href="https://github.com/webpack/webpack-cli/compare/webpack-cli@4.7.0...webpack-cli@4.7.1">4.7.1</a> (2021-06-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>not found module after ask installation (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2761">#2761</a>) (<a href="https://github.com/webpack/webpack-cli/commit/557ad05ae8168255b57698bdd2d98cbc7b53812d">557ad05</a>)</li>
<li>prettier config (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2719">#2719</a>) (<a href="https://github.com/webpack/webpack-cli/commit/181295fb1b1973c201c221813562219d85b845ae">181295f</a>)</li>
</ul>
<h2>v4.7.0</h2>
<h1><a href="https://github.com/webpack/webpack-cli/compare/webpack-cli@4.6.0...webpack-cli@4.7.0">4.7.0</a> (2021-05-06)</h1>
<h3>Bug Fixes</h3>
<ul>
<li>parsing of empty <code>--env</code> flags (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2643">#2643</a>) (<a href="https://github.com/webpack/webpack-cli/commit/bc12f1a2a833f09a0585050a0f5dd854da188f1d">bc12f1a</a>)</li>
<li>update usage info (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2594">#2594</a>) (<a href="https://github.com/webpack/webpack-cli/commit/9d07d67faf147cbaf0dddb95038403963e5f2afb">9d07d67</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>add <code>create</code> and <code>new</code> alias for <code>init</code> (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2616">#2616</a>) (<a href="https://github.com/webpack/webpack-cli/commit/5a9789db237b7696adfdc9826b0dda749fedfa9a">5a9789d</a>)</li>
<li>add <code>server</code> alias for <code>serve</code> command (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2631">#2631</a>) (<a href="https://github.com/webpack/webpack-cli/commit/c9ee947618c06447bc1f949e4d401e63f737f38d">c9ee947</a>)</li>
<li>add flag to force start finish log (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2566">#2566</a>) (<a href="https://github.com/webpack/webpack-cli/commit/281aad3ee4961f1643453eb1a926e88e0b7f019c">281aad3</a>)</li>
<li>added <code>--no-devtool</code> to webpack v4(<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2603">#2603</a>) (<a href="https://github.com/webpack/webpack-cli/commit/7c6f390a1d64d562065ffc31d8b23d833813ee9d">7c6f390</a>)</li>
<li>added support arguments description (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2659">#2659</a>) (<a href="https://github.com/webpack/webpack-cli/commit/4dfd166f757ce94130bf9b7580f2dbe2868b8f4f">4dfd166</a>)</li>
</ul>
<h2>v4.6.0</h2>
<h1><a href="https://github.com/webpack/webpack-cli/compare/webpack-cli@4.5.0...webpack-cli@4.6.0">4.6.0</a> (2021-03-27)</h1>
<h3>Bug Fixes</h3>
<ul>
<li><code>negative</code> options (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2555">#2555</a>) (<a href="https://github.com/webpack/webpack-cli/commit/f26ebc105e140992639864fa01950454abd716ac">f26ebc1</a>)</li>
<li>improve error message for help (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2482">#2482</a>) (<a href="https://github.com/webpack/webpack-cli/commit/99ae2a3b9f7ad8c1807839357360a1b4607865b1">99ae2a3</a>)</li>
<li>show <code>--node-env</code> in minimum help output (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2411">#2411</a>) (<a href="https://github.com/webpack/webpack-cli/commit/f5fc3023121f4d952a166879a46b2653c20b6349">f5fc302</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>added <code>WEBPACK_PACKAGE</code> env var to use custom <code>webpack</code> package (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2556">#2556</a>) (<a href="https://github.com/webpack/webpack-cli/commit/3d1e4855c55a6601d8a89dcb50d9d842009e3cda">3d1e485</a>)</li>
<li>added <code>WEBPACK_CLI_SKIP_IMPORT_LOCAL</code> env var to skip local import (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2546">#2546</a>) (<a href="https://github.com/webpack/webpack-cli/commit/e13082221c2da01d8b8215ebc936474bf3ca1582">e130822</a>)</li>
<li>allow string value for the <code>--hot</code> option (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2444">#2444</a>) (<a href="https://github.com/webpack/webpack-cli/commit/8656e78d788bc8a504258d4dcc609767f63d60c4">8656e78</a>)</li>
<li>display used config path when logging level=log (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2431">#2431</a>) (<a href="https://github.com/webpack/webpack-cli/commit/f8406e1c5253849fad741eb45f1ece23a7c603f4">f8406e1</a>)</li>
</ul>
<h2>v4.5.0</h2>
<h1><a href="https://github.com/webpack/webpack-cli/compare/webpack-cli@4.4.0...webpack-cli@4.5.0">4.5.0</a> (2021-02-02)</h1>
<h3>Notes</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack-cli/blob/master/CHANGELOG.md">webpack-cli's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/webpack/webpack-cli/compare/webpack-cli@4.7.1...webpack-cli@4.7.2">4.7.2</a> (2021-06-07)</h2>
<p><strong>Note:</strong> Version bump only for package webpack-cli (due <code>@webpack-cli/serve</code>)</p>
<h2><a href="https://github.com/webpack/webpack-cli/compare/webpack-cli@4.7.0...webpack-cli@4.7.1">4.7.1</a> (2021-06-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>not found module after ask installation (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2761">#2761</a>) (<a href="https://github.com/webpack/webpack-cli/commit/557ad05ae8168255b57698bdd2d98cbc7b53812d">557ad05</a>)</li>
<li>prettier config (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2719">#2719</a>) (<a href="https://github.com/webpack/webpack-cli/commit/181295fb1b1973c201c221813562219d85b845ae">181295f</a>)</li>
</ul>
<h1><a href="https://github.com/webpack/webpack-cli/compare/webpack-cli@4.6.0...webpack-cli@4.7.0">4.7.0</a> (2021-05-06)</h1>
<h3>Bug Fixes</h3>
<ul>
<li>parsing of empty <code>--env</code> flags (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2643">#2643</a>) (<a href="https://github.com/webpack/webpack-cli/commit/bc12f1a2a833f09a0585050a0f5dd854da188f1d">bc12f1a</a>)</li>
<li>update usage info (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2594">#2594</a>) (<a href="https://github.com/webpack/webpack-cli/commit/9d07d67faf147cbaf0dddb95038403963e5f2afb">9d07d67</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>add <code>create</code> and <code>new</code> alias for <code>init</code> (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2616">#2616</a>) (<a href="https://github.com/webpack/webpack-cli/commit/5a9789db237b7696adfdc9826b0dda749fedfa9a">5a9789d</a>)</li>
<li>add <code>server</code> alias for <code>serve</code> command (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2631">#2631</a>) (<a href="https://github.com/webpack/webpack-cli/commit/c9ee947618c06447bc1f949e4d401e63f737f38d">c9ee947</a>)</li>
<li>add flag to force start finish log (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2566">#2566</a>) (<a href="https://github.com/webpack/webpack-cli/commit/281aad3ee4961f1643453eb1a926e88e0b7f019c">281aad3</a>)</li>
<li>added <code>--no-devtool</code> to webpack v4(<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2603">#2603</a>) (<a href="https://github.com/webpack/webpack-cli/commit/7c6f390a1d64d562065ffc31d8b23d833813ee9d">7c6f390</a>)</li>
<li>added support arguments description (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2659">#2659</a>) (<a href="https://github.com/webpack/webpack-cli/commit/4dfd166f757ce94130bf9b7580f2dbe2868b8f4f">4dfd166</a>)</li>
</ul>
<h1><a href="https://github.com/webpack/webpack-cli/compare/webpack-cli@4.5.0...webpack-cli@4.6.0">4.6.0</a> (2021-03-27)</h1>
<h3>Bug Fixes</h3>
<ul>
<li><code>negative</code> options (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2555">#2555</a>) (<a href="https://github.com/webpack/webpack-cli/commit/f26ebc105e140992639864fa01950454abd716ac">f26ebc1</a>)</li>
<li>improve error message for help (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2482">#2482</a>) (<a href="https://github.com/webpack/webpack-cli/commit/99ae2a3b9f7ad8c1807839357360a1b4607865b1">99ae2a3</a>)</li>
<li>show <code>--node-env</code> in minimum help output (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2411">#2411</a>) (<a href="https://github.com/webpack/webpack-cli/commit/f5fc3023121f4d952a166879a46b2653c20b6349">f5fc302</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>added <code>WEBPACK_PACKAGE</code> env var to use custom <code>webpack</code> package (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2556">#2556</a>) (<a href="https://github.com/webpack/webpack-cli/commit/3d1e4855c55a6601d8a89dcb50d9d842009e3cda">3d1e485</a>)</li>
<li>added <code>WEBPACK_CLI_SKIP_IMPORT_LOCAL</code> env var to skip local import (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2546">#2546</a>) (<a href="https://github.com/webpack/webpack-cli/commit/e13082221c2da01d8b8215ebc936474bf3ca1582">e130822</a>)</li>
<li>allow string value for the <code>--hot</code> option (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2444">#2444</a>) (<a href="https://github.com/webpack/webpack-cli/commit/8656e78d788bc8a504258d4dcc609767f63d60c4">8656e78</a>)</li>
<li>display used config path when logging level=log (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2431">#2431</a>) (<a href="https://github.com/webpack/webpack-cli/commit/f8406e1c5253849fad741eb45f1ece23a7c603f4">f8406e1</a>)</li>
</ul>
<h1><a href="https://github.com/webpack/webpack-cli/compare/webpack-cli@4.4.0...webpack-cli@4.5.0">4.5.0</a> (2021-02-02)</h1>
<h3>Notes</h3>
<ul>
<li>now you can use <code>webpack.config.mjs</code> and <code>webpack.config.js</code> with <code>{ &quot;type&quot;: &quot;module&quot; }</code> in <code>package.json</code></li>
<li>you can avoid using the <code>cross-env</code> package:</li>
</ul>
<p>Before:</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack-cli/commit/68ef0563afd105652dc0fd0b2391a0a766cd24fe"><code>68ef056</code></a> chore(release): publish new version</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/2d7ab3549c429193b4ed5fbc6174153c847e0330"><code>2d7ab35</code></a> fix: broken serve with new CLI API (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2770">#2770</a>)</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/060268b770c9623e457afc849e3933364914951d"><code>060268b</code></a> docs: update CHANGELOG</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/2be9b9254009598e021b830091fba8832dfdb57b"><code>2be9b92</code></a> chore(release): publish new version</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/598008a0a3e90ea8dd8c415a3c08700b750774b5"><code>598008a</code></a> chore(deps-dev): bump ts-jest from 27.0.2 to 27.0.3 (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2764">#2764</a>)</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/625b4fd88ab38f3381c3fbd2df3ae2d813fe784f"><code>625b4fd</code></a> chore(deps-dev): bump prettier from 2.3.0 to 2.3.1 (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2765">#2765</a>)</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/bb7c9d3c9b0dca11242e2febcd41805c063e1317"><code>bb7c9d3</code></a> feat: new CLI options API for serve (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2754">#2754</a>)</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/557ad05ae8168255b57698bdd2d98cbc7b53812d"><code>557ad05</code></a> fix: not found module after ask installation (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2761">#2761</a>)</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/c8fef37c06874d62479e65145f764cd72dc3a82e"><code>c8fef37</code></a> chore(deps-dev): bump <code>@​typescript-eslint/parser</code></li>
<li><a href="https://github.com/webpack/webpack-cli/commit/368778d128474dad7a0a341985ee31e35d10a697"><code>368778d</code></a> fix: add node 16 to CI (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2760">#2760</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack-cli/compare/v3.3.10...webpack-cli@4.7.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~evilebottnawi">evilebottnawi</a>, a new releaser for webpack-cli since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack-cli&package-manager=npm_and_yarn&previous-version=3.3.10&new-version=4.7.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-07-14 22:13:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2880" class=".btn">#2880</a>
            </td>
            <td>
                <b>
                    chore: disable dependabot PRs on gomod
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - the other gomod in the repo need to be updated in sync.

Signed-off-by: Troy Ronda <troy@troyronda.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 20:37:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2879" class=".btn">#2879</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump file-loader from 5.0.2 to 6.2.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [file-loader](https://github.com/webpack-contrib/file-loader) from 5.0.2 to 6.2.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack-contrib/file-loader/releases">file-loader's releases</a>.</em></p>
<blockquote>
<h2>v6.2.0</h2>
<h2><a href="https://github.com/webpack-contrib/file-loader/compare/v6.1.1...v6.2.0">6.2.0</a> (2020-10-27)</h2>
<h3>Features</h3>
<ul>
<li>added the <code>sourceFilename</code> property to asset info with original filename (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/393">#393</a>) (<a href="https://github.com/webpack-contrib/file-loader/commit/654e0d641ec067089f6a2d12e30ec3520f00d808">654e0d6</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>immutable flag when the <code>name</code> option have hash in query string (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/392">#392</a>) (<a href="https://github.com/webpack-contrib/file-loader/commit/381d8bda3f2494487bfe840386e365b97b6025fe">381d8bd</a>)</li>
</ul>
<h2>v6.1.1</h2>
<h3><a href="https://github.com/webpack-contrib/file-loader/compare/v6.1.0...v6.1.1">6.1.1</a> (2020-10-09)</h3>
<h3>Chore</h3>
<ul>
<li>update <code>schema-utils</code></li>
</ul>
<h2>v6.1.0</h2>
<h2><a href="https://github.com/webpack-contrib/file-loader/compare/v6.0.0...v6.1.0">6.1.0</a> (2020-08-31)</h2>
<h3>Features</h3>
<ul>
<li>pass immutable flag to asset info (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/383">#383</a>) (<a href="https://github.com/webpack-contrib/file-loader/commit/40fcde81681d4f8ee19d2ee3845fd34e24459195">40fcde8</a>)</li>
</ul>
<h2>v6.0.0</h2>
<h2><a href="https://github.com/webpack-contrib/file-loader/compare/v5.1.0...v6.0.0">6.0.0</a> (2020-03-17)</h2>
<h3>⚠ BREAKING CHANGES</h3>
<ul>
<li>use <code>md4</code> by default for hashing (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/369">#369</a>) (<a href="https://github.com/webpack-contrib/file-loader/commit/ad3902284d28adeddf667212a39faa4c6bfb2964">ad39022</a>)</li>
</ul>
<h2>v5.1.0</h2>
<h2><a href="https://github.com/webpack-contrib/file-loader/compare/v5.0.2...v5.1.0">5.1.0</a> (2020-02-19)</h2>
<h3>Features</h3>
<ul>
<li>support the <code>query</code> template for the <code>name</code> option (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/366">#366</a>) (<a href="https://github.com/webpack-contrib/file-loader/commit/cd8698b1d9fd560d85e912acca9a1e24f00e18f8">cd8698b</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/webpack-contrib/file-loader/blob/master/CHANGELOG.md">file-loader's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/webpack-contrib/file-loader/compare/v6.1.1...v6.2.0">6.2.0</a> (2020-10-27)</h2>
<h3>Features</h3>
<ul>
<li>added the <code>sourceFilename</code> property to asset info with original filename (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/393">#393</a>) (<a href="https://github.com/webpack-contrib/file-loader/commit/654e0d641ec067089f6a2d12e30ec3520f00d808">654e0d6</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>immutable flag when the <code>name</code> option have hash in query string (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/392">#392</a>) (<a href="https://github.com/webpack-contrib/file-loader/commit/381d8bda3f2494487bfe840386e365b97b6025fe">381d8bd</a>)</li>
</ul>
<h3><a href="https://github.com/webpack-contrib/file-loader/compare/v6.1.0...v6.1.1">6.1.1</a> (2020-10-09)</h3>
<h3>Chore</h3>
<ul>
<li>update <code>schema-utils</code></li>
</ul>
<h2><a href="https://github.com/webpack-contrib/file-loader/compare/v6.0.0...v6.1.0">6.1.0</a> (2020-08-31)</h2>
<h3>Features</h3>
<ul>
<li>pass immutable flag to asset info (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/383">#383</a>) (<a href="https://github.com/webpack-contrib/file-loader/commit/40fcde81681d4f8ee19d2ee3845fd34e24459195">40fcde8</a>)</li>
</ul>
<h2><a href="https://github.com/webpack-contrib/file-loader/compare/v5.1.0...v6.0.0">6.0.0</a> (2020-03-17)</h2>
<h3>⚠ BREAKING CHANGES</h3>
<ul>
<li>use <code>md4</code> by default for hashing (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/369">#369</a>) (<a href="https://github.com/webpack-contrib/file-loader/commit/ad3902284d28adeddf667212a39faa4c6bfb2964">ad39022</a>)</li>
</ul>
<h2><a href="https://github.com/webpack-contrib/file-loader/compare/v5.0.2...v5.1.0">5.1.0</a> (2020-02-19)</h2>
<h3>Features</h3>
<ul>
<li>support the <code>query</code> template for the <code>name</code> option (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/366">#366</a>) (<a href="https://github.com/webpack-contrib/file-loader/commit/cd8698b1d9fd560d85e912acca9a1e24f00e18f8">cd8698b</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack-contrib/file-loader/commit/c423008dce1b16e1253b89b792f03774ffeb47de"><code>c423008</code></a> chore(release): 6.2.0</li>
<li><a href="https://github.com/webpack-contrib/file-loader/commit/654e0d641ec067089f6a2d12e30ec3520f00d808"><code>654e0d6</code></a> feat: added the <code>sourceFilename</code> property to asset info with original filenam...</li>
<li><a href="https://github.com/webpack-contrib/file-loader/commit/381d8bda3f2494487bfe840386e365b97b6025fe"><code>381d8bd</code></a> fix: immutable flag when the <code>name</code> option have hash in query string (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/392">#392</a>)</li>
<li><a href="https://github.com/webpack-contrib/file-loader/commit/14ed4c9b47f2e580f5b04b71f742cafe9e554565"><code>14ed4c9</code></a> ci: updated webpack versions (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/389">#389</a>)</li>
<li><a href="https://github.com/webpack-contrib/file-loader/commit/6fadfbe9fe43ca86095c836a3c521dfbbac408aa"><code>6fadfbe</code></a> chore(release): 6.1.1</li>
<li><a href="https://github.com/webpack-contrib/file-loader/commit/60508cf17c2689a8c96d8f56ffc6bbc0ed82d553"><code>60508cf</code></a> chore(deps): update</li>
<li><a href="https://github.com/webpack-contrib/file-loader/commit/25e2668f75ae3e8f78adeb99297caa258b2479f3"><code>25e2668</code></a> chore(release): 6.1.0</li>
<li><a href="https://github.com/webpack-contrib/file-loader/commit/6e22f6e78fe17eea052a20a0b417640035e919b3"><code>6e22f6e</code></a> test: fix</li>
<li><a href="https://github.com/webpack-contrib/file-loader/commit/40fcde81681d4f8ee19d2ee3845fd34e24459195"><code>40fcde8</code></a> feat: pass immutable flag to asset info (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/383">#383</a>)</li>
<li><a href="https://github.com/webpack-contrib/file-loader/commit/718aef5f992d325945b1d13b675ac8c6d187a3bb"><code>718aef5</code></a> chore(deps): update (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/375">#375</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/webpack-contrib/file-loader/compare/v5.0.2...v6.2.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=file-loader&package-manager=npm_and_yarn&previous-version=5.0.2&new-version=6.2.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-07-14 18:21:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2878" class=".btn">#2878</a>
            </td>
            <td>
                <b>
                    feat: Document loader for agent-mobile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - added document loader as an option for agent mobile

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 15:50:59 +0000 UTC
    </div>
</div>

