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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3003" class=".btn">#3003</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.55.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.55.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/5db30851c7ed007d8f94150ee2c6a1b47d10d388"><code>5db3085</code></a> 5.55.0</li>
<li><a href="https://github.com/webpack/webpack/commit/3a0d5ff8e45eeade8f107c3e67f8ba7e4251a9a1"><code>3a0d5ff</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14350">#14350</a> from webpack/perf/lazy-assign-connections</li>
<li><a href="https://github.com/webpack/webpack/commit/9e4c259cce6301697c7e82c99c23bf0b502f7ecb"><code>9e4c259</code></a> fix some cases where undefined modules are used</li>
<li><a href="https://github.com/webpack/webpack/commit/daa2c3808e57723d7a569688081f75ceef2fd9b2"><code>daa2c38</code></a> lazy assign connections to dependencies</li>
<li><a href="https://github.com/webpack/webpack/commit/449f7ef39b1096bdacd384d917baec954a0aaca2"><code>449f7ef</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14342">#14342</a> from webpack/perf/unsafe-cache</li>
<li><a href="https://github.com/webpack/webpack/commit/8ef452a5b813986ce95b590fc2d51ec510a7ca3c"><code>8ef452a</code></a> disable unsafeCache in test case as changes won't be detected otherwise</li>
<li><a href="https://github.com/webpack/webpack/commit/931d14615fac325ae192b91da4600297af60c458"><code>931d146</code></a> move unsafe cache from NormalModuleFactory to Compilation to skip more proces...</li>
<li><a href="https://github.com/webpack/webpack/commit/da9a987bd208cbf5d8d29e86c49dea7ea98a122d"><code>da9a987</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14341">#14341</a> from webpack/perf/seal</li>
<li><a href="https://github.com/webpack/webpack/commit/17bc78fe7983bd5b59b6fa99eed4646e39cb6b93"><code>17bc78f</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14337">#14337</a> from webpack/dependabot/npm_and_yarn/pretty-format-...</li>
<li><a href="https://github.com/webpack/webpack/commit/224ed2ac0ce8f1a8dae571fd5efe63b5e3bdca3c"><code>224ed2a</code></a> change ModuleGraph storage to WeakMap</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.55.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.55.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-09-29 08:15:54 +0000 UTC
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3001" class=".btn">#3001</a>
            </td>
            <td>
                <b>
                    chore(deps): bump actions/setup-node from 2.4.0 to 2.4.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/setup-node](https://github.com/actions/setup-node) from 2.4.0 to 2.4.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/setup-node/releases">actions/setup-node's releases</a>.</em></p>
<blockquote>
<h2>Add &quot;cache-hit&quot; output</h2>
<p>This release introduces a new output: <code>cache-hit</code> (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/327">#327</a>).</p>
<p>The <code>cache-hit</code> output contains boolean value indicating that an exact match was found for the key. It shows that the action uses already existing cache or not. The output is available only if cache is enabled.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/setup-node/commit/270253e841af726300e85d718a5f606959b2903c"><code>270253e</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/327">#327</a> from WtfJoke/addCacheHitOutPut</li>
<li><a href="https://github.com/actions/setup-node/commit/d1178716dbbe024f9d459612c22072517a781faa"><code>d117871</code></a> Add 'cache-hit' as output</li>
<li><a href="https://github.com/actions/setup-node/commit/041bafb67276a76a9cc88cd8a4e99165e9eb287d"><code>041bafb</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/322">#322</a> from brcrista/brcrista/check-dist</li>
<li><a href="https://github.com/actions/setup-node/commit/996306e892eb8e97c8cfe8226ee043ae86a8f377"><code>996306e</code></a> rm <strong>tests</strong>/verify-no-unstaged-changes.sh</li>
<li><a href="https://github.com/actions/setup-node/commit/85d412253086d787de7add5f46dcf5964224c032"><code>85d4122</code></a> Fix triggers in licensed.yml</li>
<li><a href="https://github.com/actions/setup-node/commit/928244ce450fb5cb7a3cced763a904067e48394c"><code>928244c</code></a> Add check-dist.yml</li>
<li>See full diff in <a href="https://github.com/actions/setup-node/compare/v2.4.0...v2.4.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/setup-node&package-manager=github_actions&previous-version=2.4.0&new-version=2.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-09-28 08:12:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2998" class=".btn">#2998</a>
            </td>
            <td>
                <b>
                    refactor: use Mediatype Profile instead of MediaType as default
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
        Created At 2021-09-23 16:57:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2997" class=".btn">#2997</a>
            </td>
            <td>
                <b>
                    chore(deps): bump axios from 0.21.2 to 0.21.4 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [axios](https://github.com/axios/axios) from 0.21.2 to 0.21.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/releases">axios's releases</a>.</em></p>
<blockquote>
<h2>v0.21.4</h2>
<h3>0.21.4 (September 6, 2021)</h3>
<p>Fixes and Functionality:</p>
<ul>
<li>Fixing JSON transform when data is stringified. Providing backward compatibility and complying to the JSON RFC standard (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4020">#4020</a>)</li>
</ul>
<p>Huge thanks to everyone who contributed to this release via code (authors listed below) or via reviews and triaging on GitHub:</p>
<ul>
<li><a href="https://github.com/gfortaine">Guillaume Fortaine</a></li>
<li><a href="https://github.com/kawanet">Yusuke Kawasaki</a></li>
<li><a href="https://github.com/DigitalBrainJS">Dmitriy Mozgovoy</a></li>
</ul>
<h2>v0.21.3</h2>
<h3>0.21.3 (September 4, 2021)</h3>
<p>Fixes and Functionality:</p>
<ul>
<li>Fixing response interceptor not being called when request interceptor is attached (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4013">#4013</a>)</li>
</ul>
<p>Huge thanks to everyone who contributed to this release via code (authors listed below) or via reviews and triaging on GitHub:</p>
<ul>
<li><a href="https://github.com/nerdbeere">Julian Hollmann</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/blob/master/CHANGELOG.md">axios's changelog</a>.</em></p>
<blockquote>
<h3>0.21.4 (September 6, 2021)</h3>
<p>Fixes and Functionality:</p>
<ul>
<li>Fixing JSON transform when data is stringified. Providing backward compatability and complying to the JSON RFC standard (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4020">#4020</a>)</li>
</ul>
<p>Huge thanks to everyone who contributed to this release via code (authors listed below) or via reviews and triaging on GitHub:</p>
<ul>
<li><a href="https://github.com/axios/axios/blob/master/mailto:jasonsaayman@gmail.com">Jay</a></li>
<li><a href="https://github.com/gfortaine">Guillaume Fortaine</a></li>
<li><a href="https://github.com/kawanet">Yusuke Kawasaki</a></li>
<li><a href="https://github.com/DigitalBrainJS">Dmitriy Mozgovoy</a></li>
</ul>
<h3>0.21.3 (September 4, 2021)</h3>
<p>Fixes and Functionality:</p>
<ul>
<li>Fixing response interceptor not being called when request interceptor is attached (<a href="https://github-redirect.dependabot.com/axios/axios/pull/4013">#4013</a>)</li>
</ul>
<p>Huge thanks to everyone who contributed to this release via code (authors listed below) or via reviews and triaging on GitHub:</p>
<ul>
<li><a href="https://github.com/axios/axios/blob/master/mailto:jasonsaayman@gmail.com">Jay</a></li>
<li><a href="https://github.com/nerdbeere">Julian Hollmann</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/axios/axios/commit/66c46020bd01b39081259ae74edc2afc283818fa"><code>66c4602</code></a> Merge branch 'master' into release/0.21.4</li>
<li><a href="https://github.com/axios/axios/commit/fc15665cc372bc7d2c59901e04c216c590364a67"><code>fc15665</code></a> [Releasing] v0.21.4</li>
<li><a href="https://github.com/axios/axios/commit/c2714f08e5db79382b3e059cb6bd52134b320f7d"><code>c2714f0</code></a> [Updating] incorrect JSON syntax in README.md</li>
<li><a href="https://github.com/axios/axios/commit/0fc7248cc3db1ea0680b7994eb2ab96b8f6e075f"><code>0fc7248</code></a> fix json transform when data is pre-stringified (<a href="https://github-redirect.dependabot.com/axios/axios/issues/4020">#4020</a>)</li>
<li><a href="https://github.com/axios/axios/commit/90205f8ab7f73e6b3a2507bdd67a4f47ef57af9e"><code>90205f8</code></a> Change headers type to string record (<a href="https://github-redirect.dependabot.com/axios/axios/issues/3021">#3021</a>)</li>
<li><a href="https://github.com/axios/axios/commit/92b29d2775bd4cadb3f077fe639fa29c8cf0de8e"><code>92b29d2</code></a> Make the default type of response data never (<a href="https://github-redirect.dependabot.com/axios/axios/issues/3002">#3002</a>)</li>
<li><a href="https://github.com/axios/axios/commit/4eeb3b17e28581e6931ad7b78dcc025cf3f99bc8"><code>4eeb3b1</code></a> Improved type-safety for AxiosRequestConfig (<a href="https://github-redirect.dependabot.com/axios/axios/issues/2995">#2995</a>)</li>
<li><a href="https://github.com/axios/axios/commit/cd7ff042b0b80f6f02e5564d184019131c90cacd"><code>cd7ff04</code></a> Adding HTTP status code to error.toJSON (<a href="https://github-redirect.dependabot.com/axios/axios/issues/2956">#2956</a>)</li>
<li><a href="https://github.com/axios/axios/commit/b5a1a67b3c2b20f5d6e78e7e80297e71da4ab74c"><code>b5a1a67</code></a> Adding nodejs http.request option: insecureHTTPParser (<a href="https://github-redirect.dependabot.com/axios/axios/issues/2930">#2930</a>)</li>
<li><a href="https://github.com/axios/axios/commit/4f25380b3188816300d8ec7cad125d5e9ccf57d8"><code>4f25380</code></a> Exposing the Axios constructor in index.d.ts (<a href="https://github-redirect.dependabot.com/axios/axios/issues/2872">#2872</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/axios/axios/compare/v0.21.2...v0.21.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=axios&package-manager=npm_and_yarn&previous-version=0.21.2&new-version=0.21.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-09-23 08:17:16 +0000 UTC
    </div>
</div>

