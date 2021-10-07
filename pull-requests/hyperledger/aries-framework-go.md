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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3008" class=".btn">#3008</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.57.1 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.57.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
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
<h2>v5.55.0</h2>
<h1>Performance</h1>
<ul>
<li><code>experiments.cacheUnaffected</code>
<ul>
<li>reduce cache memory usage</li>
<li>make memCache per module</li>
<li>cache ESM reexport computation</li>
</ul>
</li>
<li><code>module.unsafeCache</code>
<ul>
<li>make it faster by moving it to Compilation-level instead of in NormalModuleFactory</li>
<li>omit tracking resolve dependencies since they are not used when unsafe cache is enabled</li>
</ul>
</li>
<li>module graph
<ul>
<li>lazy assign ModuleGraphConnections to Dependencies since that is only accessed when uncached</li>
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
<li><a href="https://github.com/webpack/webpack/commit/0581bb3c1c32bcb3e182a0f732b862a6c5bb7846"><code>0581bb3</code></a> 5.57.1</li>
<li><a href="https://github.com/webpack/webpack/commit/48c3d290c5c49152f0b1fc71ed2388e3a426e9c9"><code>48c3d29</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14413">#14413</a> from webpack/bugfix/cache-unaffected</li>
<li><a href="https://github.com/webpack/webpack/commit/07ad896f7aedee7d32e8247323b54b759b7637e5"><code>07ad896</code></a> bugfix cacheUnaffected</li>
<li><a href="https://github.com/webpack/webpack/commit/e841ab01417f8e1dd6a2533638f848b5ad0c7d16"><code>e841ab0</code></a> 5.57.0</li>
<li><a href="https://github.com/webpack/webpack/commit/9e3e71813f30b716e32fb197a6c331fd6c9c4f56"><code>9e3e718</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14410">#14410</a> from webpack/bugfix/allow-side-effects</li>
<li><a href="https://github.com/webpack/webpack/commit/da098d7872b72415f820510841a8f0263996e460"><code>da098d7</code></a> optimization.sideEffects is compatible with cacheUnaffected</li>
<li><a href="https://github.com/webpack/webpack/commit/56653f827592f72aea0cb5e7bd9c54253363f532"><code>56653f8</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14406">#14406</a> from webpack/bugfix/cache-unaffected-ids</li>
<li><a href="https://github.com/webpack/webpack/commit/f05246efcba907f1ce7e31ff78817e138e1c56d8"><code>f05246e</code></a> use buildInfo instead of hash for cacheUnaffected</li>
<li><a href="https://github.com/webpack/webpack/commit/4c688339be60f229e7fae43446c55a1ff39f6579"><code>4c68833</code></a> run test cases for cacheUnaffected</li>
<li><a href="https://github.com/webpack/webpack/commit/91b69721442d42c03b94307271f0c701004ddf95"><code>91b6972</code></a> add memCache2 for mem caching with module/chunk ids</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.57.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.57.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-10-06 08:18:56 +0000 UTC
    </div>
</div>

