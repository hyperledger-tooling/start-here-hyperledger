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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3011" class=".btn">#3011</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.58.1 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.58.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
<h2>v5.58.1</h2>
<h1>Bugfixes</h1>
<ul>
<li>fix <code>.webpack[]</code> suffix to not execute rules</li>
<li>revert performance optimization that has too large memory usage in large builds</li>
</ul>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/2eecffb2739d13d3095568d118ffc0baacec5cd8"><code>2eecffb</code></a> 5.58.1</li>
<li><a href="https://github.com/webpack/webpack/commit/d106f00db56e5b9a1c2ed43266f1837f846f4ce8"><code>d106f00</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14436">#14436</a> from webpack/revert/chunk-combinations</li>
<li><a href="https://github.com/webpack/webpack/commit/ada210827ac918efeae3d1a7cfc8d2276d448140"><code>ada2108</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14435">#14435</a> from webpack/bugfix/webpack-extension</li>
<li><a href="https://github.com/webpack/webpack/commit/1ee6f808d3688ac80d07d67e65f3d76ec9701938"><code>1ee6f80</code></a> Revert &quot;track chunk combinations for modules&quot;</li>
<li><a href="https://github.com/webpack/webpack/commit/67d6c7a31bd56a0163d78d6e96967fed26fc4a9d"><code>67d6c7a</code></a> fix <code>.webpack[]</code> suffix to not execute rules</li>
<li><a href="https://github.com/webpack/webpack/commit/7666277551be32947227e80fb2fccdbbe656254b"><code>7666277</code></a> 5.58.0</li>
<li><a href="https://github.com/webpack/webpack/commit/59581f53acf51c5d22b3e697a3f66bff7bd7de28"><code>59581f5</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14427">#14427</a> from webpack/perf/chunk-combinations</li>
<li><a href="https://github.com/webpack/webpack/commit/0c71073adb4225905eef5829d7a2b61e40cc995b"><code>0c71073</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14426">#14426</a> from Zhangdroid/main</li>
<li><a href="https://github.com/webpack/webpack/commit/049b859879017ad89fefe91b7842b8efd7f66a1e"><code>049b859</code></a> compute depth faster</li>
<li><a href="https://github.com/webpack/webpack/commit/643f1200c0ee610c724d4ee443567c39ff224ec8"><code>643f120</code></a> skip chunk conditions faster</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.58.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.58.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-10-11 08:18:17 +0000 UTC
    </div>
</div>

