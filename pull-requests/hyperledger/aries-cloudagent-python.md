---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3093" class=".btn">#3093</a>
            </td>
            <td>
                <b>
                    Draft: Add DIF presentation exchange context and cache document
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2634
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-09 03:51:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3092" class=".btn">#3092</a>
            </td>
            <td>
                <b>
                    1.0.0rc4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The release is (I think) ready to go.  Please review the changelog entry and propose any changes to it -- items that should be highlighted, and breaking changes.

I noticed that a number of the dockerfiles reference a container image for what I assume is the latest release -- `3.9-01.12.1`.  When do those get updated following a release?  I assume they don't happen as part of a release -- or do they?  Should I update those in this PR?

Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 21:33:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3090" class=".btn">#3090</a>
            </td>
            <td>
                <b>
                    :bug: fix IndyAttrValue bad reference in OpenAPI spec
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #3086

See comment for detail: https://github.com/hyperledger/aries-cloudagent-python/issues/3086#issuecomment-2213956023

___

You'll see in the commit logs I first regenerated the OpenAPI spec, to capture all the latest changes since 0.12.1.
Then I upgraded the openapi gen tools to latest versions, which just improves the default model names in a couple cases:
- `IndyProofProofProofsProof_non_revoc_proof` -> `IndyNonRevocProof` 
- `IndyPrimaryProof_eq_proof` -> `IndyEQProof`

No other changes from upgrading the openapi generators to latest versions.

