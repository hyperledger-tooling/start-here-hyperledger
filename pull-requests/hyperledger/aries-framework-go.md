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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2911" class=".btn">#2911</a>
            </td>
            <td>
                <b>
                    chore(deps): bump actions/setup-node from 2.3.0 to 2.4.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/setup-node](https://github.com/actions/setup-node) from 2.3.0 to 2.4.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/setup-node/releases">actions/setup-node's releases</a>.</em></p>
<blockquote>
<h2>Support caching for mono repos and repositories with complex structure</h2>
<p>This release introduces dependency caching support for mono repos and repositories with complex structure (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/305">#305</a>).</p>
<p>By default, the action searches for the dependency file (<code>package-lock.json</code> or <code>yarn.lock</code>) in the repository root. Use the <code>cache-dependency-path</code> input for cases when multiple dependency files are used, or they are located in different subdirectories. This input supports wildcards or a list of file names for caching multiple dependencies.</p>
<p>Yaml example:</p>
<pre lang="yml"><code>steps:
- uses: actions/checkout@v2
- uses: actions/setup-node@v2
  with:
    node-version: 14
    cache: npm
    cache-dependency-path: 'sub-project/package-lock.json'
</code></pre>
<p>For more examples of using <code>cache-dependency-path</code> input, see the <a href="https://github.com/actions/setup-node/blob/25316bbc1f10ac9d8798711f44914b1cf3c4e954/docs/advanced-usage.md#caching-packages-dependencies">Advanced usage</a> guide.</p>
<h2>Revert temporary fix</h2>
<p>We had to disable pre-cached Node.js usage in the previous version due to the broken image cache. Now cache is fixed, so we can safely enable its usage again.
Thank you for understanding.</p>
<h2>Temporary maintenance fix.</h2>
<p>Temporarily disabled usage of pre-cached Node.js.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/setup-node/commit/25316bbc1f10ac9d8798711f44914b1cf3c4e954"><code>25316bb</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/305">#305</a> from MaksimZhukov/mazhuk/adding-support-for-monorepos</li>
<li><a href="https://github.com/actions/setup-node/commit/76a4cff9ae9abd877db3173c31637296d870a25b"><code>76a4cff</code></a> update readme and dist files</li>
<li><a href="https://github.com/actions/setup-node/commit/a869e7cc2db593443fe4273b3566c2446337c3d1"><code>a869e7c</code></a> Merge branch 'main' of <a href="https://github.com/MaksimZhukov/setup-node">https://github.com/MaksimZhukov/setup-node</a> into mazhuk...</li>
<li><a href="https://github.com/actions/setup-node/commit/a0cdab1110ea1f0f4fb59851ef15f68231289f7b"><code>a0cdab1</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/299">#299</a> from actions/malob/adr-caching-monorepos</li>
<li><a href="https://github.com/actions/setup-node/commit/4d0182af5ead0b7bf53e87e49aa959476f5501d3"><code>4d0182a</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/310">#310</a> from actions/revert-308-v-alsvir/disable-cache-usage-...</li>
<li><a href="https://github.com/actions/setup-node/commit/896ee80599ea831592cc8484629043410040b226"><code>896ee80</code></a> Restore YARN flag</li>
<li><a href="https://github.com/actions/setup-node/commit/d21ecc7c5be116ff576d1e1dd67cf7eefbb22ed3"><code>d21ecc7</code></a> Revert &quot;Temporarily disabled cache usage for v2&quot;</li>
<li><a href="https://github.com/actions/setup-node/commit/d6e3b5539ed7e5ccd26c3459e26c7c817f4e9068"><code>d6e3b55</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/308">#308</a> from actions/v-alsvir/disable-cache-usage-temp-v2</li>
<li><a href="https://github.com/actions/setup-node/commit/db716f881ae727ff1c231028cc3926681f7d2e7b"><code>db716f8</code></a> Add yarn env variable</li>
<li><a href="https://github.com/actions/setup-node/commit/c24389f79e91ba615d93590929027ff3d63575ae"><code>c24389f</code></a> Staging unstaged</li>
<li>Additional commits viewable in <a href="https://github.com/actions/setup-node/compare/v2.3.0...v2.4.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/setup-node&package-manager=github_actions&previous-version=2.3.0&new-version=2.4.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-08-06 08:19:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2909" class=".btn">#2909</a>
            </td>
            <td>
                <b>
                    fix: Fixes DIDs resolution when inbound message received.
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
        Created At 2021-08-05 06:38:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2908" class=".btn">#2908</a>
            </td>
            <td>
                <b>
                    chore(deps): bump tar from 6.1.0 to 6.1.6 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [tar](https://github.com/npm/node-tar) from 6.1.0 to 6.1.6.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/node-tar/commit/9bc1729939eec1c822b528385b1cc513b9888835"><code>9bc1729</code></a> 6.1.6</li>
<li><a href="https://github.com/npm/node-tar/commit/bdf4f5171340b890a62a5e578962ac143d34b3a9"><code>bdf4f51</code></a> fix: properly prefix hard links</li>
<li><a href="https://github.com/npm/node-tar/commit/94b2a740115fdce20f265a029b0404d53c0a18c6"><code>94b2a74</code></a> chore: remove benchmarks from git repo</li>
<li><a href="https://github.com/npm/node-tar/commit/ecaafb4777b7137421f2f0d6f40ab827654f9247"><code>ecaafb4</code></a> update deps</li>
<li><a href="https://github.com/npm/node-tar/commit/bd4691c90478f41b2649a97048199e34927dc046"><code>bd4691c</code></a> 6.1.5</li>
<li><a href="https://github.com/npm/node-tar/commit/d694c4f810d864badf223efa35d24a000d780179"><code>d694c4f</code></a> ci: test on node 16</li>
<li><a href="https://github.com/npm/node-tar/commit/84acbd31288541100910a528e437f901f8012214"><code>84acbd3</code></a> fix(unpack): fix hang on large file on open() fail</li>
<li><a href="https://github.com/npm/node-tar/commit/97c46fcee7e4e7849ea3432086c4537fb6197025"><code>97c46fc</code></a> fix(unpack): always resume parsing after an entry error</li>
<li><a href="https://github.com/npm/node-tar/commit/488ab8c01de69379406d937419fa3e5550e651c0"><code>488ab8c</code></a> chore: WriteEntry cleaner write() handling</li>
<li><a href="https://github.com/npm/node-tar/commit/be89aafd95296e9721e124b77eee7c745e1c1e97"><code>be89aaf</code></a> WriteEntry backpressure</li>
<li>Additional commits viewable in <a href="https://github.com/npm/node-tar/compare/v6.1.0...v6.1.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tar&package-manager=npm_and_yarn&previous-version=6.1.0&new-version=6.1.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-08-04 19:37:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2904" class=".btn">#2904</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.48.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.48.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
<h2>v5.48.0</h2>
<h1>Features</h1>
<ul>
<li>enable import assertions again</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>upgrade webpack-sources for fixes regarding source maps</li>
<li>fix infinite loop in HMR runtime code</li>
</ul>
<h2>v5.47.1</h2>
<h1>Bugfixes</h1>
<ul>
<li>upgrade webpack-sources for a bunch of bugfixes regarding source maps and missing chars in output</li>
</ul>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/67f3aef3c11e2a8d9e7dc1e0300350588ebd7aec"><code>67f3aef</code></a> 5.48.0</li>
<li><a href="https://github.com/webpack/webpack/commit/747c20b9c0d860052bb7952408836d00a56e8776"><code>747c20b</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13815">#13815</a> from xtuc/sven/bump-acorn-import-assertions-1.7.2</li>
<li><a href="https://github.com/webpack/webpack/commit/dad2aca1365e89cc2ed029463e4436899bf75d25"><code>dad2aca</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13911">#13911</a> from webpack/bugfix/webpack-sources</li>
<li><a href="https://github.com/webpack/webpack/commit/1c1af83e12b6ed15f80396fc668efa4bda7586f7"><code>1c1af83</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13877">#13877</a> from axules/bugfix/hot-poll-infinity</li>
<li><a href="https://github.com/webpack/webpack/commit/c3a12b7bb6df0f7b6cc9a6d6fdd1dd3c9740bac0"><code>c3a12b7</code></a> upgrade webpack-sources to 3.2.0</li>
<li><a href="https://github.com/webpack/webpack/commit/551f64a59030c9250fdf97ce05b49d98efb45dab"><code>551f64a</code></a> fix empty updatedModules check</li>
<li><a href="https://github.com/webpack/webpack/commit/b573514987e53fbf248af30b0028540f411147b7"><code>b573514</code></a> fix hot/signal infinity recursion</li>
<li><a href="https://github.com/webpack/webpack/commit/3f353b6ae29ae6d96e0ab86e7233b4c785f99c60"><code>3f353b6</code></a> 5.47.1</li>
<li><a href="https://github.com/webpack/webpack/commit/6b6f4fead714a9c301c30417b49c58aba153aae6"><code>6b6f4fe</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13888">#13888</a> from webpack/bugfix/webpack-sources</li>
<li><a href="https://github.com/webpack/webpack/commit/5fc7008c3e2ade90dc7561a51eceb484ae305453"><code>5fc7008</code></a> update webpack-sources to 3.1.1</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.48.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.48.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-08-03 08:20:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2903" class=".btn">#2903</a>
            </td>
            <td>
                <b>
                    fix: presentation schema filtering respects schema IDs in contexts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2756

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-03 06:16:11 +0000 UTC
    </div>
</div>

