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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2891" class=".btn">#2891</a>
            </td>
            <td>
                <b>
                    docs: remove image binary
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Part of #2433

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 14:24:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2889" class=".btn">#2889</a>
            </td>
            <td>
                <b>
                    docs: vcwallet docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - vc wallet docs covering detailed information about all wallet
features, data models, interfaces and bindings are added
- Part of #2433

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 02:35:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2888" class=".btn">#2888</a>
            </td>
            <td>
                <b>
                    feat: use only did:key in didcomm
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change removes Base58 key encoding and only uses did:key for both sender and recipient keys.
It also includes vdr peer did creation with all KeyAgreement keys, not only the first key.
It moves jwk out of the jose package to be a separate package called jwk along with common jwk code in jwksupport subpackage to avoid circular dependency.
This change also changes webkms log traces level to Debug.

closes #1604
closes #1207

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-21 22:02:41 +0000 UTC
    </div>
</div>

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

