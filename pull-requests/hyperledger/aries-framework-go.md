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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2881" class=".btn">#2881</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack-cli from 3.3.10 to 4.7.2 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack-cli](https://github.com/webpack/webpack-cli) from 3.3.10 to 4.7.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack-cli/releases">webpack-cli's releases</a>.</em></p>
<blockquote>
<h2>v4.7.2</h2>
<h2><a href="https://github.com/webpack/webpack-cli/compare/webpack-cli@4.7.1...webpack-cli@4.7.2">4.7.2</a> (2021-06-07)</h2>
<p><strong>Note:</strong> Version bump only for package webpack-cli</p>
<h2>v4.7.1</h2>
<h2><a href="https://github.com/webpack/webpack-cli/compare/webpack-cli@4.7.0...webpack-cli@4.7.1">4.7.1</a> (2021-06-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>not found module after ask installation (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2761">#2761</a>) (<a href="https://github.com/webpack/webpack-cli/commit/557ad05ae8168255b57698bdd2d98cbc7b53812d">557ad05</a>)</li>
<li>prettier config (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2719">#2719</a>) (<a href="https://github.com/webpack/webpack-cli/commit/181295fb1b1973c201c221813562219d85b845ae">181295f</a>)</li>
</ul>
<h2>v4.7.0</h2>
<h1><a href="https://github.com/webpack/webpack-cli/compare/webpack-cli@4.6.0...webpack-cli@4.7.0">4.7.0</a> (2021-05-06)</h1>
<h3>Bug Fixes</h3>
<ul>
<li>parsing of empty <code>--env</code> flags (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2643">#2643</a>) (<a href="https://github.com/webpack/webpack-cli/commit/bc12f1a2a833f09a0585050a0f5dd854da188f1d">bc12f1a</a>)</li>
<li>update usage info (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2594">#2594</a>) (<a href="https://github.com/webpack/webpack-cli/commit/9d07d67faf147cbaf0dddb95038403963e5f2afb">9d07d67</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>add <code>create</code> and <code>new</code> alias for <code>init</code> (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2616">#2616</a>) (<a href="https://github.com/webpack/webpack-cli/commit/5a9789db237b7696adfdc9826b0dda749fedfa9a">5a9789d</a>)</li>
<li>add <code>server</code> alias for <code>serve</code> command (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2631">#2631</a>) (<a href="https://github.com/webpack/webpack-cli/commit/c9ee947618c06447bc1f949e4d401e63f737f38d">c9ee947</a>)</li>
<li>add flag to force start finish log (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2566">#2566</a>) (<a href="https://github.com/webpack/webpack-cli/commit/281aad3ee4961f1643453eb1a926e88e0b7f019c">281aad3</a>)</li>
<li>added <code>--no-devtool</code> to webpack v4(<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2603">#2603</a>) (<a href="https://github.com/webpack/webpack-cli/commit/7c6f390a1d64d562065ffc31d8b23d833813ee9d">7c6f390</a>)</li>
<li>added support arguments description (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2659">#2659</a>) (<a href="https://github.com/webpack/webpack-cli/commit/4dfd166f757ce94130bf9b7580f2dbe2868b8f4f">4dfd166</a>)</li>
</ul>
<h2>v4.6.0</h2>
<h1><a href="https://github.com/webpack/webpack-cli/compare/webpack-cli@4.5.0...webpack-cli@4.6.0">4.6.0</a> (2021-03-27)</h1>
<h3>Bug Fixes</h3>
<ul>
<li><code>negative</code> options (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2555">#2555</a>) (<a href="https://github.com/webpack/webpack-cli/commit/f26ebc105e140992639864fa01950454abd716ac">f26ebc1</a>)</li>
<li>improve error message for help (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2482">#2482</a>) (<a href="https://github.com/webpack/webpack-cli/commit/99ae2a3b9f7ad8c1807839357360a1b4607865b1">99ae2a3</a>)</li>
<li>show <code>--node-env</code> in minimum help output (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2411">#2411</a>) (<a href="https://github.com/webpack/webpack-cli/commit/f5fc3023121f4d952a166879a46b2653c20b6349">f5fc302</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>added <code>WEBPACK_PACKAGE</code> env var to use custom <code>webpack</code> package (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2556">#2556</a>) (<a href="https://github.com/webpack/webpack-cli/commit/3d1e4855c55a6601d8a89dcb50d9d842009e3cda">3d1e485</a>)</li>
<li>added <code>WEBPACK_CLI_SKIP_IMPORT_LOCAL</code> env var to skip local import (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2546">#2546</a>) (<a href="https://github.com/webpack/webpack-cli/commit/e13082221c2da01d8b8215ebc936474bf3ca1582">e130822</a>)</li>
<li>allow string value for the <code>--hot</code> option (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2444">#2444</a>) (<a href="https://github.com/webpack/webpack-cli/commit/8656e78d788bc8a504258d4dcc609767f63d60c4">8656e78</a>)</li>
<li>display used config path when logging level=log (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2431">#2431</a>) (<a href="https://github.com/webpack/webpack-cli/commit/f8406e1c5253849fad741eb45f1ece23a7c603f4">f8406e1</a>)</li>
</ul>
<h2>v4.5.0</h2>
<h1><a href="https://github.com/webpack/webpack-cli/compare/webpack-cli@4.4.0...webpack-cli@4.5.0">4.5.0</a> (2021-02-02)</h1>
<h3>Notes</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack-cli/blob/master/CHANGELOG.md">webpack-cli's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/webpack/webpack-cli/compare/webpack-cli@4.7.1...webpack-cli@4.7.2">4.7.2</a> (2021-06-07)</h2>
<p><strong>Note:</strong> Version bump only for package webpack-cli (due <code>@webpack-cli/serve</code>)</p>
<h2><a href="https://github.com/webpack/webpack-cli/compare/webpack-cli@4.7.0...webpack-cli@4.7.1">4.7.1</a> (2021-06-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>not found module after ask installation (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2761">#2761</a>) (<a href="https://github.com/webpack/webpack-cli/commit/557ad05ae8168255b57698bdd2d98cbc7b53812d">557ad05</a>)</li>
<li>prettier config (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2719">#2719</a>) (<a href="https://github.com/webpack/webpack-cli/commit/181295fb1b1973c201c221813562219d85b845ae">181295f</a>)</li>
</ul>
<h1><a href="https://github.com/webpack/webpack-cli/compare/webpack-cli@4.6.0...webpack-cli@4.7.0">4.7.0</a> (2021-05-06)</h1>
<h3>Bug Fixes</h3>
<ul>
<li>parsing of empty <code>--env</code> flags (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2643">#2643</a>) (<a href="https://github.com/webpack/webpack-cli/commit/bc12f1a2a833f09a0585050a0f5dd854da188f1d">bc12f1a</a>)</li>
<li>update usage info (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2594">#2594</a>) (<a href="https://github.com/webpack/webpack-cli/commit/9d07d67faf147cbaf0dddb95038403963e5f2afb">9d07d67</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>add <code>create</code> and <code>new</code> alias for <code>init</code> (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2616">#2616</a>) (<a href="https://github.com/webpack/webpack-cli/commit/5a9789db237b7696adfdc9826b0dda749fedfa9a">5a9789d</a>)</li>
<li>add <code>server</code> alias for <code>serve</code> command (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2631">#2631</a>) (<a href="https://github.com/webpack/webpack-cli/commit/c9ee947618c06447bc1f949e4d401e63f737f38d">c9ee947</a>)</li>
<li>add flag to force start finish log (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2566">#2566</a>) (<a href="https://github.com/webpack/webpack-cli/commit/281aad3ee4961f1643453eb1a926e88e0b7f019c">281aad3</a>)</li>
<li>added <code>--no-devtool</code> to webpack v4(<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2603">#2603</a>) (<a href="https://github.com/webpack/webpack-cli/commit/7c6f390a1d64d562065ffc31d8b23d833813ee9d">7c6f390</a>)</li>
<li>added support arguments description (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2659">#2659</a>) (<a href="https://github.com/webpack/webpack-cli/commit/4dfd166f757ce94130bf9b7580f2dbe2868b8f4f">4dfd166</a>)</li>
</ul>
<h1><a href="https://github.com/webpack/webpack-cli/compare/webpack-cli@4.5.0...webpack-cli@4.6.0">4.6.0</a> (2021-03-27)</h1>
<h3>Bug Fixes</h3>
<ul>
<li><code>negative</code> options (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2555">#2555</a>) (<a href="https://github.com/webpack/webpack-cli/commit/f26ebc105e140992639864fa01950454abd716ac">f26ebc1</a>)</li>
<li>improve error message for help (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2482">#2482</a>) (<a href="https://github.com/webpack/webpack-cli/commit/99ae2a3b9f7ad8c1807839357360a1b4607865b1">99ae2a3</a>)</li>
<li>show <code>--node-env</code> in minimum help output (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2411">#2411</a>) (<a href="https://github.com/webpack/webpack-cli/commit/f5fc3023121f4d952a166879a46b2653c20b6349">f5fc302</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>added <code>WEBPACK_PACKAGE</code> env var to use custom <code>webpack</code> package (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2556">#2556</a>) (<a href="https://github.com/webpack/webpack-cli/commit/3d1e4855c55a6601d8a89dcb50d9d842009e3cda">3d1e485</a>)</li>
<li>added <code>WEBPACK_CLI_SKIP_IMPORT_LOCAL</code> env var to skip local import (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2546">#2546</a>) (<a href="https://github.com/webpack/webpack-cli/commit/e13082221c2da01d8b8215ebc936474bf3ca1582">e130822</a>)</li>
<li>allow string value for the <code>--hot</code> option (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2444">#2444</a>) (<a href="https://github.com/webpack/webpack-cli/commit/8656e78d788bc8a504258d4dcc609767f63d60c4">8656e78</a>)</li>
<li>display used config path when logging level=log (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2431">#2431</a>) (<a href="https://github.com/webpack/webpack-cli/commit/f8406e1c5253849fad741eb45f1ece23a7c603f4">f8406e1</a>)</li>
</ul>
<h1><a href="https://github.com/webpack/webpack-cli/compare/webpack-cli@4.4.0...webpack-cli@4.5.0">4.5.0</a> (2021-02-02)</h1>
<h3>Notes</h3>
<ul>
<li>now you can use <code>webpack.config.mjs</code> and <code>webpack.config.js</code> with <code>{ &quot;type&quot;: &quot;module&quot; }</code> in <code>package.json</code></li>
<li>you can avoid using the <code>cross-env</code> package:</li>
</ul>
<p>Before:</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack-cli/commit/68ef0563afd105652dc0fd0b2391a0a766cd24fe"><code>68ef056</code></a> chore(release): publish new version</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/2d7ab3549c429193b4ed5fbc6174153c847e0330"><code>2d7ab35</code></a> fix: broken serve with new CLI API (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2770">#2770</a>)</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/060268b770c9623e457afc849e3933364914951d"><code>060268b</code></a> docs: update CHANGELOG</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/2be9b9254009598e021b830091fba8832dfdb57b"><code>2be9b92</code></a> chore(release): publish new version</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/598008a0a3e90ea8dd8c415a3c08700b750774b5"><code>598008a</code></a> chore(deps-dev): bump ts-jest from 27.0.2 to 27.0.3 (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2764">#2764</a>)</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/625b4fd88ab38f3381c3fbd2df3ae2d813fe784f"><code>625b4fd</code></a> chore(deps-dev): bump prettier from 2.3.0 to 2.3.1 (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2765">#2765</a>)</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/bb7c9d3c9b0dca11242e2febcd41805c063e1317"><code>bb7c9d3</code></a> feat: new CLI options API for serve (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2754">#2754</a>)</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/557ad05ae8168255b57698bdd2d98cbc7b53812d"><code>557ad05</code></a> fix: not found module after ask installation (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2761">#2761</a>)</li>
<li><a href="https://github.com/webpack/webpack-cli/commit/c8fef37c06874d62479e65145f764cd72dc3a82e"><code>c8fef37</code></a> chore(deps-dev): bump <code>@​typescript-eslint/parser</code></li>
<li><a href="https://github.com/webpack/webpack-cli/commit/368778d128474dad7a0a341985ee31e35d10a697"><code>368778d</code></a> fix: add node 16 to CI (<a href="https://github-redirect.dependabot.com/webpack/webpack-cli/issues/2760">#2760</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack-cli/compare/v3.3.10...webpack-cli@4.7.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~evilebottnawi">evilebottnawi</a>, a new releaser for webpack-cli since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack-cli&package-manager=npm_and_yarn&previous-version=3.3.10&new-version=4.7.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-07-14 22:13:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2880" class=".btn">#2880</a>
            </td>
            <td>
                <b>
                    chore: disable dependabot PRs on gomod
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - the other gomod in the repo need to be updated in sync.

Signed-off-by: Troy Ronda <troy@troyronda.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 20:37:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2879" class=".btn">#2879</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump file-loader from 5.0.2 to 6.2.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [file-loader](https://github.com/webpack-contrib/file-loader) from 5.0.2 to 6.2.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack-contrib/file-loader/releases">file-loader's releases</a>.</em></p>
<blockquote>
<h2>v6.2.0</h2>
<h2><a href="https://github.com/webpack-contrib/file-loader/compare/v6.1.1...v6.2.0">6.2.0</a> (2020-10-27)</h2>
<h3>Features</h3>
<ul>
<li>added the <code>sourceFilename</code> property to asset info with original filename (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/393">#393</a>) (<a href="https://github.com/webpack-contrib/file-loader/commit/654e0d641ec067089f6a2d12e30ec3520f00d808">654e0d6</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>immutable flag when the <code>name</code> option have hash in query string (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/392">#392</a>) (<a href="https://github.com/webpack-contrib/file-loader/commit/381d8bda3f2494487bfe840386e365b97b6025fe">381d8bd</a>)</li>
</ul>
<h2>v6.1.1</h2>
<h3><a href="https://github.com/webpack-contrib/file-loader/compare/v6.1.0...v6.1.1">6.1.1</a> (2020-10-09)</h3>
<h3>Chore</h3>
<ul>
<li>update <code>schema-utils</code></li>
</ul>
<h2>v6.1.0</h2>
<h2><a href="https://github.com/webpack-contrib/file-loader/compare/v6.0.0...v6.1.0">6.1.0</a> (2020-08-31)</h2>
<h3>Features</h3>
<ul>
<li>pass immutable flag to asset info (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/383">#383</a>) (<a href="https://github.com/webpack-contrib/file-loader/commit/40fcde81681d4f8ee19d2ee3845fd34e24459195">40fcde8</a>)</li>
</ul>
<h2>v6.0.0</h2>
<h2><a href="https://github.com/webpack-contrib/file-loader/compare/v5.1.0...v6.0.0">6.0.0</a> (2020-03-17)</h2>
<h3>⚠ BREAKING CHANGES</h3>
<ul>
<li>use <code>md4</code> by default for hashing (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/369">#369</a>) (<a href="https://github.com/webpack-contrib/file-loader/commit/ad3902284d28adeddf667212a39faa4c6bfb2964">ad39022</a>)</li>
</ul>
<h2>v5.1.0</h2>
<h2><a href="https://github.com/webpack-contrib/file-loader/compare/v5.0.2...v5.1.0">5.1.0</a> (2020-02-19)</h2>
<h3>Features</h3>
<ul>
<li>support the <code>query</code> template for the <code>name</code> option (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/366">#366</a>) (<a href="https://github.com/webpack-contrib/file-loader/commit/cd8698b1d9fd560d85e912acca9a1e24f00e18f8">cd8698b</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/webpack-contrib/file-loader/blob/master/CHANGELOG.md">file-loader's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/webpack-contrib/file-loader/compare/v6.1.1...v6.2.0">6.2.0</a> (2020-10-27)</h2>
<h3>Features</h3>
<ul>
<li>added the <code>sourceFilename</code> property to asset info with original filename (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/393">#393</a>) (<a href="https://github.com/webpack-contrib/file-loader/commit/654e0d641ec067089f6a2d12e30ec3520f00d808">654e0d6</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>immutable flag when the <code>name</code> option have hash in query string (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/392">#392</a>) (<a href="https://github.com/webpack-contrib/file-loader/commit/381d8bda3f2494487bfe840386e365b97b6025fe">381d8bd</a>)</li>
</ul>
<h3><a href="https://github.com/webpack-contrib/file-loader/compare/v6.1.0...v6.1.1">6.1.1</a> (2020-10-09)</h3>
<h3>Chore</h3>
<ul>
<li>update <code>schema-utils</code></li>
</ul>
<h2><a href="https://github.com/webpack-contrib/file-loader/compare/v6.0.0...v6.1.0">6.1.0</a> (2020-08-31)</h2>
<h3>Features</h3>
<ul>
<li>pass immutable flag to asset info (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/383">#383</a>) (<a href="https://github.com/webpack-contrib/file-loader/commit/40fcde81681d4f8ee19d2ee3845fd34e24459195">40fcde8</a>)</li>
</ul>
<h2><a href="https://github.com/webpack-contrib/file-loader/compare/v5.1.0...v6.0.0">6.0.0</a> (2020-03-17)</h2>
<h3>⚠ BREAKING CHANGES</h3>
<ul>
<li>use <code>md4</code> by default for hashing (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/369">#369</a>) (<a href="https://github.com/webpack-contrib/file-loader/commit/ad3902284d28adeddf667212a39faa4c6bfb2964">ad39022</a>)</li>
</ul>
<h2><a href="https://github.com/webpack-contrib/file-loader/compare/v5.0.2...v5.1.0">5.1.0</a> (2020-02-19)</h2>
<h3>Features</h3>
<ul>
<li>support the <code>query</code> template for the <code>name</code> option (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/366">#366</a>) (<a href="https://github.com/webpack-contrib/file-loader/commit/cd8698b1d9fd560d85e912acca9a1e24f00e18f8">cd8698b</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack-contrib/file-loader/commit/c423008dce1b16e1253b89b792f03774ffeb47de"><code>c423008</code></a> chore(release): 6.2.0</li>
<li><a href="https://github.com/webpack-contrib/file-loader/commit/654e0d641ec067089f6a2d12e30ec3520f00d808"><code>654e0d6</code></a> feat: added the <code>sourceFilename</code> property to asset info with original filenam...</li>
<li><a href="https://github.com/webpack-contrib/file-loader/commit/381d8bda3f2494487bfe840386e365b97b6025fe"><code>381d8bd</code></a> fix: immutable flag when the <code>name</code> option have hash in query string (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/392">#392</a>)</li>
<li><a href="https://github.com/webpack-contrib/file-loader/commit/14ed4c9b47f2e580f5b04b71f742cafe9e554565"><code>14ed4c9</code></a> ci: updated webpack versions (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/389">#389</a>)</li>
<li><a href="https://github.com/webpack-contrib/file-loader/commit/6fadfbe9fe43ca86095c836a3c521dfbbac408aa"><code>6fadfbe</code></a> chore(release): 6.1.1</li>
<li><a href="https://github.com/webpack-contrib/file-loader/commit/60508cf17c2689a8c96d8f56ffc6bbc0ed82d553"><code>60508cf</code></a> chore(deps): update</li>
<li><a href="https://github.com/webpack-contrib/file-loader/commit/25e2668f75ae3e8f78adeb99297caa258b2479f3"><code>25e2668</code></a> chore(release): 6.1.0</li>
<li><a href="https://github.com/webpack-contrib/file-loader/commit/6e22f6e78fe17eea052a20a0b417640035e919b3"><code>6e22f6e</code></a> test: fix</li>
<li><a href="https://github.com/webpack-contrib/file-loader/commit/40fcde81681d4f8ee19d2ee3845fd34e24459195"><code>40fcde8</code></a> feat: pass immutable flag to asset info (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/383">#383</a>)</li>
<li><a href="https://github.com/webpack-contrib/file-loader/commit/718aef5f992d325945b1d13b675ac8c6d187a3bb"><code>718aef5</code></a> chore(deps): update (<a href="https://github-redirect.dependabot.com/webpack-contrib/file-loader/issues/375">#375</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/webpack-contrib/file-loader/compare/v5.0.2...v6.2.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=file-loader&package-manager=npm_and_yarn&previous-version=5.0.2&new-version=6.2.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-07-14 18:21:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2878" class=".btn">#2878</a>
            </td>
            <td>
                <b>
                    feat: Document loader for agent-mobile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - added document loader as an option for agent mobile

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 15:50:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2877" class=".btn">#2877</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump copy-webpack-plugin from 5.1.2 to 6.4.1 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [copy-webpack-plugin](https://github.com/webpack-contrib/copy-webpack-plugin) from 5.1.2 to 6.4.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack-contrib/copy-webpack-plugin/releases">copy-webpack-plugin's releases</a>.</em></p>
<blockquote>
<h2>v6.4.1</h2>
<h3><a href="https://github.com/webpack-contrib/copy-webpack-plugin/compare/v6.4.0...v6.4.1">6.4.1</a> (2020-12-16)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>compatibility with webpack 4 file system (<a href="https://github-redirect.dependabot.com/webpack-contrib/copy-webpack-plugin/issues/570">#570</a>) (<a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/720026ad0c526e003ab7270f1712fd712d4fdfad">720026a</a>)</li>
</ul>
<h2>v6.4.0</h2>
<h2><a href="https://github.com/webpack-contrib/copy-webpack-plugin/compare/v6.3.2...v6.4.0">6.4.0</a> (2020-12-07)</h2>
<h3>Features</h3>
<ul>
<li>added the <code>info</code> option (<a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/db53937016b7dbf494bc728f00242cd26541f6a3">db53937</a>)</li>
<li>added type <code>Function</code> for the <code>to</code> option (<a href="https://github-redirect.dependabot.com/webpack-contrib/copy-webpack-plugin/issues/563">#563</a>) (<a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/9bc541694c0d0975c59586cedfea4a51d11f5278">9bc5416</a>)</li>
</ul>
<h2>v6.3.2</h2>
<h3><a href="https://github.com/webpack-contrib/copy-webpack-plugin/compare/v6.3.1...v6.3.2">6.3.2</a> (2020-11-19)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>watching directories (<a href="https://github-redirect.dependabot.com/webpack-contrib/copy-webpack-plugin/issues/558">#558</a>) (<a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/7b58fd9a89e9b29578b30cb3119453e78e036ec2">7b58fd9</a>)</li>
</ul>
<h2>v6.3.1</h2>
<h3><a href="https://github.com/webpack-contrib/copy-webpack-plugin/compare/v6.3.0...v6.3.1">6.3.1</a> (2020-11-13)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>watching (<a href="https://github-redirect.dependabot.com/webpack-contrib/copy-webpack-plugin/issues/555">#555</a>) (<a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/b9969230321df68ed235ed1861729837f234750e">b996923</a>)</li>
</ul>
<h2>v6.3.0</h2>
<h2><a href="https://github.com/webpack-contrib/copy-webpack-plugin/compare/v6.2.1...v6.3.0">6.3.0</a> (2020-11-03)</h2>
<h3>Features</h3>
<ul>
<li>added the <code>sourceFilename</code> info (original source filename) to assets info (<a href="https://github-redirect.dependabot.com/webpack-contrib/copy-webpack-plugin/issues/542">#542</a>) (<a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/db2e3bfae9322592c3a9af1e45d25df165b6b4e0">db2e3bf</a>)</li>
<li>persistent cache between compilations (webpack@5 only) (<a href="https://github-redirect.dependabot.com/webpack-contrib/copy-webpack-plugin/issues/541">#541</a>) (<a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/c8924512a34391ce92715a2b61fc4b0b91a9e10f">c892451</a>)</li>
</ul>
<h2>v6.2.1</h2>
<h3><a href="https://github.com/webpack-contrib/copy-webpack-plugin/compare/v6.2.0...v6.2.1">6.2.1</a> (2020-10-09)</h3>
<h3>Chore</h3>
<ul>
<li>update <code>schema-utils</code></li>
</ul>
<h2>v6.2.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/webpack-contrib/copy-webpack-plugin/blob/v6.4.1/CHANGELOG.md">copy-webpack-plugin's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/webpack-contrib/copy-webpack-plugin/compare/v6.4.0...v6.4.1">6.4.1</a> (2020-12-16)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>compatibility with webpack 4 file system (<a href="https://github-redirect.dependabot.com/webpack-contrib/copy-webpack-plugin/issues/570">#570</a>) (<a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/720026ad0c526e003ab7270f1712fd712d4fdfad">720026a</a>)</li>
</ul>
<h2><a href="https://github.com/webpack-contrib/copy-webpack-plugin/compare/v6.3.2...v6.4.0">6.4.0</a> (2020-12-07)</h2>
<h3>Features</h3>
<ul>
<li>added the <code>info</code> option (<a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/db53937016b7dbf494bc728f00242cd26541f6a3">db53937</a>)</li>
<li>added type <code>Function</code> for the <code>to</code> option (<a href="https://github-redirect.dependabot.com/webpack-contrib/copy-webpack-plugin/issues/563">#563</a>) (<a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/9bc541694c0d0975c59586cedfea4a51d11f5278">9bc5416</a>)</li>
</ul>
<h3><a href="https://github.com/webpack-contrib/copy-webpack-plugin/compare/v6.3.1...v6.3.2">6.3.2</a> (2020-11-19)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>watching directories (<a href="https://github-redirect.dependabot.com/webpack-contrib/copy-webpack-plugin/issues/558">#558</a>) (<a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/7b58fd9a89e9b29578b30cb3119453e78e036ec2">7b58fd9</a>)</li>
</ul>
<h3><a href="https://github.com/webpack-contrib/copy-webpack-plugin/compare/v6.3.0...v6.3.1">6.3.1</a> (2020-11-13)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>watching (<a href="https://github-redirect.dependabot.com/webpack-contrib/copy-webpack-plugin/issues/555">#555</a>) (<a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/b9969230321df68ed235ed1861729837f234750e">b996923</a>)</li>
</ul>
<h2><a href="https://github.com/webpack-contrib/copy-webpack-plugin/compare/v6.2.1...v6.3.0">6.3.0</a> (2020-11-03)</h2>
<h3>Features</h3>
<ul>
<li>added the <code>sourceFilename</code> info (original source filename) to assets info (<a href="https://github-redirect.dependabot.com/webpack-contrib/copy-webpack-plugin/issues/542">#542</a>) (<a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/db2e3bfae9322592c3a9af1e45d25df165b6b4e0">db2e3bf</a>)</li>
<li>persistent cache between compilations (webpack@5 only) (<a href="https://github-redirect.dependabot.com/webpack-contrib/copy-webpack-plugin/issues/541">#541</a>) (<a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/c8924512a34391ce92715a2b61fc4b0b91a9e10f">c892451</a>)</li>
</ul>
<h3><a href="https://github.com/webpack-contrib/copy-webpack-plugin/compare/v6.2.0...v6.2.1">6.2.1</a> (2020-10-09)</h3>
<h3>Chore</h3>
<ul>
<li>update <code>schema-utils</code></li>
</ul>
<h2><a href="https://github.com/webpack-contrib/copy-webpack-plugin/compare/v6.1.1...v6.2.0">6.2.0</a> (2020-10-02)</h2>
<h3>Features</h3>
<ul>
<li>use webpack input filesystem (only webpack@5) (<a href="https://github-redirect.dependabot.com/webpack-contrib/copy-webpack-plugin/issues/531">#531</a>) (<a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/6f2f455b9411ac69ef6aa3b953474f1d7fa23808">6f2f455</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/1eceb4bbf906996cb932a532a708c2af50134426"><code>1eceb4b</code></a> chore(release): 6.4.1</li>
<li><a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/720026ad0c526e003ab7270f1712fd712d4fdfad"><code>720026a</code></a> fix: compatibility with webpack 4 file system (<a href="https://github-redirect.dependabot.com/webpack-contrib/copy-webpack-plugin/issues/570">#570</a>)</li>
<li><a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/6c11e21a5460052233dccaad54421daccb3366f3"><code>6c11e21</code></a> chore(release): 6.4.0</li>
<li><a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/db53937016b7dbf494bc728f00242cd26541f6a3"><code>db53937</code></a> feat: added the <code>info</code> option</li>
<li><a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/9bc541694c0d0975c59586cedfea4a51d11f5278"><code>9bc5416</code></a> feat: added type <code>Function</code> for the <code>to</code> option (<a href="https://github-redirect.dependabot.com/webpack-contrib/copy-webpack-plugin/issues/563">#563</a>)</li>
<li><a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/71676457b5257ada0440aca4aea70ba1fceeaac0"><code>7167645</code></a> chore(release): 6.3.2</li>
<li><a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/7b58fd9a89e9b29578b30cb3119453e78e036ec2"><code>7b58fd9</code></a> fix: watching directories (<a href="https://github-redirect.dependabot.com/webpack-contrib/copy-webpack-plugin/issues/558">#558</a>)</li>
<li><a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/521572190800ece87756a4a6cf17f43753092408"><code>5215721</code></a> chore(release): 6.3.1</li>
<li><a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/c92b5ee1671f05b75b74fdb22072dede2cc2fcc3"><code>c92b5ee</code></a> style: default prettier options (<a href="https://github-redirect.dependabot.com/webpack-contrib/copy-webpack-plugin/issues/556">#556</a>)</li>
<li><a href="https://github.com/webpack-contrib/copy-webpack-plugin/commit/b9969230321df68ed235ed1861729837f234750e"><code>b996923</code></a> fix: watching (<a href="https://github-redirect.dependabot.com/webpack-contrib/copy-webpack-plugin/issues/555">#555</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/webpack-contrib/copy-webpack-plugin/compare/v5.1.2...v6.4.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=copy-webpack-plugin&package-manager=npm_and_yarn&previous-version=5.1.2&new-version=6.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-07-12 08:17:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2876" class=".btn">#2876</a>
            </td>
            <td>
                <b>
                    chore(deps): bump actions/setup-node from 1.4.4 to 2.2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/setup-node](https://github.com/actions/setup-node) from 1.4.4 to 2.2.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/setup-node/releases">actions/setup-node's releases</a>.</em></p>
<blockquote>
<h2>Support caching dependencies and LTS aliases</h2>
<p>This release brings two major features:</p>
<ul>
<li>[Support LTS aliases <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/270">#270</a>](<a href="https://github-redirect.dependabot.com/actions/setup-node/pull/270">actions/setup-node#270</a>)</li>
<li>[Implementation of node's caching <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/272">#272</a>](<a href="https://github-redirect.dependabot.com/actions/setup-node/pull/272">actions/setup-node#272</a>)</li>
</ul>
<h3>Supported version syntax</h3>
<p>The <code>node-version</code> input supports the following syntax:</p>
<p>major versions: <code>12</code>, <code>14</code>, <code>16</code><br />
more specific versions: <code>10.15</code>, <code>14.2.0</code>, <code>16.3.0</code><br />
nvm LTS syntax: <code>lts/erbium</code>, <code>lts/fermium</code>, <code>lts/*</code></p>
<h3>Caching dependencies</h3>
<p>The action has a built-in functionality for caching and restoring npm/yarn dependencies. Supported package managers are <code>npm</code>, <code>yarn</code>. The <code>cache</code> input is optional, and caching is turned off by default.</p>
<p><strong>Caching npm dependencies:</strong></p>
<pre lang="yaml"><code>steps:
- uses: actions/checkout@v2
- uses: actions/setup-node@v2
  with:
    node-version: '14'
    cache: 'npm'
- run: npm install
- run: npm test
</code></pre>
<p><strong>Caching yarn dependencies:</strong></p>
<pre lang="yaml"><code>steps:
- uses: actions/checkout@v2
- uses: actions/setup-node@v2
  with:
    node-version: '14'
    cache: 'yarn'
- run: yarn install
- run: yarn test
</code></pre>
<p>Yarn caching handles both yarn versions: 1 or 2.</p>
<blockquote>
<p>At the moment, only <code>lock</code> files in the project root are supported.</p>
</blockquote>
<h2>v2.1.5 Release</h2>
<p>Improve error and warning line number handling (problem matcher regex)</p>
<h2>v2.1.4</h2>
<p>The first stable release of actions/setup-node V2</p>
<h2>v2.1.3 (beta)</h2>
<ul>
<li>Add support for specifying architecture of Node.JS</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/setup-node/commit/38d90ce44d5275ad62cc48384b3d8a58c500bb5f"><code>38d90ce</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/277">#277</a> from actions/malob/update-readme</li>
<li><a href="https://github.com/actions/setup-node/commit/e1e1d4c85364e81d35f092df54e57f47c51f8ad9"><code>e1e1d4c</code></a> Update README.md</li>
<li><a href="https://github.com/actions/setup-node/commit/40f85c8c9749fde9bb1f49ac6f38d0acc30cb80a"><code>40f85c8</code></a> update readme</li>
<li><a href="https://github.com/actions/setup-node/commit/e215578cb0305f14eb5d11939e0f4610ae5bf7e6"><code>e215578</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/272">#272</a> from akv-platform/add-caching-for-node-dependencies</li>
<li><a href="https://github.com/actions/setup-node/commit/9af89732f052e88905c85ff7ab78062ae0c3c536"><code>9af8973</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/274">#274</a> from actions/v-mazhuk/automate-releasing-new-versions</li>
<li><a href="https://github.com/actions/setup-node/commit/cfe70f9fe8ca345bad2e02a88695dd317e6172c0"><code>cfe70f9</code></a> update dependencies</li>
<li><a href="https://github.com/actions/setup-node/commit/b259ba49fed412baf54f73304eba7f06fdfde3ae"><code>b259ba4</code></a> rebuild project</li>
<li><a href="https://github.com/actions/setup-node/commit/55e10498cf770f182fe51eb7f48df9a0a1f7ab0c"><code>55e1049</code></a> Merge branch 'main' into add-caching-for-node-dependencies</li>
<li><a href="https://github.com/actions/setup-node/commit/bcb4cecf9b616a784bae71216cc4707c46b9573f"><code>bcb4cec</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/270">#270</a> from gordey4doronin/gordey/support-lts-syntax</li>
<li><a href="https://github.com/actions/setup-node/commit/72922790cb23732db6a33f911db23457504c50ea"><code>7292279</code></a> fix for documentation</li>
<li>Additional commits viewable in <a href="https://github.com/actions/setup-node/compare/v1.4.4...v2.2.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/setup-node&package-manager=github_actions&previous-version=1.4.4&new-version=2.2.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-07-12 08:16:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2875" class=".btn">#2875</a>
            </td>
            <td>
                <b>
                    chore: update to latest bbs12-381 module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Troy Ronda <troy@troyronda.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-09 16:44:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2874" class=".btn">#2874</a>
            </td>
            <td>
                <b>
                    chore: update kilic bls12-381 fork to latest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Troy Ronda <troy@troyronda.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-09 16:03:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2872" class=".btn">#2872</a>
            </td>
            <td>
                <b>
                    fix: typo fix in didexchange interop did doc attachment signing
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
        Created At 2021-07-09 15:57:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2871" class=".btn">#2871</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.41.5 to 4.46.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.41.5 to 4.46.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
<h2>v4.46.0</h2>
<h1>Bugfixes</h1>
<ul>
<li>fix behavior of defaults for <code>resolve.roots</code> to be backward-compatible</li>
</ul>
<h2>v4.45.0</h2>
<h1>Features</h1>
<ul>
<li>resolve server-relative requests relative to project context by default</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>fix a bug where <code>splitChunk</code> <code>minSize</code> is not handled correctly</li>
<li>fix a bug where the order of <code>splitChunk</code> <code>cacheGroups</code> is not handled correctly</li>
</ul>
<h2>v4.44.2</h2>
<h1>Bugfixes</h1>
<ul>
<li>make sure to generate correct chunk connection for blocks that are only connected in some runtimes
<ul>
<li>fixes a bug where filename contains undefined hash at runtime</li>
</ul>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/444e59f8a427f94f0064cae6765e5a3c4b78596d"><code>444e59f</code></a> 4.46.0</li>
<li><a href="https://github.com/webpack/webpack/commit/758bb253528cf9840eb7eb1bb0f1552d79492f7a"><code>758bb25</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/12387">#12387</a> from webpack/bugfix/12386</li>
<li><a href="https://github.com/webpack/webpack/commit/79de1a2166272ce8692fd1e9cc80a0762b983d22"><code>79de1a2</code></a> enable backward-compatibility for resolve.roots</li>
<li><a href="https://github.com/webpack/webpack/commit/ef75c040709f646f4b9b6b3b5359ca99141c7511"><code>ef75c04</code></a> Fix filename in azure pipeline</li>
<li><a href="https://github.com/webpack/webpack/commit/77149535e8475259e67be0938b7857693e68ad3b"><code>7714953</code></a> add test case</li>
<li><a href="https://github.com/webpack/webpack/commit/03313223fd4a0d4e570b8c79971e61b28cb3aeae"><code>0331322</code></a> 4.45.0</li>
<li><a href="https://github.com/webpack/webpack/commit/e43bb4b956d5f8fe3120c313b226d7c3a084d53f"><code>e43bb4b</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/12372">#12372</a> from webpack/bugfix/split-chunks-min-size-4</li>
<li><a href="https://github.com/webpack/webpack/commit/4de8451af5be200528c11be0bb5641afeaa198cf"><code>4de8451</code></a> fix bug where cacheGroup index was inverted</li>
<li><a href="https://github.com/webpack/webpack/commit/3f69f3c50a7053cd659463221cf6b305812b97db"><code>3f69f3c</code></a> fix bug where module size is added multiple times to the split chunk info</li>
<li><a href="https://github.com/webpack/webpack/commit/c572c15a413ef7d086b52ccc78d9512a192954d7"><code>c572c15</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/11831">#11831</a> from Pyrolistical/patch-1</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.41.5...v4.46.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.41.5&new-version=4.46.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-07-09 15:27:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2870" class=".btn">#2870</a>
            </td>
            <td>
                <b>
                    chore(deps): bump codecov/codecov-action from 1.0.13 to 1.5.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [codecov/codecov-action](https://github.com/codecov/codecov-action) from 1.0.13 to 1.5.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/codecov/codecov-action/releases">codecov/codecov-action's releases</a>.</em></p>
<blockquote>
<h2>v1.5.2</h2>
<h2>1.5.2</h2>
<h3>Fixes</h3>
<ul>
<li>
<h1>fix: Import version properly as string not object</h1>
</li>
</ul>
<h2>v1.5.1</h2>
<h2>1.5.1</h2>
<h3>Fixes</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/320">#320</a> doc: add github actions badge</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/336">#336</a> Update bash uploader to 1.0.3</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/339">#339</a> fix: Add action version</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/302">#302</a> Bump <code>@​typescript-eslint/eslint-plugin</code> from 4.22.0 to 4.22.1</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/303">#303</a> Bump <code>@​typescript-eslint/parser</code> from 4.22.0 to 4.22.1</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/304">#304</a> Bump ts-jest from 26.5.5 to 26.5.6</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/309">#309</a> Bump lodash from 4.17.19 to 4.17.21</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/310">#310</a> Bump hosted-git-info from 2.8.8 to 2.8.9</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/311">#311</a> Bump <code>@​actions/github</code> from 4.0.0 to 5.0.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/314">#314</a> Bump eslint from 7.25.0 to 7.27.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/315">#315</a> Bump <code>@​actions/core</code> from 1.2.7 to 1.3.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/316">#316</a> Bump <code>@​typescript-eslint/parser</code> from 4.22.1 to 4.25.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/317">#317</a> Bump <code>@​typescript-eslint/eslint-plugin</code> from 4.22.1 to 4.25.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/319">#319</a> Bump jest-junit from 12.0.0 to 12.1.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/321">#321</a> Bump typescript from 4.2.4 to 4.3.2</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/323">#323</a> Bump ws from 7.3.1 to 7.4.6</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/331">#331</a> Bump eslint from 7.27.0 to 7.28.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/332">#332</a> Bump <code>@​actions/exec</code> from 1.0.4 to 1.1.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/333">#333</a> Bump <code>@​typescript-eslint/parser</code> from 4.25.0 to 4.26.1</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/334">#334</a> Bump <code>@​typescript-eslint/eslint-plugin</code> from 4.25.0 to 4.26.1</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/335">#335</a> Bump <code>@​actions/core</code> from 1.3.0 to 1.4.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/337">#337</a> Bump glob-parent from 5.1.1 to 5.1.2</li>
</ul>
<h2>v1.5.0</h2>
<h2>1.5.0</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/299">#299</a> Pull Codecov bash script into the action</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/271">#271</a> Bump typescript from 4.2.3 to 4.2.4</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/277">#277</a> Bump <code>@​typescript-eslint/eslint-plugin</code> from 4.16.1 to 4.22.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/278">#278</a> Bump <code>@​typescript-eslint/parser</code> from 4.20.0 to 4.22.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/279">#279</a> Bump <code>@​actions/core</code> from 1.2.6 to 1.2.7</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/292">#292</a> Bump ts-jest from 26.5.3 to 26.5.5</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/293">#293</a> Bump eslint from 7.21.0 to 7.25.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/297">#297</a> Bump <code>@​types/jest</code> from 26.0.20 to 26.0.23</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/298">#298</a> Upgrade to GitHub-native Dependabot</li>
</ul>
<h2>v1.4.1</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/codecov/codecov-action/blob/master/CHANGELOG.md">codecov/codecov-action's changelog</a>.</em></p>
<blockquote>
<h2>1.5.2</h2>
<h3>Fixes</h3>
<ul>
<li>
<h1>fix: Import version properly as string not object</h1>
</li>
</ul>
<h2>1.5.1</h2>
<h3>Fixes</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/320">#320</a> doc: add github actions badge</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/336">#336</a> Update bash uploader to 1.0.3</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/339">#339</a> fix: Add action version</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/302">#302</a> Bump <code>@​typescript-eslint/eslint-plugin</code> from 4.22.0 to 4.22.1</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/303">#303</a> Bump <code>@​typescript-eslint/parser</code> from 4.22.0 to 4.22.1</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/304">#304</a> Bump ts-jest from 26.5.5 to 26.5.6</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/309">#309</a> Bump lodash from 4.17.19 to 4.17.21</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/310">#310</a> Bump hosted-git-info from 2.8.8 to 2.8.9</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/311">#311</a> Bump <code>@​actions/github</code> from 4.0.0 to 5.0.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/314">#314</a> Bump eslint from 7.25.0 to 7.27.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/315">#315</a> Bump <code>@​actions/core</code> from 1.2.7 to 1.3.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/316">#316</a> Bump <code>@​typescript-eslint/parser</code> from 4.22.1 to 4.25.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/317">#317</a> Bump <code>@​typescript-eslint/eslint-plugin</code> from 4.22.1 to 4.25.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/319">#319</a> Bump jest-junit from 12.0.0 to 12.1.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/321">#321</a> Bump typescript from 4.2.4 to 4.3.2</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/323">#323</a> Bump ws from 7.3.1 to 7.4.6</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/331">#331</a> Bump eslint from 7.27.0 to 7.28.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/332">#332</a> Bump <code>@​actions/exec</code> from 1.0.4 to 1.1.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/333">#333</a> Bump <code>@​typescript-eslint/parser</code> from 4.25.0 to 4.26.1</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/334">#334</a> Bump <code>@​typescript-eslint/eslint-plugin</code> from 4.25.0 to 4.26.1</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/335">#335</a> Bump <code>@​actions/core</code> from 1.3.0 to 1.4.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/337">#337</a> Bump glob-parent from 5.1.1 to 5.1.2</li>
</ul>
<h2>1.5.0</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/299">#299</a> Pull Codecov bash script into the action</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/271">#271</a> Bump typescript from 4.2.3 to 4.2.4</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/277">#277</a> Bump <code>@​typescript-eslint/eslint-plugin</code> from 4.16.1 to 4.22.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/278">#278</a> Bump <code>@​typescript-eslint/parser</code> from 4.20.0 to 4.22.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/279">#279</a> Bump <code>@​actions/core</code> from 1.2.6 to 1.2.7</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/292">#292</a> Bump ts-jest from 26.5.3 to 26.5.5</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/293">#293</a> Bump eslint from 7.21.0 to 7.25.0</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/297">#297</a> Bump <code>@​types/jest</code> from 26.0.20 to 26.0.23</li>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/298">#298</a> Upgrade to GitHub-native Dependabot</li>
</ul>
<h2>1.4.1</h2>
<h3>Fixes</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/287">#287</a> Update VERSION regex to restrict on digits and dot and move checksums into script</li>
</ul>
<h2>1.4.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/codecov/codecov-action/commit/29386c70ef20e286228c72b668a06fd0e8399192"><code>29386c7</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/342">#342</a> from codecov/1.5.2</li>
<li><a href="https://github.com/codecov/codecov-action/commit/52497068bd2117dbc668797d4e5a9c1722c041a6"><code>5249706</code></a> fix: Import version properly as string not object</li>
<li><a href="https://github.com/codecov/codecov-action/commit/fbeda37de967cc17491cd6587ec90ab98e3a3da0"><code>fbeda37</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/338">#338</a> from codecov/1.5.1</li>
<li><a href="https://github.com/codecov/codecov-action/commit/ebcf63d8f0a2b5ec95a5edf47b54d7bd6f49d094"><code>ebcf63d</code></a> Update changelog</li>
<li><a href="https://github.com/codecov/codecov-action/commit/a3e633d744fc75e7d36ab1666ee33a884b2acffd"><code>a3e633d</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/339">#339</a> from codecov/action-version</li>
<li><a href="https://github.com/codecov/codecov-action/commit/b8f68524afdfa99b19eb050a7facfe1341594954"><code>b8f6852</code></a> lint</li>
<li><a href="https://github.com/codecov/codecov-action/commit/c9d0b8155c1a7ca4f072a580cdcb3df48a9137a4"><code>c9d0b81</code></a> fix: Add action version</li>
<li><a href="https://github.com/codecov/codecov-action/commit/8f0855a85cc368b858984ca274721562a591ed26"><code>8f0855a</code></a> Bump to 1.5.1</li>
<li><a href="https://github.com/codecov/codecov-action/commit/c53d6ba320e1a46702ab7ccb976e266fd7effb71"><code>c53d6ba</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/337">#337</a> from codecov/dependabot/npm_and_yarn/glob-parent-5.1.2</li>
<li><a href="https://github.com/codecov/codecov-action/commit/67f597a1c4d83f8490454cbad4c43f06cbe2f466"><code>67f597a</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/codecov/codecov-action/issues/336">#336</a> from slarse/update-bash-uploader-to-1.0.3</li>
<li>Additional commits viewable in <a href="https://github.com/codecov/codecov-action/compare/v1.0.13...v1.5.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=codecov/codecov-action&package-manager=github_actions&previous-version=1.0.13&new-version=1.5.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-07-09 14:53:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2869" class=".btn">#2869</a>
            </td>
            <td>
                <b>
                    ci: npm dependabot config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Troy Ronda <troy@troyronda.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-09 14:52:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2867" class=".btn">#2867</a>
            </td>
            <td>
                <b>
                    chore(deps): bump actions/upload-artifact from 1 to 2.2.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/upload-artifact](https://github.com/actions/upload-artifact) from 1 to 2.2.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/upload-artifact/releases">actions/upload-artifact's releases</a>.</em></p>
<blockquote>
<h2>v2.2.4</h2>
<ul>
<li>Retry on HTTP 500 responses from the service</li>
</ul>
<h2>v2.2.3</h2>
<ul>
<li>Fixes for proxy related issues</li>
</ul>
<h2>v2.2.2</h2>
<ul>
<li>Improved retryability and error handling</li>
</ul>
<h2>v2.2.1</h2>
<ul>
<li>Update used actions/core package to the latest version</li>
</ul>
<h2>v2.2.0</h2>
<ul>
<li>Support for artifact retention</li>
</ul>
<h2>v2.1.4</h2>
<ul>
<li>Add Third Party License Information</li>
</ul>
<h2>v2.1.3</h2>
<ul>
<li>Use updated version of the <code>@action/artifact</code> NPM package</li>
</ul>
<h2>v2.1.2</h2>
<ul>
<li>Increase upload chunk size from 4MB to 8MB</li>
<li>Detect case insensitive file uploads</li>
</ul>
<h2>v2.1.1</h2>
<ul>
<li>Fix for certain symlinks not correctly being identified as directories before starting uploads</li>
</ul>
<h2>v2.1.0</h2>
<ul>
<li>Support for uploading artifacts with multiple paths</li>
<li>Support for using exclude paths</li>
<li>Updates to dependencies</li>
</ul>
<h2>v2.0.1</h2>
<ul>
<li>Fixes an issue with uploads unsuccessfully retrying after a connection error has been encountered</li>
<li>Changes to when the action fails
<ul>
<li>Previously if a file failed to upload, the action would continue uploading any remaining files with only an error in the logs</li>
<li>Now if a file fails to upload after hitting a retry limit, any remaining uploads stop and the step fails. Partial artifacts will still be available for download</li>
</ul>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/upload-artifact/commit/27121b0bdffd731efa15d66772be8dc71245d074"><code>27121b0</code></a> Ingest v0.5.2 of <code>@​actions/artifact</code> (<a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/224">#224</a>)</li>
<li><a href="https://github.com/actions/upload-artifact/commit/4537e112f4e46fdaa3b4847da80f2c8540a94bf7"><code>4537e11</code></a> Bump ws from 7.2.3 to 7.5.0 (<a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/221">#221</a>)</li>
<li><a href="https://github.com/actions/upload-artifact/commit/2368feccd5553bf6938d56d091abec4601b4fd1a"><code>2368fec</code></a> Avoid triggering push for Dependabot branches (again) (<a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/223">#223</a>)</li>
<li><a href="https://github.com/actions/upload-artifact/commit/52a3c6b9754867518f180c7611590f2ef96635b9"><code>52a3c6b</code></a> Bump glob-parent from 5.1.1 to 5.1.2 (<a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/219">#219</a>)</li>
<li><a href="https://github.com/actions/upload-artifact/commit/76f4433885dedef9c997f9d03db51c2c9275438e"><code>76f4433</code></a> Bump hosted-git-info from 2.8.5 to 2.8.9 (<a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/203">#203</a>)</li>
<li><a href="https://github.com/actions/upload-artifact/commit/46426468d3d2c3b79e12716101f0a3381ccfc5ba"><code>4642646</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/222">#222</a> from actions/brcrista/dependabot-push</li>
<li><a href="https://github.com/actions/upload-artifact/commit/85076876532a28367eb508944031234ac9ec350b"><code>8507687</code></a> avoid triggering push for Dependabot branches</li>
<li><a href="https://github.com/actions/upload-artifact/commit/0482dbbe7aad90dfa862cc6ff445c507fe26dfbf"><code>0482dbb</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/202">#202</a> from actions/dependabot/npm_and_yarn/lodash-4.17.21</li>
<li><a href="https://github.com/actions/upload-artifact/commit/58518184d2dfe60a9c84c3dcff40cf853fdadeca"><code>5851818</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/211">#211</a> from JasonGross/patch-1</li>
<li><a href="https://github.com/actions/upload-artifact/commit/4db8255e70a22a94e2ae16f87d2594b19dd9aea3"><code>4db8255</code></a> Fix the grammar in a warning message</li>
<li>Additional commits viewable in <a href="https://github.com/actions/upload-artifact/compare/v1...v2.2.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/upload-artifact&package-manager=github_actions&previous-version=1&new-version=2.2.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-07-09 14:37:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2866" class=".btn">#2866</a>
            </td>
            <td>
                <b>
                    ci: dependabot configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Troy Ronda <troy@troyronda.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-09 14:28:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2864" class=".btn">#2864</a>
            </td>
            <td>
                <b>
                    fix: resolve local did key references when handling request via implicit invitation
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
        Created At 2021-07-08 21:40:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2863" class=".btn">#2863</a>
            </td>
            <td>
                <b>
                    chore: Update storage module versions
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
        Created At 2021-07-08 21:07:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2861" class=".btn">#2861</a>
            </td>
            <td>
                <b>
                    feat: add option to use http for web vdr
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
        Created At 2021-07-08 07:20:10 +0000 UTC
    </div>
</div>

