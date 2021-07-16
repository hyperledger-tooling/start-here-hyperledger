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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2884" class=".btn">#2884</a>
            </td>
            <td>
                <b>
                    fix: Checks API error (webkms)
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
        Created At 2021-07-16 13:56:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2882" class=".btn">#2882</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack-merge from 4.2.2 to 5.8.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack-merge](https://github.com/survivejs/webpack-merge) from 4.2.2 to 5.8.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/survivejs/webpack-merge/blob/develop/CHANGELOG.md">webpack-merge's changelog</a>.</em></p>
<blockquote>
<h2>5.8.0 / 2021-06-07</h2>
<ul>
<li>Docs - Update <code>env</code> example to be webpack 5 compatible. <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/177">#177</a>, <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/180">#180</a></li>
<li>Feat - Support strings as rules for TypeScript, not just enums. <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/179">#179</a>, <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/185">#185</a></li>
</ul>
<h2>5.7.3 / 2020-12-22</h2>
<ul>
<li>Fix - Don't merge strings with objects in <code>mergeWithRules</code>. <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/172">#172</a></li>
</ul>
<h2>5.7.2 / 2020-12-16</h2>
<ul>
<li>Fix - If there's no match when using <code>merge</code> operation with <code>mergeWithRules</code>, use default merge behavior as a fallback. <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/167">#167</a></li>
</ul>
<h2>5.7.1 / 2020-12-16</h2>
<ul>
<li>Fix - Fix a merge failure for <code>mergeWithRules</code> when non-array matches are merged. <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/166">#166</a></li>
</ul>
<h2>5.7.0 / 2020-12-12</h2>
<ul>
<li>Feat - Throw a <code>TypeError</code> if trying to use <code>mergeWithRules</code> with invalid configuration types for <code>append</code>/<code>prepend</code>/<code>merge</code> operations.</li>
</ul>
<h2>5.6.1 / 2020-12-11</h2>
<ul>
<li>Fix - Drop extraneous logging.</li>
</ul>
<h2>5.6.0 / 2020-12-11</h2>
<ul>
<li>Feat - Support <code>merge</code> (<code>CustomizeRule.Merge</code>) for objects at <code>mergeWithRules</code>. This is useful for merging loader options for example. <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/163">#163</a></li>
</ul>
<h2>5.5.0 / 2020-12-10</h2>
<ul>
<li>Feat - Allow <code>mergeWithRules</code> to merge based on rules without a match. <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/151">#151</a> <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/159">#159</a></li>
</ul>
<h2>5.4.1 / 2020-12-08</h2>
<ul>
<li>Fix - Allow <code>mergeUnique</code> to work with arbitrary order. <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/161">#161</a></li>
</ul>
<h2>5.4.0 / 2020-10-30</h2>
<ul>
<li>Fix - Fall back correctly in <code>mergeWithRules</code> for cases that aren't matched. <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/157">#157</a> <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/158">#158</a></li>
<li>Fix - Don't throw if using <code>mergeWithRules</code> without a rule <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/151">#151</a></li>
<li>Feat - Throw if <code>undefined</code> is passed to <code>merge</code> as a structure to merge</li>
</ul>
<h2>5.3.0 / 2020-10-30</h2>
<ul>
<li>Fix - Expose <code>Configuration</code> type through a generic to TypeScript to support both webpack 4 and 5 <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/141">#141</a> <a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/154">#154</a></li>
</ul>
<p>In case you use webpack 4, please change your typing as instructed in the readme as the default type is loose but non-breaking.</p>
<h2>5.2.0 / 2020-10-07</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/survivejs/webpack-merge/commit/7a99833bd9faecd30bbcaeec8a9a10f6bab1d300"><code>7a99833</code></a> 5.8.0</li>
<li><a href="https://github.com/survivejs/webpack-merge/commit/df2b5cf6b28cc8f184dc53ec7a5622a44a7a8080"><code>df2b5cf</code></a> chore: Update changelog</li>
<li><a href="https://github.com/survivejs/webpack-merge/commit/5cb501e60481fb74f38595479c246f7d99d115c2"><code>5cb501e</code></a> feat: Support rules as strings (<a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/185">#185</a>)</li>
<li><a href="https://github.com/survivejs/webpack-merge/commit/72b52ced453ed642cd90de445bcfc4d8e338a412"><code>72b52ce</code></a> chore: Update changelog</li>
<li><a href="https://github.com/survivejs/webpack-merge/commit/afe55817106a61af03c9a25d03e06fab2de7c231"><code>afe5581</code></a> docs: update  example code of Limitations (<a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/180">#180</a>)</li>
<li><a href="https://github.com/survivejs/webpack-merge/commit/1062b06cfbbc2c9f5e7f9f21ab9d2cf0c6851296"><code>1062b06</code></a> chore: Update dependencies</li>
<li><a href="https://github.com/survivejs/webpack-merge/commit/3da07b210cda525ed0b124153d6472c23c88b2f2"><code>3da07b2</code></a> chore(deps): bump y18n from 4.0.0 to 4.0.1 (<a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/178">#178</a>)</li>
<li><a href="https://github.com/survivejs/webpack-merge/commit/53bac19aebff060116fd3b16a581e4bf06c7ac1e"><code>53bac19</code></a> chore(deps): bump lodash from 4.17.20 to 4.17.21 (<a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/181">#181</a>)</li>
<li><a href="https://github.com/survivejs/webpack-merge/commit/936ed0321bee2a2239abfe62f05d201dd46267b0"><code>936ed03</code></a> chore(deps): bump hosted-git-info from 2.8.8 to 2.8.9 (<a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/182">#182</a>)</li>
<li><a href="https://github.com/survivejs/webpack-merge/commit/d70de5320c94037ae2892bf9d76e5bafbfcf49bc"><code>d70de53</code></a> chore(deps): bump browserslist from 4.14.5 to 4.16.6 (<a href="https://github-redirect.dependabot.com/survivejs/webpack-merge/issues/183">#183</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/survivejs/webpack-merge/compare/v4.2.2...v5.8.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack-merge&package-manager=npm_and_yarn&previous-version=4.2.2&new-version=5.8.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-07-15 08:18:41 +0000 UTC
    </div>
</div>

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

