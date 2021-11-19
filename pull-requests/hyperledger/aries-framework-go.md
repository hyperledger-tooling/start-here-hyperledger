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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3063" class=".btn">#3063</a>
            </td>
            <td>
                <b>
                    feat: oobv2 controllers & bdd tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change introduces out-of-band v2 controllers and commands and includes bdd tests
It also removes unused Actions in OOB v2 service

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-19 00:25:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3060" class=".btn">#3060</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.64.1 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.64.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
<h2>v5.64.1</h2>
<h1>Bugfixes</h1>
<ul>
<li>fix regexp in managedPaths to exclude additional slash</li>
<li>make module.accept errorHandler optional in typings</li>
<li>correctly create an async chunk when using a <code>require(...).property</code> in <code>require.ensure</code></li>
<li>fix cleaning of symlinks in <code>output.clean: true</code></li>
<li>fix change detection with <code>unsafeCache</code> within <code>managedPaths</code> (node_modules)</li>
<li>bump webpack-sources for Stack Overflow bugfix</li>
</ul>
<h2>v5.64.0</h2>
<h1>Features</h1>
<ul>
<li>add <code>asyncChunks: boolean</code> option to disable creation of async chunks</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>fix ProfilingPlugin for <code>experiments.backCompat: false</code></li>
</ul>
<h1>Performance</h1>
<ul>
<li>avoid running regexp twice over the file list</li>
</ul>
<h2>v5.63.0</h2>
<h1>Features</h1>
<ul>
<li>allow passing <code>chunkLoading: false</code> to disable on-demand loading</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>fix <code>import 'single-quote'</code> in esm build dependencies</li>
</ul>
<h2>v5.62.2</h2>
<h1>Bugfixes</h1>
<ul>
<li>fix <code>__system_context__</code> injection when using the <code>library</code> option on entrypoint</li>
<li>enable <code>exportsPresence: &quot;error&quot;</code> by default in <code>futureDefaults</code></li>
<li>fix bad performance for a RegExp in Stats printing (with large error messages)</li>
<li>fix <code>exportPresence</code> -&gt; <code>exportsPresence</code> typo</li>
<li>fix a bug with module invalidation when only module id changes with <code>experiments.cacheUnaffected</code></li>
</ul>
<h2>v5.62.1</h2>
<h1>Bugfix</h1>
<ul>
<li>fix invalid generated code when omitting <code>;</code></li>
</ul>
<h2>v5.62.0</h2>
<h1>Features</h1>
<ul>
<li>add options to configure export presence checking</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/3d5503a5b535b89bbdde78535c1839cefd88e4fa"><code>3d5503a</code></a> 5.64.1</li>
<li><a href="https://github.com/webpack/webpack/commit/1f75ab01fea4952a244752769d126b2ebf3d9226"><code>1f75ab0</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14737">#14737</a> from webpack/dependabot/npm_and_yarn/webpack-source...</li>
<li><a href="https://github.com/webpack/webpack/commit/0f90f75a0e1dabc3c5ec15493cf0e9884687c08e"><code>0f90f75</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14736">#14736</a> from webpack/dependabot/npm_and_yarn/terser-5.10.0</li>
<li><a href="https://github.com/webpack/webpack/commit/0fd96aca4f70dcdb74cf7349181d3a1a44107615"><code>0fd96ac</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14735">#14735</a> from webpack/bugfix/unsafe-cache-managed-paths</li>
<li><a href="https://github.com/webpack/webpack/commit/cae22d1888f7aff66dedc44bf3b9206035d2d85e"><code>cae22d1</code></a> fallback to normal snapshotting when managed path optimization fails</li>
<li><a href="https://github.com/webpack/webpack/commit/98ea582bf0553302a6db1fb3c94a04c5f23e3a58"><code>98ea582</code></a> watch package.json for managed directories</li>
<li><a href="https://github.com/webpack/webpack/commit/bbd039a7ac5321cab00193a50664f719a3a45c3c"><code>bbd039a</code></a> update package.json</li>
<li><a href="https://github.com/webpack/webpack/commit/5cba448bfb780a05c19790a604afb8b892ef9717"><code>5cba448</code></a> update snapshot</li>
<li><a href="https://github.com/webpack/webpack/commit/d73bd6996ca2044255d4e6ca8a9b84ba48d4af83"><code>d73bd69</code></a> chore(deps): bump webpack-sources from 3.2.1 to 3.2.2</li>
<li><a href="https://github.com/webpack/webpack/commit/65d795e5a79f66d53146def3e344a35c0f9dd23a"><code>65d795e</code></a> chore(deps-dev): bump terser from 5.9.0 to 5.10.0</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.64.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.64.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-11-16 08:24:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3059" class=".btn">#3059</a>
            </td>
            <td>
                <b>
                    fix: TransactionTime in UnpublishedOperations and PublishedOperations
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
        Created At 2021-11-15 17:47:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3058" class=".btn">#3058</a>
            </td>
            <td>
                <b>
                    feat: Add unpublishedOperations and publishedOperations to DID Doc
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
        Created At 2021-11-15 17:04:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3057" class=".btn">#3057</a>
            </td>
            <td>
                <b>
                    fix: allow payloads of any size in hkdf and pbkdf2 encrypt
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrii Holovko <andriy.holovko@gmail.com>



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-15 16:39:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3056" class=".btn">#3056</a>
            </td>
            <td>
                <b>
                    feat: add support of general key prefixes for LocalKMS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Volodymyr Kubiv <volodymyr.kubiv@euristiq.com>


**Title:**
Add support of general key prefixes for LocalKMS

**Summary:**

Now LocalKMS support not only local key prefix but other prefixes with the form "anyprefixname://".


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-15 11:51:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3055" class=".btn">#3055</a>
            </td>
            <td>
                <b>
                    feat: add target service triggering in OOBv2 invitations
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
        Created At 2021-11-12 21:25:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3054" class=".btn">#3054</a>
            </td>
            <td>
                <b>
                    fix: incorrect DID resolution response from vdr controller
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-12 19:52:13 +0000 UTC
    </div>
</div>

