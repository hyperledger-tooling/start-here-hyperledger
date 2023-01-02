---
layout: default
title: firefly-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-samples
---

# firefly-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-samples/pull/49" class=".btn">#49</a>
            </td>
            <td>
                <b>
                    Bump json5 and react-scripts in /private-data-transfer-ui
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [json5](https://github.com/json5/json5) to 2.2.3 and updates ancestor dependency [react-scripts](https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts). These dependencies need to be updated together.

Updates `json5` from 1.0.1 to 2.2.3
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
<li>Additional commits viewable in <a href="https://github.com/json5/json5/compare/v1.0.1...v2.2.3">compare view</a></li>
</ul>
</details>
<br />

Updates `react-scripts` from 4.0.3 to 5.0.1
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/facebook/create-react-app/commit/19fa58d527ae74f2b6baa0867463eea1d290f9a5"><code>19fa58d</code></a> Publish</li>
<li><a href="https://github.com/facebook/create-react-app/commit/9802941ff049a28da2682801bc182a29761b71f4"><code>9802941</code></a> fix: webpack noise printed only if error or warning (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/12245">#12245</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/2eef1d0a1db2e84cdcd6e7ca941c85a48cc7cc65"><code>2eef1d0</code></a> Update templates to use React 18 <code>createRoot</code> (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/12220">#12220</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/221e511730ca51c036c6954a9d2ee7659ff860f9"><code>221e511</code></a> Publish</li>
<li><a href="https://github.com/facebook/create-react-app/commit/5614c87bfbaae0ce52ac15aedd2cd0f91ffd420d"><code>5614c87</code></a> Add support for Tailwind (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11717">#11717</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/20edab4894b301f6b90dad0f90a2f82c52a7ac66"><code>20edab4</code></a> fix(webpackDevServer): disable overlay for warnings (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11413">#11413</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/3afbbc0ab922fb982bb275ccb3fe5beecdf5f889"><code>3afbbc0</code></a> Update all dependencies (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11624">#11624</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/f5467d5e77d51a3f23dd5fa70697dbab79832489"><code>f5467d5</code></a> feat(eslint-config-react-app): support ESLint 8.x (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11375">#11375</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/c7627ce96c4674f327081f101dd0e2771be4d045"><code>c7627ce</code></a> Update webpack and dev server (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11646">#11646</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/544befeb536a89b0ff95792df70bb037b17f55b9"><code>544befe</code></a> Update package.json (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11597">#11597</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/facebook/create-react-app/commits/react-scripts@5.0.1/packages/react-scripts">compare view</a></li>
</ul>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/firefly-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-02 12:50:37 +0000 UTC
    </div>
</div>

