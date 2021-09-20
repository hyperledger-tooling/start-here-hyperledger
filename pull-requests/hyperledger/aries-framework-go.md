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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2991" class=".btn">#2991</a>
            </td>
            <td>
                <b>
                    chore: increase coverage for verifiable command fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-17 13:59:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2990" class=".btn">#2990</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.53.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.53.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
<h2>v5.53.0</h2>
<h1>Features</h1>
<ul>
<li>add <code>node.__dirname/__filename: &quot;warn-mock&quot;</code> which warns on usage (will be enabled in webpack 6 by default)</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>add <code>stream/web</code> to Node.js externals</li>
<li>fix IgnorePluginSchema</li>
<li>fix builds with persistent caching taking 1 minute to build at least</li>
</ul>
<h1>Experiments</h1>
<ul>
<li>add <code>experiments.futureDefaults</code> to enable defaults for webpack 6</li>
</ul>
<h2>v5.52.1</h2>
<h1>Performance</h1>
<ul>
<li>split fresh created persistent cache files by time to avoid creating very large files</li>
</ul>
<h2>v5.52.0</h2>
<h1>Feature</h1>
<ul>
<li><code>experiments.executeModule</code> is enabled by default and the option is removed
<ul>
<li>loaders are now free to use <code>this.importModule</code></li>
</ul>
</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>fix generated <code>__WEBPACK_EXTERNAL_MODULE_null__</code>, which leads to merged externals</li>
<li><code>.webpack[...]</code> extension is not part of matching and module name</li>
</ul>
<h2>v5.51.2</h2>
<h1>Bugfixes</h1>
<ul>
<li>fix crash in FileSystemInfo when errors occur</li>
<li>avoid property access of reserved properties</li>
<li>fix reexports from async modules</li>
<li>automatically close an active watching when closing the compiler</li>
<li>when filenames of other runtimes are referenced that need a full hash, upgrade referencing runtime moduel to full hash mode too
<ul>
<li>fixes a bug where <code>[contenthash]</code> is undefined when using <code>new Worker</code></li>
</ul>
</li>
</ul>
<h2>v5.51.1</h2>
<h1>Bugfixes</h1>
<ul>
<li><code>library: &quot;module&quot;</code> propages top-level-await correctly</li>
<li>fix crash in filesystem snapshotting when trying to snapshot a non-existing directory</li>
<li>fix some context-dependent logic in concatenated modules and source url handling</li>
</ul>
<h2>v5.51.0</h2>
<h1>Bugfixes</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/6796b73a1ab83739f0e722d914676c9dd58d65e2"><code>6796b73</code></a> 5.53.0</li>
<li><a href="https://github.com/webpack/webpack/commit/6458896639a484437f7f05d61a62161a2096cf59"><code>6458896</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14264">#14264</a> from webpack/bugfix/hanging</li>
<li><a href="https://github.com/webpack/webpack/commit/ff69b3f61771ccc3f0a70d91876cb89059e1f035"><code>ff69b3f</code></a> allow process to exist and cancel timeout again</li>
<li><a href="https://github.com/webpack/webpack/commit/20da4b1ef83cd86480abc19206faebfe477b0a15"><code>20da4b1</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14244">#14244</a> from webpack/revert-14175-ci/node-version</li>
<li><a href="https://github.com/webpack/webpack/commit/562f17a8c04be426cb6ec9be474a37fb4dd2f6f7"><code>562f17a</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14212">#14212</a> from webpack/fix-14210</li>
<li><a href="https://github.com/webpack/webpack/commit/76bdcbfee7645e15e3a56ff4659935882f4b9773"><code>76bdcbf</code></a> Revert &quot;fix node.js because of v8 bug&quot;</li>
<li><a href="https://github.com/webpack/webpack/commit/3e3b528e547f5b67992b1bcdd5ae2ff108c210c3"><code>3e3b528</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14211">#14211</a> from webpack/fix-13557</li>
<li><a href="https://github.com/webpack/webpack/commit/5592f6616f4d361a24f5ad39b25cf7987f87f30f"><code>5592f66</code></a> add experiments.futureDefaults</li>
<li><a href="https://github.com/webpack/webpack/commit/200ce6248a45d53a19fd2e4c124b75e2ccd78ee4"><code>200ce62</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14145">#14145</a> from webpack/dependabot/npm_and_yarn/simple-git-2.45.1</li>
<li><a href="https://github.com/webpack/webpack/commit/e91262cad7c7dc67e04b3c88aa4e2bab3462d5bb"><code>e91262c</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13986">#13986</a> from webpack/dependabot/npm_and_yarn/types/jest-27.0.1</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.53.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.53.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-09-17 08:14:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2988" class=".btn">#2988</a>
            </td>
            <td>
                <b>
                    fix: verifiable command building KID from didDoc.VM
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                when didDoc.VM.ID has a #key-X suffix, the kms KID must be built from the VM.Value or VM.JWK() instead of being extracted from VM.ID

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 15:26:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2987" class=".btn">#2987</a>
            </td>
            <td>
                <b>
                    feat: extend support cases for VC BBS derivation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - support embedded contexts: include custom contexts in bbs limited credential template
