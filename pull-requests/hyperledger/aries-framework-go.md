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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3007" class=".btn">#3007</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.56.1 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.56.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
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
<h2>v5.54.0</h2>
<h1>Features</h1>
<ul>
<li>improve constant folding to allow to skip more branches for <code>&amp;&amp;</code> <code>||</code> and <code>??</code></li>
<li>allow all hashing using in webpack to be configured with <code>output.hashFunction</code></li>
<li>no longer bailout completely from inner graph analysis when <code>eval</code> is used in a module</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>force bump enhanced-resolve for bugfixes</li>
</ul>
<h1>Performance</h1>
<ul>
<li>reduce number of allocation when creating snapshots</li>
<li>add <code>output.hashFunction: &quot;xxhash64&quot;</code> for a super fast wasm based hash function</li>
<li>improve utf-8 conversion when serializing short strings</li>
<li>improve hashing performance for dependencies</li>
<li>add <code>experiments.cacheUnaffected</code> which caches computations for modules that are unchanged and reference only unchanged modules</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/ed55e200efb0dad7716d509c82a6ed82aee86c51"><code>ed55e20</code></a> 5.56.1</li>
<li><a href="https://github.com/webpack/webpack/commit/835240024d89321095ab9a0cfeff2b8a6ae9eb44"><code>8352400</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14393">#14393</a> from webpack/bugfix/define-plugin</li>
<li><a href="https://github.com/webpack/webpack/commit/ebc25510605783f4133f75d2fbf23be5a3f6b171"><code>ebc2551</code></a> give DefinePlugin a different key to avoid conflicting with different variant...</li>
<li><a href="https://github.com/webpack/webpack/commit/4eb122092d9696ac5286bc2dcf3eacfb901f4fed"><code>4eb1220</code></a> 5.56.0</li>
<li><a href="https://github.com/webpack/webpack/commit/b7f382878e50452d02c7ad1eeaf28f14d40b29ce"><code>b7f3828</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14366">#14366</a> from webpack/perf/define-hash</li>
<li><a href="https://github.com/webpack/webpack/commit/5f22bffdd1d8808a4fe7cc5d65deeb72fb8e4c62"><code>5f22bff</code></a> use a hash instead of a list to track DefinePlugin dependency</li>
<li><a href="https://github.com/webpack/webpack/commit/e78403d6a8d4e682fbd4a0eb58f042866cfde42a"><code>e78403d</code></a> 5.55.1</li>
<li><a href="https://github.com/webpack/webpack/commit/0c3fab62ab340faeccd23d3a5f48f621c2d340db"><code>0c3fab6</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14358">#14358</a> from webpack/bugfix/shared-cache</li>
<li><a href="https://github.com/webpack/webpack/commit/61569e26b9f3783e72756e0c5104cb245f4e6191"><code>61569e2</code></a> compare references modules when restoring mem cache</li>
<li><a href="https://github.com/webpack/webpack/commit/6c6e48c3826216e055c3ee4f99b3cf160d21a47a"><code>6c6e48c</code></a> avoid RuntimeSpecMap in favor of directly setting on memCache</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.56.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.56.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-10-04 08:19:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3005" class=".btn">#3005</a>
            </td>
            <td>
                <b>
                    fix: include status in issue-cred ack
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 19:24:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3004" class=".btn">#3004</a>
            </td>
            <td>
                <b>
                    docs: Added optional multi-tag querying to SPI store query docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 18:54:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3002" class=".btn">#3002</a>
            </td>
            <td>
                <b>
                    feat: support present proof v2 interop with acapy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add present proof ack status
- Separate inbound/outbound message handling in present proof
- Set presentation format attach_id when constructing presentation message
- Use interop-compatible time format for LD signing when in interop mode

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 19:51:54 +0000 UTC
    </div>
</div>

