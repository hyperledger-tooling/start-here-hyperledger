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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3013" class=".btn">#3013</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.58.2 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.58.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
<h2>v5.58.2</h2>
<h1>Bugfixes</h1>
<ul>
<li>fix serialization context passed</li>
<li>fix a bug which caused module duplication when using persistent caching, unsafe cache and memory cache with GC</li>
<li>fix validation of snapshots of non-existing directories</li>
</ul>
<h1>Performance</h1>
<ul>
<li>store a hash in first bits of bigint to workaround v8 hashing: <a href="https://github.com/v8/v8/blob/b704bc0958e2e26305a68e89d215af1aee011148/src/objects/bigint.h#L192-L195">https://github.com/v8/v8/blob/b704bc0958e2e26305a68e89d215af1aee011148/src/objects/bigint.h#L192-L195</a></li>
</ul>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/8a6d156c156282dd3d0ba001187c282402a1177f"><code>8a6d156</code></a> 5.58.2</li>
<li><a href="https://github.com/webpack/webpack/commit/bf0cb5bfc7198e50ee9d3fa7abfc2d03329f3b88"><code>bf0cb5b</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14474">#14474</a> from webpack/bugfix/filesysteminfo-snapshot</li>
<li><a href="https://github.com/webpack/webpack/commit/e26ac7540a4dc10cfb473a5bd952ece2e94a8cfd"><code>e26ac75</code></a> handle non-existing directories</li>
<li><a href="https://github.com/webpack/webpack/commit/1891b64d6bdf3ad719f892f254b2124c8c4f466f"><code>1891b64</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14468">#14468</a> from webpack/bugfix/unsafe-cache-duplication</li>
<li><a href="https://github.com/webpack/webpack/commit/7e9534a67bbacf8aba60c509f1f8012e67eb73eb"><code>7e9534a</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14469">#14469</a> from webpack/perf/hashing-bigint</li>
<li><a href="https://github.com/webpack/webpack/commit/80b1e77705c1810ae7e95dea4453035da2ef652a"><code>80b1e77</code></a> fix duplication due to unsafe cache</li>
<li><a href="https://github.com/webpack/webpack/commit/3fa83c6c77de88b9874ecd06322ada787b90ac25"><code>3fa83c6</code></a> help v8 hashing the bigint</li>
<li><a href="https://github.com/webpack/webpack/commit/2306d13fbc58f48dc2a2ea99a95c24f0b6c3f3c2"><code>2306d13</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14457">#14457</a> from webpack/fix-serialization-context</li>
<li><a href="https://github.com/webpack/webpack/commit/dfbce79f3cbe7b85f1577b27df6cca534f3f1922"><code>dfbce79</code></a> fix: provide correct serialization context</li>
<li><a href="https://github.com/webpack/webpack/commit/2eecffb2739d13d3095568d118ffc0baacec5cd8"><code>2eecffb</code></a> 5.58.1</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.58.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.58.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-10-14 08:17:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3012" class=".btn">#3012</a>
            </td>
            <td>
                <b>
                    feat: OOB create/accept invitation commands use accept/mediatypeprofile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                CreateInvitation:
- Add accept parameter to command
- If accept parameter not present, use agent's first MediaTypeProfile.
  If agent doesn't have any MediaTypeProfile set, default to the aip2 rfc19
  profile, as before.

AcceptInvitation:
- use agent's media type profiles to validate oob accept handshake

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-13 23:02:39 +0000 UTC
    </div>
</div>