- support ID being optional: allow json-ld Processor to Frame docs with blank ID

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 06:33:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2986" class=".btn">#2986</a>
            </td>
            <td>
                <b>
                    chore: complete release 0.1.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Firas Qutishat <firas.qutishat@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 20:36:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2985" class=".btn">#2985</a>
            </td>
            <td>
                <b>
                    chore: Release 0.1.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Firas Qutishat <firas.qutishat@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 19:05:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2984" class=".btn">#2984</a>
            </td>
            <td>
                <b>
                    feat: add mediatype profiles and key types to agent-rest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 18:01:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2983" class=".btn">#2983</a>
            </td>
            <td>
                <b>
                    feat: Present proof v3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrii Soluk <isoluchok@gmail.com>
Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 17:56:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2982" class=".btn">#2982</a>
            </td>
            <td>
                <b>
                    chore(deps): bump codecov/codecov-action from 2.0.2 to 2.1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [codecov/codecov-action](https://github.com/codecov/codecov-action) from 2.0.2 to 2.1.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/codecov/codecov-action/releases">codecov/codecov-action's releases</a>.</em></p>
<blockquote>
<h2>v2.1.0</h2>
<h2>2.1.0</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/515">#515</a> Allow specifying version of Codecov uploader</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/499">#499</a> build(deps-dev): bump <code>@​vercel/ncc</code> from 0.29.0 to 0.30.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/508">#508</a> build(deps): bump openpgp from 5.0.0-5 to 5.0.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/514">#514</a> build(deps-dev): bump <code>@​types/node</code> from 16.6.0 to 16.9.0</li>
</ul>
<h2>v2.0.3</h2>
<h2>2.0.3</h2>
<h3>Fixes</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/464">#464</a> Fix wrong link in the readme</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/485">#485</a> fix: Add override OS and linux default to platform</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/447">#447</a> build(deps): bump openpgp from 5.0.0-4 to 5.0.0-5</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/458">#458</a> build(deps-dev): bump eslint from 7.31.0 to 7.32.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/465">#465</a> build(deps-dev): bump <code>@​typescript-eslint/eslint-plugin</code> from 4.28.4 to 4.29.1</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/466">#466</a> build(deps-dev): bump <code>@​typescript-eslint/parser</code> from 4.28.4 to 4.29.1</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/468">#468</a> build(deps-dev): bump <code>@​types/jest</code> from 26.0.24 to 27.0.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/470">#470</a> build(deps-dev): bump <code>@​types/node</code> from 16.4.0 to 16.6.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/472">#472</a> build(deps): bump path-parse from 1.0.6 to 1.0.7</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/473">#473</a> build(deps-dev): bump <code>@​types/jest</code> from 27.0.0 to 27.0.1</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/478">#478</a> build(deps-dev): bump <code>@​typescript-eslint/parser</code> from 4.29.1 to 4.29.2</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/479">#479</a> build(deps-dev): bump <code>@​typescript-eslint/eslint-plugin</code> from 4.29.1 to 4.29.2</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/481">#481</a> build(deps-dev): bump <code>@​types/node</code> from 16.6.0 to 16.6.2</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/483">#483</a> build(deps-dev): bump <code>@​vercel/ncc</code> from 0.29.0 to 0.29.2</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/484">#484</a> build(deps): bump <code>@​actions/core</code> from 1.4.0 to 1.5.0</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/codecov/codecov-action/blob/master/CHANGELOG.md">codecov/codecov-action's changelog</a>.</em></p>
<blockquote>
<h2>2.1.0</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/515">#515</a> Allow specifying version of Codecov uploader</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/499">#499</a> build(deps-dev): bump <code>@​vercel/ncc</code> from 0.29.0 to 0.30.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/508">#508</a> build(deps): bump openpgp from 5.0.0-5 to 5.0.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/514">#514</a> build(deps-dev): bump <code>@​types/node</code> from 16.6.0 to 16.9.0</li>
</ul>
<h2>2.0.3</h2>
<h3>Fixes</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/464">#464</a> Fix wrong link in the readme</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/485">#485</a> fix: Add override OS and linux default to platform</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/447">#447</a> build(deps): bump openpgp from 5.0.0-4 to 5.0.0-5</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/458">#458</a> build(deps-dev): bump eslint from 7.31.0 to 7.32.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/465">#465</a> build(deps-dev): bump <code>@​typescript-eslint/eslint-plugin</code> from 4.28.4 to 4.29.1</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/466">#466</a> build(deps-dev): bump <code>@​typescript-eslint/parser</code> from 4.28.4 to 4.29.1</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/468">#468</a> build(deps-dev): bump <code>@​types/jest</code> from 26.0.24 to 27.0.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/470">#470</a> build(deps-dev): bump <code>@​types/node</code> from 16.4.0 to 16.6.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/472">#472</a> build(deps): bump path-parse from 1.0.6 to 1.0.7</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/473">#473</a> build(deps-dev): bump <code>@​types/jest</code> from 27.0.0 to 27.0.1</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/478">#478</a> build(deps-dev): bump <code>@​typescript-eslint/parser</code> from 4.29.1 to 4.29.2</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/479">#479</a> build(deps-dev): bump <code>@​typescript-eslint/eslint-plugin</code> from 4.29.1 to 4.29.2</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/481">#481</a> build(deps-dev): bump <code>@​types/node</code> from 16.6.0 to 16.6.2</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/483">#483</a> build(deps-dev): bump <code>@​vercel/ncc</code> from 0.29.0 to 0.29.2</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/484">#484</a> build(deps): bump <code>@​actions/core</code> from 1.4.0 to 1.5.0</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/codecov/codecov-action/commit/f32b3a3741e1053eb607407145bc9619351dc93b"><code>f32b3a3</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/515">#515</a> from codecov/specify-version</li>
<li><a href="https://github.com/codecov/codecov-action/commit/72dfd4782ebb39e122c34a1c156c26573f9b412e"><code>72dfd47</code></a> Allow specifying version of Codecov uploader</li>
<li><a href="https://github.com/codecov/codecov-action/commit/46edaeda0ce748dd0d8545e755226bd7d09d57bd"><code>46edaed</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/499">#499</a> from codecov/dependabot/npm_and_yarn/vercel/ncc-0.30.0</li>
<li><a href="https://github.com/codecov/codecov-action/commit/b6fd8cc98b58344afa1069a491dbceae20ea9ed0"><code>b6fd8cc</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/508">#508</a> from codecov/dependabot/npm_and_yarn/openpgp-5.0.0</li>
<li><a href="https://github.com/codecov/codecov-action/commit/07a4e975bb0a7b708fd8c7100cfc330af5857bba"><code>07a4e97</code></a> build(deps-dev): bump <code>@​vercel/ncc</code> from 0.29.0 to 0.30.0</li>
<li><a href="https://github.com/codecov/codecov-action/commit/c071c7087fd09c2f7de288160514795d076f4e1d"><code>c071c70</code></a> build(deps): bump openpgp from 5.0.0-5 to 5.0.0</li>
<li><a href="https://github.com/codecov/codecov-action/commit/f6d4366a4c53a2980bd8577dd75fd2420322c647"><code>f6d4366</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/514">#514</a> from codecov/dependabot/npm_and_yarn/types/node-16.9.0</li>
<li><a href="https://github.com/codecov/codecov-action/commit/2bbefc9105ffc55315a3982cc3c8c0ab019fcace"><code>2bbefc9</code></a> build(deps-dev): bump <code>@​types/node</code> from 16.6.0 to 16.9.0</li>
<li><a href="https://github.com/codecov/codecov-action/commit/5a8bb4701eca7ba3673f21664b887f652c58d0a3"><code>5a8bb47</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/485">#485</a> from codecov/alternate-os</li>
<li><a href="https://github.com/codecov/codecov-action/commit/3e9a2814f275c203e54e7d52a37d6510f7b927c0"><code>3e9a281</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/481">#481</a> from codecov/dependabot/npm_and_yarn/types/node-16.6.2</li>
<li>Additional commits viewable in <a href="https://github.com/codecov/codecov-action/compare/v2.0.2...v2.1.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=codecov/codecov-action&package-manager=github_actions&previous-version=2.0.2&new-version=2.1.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-09-14 08:14:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2981" class=".btn">#2981</a>
            </td>
            <td>
                <b>
                    fix: anchor origin to string
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Firas Qutishat <firas.qutishat@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 15:09:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2980" class=".btn">#2980</a>
            </td>
            <td>
                <b>
                    chore: add anchorOrigin to MethodMetadata
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Firas Qutishat <firas.qutishat@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 14:42:17 +0000 UTC
    </div>
</div>

