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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2894" class=".btn">#2894</a>
            </td>
            <td>
                <b>
                    fix: presexch shouldn't use only the final schema match when checking for schema match
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also include context needed for test harness tests.

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-27 21:54:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2893" class=".btn">#2893</a>
            </td>
            <td>
                <b>
                    chore(deps): bump codecov/codecov-action from 2.0.1 to 2.0.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [codecov/codecov-action](https://github.com/codecov/codecov-action) from 2.0.1 to 2.0.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/codecov/codecov-action/releases">codecov/codecov-action's releases</a>.</em></p>
<blockquote>
<h2>v2.0.2</h2>
<h3>Fixes</h3>
<ul>
<li>Underlying uploader fixes issues with tokens not being sent properly for users seeing
<code>Error!: Error: Error uploading to https://codecov.io: Error: Error uploading to Codecov: Error: Not Found</code></li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/432">#432</a> fix: use import to destructure package.json</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/434">#434</a> fix: openpgp and asn1.js</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/440">#440</a> 2.0.2 token fixes</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/420">#420</a> Bump eslint from 7.30.0 to 7.31.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/433">#433</a> build(deps-dev): bump <code>@​types/node</code> from 16.3.3 to 16.4.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/425">#425</a> build(deps-dev): bump <code>@​typescript-eslint/eslint-plugin</code> from 4.28.3 to 4.28.4</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/426">#426</a> build(deps-dev): bump <code>@​typescript-eslint/parser</code> from 4.28.3 to 4.28.4</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/438">#438</a> Set up Dependabot for github-actions dependencies</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/codecov/codecov-action/blob/master/CHANGELOG.md">codecov/codecov-action's changelog</a>.</em></p>
<blockquote>
<h2>2.0.2</h2>
<h3>Fixes</h3>
<ul>
<li>Underlying uploader fixes issues with tokens not being sent properly for users seeing
<code>Error!: Error: Error uploading to https://codecov.io: Error: Error uploading to Codecov: Error: Not Found</code></li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/440">#440</a> fix: Validation ordering</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/codecov/codecov-action/commit/51d810878be5422784e86451c0e7c14e5860ec47"><code>51d8108</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/440">#440</a> from codecov/2.0.2-token-fixes</li>
<li><a href="https://github.com/codecov/codecov-action/commit/88c796db184decd9587ce608896441b1c96fb3d9"><code>88c796d</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/438">#438</a> from mmorel-35/chore/dependabot</li>
<li><a href="https://github.com/codecov/codecov-action/commit/0bbb08247af9376cc8aa170281fce5b5e48bfde4"><code>0bbb082</code></a> fix: Update validation</li>
<li><a href="https://github.com/codecov/codecov-action/commit/53f686aaf8540352482d0bea7b92248ef1e2cb0a"><code>53f686a</code></a> fix: Update validation</li>
<li><a href="https://github.com/codecov/codecov-action/commit/6ab08a75e2ef9b04e5402468f88c8f08039017c0"><code>6ab08a7</code></a> Bump to 2.0.2</li>
<li><a href="https://github.com/codecov/codecov-action/commit/f2242e1815c6a47d64639e34b6aad38aef3fc4e1"><code>f2242e1</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/425">#425</a> from codecov/dependabot/npm_and_yarn/typescript-eslin...</li>
<li><a href="https://github.com/codecov/codecov-action/commit/fc2878a5309ea34776e2a8fb3853258d64710d6d"><code>fc2878a</code></a> build(deps-dev): bump <code>@​typescript-eslint/eslint-plugin</code></li>
<li><a href="https://github.com/codecov/codecov-action/commit/e00e953908be2880a844c7917679fe2adc0f6c83"><code>e00e953</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/426">#426</a> from codecov/dependabot/npm_and_yarn/typescript-eslin...</li>
<li><a href="https://github.com/codecov/codecov-action/commit/8dcb1d2117f92afad705f41f41974505a1ed3fd8"><code>8dcb1d2</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/433">#433</a> from codecov/dependabot/npm_and_yarn/types/node-16.4.0</li>
<li><a href="https://github.com/codecov/codecov-action/commit/c5857ba40cc009e8157219891e3a99dbc86718ba"><code>c5857ba</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/434">#434</a> from RA80533/fix/openpgp</li>
<li>Additional commits viewable in <a href="https://github.com/codecov/codecov-action/compare/v2.0.1...v2.0.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=codecov/codecov-action&package-manager=github_actions&previous-version=2.0.1&new-version=2.0.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-07-26 08:17:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2892" class=".btn">#2892</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.46.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.46.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
<h2>v5.46.0</h2>
<h1>Features</h1>
<ul>
<li>status handlers in HMR api can now return Promises to delay the HMR process</li>
<li>reasons in stats can now be grouped and collapsed
<ul>
<li>add <code>stats.reasonsSpace</code> and <code>stats.groupReasonsByOrigin</code></li>
</ul>
</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>fix a crash in asset modules when updating persistent cached modules from unsafe cached modules</li>
</ul>
<h1>Performance</h1>
<ul>
<li>detailed preset limits all spaces to 1000 by default</li>
<li>upgrade webpack-sources for a performance bugfix</li>
</ul>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/a32b0fd041260f3303b9329c9a65cc4afe102390"><code>a32b0fd</code></a> 5.46.0</li>
<li><a href="https://github.com/webpack/webpack/commit/e83587cfef25db91dc5b86be5b729288fd1bafdd"><code>e83587c</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13837">#13837</a> from webpack/bugfix/13827</li>
<li><a href="https://github.com/webpack/webpack/commit/e293d2b222a8673a29c5ac4b390176dce56ac921"><code>e293d2b</code></a> add missing lint step in azure</li>
<li><a href="https://github.com/webpack/webpack/commit/d8c37d7cdd31c925a4b0d7fb9bea794e8bd4d93a"><code>d8c37d7</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13836">#13836</a> from webpack/dependabot/npm_and_yarn/eslint-plugin-...</li>
<li><a href="https://github.com/webpack/webpack/commit/c23e8ce5c7c381e330ad70dbb999024e0d89bee0"><code>c23e8ce</code></a> fix problems with compiling twice</li>
<li><a href="https://github.com/webpack/webpack/commit/cdc9efefbeb8b7071abdd38498f16478f5012796"><code>cdc9efe</code></a> avoid copying source types and sizes cache from unsafe cache to cached module</li>
<li><a href="https://github.com/webpack/webpack/commit/df5031bd356fcba8fcc0f55ebe7714ed3f9e2415"><code>df5031b</code></a> chore(deps-dev): bump eslint-plugin-jest from 24.3.6 to 24.4.0</li>
<li><a href="https://github.com/webpack/webpack/commit/1a134d955f050465899adea0b74560936caa5860"><code>1a134d9</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13826">#13826</a> from webpack/dependabot/npm_and_yarn/schema-utils-3...</li>
<li><a href="https://github.com/webpack/webpack/commit/937957fc545fae96a15ce0ea3fb9b7910de41f7e"><code>937957f</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13828">#13828</a> from webpack/perf/many-replacements</li>
<li><a href="https://github.com/webpack/webpack/commit/d3f8e16810581791de6bd3e2ccc944541779b4a2"><code>d3f8e16</code></a> update webpack-sources for performance problem in hashing</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.46.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.46.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-07-23 08:19:57 +0000 UTC
    </div>
</div>

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
This change also updates webkms log traces level to Debug.
Finally this change adds all keyAgreement VMs in the DID doc into the DIDComm service bloc (instead of only the first key).

closes #1604
closes #1207
closes #1659  
closes #1847


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

