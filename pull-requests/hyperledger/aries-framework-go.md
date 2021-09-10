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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2973" class=".btn">#2973</a>
            </td>
            <td>
                <b>
                    WIP: do not merge. fix: get MyDID and TheirDID when kid is KeyAgreement.ID
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
        Created At 2021-09-09 20:01:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2972" class=".btn">#2972</a>
            </td>
            <td>
                <b>
                    feat: Present Proof v3 - REST API
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
        Created At 2021-09-09 06:54:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2971" class=".btn">#2971</a>
            </td>
            <td>
                <b>
                    feat: Present Proof v3 client implementation
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
        Created At 2021-09-08 06:00:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2970" class=".btn">#2970</a>
            </td>
            <td>
                <b>
                    feat: Present proof v3 service implementation
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
        Created At 2021-09-06 10:25:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2969" class=".btn">#2969</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.52.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.52.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
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
<ul>
<li>correctly keep chunk loading state when the chunk loading logic is HMR updated
<ul>
<li>This fixes some edge cases that e. g. occur when using lazy compilation for entrypoints. It is now able to HMR update that instead of needing a manual reload. Also see fixes in webpack-dev-server@4.</li>
</ul>
</li>
<li>track and resolve symlinks for filesystem snapshotting
<ul>
<li>This fixes some cases of circular <code>yarn link</code>ing of dependencies.</li>
<li>It also fixes some problems when using package managers that use symlinks to deduplicate (e. g. cnpm or pnpm)</li>
</ul>
</li>
<li>pass the resulting module in the callbacks of <code>Compilation.addModuleChain</code> and <code>Compilation.addModuleTree</code></li>
</ul>
<h2>v5.50.0</h2>
<h1>Features</h1>
<ul>
<li>hashbangs (<code>#! ...</code>) are now handled by webpack
<ul>
<li><a href="https://github.com/tc39/proposal-hashbang">https://github.com/tc39/proposal-hashbang</a></li>
</ul>
</li>
</ul>
<h1>Performance</h1>
<ul>
<li>disable cache compression by default as it tend to make performance worse
<ul>
<li>I could still be enabled again for specific scenarios</li>
</ul>
</li>
<li>reduce the number of allocations during cache serialization
<ul>
<li>This improves performance and memory usage</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/4edd3800567f279edd7091af14b3385552a8972f"><code>4edd380</code></a> 5.52.0</li>
<li><a href="https://github.com/webpack/webpack/commit/d05648611aa6f554860a08940c3bf784b499c3a9"><code>d056486</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14134">#14134</a> from webpack/bugfix/webpack-extension</li>
<li><a href="https://github.com/webpack/webpack/commit/a513b1381a6e0248d1b44446a471b0bd6711a9b2"><code>a513b13</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14118">#14118</a> from webpack/bugfix/multiple-module-externals</li>
<li><a href="https://github.com/webpack/webpack/commit/825bbc1b61d562774dbe74ee3a84b4c0920b0a53"><code>825bbc1</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14004">#14004</a> from webpack/dependabot/npm_and_yarn/webpack-cli-4.8.0</li>
<li><a href="https://github.com/webpack/webpack/commit/0d25c2f6889e8dd6199eca94e3a69ae5fee28474"><code>0d25c2f</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14100">#14100</a> from webpack/dependabot/npm_and_yarn/eslint-plugin-...</li>
<li><a href="https://github.com/webpack/webpack/commit/1220f75bc52ed30e4eaee9f887182414d0b64c2a"><code>1220f75</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14126">#14126</a> from webpack/dependabot/npm_and_yarn/core-js-3.17.2</li>
<li><a href="https://github.com/webpack/webpack/commit/8cc4bda0b3f9b0f3241b4c5e0864239d6a306b14"><code>8cc4bda</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14127">#14127</a> from webpack/dependabot/npm_and_yarn/memfs-3.2.4</li>
<li><a href="https://github.com/webpack/webpack/commit/bc117e1e9782c7a267d97f9079816f77108c0c02"><code>bc117e1</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14129">#14129</a> from webpack/dependabot/npm_and_yarn/fork-ts-checke...</li>
<li><a href="https://github.com/webpack/webpack/commit/765101bded6bf9dc9693fac6af18771d11b37eed"><code>765101b</code></a> match resource should not include special <code>.webpack[...]</code> extension</li>
<li><a href="https://github.com/webpack/webpack/commit/2ce5458404fa2db2bf91cec57f91142a2216fbfe"><code>2ce5458</code></a> chore(deps-dev): bump fork-ts-checker-webpack-plugin from 6.3.2 to 6.3.3</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.52.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.52.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-09-04 07:05:12 +0000 UTC
    </div>
</div>