Then, I removed the description metadata from the `IndyAttrValue` field in `DictWithIndyAttrValueSchema`, and regenerated the spec. That solves the bad reference.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 12:43:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3089" class=".btn">#3089</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump mkdocs-material from 9.5.27 to 9.5.28
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [mkdocs-material](https://github.com/squidfunk/mkdocs-material) from 9.5.27 to 9.5.28.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/releases">mkdocs-material's releases</a>.</em></p>
<blockquote>
<h2>mkdocs-material-9.5.28</h2>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7313">#7313</a>: Improved tooltips mounted in sidebar when feature is disabled</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/squidfunk/mkdocs-material/blob/master/CHANGELOG">mkdocs-material's changelog</a>.</em></p>
<blockquote>
<p>mkdocs-material-9.5.28 (2024-07-02)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7313">#7313</a>: Improved tooltips mounted in sidebar when feature is disabled</li>
</ul>
<p>mkdocs-material-9.5.27 (2024-06-16)</p>
<ul>
<li>Updated Estonian translations</li>
</ul>
<p>mkdocs-material-9.5.26 (2024-06-06)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7232">#7232</a>: Tab switches on scroll when linking tabs (9.5.19 regression)</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7230">#7230</a>: Blog author avatar broken when referring to local file</li>
</ul>
<p>mkdocs-material-9.5.25+insiders-4.53.11 (2024-05-27)</p>
<ul>
<li>Fixed projects plugin crashing when serving before building subprojects</li>
</ul>
<p>mkdocs-material-9.5.25 (2024-05-27)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7209">#7209</a>: Tags plugin crashing on numeric tags</li>
</ul>
<p>mkdocs-material-9.5.24+insiders-4.53.10 (2024-05-20)</p>
<ul>
<li>Fixed projects plugin crashing in serve mode when disabled</li>
<li>Fixed projects plugin crashing when building nested projects</li>
</ul>
<p>mkdocs-material-9.5.24+insiders-4.53.9 (2024-05-20)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7191">#7191</a>: Tags listings not rendering when toc_depth is changed</li>
</ul>
<p>mkdocs-material-9.5.24 (2024-05-20)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7187">#7187</a>: Version selector title rendering issue</li>
</ul>
<p>mkdocs-material-9.5.23 (2024-05-15)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7183">#7183</a>: Edge case in anchor navigation when using instant navigation</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/6436">#6436</a>: Version selector not showing version alias</li>
</ul>
<p>mkdocs-material-9.5.22 (2024-05-12)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7170">#7170</a>: Copy button adds empty lines for line spans (9.5.18 regression)</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7160">#7160</a>: Version switching doesn't stay on page (9.5.5 regression)</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/5619">#5619</a>: Links in Mermaid.js diagrams not discernible</li>
</ul>
<p>mkdocs-material-9.5.21 (2024-05-03)</p>
<ul>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7133">#7133</a>: Ensure latest version of Mermaid.js is used</li>
<li>Fixed <a href="https://redirect.github.com/squidfunk/mkdocs-material/issues/7125">#7125</a>: Added warning for dotfiles in info plugin</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/1b78c2c5cc1c430c4923d43d5a5c27c9efffc1b4"><code>1b78c2c</code></a> Prepare 9.5.28 release</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/c5fd98c94e6e6eea3d3db88832827729b10a564f"><code>c5fd98c</code></a> Fixed links in sponsors section</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/fa04d0ca6324282ff11e1033c0743e76ae7f3af4"><code>fa04d0c</code></a> Updated dependencies</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/845fc610b0b65842538997eac8d1c3eb05ac82f7"><code>845fc61</code></a> Fixed improved tooltips mounted when disabled</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/12a8e82837fe400dd1f123e41d75b32987a11744"><code>12a8e82</code></a> Removed all references to polyfill.io</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/436860fe1725b22659aa00e1839763ba220c140b"><code>436860f</code></a> Bump docker/build-push-action from 5 to 6</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/b0484699f7b860751b7926de95e2d30d781b847d"><code>b048469</code></a> Switched to ES2018 target</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/eff555a669d420318151befc4a79bd9f747687da"><code>eff555a</code></a> Updated dependencies</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/610be26e6c9b902c465c313709de7ae9498795f5"><code>610be26</code></a> Updated README</li>
<li><a href="https://github.com/squidfunk/mkdocs-material/commit/f1ffead06ae6858584969462563bb09ab918041f"><code>f1ffead</code></a> Documentation</li>
<li>Additional commits viewable in <a href="https://github.com/squidfunk/mkdocs-material/compare/9.5.27...9.5.28">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mkdocs-material&package-manager=pip&previous-version=9.5.27&new-version=9.5.28)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 11:45:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3088" class=".btn">#3088</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump aries-askar from 0.3.1 to 0.3.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [aries-askar](https://github.com/hyperledger/aries-askar) from 0.3.1 to 0.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperledger/aries-askar/releases">aries-askar's releases</a>.</em></p>
<blockquote>
<h2>v0.3.2</h2>
<h2>What's Changed</h2>
<ul>
<li>chore(js): update to stable 0.2.0 by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/222">hyperledger/aries-askar#222</a></li>
<li>Add Dependabot configuration by <a href="https://github.com/WadeBarnes"><code>@​WadeBarnes</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/223">hyperledger/aries-askar#223</a></li>
<li>build(deps): bump the all-actions group with 7 updates by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/224">hyperledger/aries-askar#224</a></li>
<li>build(deps): bump ip from 2.0.0 to 2.0.1 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/226">hyperledger/aries-askar#226</a></li>
<li>build(deps): bump es5-ext from 0.10.62 to 0.10.64 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/228">hyperledger/aries-askar#228</a></li>
<li>build(deps): bump mio from 0.8.10 to 0.8.11 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/229">hyperledger/aries-askar#229</a></li>
<li>build(deps): bump follow-redirects from 1.15.4 to 1.15.6 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/230">hyperledger/aries-askar#230</a></li>
<li>build(deps): bump the all-actions group with 1 update by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/231">hyperledger/aries-askar#231</a></li>
<li>fix(js): update ffi-napi by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/234">hyperledger/aries-askar#234</a></li>
<li>build(deps): bump a7ul/tar-action from 1.1.3 to 1.2.0 in the all-actions group by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/235">hyperledger/aries-askar#235</a></li>
<li>build(deps): bump whoami from 1.4.1 to 1.5.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/233">hyperledger/aries-askar#233</a></li>
<li>chore: update version for js wrapper by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/236">hyperledger/aries-askar#236</a></li>
<li>fix: correctly serliaize for buffer by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/238">hyperledger/aries-askar#238</a></li>
<li>Build Javascript on multiple platforms by <a href="https://github.com/brianorwhatever"><code>@​brianorwhatever</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/239">hyperledger/aries-askar#239</a></li>
<li>build(deps): bump rustls from 0.21.10 to 0.21.11 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/240">hyperledger/aries-askar#240</a></li>
<li>P256 keys using Secure Enclave and Android StrongBox by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/245">hyperledger/aries-askar#245</a></li>
<li>chore: update minSdkVersion to get the project version or fallback to 21 by <a href="https://github.com/ja-bravo"><code>@​ja-bravo</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/248">hyperledger/aries-askar#248</a></li>
<li>chore: updating dependabot to support gha, TS, JS and rust packages by <a href="https://github.com/rajpalc7"><code>@​rajpalc7</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/249">hyperledger/aries-askar#249</a></li>
<li>chore(js): update version to 0.2.2 by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/243">hyperledger/aries-askar#243</a></li>
<li>fix: Incorrect SQLite expire check by <a href="https://github.com/dkulic"><code>@​dkulic</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/261">hyperledger/aries-askar#261</a></li>
<li>Add python requirements file and update dependabot workflow by <a href="https://github.com/ff137"><code>@​ff137</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/262">hyperledger/aries-askar#262</a></li>
<li>chore(js): add expo example app and move to pnpm by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/247">hyperledger/aries-askar#247</a></li>
<li>build(deps-dev): update pytest requirement from ~=8.2.1 to ~=8.2.2 in /wrappers/python by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/265">hyperledger/aries-askar#265</a></li>
<li>chore: update library versions by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/271">hyperledger/aries-askar#271</a></li>
<li>build: allow action to create release by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/272">hyperledger/aries-askar#272</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/WadeBarnes"><code>@​WadeBarnes</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/223">hyperledger/aries-askar#223</a></li>
<li><a href="https://github.com/brianorwhatever"><code>@​brianorwhatever</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/239">hyperledger/aries-askar#239</a></li>
<li><a href="https://github.com/ja-bravo"><code>@​ja-bravo</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/248">hyperledger/aries-askar#248</a></li>
<li><a href="https://github.com/rajpalc7"><code>@​rajpalc7</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/249">hyperledger/aries-askar#249</a></li>
<li><a href="https://github.com/dkulic"><code>@​dkulic</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/261">hyperledger/aries-askar#261</a></li>
<li><a href="https://github.com/ff137"><code>@​ff137</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/262">hyperledger/aries-askar#262</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2">https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperledger/aries-askar/commit/10f58b3984bf6b2d370b8fb2cd07a0696bd93d2f"><code>10f58b3</code></a> build: allow action to create release</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/cf0586ed0cf28bc5197af40e4760158e79a77458"><code>cf0586e</code></a> chore: update library versions</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/c5ebacad74923a462ad754c5d726a0b069a62ca9"><code>c5ebaca</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/265">#265</a> from hyperledger/dependabot/pip/wrappers/python/pytes...</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/1a2f90a52dc336368334b7f14ebc2605e9f7ccf8"><code>1a2f90a</code></a> Merge branch 'main' into dependabot/pip/wrappers/python/pytest-approx-eq-8.2.2</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/9ff1271d36b73a765a3bd05c99376fa86d454973"><code>9ff1271</code></a> chore(js): add expo example app and move to pnpm (<a href="https://redirect.github.com/hyperledger/aries-askar/issues/247">#247</a>)</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/8923c50c2c7d6daf1cd856a060af2d9b672a258d"><code>8923c50</code></a> build(deps-dev): update pytest requirement in /wrappers/python</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/95a00366e78a5b504433576a8e31ad264dcc0d6f"><code>95a0036</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/262">#262</a> from ff137/add-python-requirements</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/594c2a1d7153cef38cf46e6fb5d41304e1a990da"><code>594c2a1</code></a> Merge branch 'main' into add-python-requirements</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/19034c97e9ab5e9b9d6fb459218c4c3894863836"><code>19034c9</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/261">#261</a> from dkulic/fix/sqlite_expire_check</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/ab33405ea58f37d8a6f68ad53205be2653ca4379"><code>ab33405</code></a> Merge branch 'main' into fix/sqlite_expire_check</li>
<li>Additional commits viewable in <a href="https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=aries-askar&package-manager=pip&previous-version=0.3.1&new-version=0.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 11:45:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3087" class=".btn">#3087</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump ruff from 0.5.0 to 0.5.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.5.0 to 0.5.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>0.5.1</h2>
<h2>Release Notes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement mutable-contextvar-default (B039) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12113">#12113</a>)</li>
<li>[<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12140">#12140</a>)</li>
<li>[<code>pytest</code>] Reverse <code>PT001</code> and <code>PT0023</code> defaults (<a href="https://redirect.github.com/astral-sh/ruff/pull/12106">#12106</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>Enable token-based rules on source with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/11950">#11950</a>)</li>
<li>[<code>flake8-bandit</code>] Detect <code>httpx</code> for <code>S113</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12174">#12174</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY201</code> to include exception deprecations (<a href="https://redirect.github.com/astral-sh/ruff/pull/12065">#12065</a>)</li>
<li>[<code>pylint</code>] Generate autofix for <code>duplicate-bases</code> (<code>PLE0241</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12105">#12105</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Avoid syntax error notification for source code actions (<a href="https://redirect.github.com/astral-sh/ruff/pull/12148">#12148</a>)</li>
<li>Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/pull/12203">#12203</a>)</li>
<li>Fix replacement edit range computation (<a href="https://redirect.github.com/astral-sh/ruff/pull/12171">#12171</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Disable auto-fix when source has syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/12134">#12134</a>)</li>
<li>Fix cache key collisions for paths with separators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12159">#12159</a>)</li>
<li>Make <code>requires-python</code> inference robust to <code>==</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12091">#12091</a>)</li>
<li>Use char-wise width instead of <code>str</code>-width (<a href="https://redirect.github.com/astral-sh/ruff/pull/12135">#12135</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword followed by comma (<a href="https://redirect.github.com/astral-sh/ruff/pull/12136">#12136</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword is followed by a semicolon (<a href="https://redirect.github.com/astral-sh/ruff/pull/12095">#12095</a>)</li>
<li>[<code>pylint</code>] Skip <a href="https://docs.astral.sh/ruff/settings/#lint_dummy-variable-rgx">dummy variables</a> for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12190">#12190</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Remove allocation in <code>parse_identifier</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12103">#12103</a>)</li>
<li>Use <code>CompactString</code> for <code>Identifier</code> AST node (<a href="https://redirect.github.com/astral-sh/ruff/pull/12101">#12101</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/Peiffap"><code>@​Peiffap</code></a></li>
<li><a href="https://github.com/ThomasFaivre"><code>@​ThomasFaivre</code></a></li>
<li><a href="https://github.com/bersace"><code>@​bersace</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/github-actions"><code>@​github-actions</code></a></li>
<li><a href="https://github.com/jkauerl"><code>@​jkauerl</code></a></li>
<li><a href="https://github.com/mkniewallner"><code>@​mkniewallner</code></a></li>
<li><a href="https://github.com/mtsokol"><code>@​mtsokol</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.5.1</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement mutable-contextvar-default (B039) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12113">#12113</a>)</li>
<li>[<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12140">#12140</a>)</li>
<li>[<code>pytest</code>] Reverse <code>PT001</code> and <code>PT0023</code> defaults (<a href="https://redirect.github.com/astral-sh/ruff/pull/12106">#12106</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>Enable token-based rules on source with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/11950">#11950</a>)</li>
<li>[<code>flake8-bandit</code>] Detect <code>httpx</code> for <code>S113</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12174">#12174</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY201</code> to include exception deprecations (<a href="https://redirect.github.com/astral-sh/ruff/pull/12065">#12065</a>)</li>
<li>[<code>pylint</code>] Generate autofix for <code>duplicate-bases</code> (<code>PLE0241</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12105">#12105</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Avoid syntax error notification for source code actions (<a href="https://redirect.github.com/astral-sh/ruff/pull/12148">#12148</a>)</li>
<li>Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/pull/12203">#12203</a>)</li>
<li>Fix replacement edit range computation (<a href="https://redirect.github.com/astral-sh/ruff/pull/12171">#12171</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Disable auto-fix when source has syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/12134">#12134</a>)</li>
<li>Fix cache key collisions for paths with separators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12159">#12159</a>)</li>
<li>Make <code>requires-python</code> inference robust to <code>==</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12091">#12091</a>)</li>
<li>Use char-wise width instead of <code>str</code>-width (<a href="https://redirect.github.com/astral-sh/ruff/pull/12135">#12135</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword followed by comma (<a href="https://redirect.github.com/astral-sh/ruff/pull/12136">#12136</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword is followed by a semicolon (<a href="https://redirect.github.com/astral-sh/ruff/pull/12095">#12095</a>)</li>
<li>[<code>pylint</code>] Skip <a href="https://docs.astral.sh/ruff/settings/#lint_dummy-variable-rgx">dummy variables</a> for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12190">#12190</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Remove allocation in <code>parse_identifier</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12103">#12103</a>)</li>
<li>Use <code>CompactString</code> for <code>Identifier</code> AST node (<a href="https://redirect.github.com/astral-sh/ruff/pull/12101">#12101</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/3a72400202642f0bb340fb2b1d1c31da2b6524dd"><code>3a72400</code></a> Rename publish workflow file extension (<code>yaml</code> -&gt; <code>yml</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/12206">#12206</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1b3bff03300b2c48f0ad6c7bd6b1038e2f1fce5a"><code>1b3bff0</code></a> Bump version to 0.5.1 (<a href="https://redirect.github.com/astral-sh/ruff/issues/12205">#12205</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/0f6f73ecf3c2ebfe5b218edc0765886ccdca6f7f"><code>0f6f73e</code></a> [red-knot] Require that <code>FileSystem</code> objects implement <code>Debug</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12204">#12204</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/7910beecc42b2694890b10011c27a3cbb2db3335"><code>7910bee</code></a> Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/issues/12203">#12203</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f3ccd152e99d6bccfec58275c0b3b2ec3ffd5bdd"><code>f3ccd15</code></a> Revert &quot;Remove <code>--preview</code> as a required argument for <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12053">#12053</a>)&quot;...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1e07bfa3730db9461f51b877bf71ea31e7dd56e4"><code>1e07bfa</code></a> [<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/12140">#12140</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/5e7ba056128c8bc272ab1a2a22c9cb94a5079361"><code>5e7ba05</code></a> docs(*): fix a few typos, consistency issues and links (<a href="https://redirect.github.com/astral-sh/ruff/issues/12193">#12193</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d12570ea006d23a610e2410d9c70c3b3deae717c"><code>d12570e</code></a> docs(options): fix some typos and improve consistency (<a href="https://redirect.github.com/astral-sh/ruff/issues/12191">#12191</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2f3264e148b9cf31e32c3137feb0f5ce9532d85b"><code>2f3264e</code></a> fix(rules): skip dummy variables for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12190">#12190</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e2e0889a303e8ce9953a2eb8a426921d08176c5f"><code>e2e0889</code></a> [red-knot] Add very basic benchmark (<a href="https://redirect.github.com/astral-sh/ruff/issues/12182">#12182</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/0.5.0...0.5.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.5.0&new-version=0.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 11:45:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3085" class=".btn">#3085</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump certifi from 2024.6.2 to 2024.7.4 in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group with 1 update: [certifi](https://github.com/certifi/python-certifi).

Updates `certifi` from 2024.6.2 to 2024.7.4
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/bd8153872e9c6fc98f4023df9c2deaffea2fa463"><code>bd81538</code></a> 2024.07.04 (<a href="https://redirect.github.com/certifi/python-certifi/issues/295">#295</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/06a2cbf21f345563dde6c28b60e29d57e9b210b3"><code>06a2cbf</code></a> Bump peter-evans/create-pull-request from 6.0.5 to 6.1.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/294">#294</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/13bba02b72bac97c432c277158bc04b4d2a6bc23"><code>13bba02</code></a> Bump actions/checkout from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/293">#293</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e8abcd0e62b334c164b95d49fcabdc9ecbca0554"><code>e8abcd0</code></a> Bump pypa/gh-action-pypi-publish from 1.8.14 to 1.9.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/292">#292</a>)</li>
<li>See full diff in <a href="https://github.com/certifi/python-certifi/compare/2024.06.02...2024.07.04">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2024.6.2&new-version=2024.7.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore <dependency name> major version` will close this group update PR and stop Dependabot creating any more for the specific dependency's major version (unless you unignore this specific dependency's major version or upgrade to it yourself)
- `@dependabot ignore <dependency name> minor version` will close this group update PR and stop Dependabot creating any more for the specific dependency's minor version (unless you unignore this specific dependency's minor version or upgrade to it yourself)
- `@dependabot ignore <dependency name>` will close this group update PR and stop Dependabot creating any more for the specific dependency (unless you unignore this specific dependency or upgrade to it yourself)
- `@dependabot unignore <dependency name>` will remove all of the ignore conditions of the specified dependency
- `@dependabot unignore <dependency name> <ignore condition>` will remove the ignore condition of the specified dependency and ignore conditions
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-cloudagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-06 02:17:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3084" class=".btn">#3084</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump certifi from 2024.6.2 to 2024.7.4 in /demo/playground/examples in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /demo/playground/examples with 1 update: [certifi](https://github.com/certifi/python-certifi).

Updates `certifi` from 2024.6.2 to 2024.7.4
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/bd8153872e9c6fc98f4023df9c2deaffea2fa463"><code>bd81538</code></a> 2024.07.04 (<a href="https://redirect.github.com/certifi/python-certifi/issues/295">#295</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/06a2cbf21f345563dde6c28b60e29d57e9b210b3"><code>06a2cbf</code></a> Bump peter-evans/create-pull-request from 6.0.5 to 6.1.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/294">#294</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/13bba02b72bac97c432c277158bc04b4d2a6bc23"><code>13bba02</code></a> Bump actions/checkout from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/293">#293</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e8abcd0e62b334c164b95d49fcabdc9ecbca0554"><code>e8abcd0</code></a> Bump pypa/gh-action-pypi-publish from 1.8.14 to 1.9.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/292">#292</a>)</li>
<li>See full diff in <a href="https://github.com/certifi/python-certifi/compare/2024.06.02...2024.07.04">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2024.6.2&new-version=2024.7.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore <dependency name> major version` will close this group update PR and stop Dependabot creating any more for the specific dependency's major version (unless you unignore this specific dependency's major version or upgrade to it yourself)
- `@dependabot ignore <dependency name> minor version` will close this group update PR and stop Dependabot creating any more for the specific dependency's minor version (unless you unignore this specific dependency's minor version or upgrade to it yourself)
- `@dependabot ignore <dependency name>` will close this group update PR and stop Dependabot creating any more for the specific dependency (unless you unignore this specific dependency or upgrade to it yourself)
- `@dependabot unignore <dependency name>` will remove all of the ignore conditions of the specified dependency
- `@dependabot unignore <dependency name> <ignore condition>` will remove the ignore condition of the specified dependency and ignore conditions
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-cloudagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-06 02:16:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3083" class=".btn">#3083</a>
            </td>
            <td>
                <b>
                    :art: improve record querying logic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Minor amendments that I wanted to include before #3082 was merged.

Expands error handling for the unlikely case where json.loads fails, and improves readability / reduces complexity of nested if conditions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-04 21:58:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3082" class=".btn">#3082</a>
            </td>
            <td>
                <b>
                    :bug: fix storage record pagination with post-filter query params
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Related to: https://github.com/hyperledger/aries-cloudagent-python/issues/3001#issuecomment-2206110085

Marking as draft to first validate things work as expected (testing here: https://github.com/didx-xyz/aries-cloudapi-python/pull/850)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-03 19:25:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3081" class=".btn">#3081</a>
            </td>
            <td>
                <b>
                    Add by_format to terse webhook for presentations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix for issue #3065

Note that this is for the 2.0 presentation protocol only, do we need to apply a similar fix for 1.0?

This adds the `by_format` attribute for all webhooks, not just for status `done`, however the demo requires this to work with terse webhooks (and no additional calls to the api endpoints)

Added `by_format` for issue cred as well - was failing in the demo for json-ld :-(

Makes the terse webhooks slightly less terse, but is required if we want the webhook to contain "enough" info for the controller to respond to.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-03 17:21:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3080" class=".btn">#3080</a>
            </td>
            <td>
                <b>
                    Switch from black to ruff
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Completely removes black from the project in favour of ruff for linting and formatting.

Adjust the decontainer and the github actions workflow.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-03 02:14:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3077" class=".btn">#3077</a>
            </td>
            <td>
                <b>
                    fix: print provision messages when auto-provision is triggered
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It was recently discovered that if you set a static seed, and you have auto-provisioning enabled on the start command, there is no way to get the verkey for the created DID. The verkey is never printed out to the command line and I do not remember there being an API for retrieving the verkey (one of those, "See it once, copy it, or forever lose it" kinds of things).

After this point in the code, the only thing that "provision" enables are the print statements talking about the did/verkey being created as well as some basic profile information. It doesn't trigger any code that would make changes to the system, those lines precede the line I've added.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-02 15:39:58 +0000 UTC
    </div>
</div>

