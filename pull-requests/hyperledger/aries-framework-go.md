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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3010" class=".btn">#3010</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.58.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.58.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
<h2>v5.58.0</h2>
<h1>Features</h1>
<ul>
<li>add hook for readResource</li>
<li>add <code>diagnostics_channel</code> to node builtins</li>
</ul>
<h1>Performance</h1>
<ul>
<li>improve chunk graph creation performance
<ul>
<li>add cacheUnaffected cache support</li>
</ul>
</li>
<li>remove some caching that makes not difference</li>
<li>improve splitChunks performance</li>
<li>improve chunk conditions performance</li>
</ul>
<h2>v5.57.1</h2>
<h1>Bugfix</h1>
<ul>
<li>fix experiments.cacheUnaffected which broke by last release</li>
</ul>
<h2>v5.57.0</h2>
<h1>Performance</h1>
<ul>
<li>reduce number of hash.update calls</li>
<li>allow ExternalModules to be unsafe cached</li>
<li>improve hashing performance of module lists (StringXor)</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>experiments.cacheUnaffected
<ul>
<li>handle module/chunk id changes correctly</li>
<li>cache modules with async blocks</li>
<li>show errors when using incompatible options</li>
</ul>
</li>
</ul>
<h2>v5.56.1</h2>
<h1>Bugfix</h1>
<ul>
<li>DefinePlugin: fix conflict with older variants of the plugin</li>
</ul>
<h2>v5.56.0</h2>
<h1>Performance</h1>
<ul>
<li>make DefinePlugin rebuild check more efficient performance and memory wise</li>
</ul>
<h2>v5.55.1</h2>
<h1>Bugfixes</h1>
<ul>
<li>fixes for <code>experiments.cacheUnaffected</code>
<ul>
<li>fix accidentically shared mem caches</li>
<li>avoid RuntimeSpecMap in favor of directly setting on memCache</li>
<li>compare references modules when restoring mem cache</li>
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
<li><a href="https://github.com/webpack/webpack/commit/7666277551be32947227e80fb2fccdbbe656254b"><code>7666277</code></a> 5.58.0</li>
<li><a href="https://github.com/webpack/webpack/commit/59581f53acf51c5d22b3e697a3f66bff7bd7de28"><code>59581f5</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14427">#14427</a> from webpack/perf/chunk-combinations</li>
<li><a href="https://github.com/webpack/webpack/commit/0c71073adb4225905eef5829d7a2b61e40cc995b"><code>0c71073</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14426">#14426</a> from Zhangdroid/main</li>
<li><a href="https://github.com/webpack/webpack/commit/049b859879017ad89fefe91b7842b8efd7f66a1e"><code>049b859</code></a> compute depth faster</li>
<li><a href="https://github.com/webpack/webpack/commit/643f1200c0ee610c724d4ee443567c39ff224ec8"><code>643f120</code></a> skip chunk conditions faster</li>
<li><a href="https://github.com/webpack/webpack/commit/0e13c7dea4160f96cad7f26cca93c17ab841de20"><code>0e13c7d</code></a> track chunk combinations for modules</li>
<li><a href="https://github.com/webpack/webpack/commit/e0915a538e23ca53c98fba4acb9a29e589bb832e"><code>e0915a5</code></a> add &quot;diagnostics_channel&quot; to NodeTargetPlugin</li>
<li><a href="https://github.com/webpack/webpack/commit/48ffd04129e2578f88666aec383e1c16357ecc37"><code>48ffd04</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14425">#14425</a> from webpack/feature/hook-read-resource</li>
<li><a href="https://github.com/webpack/webpack/commit/508e8d50f234bc3ab949b6e3db1e646de21486be"><code>508e8d5</code></a> expand readResource hook to cover normal file reading</li>
<li><a href="https://github.com/webpack/webpack/commit/da74127bfeacff017c5d60842351b4136afba794"><code>da74127</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14420">#14420</a> from webpack/perf/remove-caching</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.58.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.58.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-10-08 08:17:05 +0000 UTC
    </div>
</div>

