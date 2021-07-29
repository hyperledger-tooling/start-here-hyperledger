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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2896" class=".btn">#2896</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.47.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.47.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
<h2>v5.47.0</h2>
<h1>Performance</h1>
<ul>
<li>improve source-map performance</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>avoid unnecessary <code>&quot;use strict&quot;</code>s in module mode</li>
</ul>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/efeb1287e52870036cc01b22476852205e99c31a"><code>efeb128</code></a> 5.47.0</li>
<li><a href="https://github.com/webpack/webpack/commit/61ad5ff509a7f9ce5be703e386e4d4da6216f008"><code>61ad5ff</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13873">#13873</a> from webpack/perf/webpack-sources-3</li>
<li><a href="https://github.com/webpack/webpack/commit/c3a0145b49e62fbda7fe1372b87b0cef517a6c7f"><code>c3a0145</code></a> update to webpack-sources version 3</li>
<li><a href="https://github.com/webpack/webpack/commit/beb42c64f696584ef570d8f57df448ddd0ac7238"><code>beb42c6</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13858">#13858</a> from Janpot/genrator-publicPath-override</li>
<li><a href="https://github.com/webpack/webpack/commit/d9c09ee7f20f174588f1877da65dc57ec1e2ac5a"><code>d9c09ee</code></a> Fix generator publicPath behavior when empty string</li>
<li><a href="https://github.com/webpack/webpack/commit/bdf20c2a6f531022a91960d5f3facf324577d1ec"><code>bdf20c2</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13840">#13840</a> from snitin315/patch-1</li>
<li><a href="https://github.com/webpack/webpack/commit/5f8adb0110f824c433c2619b072cdd467875434a"><code>5f8adb0</code></a> keep the eslint cache and yarn install</li>
<li><a href="https://github.com/webpack/webpack/commit/1f4e8a293dee182bcc09fb179c321ab83d1b3320"><code>1f4e8a2</code></a> ci: use <code>cache: 'yarn'</code></li>
<li><a href="https://github.com/webpack/webpack/commit/60d8968cd48cf1677df5f50ed878c6a912e9d692"><code>60d8968</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13842">#13842</a> from webpack/bugfix/use-strict</li>
<li><a href="https://github.com/webpack/webpack/commit/0bd1e789d48f9b3e3ca38d6c48db7c7be5380bcd"><code>0bd1e78</code></a> generate &quot;use strict&quot; only when really needed</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.47.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.47.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-07-28 08:19:53 +0000 UTC
    </div>
</div>

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

