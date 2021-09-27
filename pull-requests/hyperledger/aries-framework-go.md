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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2999" class=".btn">#2999</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.54.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.54.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
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
<ul>
<li>split fresh created persistent cache files by time to avoid creating very large files</li>
</ul>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/45829826701ff6582ea16bc36376d105ff264c26"><code>4582982</code></a> 5.54.0</li>
<li><a href="https://github.com/webpack/webpack/commit/88978167ea2ee438761179dbbe2e21233dc9d34d"><code>8897816</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14319">#14319</a> from webpack/feature/affected-mem-cache</li>
<li><a href="https://github.com/webpack/webpack/commit/3149e2e63448e4328ca8abc270b10b3790f1642e"><code>3149e2e</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14318">#14318</a> from webpack/feature/hashing</li>
<li><a href="https://github.com/webpack/webpack/commit/d3381768ad7d530bdd7f5f4fa5ba09d17c5e2f91"><code>d338176</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14315">#14315</a> from webpack/dependabot/npm_and_yarn/enhanced-resol...</li>
<li><a href="https://github.com/webpack/webpack/commit/e5cb12197004af846e81835eaf392cab20439087"><code>e5cb121</code></a> bump enhanced-resolve in package.json</li>
<li><a href="https://github.com/webpack/webpack/commit/91480cfbb1c4cc6104c1b88260fb79315ac4c5a0"><code>91480cf</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14320">#14320</a> from webpack/perf/write-strings-cache</li>
<li><a href="https://github.com/webpack/webpack/commit/3b48429eb564061c29d38c15579e00b4c48f13a7"><code>3b48429</code></a> add MemCache for memory caching per module which is invalidated when module o...</li>
<li><a href="https://github.com/webpack/webpack/commit/381614aecc02dffe6032201a628c5c107913c86a"><code>381614a</code></a> cache computation of values passed for hashing</li>
<li><a href="https://github.com/webpack/webpack/commit/629ac95660b18dc71a835fc13c0573fed1cfe043"><code>629ac95</code></a> write short strings more efficient to cache</li>
<li><a href="https://github.com/webpack/webpack/commit/bc6c0854b4bfd1c3e88b33b5a59331e720887f40"><code>bc6c085</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14317">#14317</a> from webpack/feature/hashing</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.54.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.54.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-09-27 08:17:27 +0000 UTC
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2996" class=".btn">#2996</a>
            </td>
            <td>
                <b>
                    fix: dynamic keyType, keyAgreementType and mediaTypeProfiles in bdd tests
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
        Created At 2021-09-23 02:01:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2995" class=".btn">#2995</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack-cli from 4.7.2 to 4.8.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack-cli](https://github.com/webpack/webpack-cli) from 4.7.2 to 4.8.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack-cli/releases">webpack-cli's releases</a>.</em></p>
