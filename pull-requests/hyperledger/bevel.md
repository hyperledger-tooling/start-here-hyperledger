---
layout: default
title: bevel
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/bevel
---

# bevel <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/bevel){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2121" class=".btn">#2121</a>
            </td>
            <td>
                <b>
                    Bump json5 from 1.0.1 to 1.0.2 in /examples/supplychain-app/fabric/chaincode_rest_server/rest-server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [json5](https://github.com/json5/json5) from 1.0.1 to 1.0.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/releases">json5's releases</a>.</em></p>
<blockquote>
<h2>v1.0.2</h2>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>). This has been backported to v1. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/298">#298</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/blob/main/CHANGELOG.md">json5's changelog</a>.</em></p>
<blockquote>
<h3>Unreleased [<a href="https://github.com/json5/json5/tree/main">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.3...HEAD">diff</a>]</h3>
<h3>v2.2.3 [<a href="https://github.com/json5/json5/tree/v2.2.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.2...v2.2.3">diff</a>]</h3>
<ul>
<li>Fix: json5@2.2.3 is now the 'latest' release according to npm instead of
v1.0.2. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/299">#299</a>)</li>
</ul>
<h3>v2.2.2 [<a href="https://github.com/json5/json5/tree/v2.2.2">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.1...v2.2.2">diff</a>]</h3>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays.
(<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by
Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>).</li>
</ul>
<h3>v2.2.1 [<a href="https://github.com/json5/json5/tree/v2.2.1">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.0...v2.2.1">diff</a>]</h3>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
<h3>v2.2.0 [<a href="https://github.com/json5/json5/tree/v2.2.0">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.3...v2.2.0">diff</a>]</h3>
<ul>
<li>New: Accurate and documented TypeScript declarations are now included. There
is no need to install <code>@types/json5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/236">#236</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/244">#244</a>)</li>
</ul>
<h3>v2.1.3 [<a href="https://github.com/json5/json5/tree/v2.1.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.2...v2.1.3">diff</a>]</h3>
<ul>
<li>Fix: An out of memory bug when parsing numbers has been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/228">#228</a>,
<a href="https://github-redirect.dependabot.com/json5/json5/issues/229">#229</a>)</li>
</ul>
<h3>v2.1.2 [<a href="https://github.com/json5/json5/tree/v2.1.2">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.1...v2.1.2">diff</a>]</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/json5/json5/commit/a62db1e51e1031d92ac260f5bb38bbed1fdbc754"><code>a62db1e</code></a> 1.0.2</li>
<li><a href="https://github.com/json5/json5/commit/e0c23fe458a77c0b2cdb271376be5d8d0908133c"><code>e0c23fe</code></a> docs: update CHANGELOG for v1.0.2</li>
<li><a href="https://github.com/json5/json5/commit/62a65408408d40aeea14c7869ed327acead12972"><code>62a6540</code></a> fix: add <strong>proto</strong> to objects and arrays</li>
<li>See full diff in <a href="https://github.com/json5/json5/compare/v1.0.1...v1.0.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=json5&package-manager=npm_and_yarn&previous-version=1.0.1&new-version=1.0.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-07 11:04:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2120" class=".btn">#2120</a>
            </td>
            <td>
                <b>
                    [ci-skip]feat(docs): update PR template
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                feat(docs): update PR template

    Primary Changes
    ---------------
    1. Updated .github/pull_request_template.md

    Results from changes done in 1)
    a. Removed reviewed_by field as github can track that information
    b. Added fixes tag for auto-linking to the issue

Fixes hyperledger#2102
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 09:02:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2118" class=".btn">#2118</a>
            </td>
            <td>
                <b>
                    Bump json5 and babel-brunch in /platforms/r3-corda/images/networkmap/website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                [//]: # (dependabot-start)
⚠️  **Dependabot is rebasing this PR** ⚠️ 

Rebasing might not happen immediately, so don't worry if this takes some time.

Note: if you make any changes to this PR yourself, they will take precedence over the rebase.

---

[//]: # (dependabot-end)

Bumps [json5](https://github.com/json5/json5) to 2.2.3 and updates ancestor dependency [babel-brunch](https://github.com/babel/babel-brunch). These dependencies need to be updated together.

Updates `json5` from 0.5.1 to 2.2.3
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/releases">json5's releases</a>.</em></p>
<blockquote>
<h2>v2.2.3</h2>
<ul>
<li>Fix: json5@2.2.3 is now the 'latest' release according to npm instead of v1.0.2. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/299">#299</a>)</li>
</ul>
<h2>v2.2.2</h2>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays.
(<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by
Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>).</li>
</ul>
<h2>v2.2.1</h2>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
<h2>v2.2.0</h2>
<ul>
<li>New: Accurate and documented TypeScript declarations are now included. There is no need to install <code>@types/json5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/236">#236</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/244">#244</a>)</li>
</ul>
<h3>v2.1.3 [<a href="https://github.com/json5/json5/tree/v2.1.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.2...v2.1.3">diff</a>]</h3>
<ul>
<li>Fix: An out of memory bug when parsing numbers has been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/228">#228</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/229">#229</a>)</li>
</ul>
<h2>v2.1.2</h2>
<ul>
<li>Fix: Bump <code>minimist</code> to <code>v1.2.5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/222">#222</a>)</li>
</ul>
<h2>v2.1.1</h2>
<ul>
<li>New: <code>package.json</code> and <code>package.json5</code> include a <code>module</code> property so
bundlers like webpack, rollup and parcel can take advantage of the ES Module
build. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/208">#208</a>)</li>
<li>Fix: <code>stringify</code> outputs <code>\0</code> as <code>\\x00</code> when followed by a digit. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/210">#210</a>)</li>
<li>Fix: Spelling mistakes have been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/196">#196</a>)</li>
</ul>
<h2>v2.1.0</h2>
<ul>
<li>New: The <code>index.mjs</code> and <code>index.min.mjs</code> browser builds in the <code>dist</code> directory support ES6 modules. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/187">#187</a>)</li>
</ul>
<h2>v2.0.1</h2>
<ul>
<li>Fix: The browser builds in the <code>dist</code> directory support ES5. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/182">#182</a>)</li>
</ul>
<h2>v2.0.0</h2>
<ul>
<li>
<p><strong>Major</strong>: JSON5 officially supports Node.js v6 and later. Support for Node.js
v4 has been dropped. Since Node.js v6 supports ES5 features, the code has been
rewritten in native ES5, and the dependence on Babel has been eliminated.</p>
</li>
<li>
<p>New: Support for Unicode 10 has been added.</p>
</li>
<li>
<p>New: The test framework has been migrated from Mocha to Tap.</p>
</li>
<li>
<p>New: The browser build at <code>dist/index.js</code> is no longer minified by default. A
minified version is available at <code>dist/index.min.js</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/181">#181</a>)</p>
</li>
<li>
<p>Fix: The warning has been made clearer when line and paragraph separators are</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/blob/main/CHANGELOG.md">json5's changelog</a>.</em></p>
<blockquote>
<h3>v2.2.3 [<a href="https://github.com/json5/json5/tree/v2.2.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.2...v2.2.3">diff</a>]</h3>
<ul>
<li>Fix: json5@2.2.3 is now the 'latest' release according to npm instead of
v1.0.2. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/299">#299</a>)</li>
</ul>
<h3>v2.2.2 [<a href="https://github.com/json5/json5/tree/v2.2.2">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.1...v2.2.2">diff</a>]</h3>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays.
(<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by
Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>).</li>
</ul>
<h3>v2.2.1 [<a href="https://github.com/json5/json5/tree/v2.2.1">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.0...v2.2.1">diff</a>]</h3>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
<h3>v2.2.0 [<a href="https://github.com/json5/json5/tree/v2.2.0">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.3...v2.2.0">diff</a>]</h3>
<ul>
<li>New: Accurate and documented TypeScript declarations are now included. There
is no need to install <code>@types/json5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/236">#236</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/244">#244</a>)</li>
</ul>
<h3>v2.1.3 [<a href="https://github.com/json5/json5/tree/v2.1.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.2...v2.1.3">diff</a>]</h3>
<ul>
<li>Fix: An out of memory bug when parsing numbers has been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/228">#228</a>,
<a href="https://github-redirect.dependabot.com/json5/json5/issues/229">#229</a>)</li>
</ul>
<h3>v2.1.2 [<a href="https://github.com/json5/json5/tree/v2.1.2">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.1...v2.1.2">diff</a>]</h3>
<ul>
<li>Fix: Bump <code>minimist</code> to <code>v1.2.5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/222">#222</a>)</li>
</ul>
<h3>v2.1.1 [<a href="https://github.com/json5/json5/tree/v2.1.1">code</a>, [diff][d2.1.1]]</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/json5/json5/commit/c3a75242772a5026a49c4017a16d9b3543b62776"><code>c3a7524</code></a> 2.2.3</li>
<li><a href="https://github.com/json5/json5/commit/94fd06d82eeed225fa172f6fb2ca27375cbd2e39"><code>94fd06d</code></a> docs: update CHANGELOG for v2.2.3</li>
<li><a href="https://github.com/json5/json5/commit/3b8cebf0c474a8b20c78bd75c89cca0c4dce84ce"><code>3b8cebf</code></a> docs(security): use GitHub security advisories</li>
<li><a href="https://github.com/json5/json5/commit/f0fd9e194dde282caff114a110f4fac635f3a62c"><code>f0fd9e1</code></a> docs: publish a security policy</li>
<li><a href="https://github.com/json5/json5/commit/6a91a05fffeda16ff6b3b5008b6b340d42d31ec0"><code>6a91a05</code></a> docs(template): bug -&gt; bug report</li>
<li><a href="https://github.com/json5/json5/commit/14f8cb186e8abdfaccf6527171da7b1224374650"><code>14f8cb1</code></a> 2.2.2</li>
<li><a href="https://github.com/json5/json5/commit/10cc7ca9169b59c5e0f5afc03dbd870cd06bcc46"><code>10cc7ca</code></a> docs: update CHANGELOG for v2.2.2</li>
<li><a href="https://github.com/json5/json5/commit/7774c1097993bc3ce9f0ac4b722a32bf7d6871c8"><code>7774c10</code></a> fix: add <strong>proto</strong> to objects and arrays</li>
<li><a href="https://github.com/json5/json5/commit/edde30abd8b22facf2c06c72586b9f6edf12700d"><code>edde30a</code></a> Readme: slight tweak to intro</li>
<li><a href="https://github.com/json5/json5/commit/97286f8bd542c89dcee096bc05dd28ed2dfc1e16"><code>97286f8</code></a> Improve example in readme</li>
<li>Additional commits viewable in <a href="https://github.com/json5/json5/compare/v0.5.1...v2.2.3">compare view</a></li>
</ul>
</details>
<br />

Updates `babel-brunch` from 6.1.1 to 7.0.1
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/babel/babel-brunch/commit/e6e1d8525abe8aa6520d41164b9f71be06d9de2f"><code>e6e1d85</code></a> 7.0.1</li>
<li><a href="https://github.com/babel/babel-brunch/commit/e814ebca6806f30eb0f5232a929501c4c51378b5"><code>e814ebc</code></a> Update dependencies</li>
<li><a href="https://github.com/babel/babel-brunch/commit/67bc0a6431ce682efe7d7d233ce7cf0396556bf0"><code>67bc0a6</code></a> Release 7.0.0.</li>
<li><a href="https://github.com/babel/babel-brunch/commit/3919b529ee664828cf71175ff6e751c43248addf"><code>3919b52</code></a> 7.0 (<a href="https://github-redirect.dependabot.com/babel/babel-brunch/issues/67">#67</a>)</li>
<li><a href="https://github.com/babel/babel-brunch/commit/c42c598076dcdd44f5dbe3c310f78e06e992c6e1"><code>c42c598</code></a> Improve pattern example (<a href="https://github-redirect.dependabot.com/babel/babel-brunch/issues/55">#55</a>)</li>
<li><a href="https://github.com/babel/babel-brunch/commit/df0e92bb3afa7d489cadf4c026675c9dfaab5e6c"><code>df0e92b</code></a> Refactoring, env, closing a bunch of issues (<a href="https://github-redirect.dependabot.com/babel/babel-brunch/issues/53">#53</a>)</li>
<li><a href="https://github.com/babel/babel-brunch/commit/2cff6ce89809d0e834c303b397467747aa5fc919"><code>2cff6ce</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/babel/babel-brunch/issues/50">#50</a> from kesha-antonov/master</li>
<li><a href="https://github.com/babel/babel-brunch/commit/f0b099baa96f6ae055d69ce955085a77ee1c9bf0"><code>f0b099b</code></a> fix typo in readme</li>
<li>See full diff in <a href="https://github.com/babel/babel-brunch/compare/6.1.1...v7.0.1">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~danez">danez</a>, a new releaser for babel-brunch since your current version.</p>
</details>
<br />


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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 02:49:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2117" class=".btn">#2117</a>
            </td>
            <td>
                <b>
                    Bump json5 and babel-brunch in /platforms/r3-corda/images/doorman/website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [json5](https://github.com/json5/json5) to 2.2.3 and updates ancestor dependency [babel-brunch](https://github.com/babel/babel-brunch). These dependencies need to be updated together.

Updates `json5` from 0.5.1 to 2.2.3
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/releases">json5's releases</a>.</em></p>
<blockquote>
<h2>v2.2.3</h2>
<ul>
<li>Fix: json5@2.2.3 is now the 'latest' release according to npm instead of v1.0.2. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/299">#299</a>)</li>
</ul>
<h2>v2.2.2</h2>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays.
(<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by
Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>).</li>
</ul>
<h2>v2.2.1</h2>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
<h2>v2.2.0</h2>
<ul>
<li>New: Accurate and documented TypeScript declarations are now included. There is no need to install <code>@types/json5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/236">#236</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/244">#244</a>)</li>
</ul>
<h3>v2.1.3 [<a href="https://github.com/json5/json5/tree/v2.1.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.2...v2.1.3">diff</a>]</h3>
<ul>
<li>Fix: An out of memory bug when parsing numbers has been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/228">#228</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/229">#229</a>)</li>
</ul>
<h2>v2.1.2</h2>
<ul>
<li>Fix: Bump <code>minimist</code> to <code>v1.2.5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/222">#222</a>)</li>
</ul>
<h2>v2.1.1</h2>
<ul>
<li>New: <code>package.json</code> and <code>package.json5</code> include a <code>module</code> property so
bundlers like webpack, rollup and parcel can take advantage of the ES Module
build. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/208">#208</a>)</li>
<li>Fix: <code>stringify</code> outputs <code>\0</code> as <code>\\x00</code> when followed by a digit. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/210">#210</a>)</li>
<li>Fix: Spelling mistakes have been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/196">#196</a>)</li>
</ul>
<h2>v2.1.0</h2>
<ul>
<li>New: The <code>index.mjs</code> and <code>index.min.mjs</code> browser builds in the <code>dist</code> directory support ES6 modules. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/187">#187</a>)</li>
</ul>
<h2>v2.0.1</h2>
<ul>
<li>Fix: The browser builds in the <code>dist</code> directory support ES5. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/182">#182</a>)</li>
</ul>
<h2>v2.0.0</h2>
<ul>
<li>
<p><strong>Major</strong>: JSON5 officially supports Node.js v6 and later. Support for Node.js
v4 has been dropped. Since Node.js v6 supports ES5 features, the code has been
rewritten in native ES5, and the dependence on Babel has been eliminated.</p>
</li>
<li>
<p>New: Support for Unicode 10 has been added.</p>
</li>
<li>
<p>New: The test framework has been migrated from Mocha to Tap.</p>
</li>
<li>
<p>New: The browser build at <code>dist/index.js</code> is no longer minified by default. A
minified version is available at <code>dist/index.min.js</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/181">#181</a>)</p>
</li>
<li>
<p>Fix: The warning has been made clearer when line and paragraph separators are</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/blob/main/CHANGELOG.md">json5's changelog</a>.</em></p>
<blockquote>
<h3>v2.2.3 [<a href="https://github.com/json5/json5/tree/v2.2.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.2...v2.2.3">diff</a>]</h3>
<ul>
<li>Fix: json5@2.2.3 is now the 'latest' release according to npm instead of
v1.0.2. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/299">#299</a>)</li>
</ul>
<h3>v2.2.2 [<a href="https://github.com/json5/json5/tree/v2.2.2">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.1...v2.2.2">diff</a>]</h3>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays.
(<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by
Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>).</li>
</ul>
<h3>v2.2.1 [<a href="https://github.com/json5/json5/tree/v2.2.1">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.0...v2.2.1">diff</a>]</h3>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
<h3>v2.2.0 [<a href="https://github.com/json5/json5/tree/v2.2.0">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.3...v2.2.0">diff</a>]</h3>
<ul>
<li>New: Accurate and documented TypeScript declarations are now included. There
is no need to install <code>@types/json5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/236">#236</a>, <a href="https://github-redirect.dependabot.com/json5/json5/issues/244">#244</a>)</li>
</ul>
<h3>v2.1.3 [<a href="https://github.com/json5/json5/tree/v2.1.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.2...v2.1.3">diff</a>]</h3>
<ul>
<li>Fix: An out of memory bug when parsing numbers has been fixed. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/228">#228</a>,
<a href="https://github-redirect.dependabot.com/json5/json5/issues/229">#229</a>)</li>
</ul>
<h3>v2.1.2 [<a href="https://github.com/json5/json5/tree/v2.1.2">code</a>, <a href="https://github.com/json5/json5/compare/v2.1.1...v2.1.2">diff</a>]</h3>
<ul>
<li>Fix: Bump <code>minimist</code> to <code>v1.2.5</code>. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/222">#222</a>)</li>
</ul>
<h3>v2.1.1 [<a href="https://github.com/json5/json5/tree/v2.1.1">code</a>, [diff][d2.1.1]]</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/json5/json5/commit/c3a75242772a5026a49c4017a16d9b3543b62776"><code>c3a7524</code></a> 2.2.3</li>
<li><a href="https://github.com/json5/json5/commit/94fd06d82eeed225fa172f6fb2ca27375cbd2e39"><code>94fd06d</code></a> docs: update CHANGELOG for v2.2.3</li>
<li><a href="https://github.com/json5/json5/commit/3b8cebf0c474a8b20c78bd75c89cca0c4dce84ce"><code>3b8cebf</code></a> docs(security): use GitHub security advisories</li>
<li><a href="https://github.com/json5/json5/commit/f0fd9e194dde282caff114a110f4fac635f3a62c"><code>f0fd9e1</code></a> docs: publish a security policy</li>
<li><a href="https://github.com/json5/json5/commit/6a91a05fffeda16ff6b3b5008b6b340d42d31ec0"><code>6a91a05</code></a> docs(template): bug -&gt; bug report</li>
<li><a href="https://github.com/json5/json5/commit/14f8cb186e8abdfaccf6527171da7b1224374650"><code>14f8cb1</code></a> 2.2.2</li>
<li><a href="https://github.com/json5/json5/commit/10cc7ca9169b59c5e0f5afc03dbd870cd06bcc46"><code>10cc7ca</code></a> docs: update CHANGELOG for v2.2.2</li>
<li><a href="https://github.com/json5/json5/commit/7774c1097993bc3ce9f0ac4b722a32bf7d6871c8"><code>7774c10</code></a> fix: add <strong>proto</strong> to objects and arrays</li>
<li><a href="https://github.com/json5/json5/commit/edde30abd8b22facf2c06c72586b9f6edf12700d"><code>edde30a</code></a> Readme: slight tweak to intro</li>
<li><a href="https://github.com/json5/json5/commit/97286f8bd542c89dcee096bc05dd28ed2dfc1e16"><code>97286f8</code></a> Improve example in readme</li>
<li>Additional commits viewable in <a href="https://github.com/json5/json5/compare/v0.5.1...v2.2.3">compare view</a></li>
</ul>
</details>
<br />

Updates `babel-brunch` from 6.1.1 to 7.0.1
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/babel/babel-brunch/commit/e6e1d8525abe8aa6520d41164b9f71be06d9de2f"><code>e6e1d85</code></a> 7.0.1</li>
<li><a href="https://github.com/babel/babel-brunch/commit/e814ebca6806f30eb0f5232a929501c4c51378b5"><code>e814ebc</code></a> Update dependencies</li>
<li><a href="https://github.com/babel/babel-brunch/commit/67bc0a6431ce682efe7d7d233ce7cf0396556bf0"><code>67bc0a6</code></a> Release 7.0.0.</li>
<li><a href="https://github.com/babel/babel-brunch/commit/3919b529ee664828cf71175ff6e751c43248addf"><code>3919b52</code></a> 7.0 (<a href="https://github-redirect.dependabot.com/babel/babel-brunch/issues/67">#67</a>)</li>
<li><a href="https://github.com/babel/babel-brunch/commit/c42c598076dcdd44f5dbe3c310f78e06e992c6e1"><code>c42c598</code></a> Improve pattern example (<a href="https://github-redirect.dependabot.com/babel/babel-brunch/issues/55">#55</a>)</li>
<li><a href="https://github.com/babel/babel-brunch/commit/df0e92bb3afa7d489cadf4c026675c9dfaab5e6c"><code>df0e92b</code></a> Refactoring, env, closing a bunch of issues (<a href="https://github-redirect.dependabot.com/babel/babel-brunch/issues/53">#53</a>)</li>
<li><a href="https://github.com/babel/babel-brunch/commit/2cff6ce89809d0e834c303b397467747aa5fc919"><code>2cff6ce</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/babel/babel-brunch/issues/50">#50</a> from kesha-antonov/master</li>
<li><a href="https://github.com/babel/babel-brunch/commit/f0b099baa96f6ae055d69ce955085a77ee1c9bf0"><code>f0b099b</code></a> fix typo in readme</li>
<li>See full diff in <a href="https://github.com/babel/babel-brunch/compare/6.1.1...v7.0.1">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~danez">danez</a>, a new releaser for babel-brunch since your current version.</p>
</details>
<br />


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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-05 23:37:20 +0000 UTC
    </div>
</div>