<blockquote>
<h2>v4.8.0</h2>
<h1><a href="https://github.com/webpack/webpack-cli/compare/webpack-cli@4.7.2...webpack-cli@4.8.0">4.8.0</a> (2021-08-15)</h1>
<h3>Bug Fixes</h3>
<ul>
<li>show default value in help output if available (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2814">#2814</a>) (<a href="https://github.com/webpack/webpack-cli/commit/7f50948bb984821449277d6b5632b98a695eb029">7f50948</a>)</li>
<li>support top multi compiler options (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2874">#2874</a>) (<a href="https://github.com/webpack/webpack-cli/commit/82b1fb7441f04595ac90626235d506f29e5bb107">82b1fb7</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>show possible values for option in help output (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2819">#2819</a>) (<a href="https://github.com/webpack/webpack-cli/commit/828e5c923719982dfc828f9935f65384d6ede2d1">828e5c9</a>)</li>
<li><strong>init-generator:</strong> add ability to specify a package manager of choice (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2769">#2769</a>) (<a href="https://github.com/webpack/webpack-cli/commit/e53f1645c729c3bbcb27ffd41c999ed321f86f9d">e53f164</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack-cli/blob/master/CHANGELOG.md">webpack-cli's changelog</a>.</em></p>
<blockquote>
<h1><a href="https://github.com/webpack/webpack-cli/compare/webpack-cli@4.7.2...webpack-cli@4.8.0">4.8.0</a> (2021-08-15)</h1>
<h3>Bug Fixes</h3>
<ul>
<li>show default value in help output if available (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2814">#2814</a>) (<a href="https://github.com/webpack/webpack-cli/commit/7f50948bb984821449277d6b5632b98a695eb029">7f50948</a>)</li>
<li>support top multi compiler options (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2874">#2874</a>) (<a href="https://github.com/webpack/webpack-cli/commit/82b1fb7441f04595ac90626235d506f29e5bb107">82b1fb7</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>show possible values for option in help output (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2819">#2819</a>) (<a href="https://github.com/webpack/webpack-cli/commit/828e5c923719982dfc828f9935f65384d6ede2d1">828e5c9</a>)</li>
<li><strong>init-generator:</strong> add ability to specify a package manager of choice (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2769">#2769</a>) (<a href="https://github.com/webpack/webpack-cli/commit/e53f1645c729c3bbcb27ffd41c999ed321f86f9d">e53f164</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack-cli/commit/b66fdc010f029f0079c7511557f5460fd555b9c1"><code>b66fdc0</code></a> chore(release): publish new version</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/c6ace9071b2c2a494c778224ad82f9e40248771b"><code>c6ace90</code></a> docs: update <code>SERVE-OPTIONS-v4</code> (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2893">#2893</a>)</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/e16b244d4db646307d02ef75a2264ee963a4d4d0"><code>e16b244</code></a> chore(deps): bump path-parse from 1.0.6 to 1.0.7 (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2890">#2890</a>)</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/f66d01f0e382b0b3ffc753ac7549eb252e19e26c"><code>f66d01f</code></a> fix: using new dev server API for v4 (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2886">#2886</a>)</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/a4c83e9f33c84ebc8f3dc723306c16c98a7d31a5"><code>a4c83e9</code></a> docs: update cli options (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2892">#2892</a>)</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/f8bd91d6e19d2171ee61c82f935491deb38486b9"><code>f8bd91d</code></a> chore(deps): bump url-parse from 1.5.1 to 1.5.3 (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2891">#2891</a>)</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/846ab5798b5e61b800ca29d48535ce68821027ee"><code>846ab57</code></a> chore(deps): bump colorette from 1.2.2 to 1.3.0 (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2888">#2888</a>)</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/0b115a6caf2078577a0e43b06fa7adeee605aa12"><code>0b115a6</code></a> chore(deps-dev): bump webpack from 5.49.0 to 5.50.0 (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2889">#2889</a>)</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/1a337aab3fa4709e3c1cab2b4f8a49f8c1915ea7"><code>1a337aa</code></a> chore(deps-dev): bump <code>@​typescript-eslint/eslint-plugin</code> (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2884">#2884</a>)</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/dfd36abe55980570e829f9c252b1549004423a03"><code>dfd36ab</code></a> chore(deps-dev): bump <code>@​typescript-eslint/parser</code></li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack-cli/compare/webpack-cli@4.7.2...webpack-cli@4.8.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack-cli&package-manager=npm_and_yarn&previous-version=4.7.2&new-version=4.8.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-09-22 08:18:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2994" class=".btn">#2994</a>
            </td>
            <td>
                <b>
                    chore: add error for did not found
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
        Created At 2021-09-22 06:55:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2993" class=".btn">#2993</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump clean-webpack-plugin from 3.0.0 to 4.0.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [clean-webpack-plugin](https://github.com/johnagan/clean-webpack-plugin) from 3.0.0 to 4.0.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/johnagan/clean-webpack-plugin/releases">clean-webpack-plugin's releases</a>.</em></p>
<blockquote>
<h2>v4.0.0</h2>
<p>Changes</p>
<ul>
<li>Added support for NodeJS 14</li>
<li>Added support for webpack 5</li>
</ul>
<p>Breaking changes:</p>
<ul>
<li>Dropped support for NodeJS 8</li>
<li>Dropped support for webpack 3</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/johnagan/clean-webpack-plugin/commit/0207fe42de3da90c30ad492fd1dbe042dec2623b"><code>0207fe4</code></a> moved out of alpha, closes <a href="https://github-redirect.dependabot.com/johnagan/clean-webpack-plugin/issues/199">#199</a></li>
<li><a href="https://github.com/johnagan/clean-webpack-plugin/commit/8190568b36987e901744d9656f6cefa041d18f5a"><code>8190568</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/johnagan/clean-webpack-plugin/issues/195">#195</a> from strootje/update-webpack-v5</li>
<li><a href="https://github.com/johnagan/clean-webpack-plugin/commit/6d8a2323a4700f2e01614c8606d1ed26853a63ce"><code>6d8a232</code></a> updated readme, cleaned up code as per PR suggestions</li>
<li><a href="https://github.com/johnagan/clean-webpack-plugin/commit/a164c19d1a24aba38872e7b56141c7dab419ecac"><code>a164c19</code></a> Merge branch 'master' into update-webpack-v5</li>
<li><a href="https://github.com/johnagan/clean-webpack-plugin/commit/c0749f539df37d8cdb730b39bab3f5cbd836e321"><code>c0749f5</code></a> updated code to not be to strictly typed, webpack fixed their types</li>
<li><a href="https://github.com/johnagan/clean-webpack-plugin/commit/f43ed055eef03dc26fe9839c216000f67e4fee5e"><code>f43ed05</code></a> Removed <code>@​types/webpack</code> dependency. This breaks with webpack 5</li>
<li><a href="https://github.com/johnagan/clean-webpack-plugin/commit/12649d84b8a262b69b0b2cf25a20cb257931d20e"><code>12649d8</code></a> fixed lint issue</li>
<li><a href="https://github.com/johnagan/clean-webpack-plugin/commit/4f7317a2074b1cc9a6f48392cda6609c855b9e25"><code>4f7317a</code></a> refactored code to match styling more, updated webpack typings</li>
<li><a href="https://github.com/johnagan/clean-webpack-plugin/commit/b2dccbbcd626a151772332ec1ba567473458a8c2"><code>b2dccbb</code></a> updated tests to match</li>
<li><a href="https://github.com/johnagan/clean-webpack-plugin/commit/0edf40f773d0868da2f7822beaec5dbb2611146d"><code>0edf40f</code></a> peerdependency correction</li>
<li>Additional commits viewable in <a href="https://github.com/johnagan/clean-webpack-plugin/compare/v3.0.0...v4.0.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=clean-webpack-plugin&package-manager=npm_and_yarn&previous-version=3.0.0&new-version=4.0.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-09-21 08:13:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2992" class=".btn">#2992</a>
            </td>
            <td>
                <b>
                    fix: add interop support to new didexchange key handling
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
        Created At 2021-09-21 00:16:40 +0000 UTC
    </div>
</div>

