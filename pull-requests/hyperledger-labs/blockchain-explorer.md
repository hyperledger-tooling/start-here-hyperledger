---
layout: default
title: blockchain-explorer
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-explorer
---

# blockchain-explorer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-explorer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/309" class=".btn">#309</a>
            </td>
            <td>
                <b>
                    Bump loader-utils and react-scripts in /client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [loader-utils](https://github.com/webpack/loader-utils) to 2.0.4 and updates ancestor dependency [react-scripts](https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts). These dependencies need to be updated together.

Updates `loader-utils` from 1.2.3 to 2.0.4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/loader-utils/releases">loader-utils's releases</a>.</em></p>
<blockquote>
<h2>v2.0.4</h2>
<h3><a href="https://github.com/webpack/loader-utils/compare/v2.0.3...v2.0.4">2.0.4</a> (2022-11-11)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>ReDoS problem (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/225">#225</a>) (<a href="https://github.com/webpack/loader-utils/commit/ac09944dfacd7c4497ef692894b09e63e09a5eeb">ac09944</a>)</li>
</ul>
<h2>v2.0.3</h2>
<h3><a href="https://github.com/webpack/loader-utils/compare/v2.0.1...v2.0.3">2.0.3</a> (2022-10-20)</h3>
<h3>Bug Fixes</h3>
<ul>
<li><strong>security:</strong> prototype pollution exploit (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/217">#217</a>) (<a href="https://github.com/webpack/loader-utils/commit/a93cf6f4702012030f6b5ee8340d5c95ec1c7d4c">a93cf6f</a>)</li>
</ul>
<h2>v2.0.2</h2>
<h3><a href="https://github.com/webpack/loader-utils/compare/v2.0.1...v2.0.2">2.0.2</a> (2021-11-04)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>base64 generation and unicode characters (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/197">#197</a>) (<a href="https://github.com/webpack/loader-utils/commit/8c2d24ee400bc4567335e97ee6004c3baa6ef66f">8c2d24e</a>)</li>
</ul>
<h2>v2.0.1</h2>
<h3><a href="https://github.com/webpack/loader-utils/compare/v2.0.0...v2.0.1">2.0.1</a> (2021-10-29)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>md4 support on Node.js v17 (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/193">#193</a>) (<a href="https://github.com/webpack/loader-utils/commit/1069f61284a571614ee4acdde6e6087174be118a">1069f61</a>)</li>
</ul>
<h2>v2.0.0</h2>
<h2><a href="https://github.com/webpack/loader-utils/compare/v1.4.0...v2.0.0">2.0.0</a> (2020-03-17)</h2>
<h3>⚠ BREAKING CHANGES</h3>
<ul>
<li>minimum required <code>Node.js</code> version is <code>8.9.0</code> (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/166">#166</a>) (<a href="https://github.com/webpack/loader-utils/commit/c937e8c77231b42018be616b784a6b45eac86f8a">c937e8c</a>)</li>
<li>the <code>getOptions</code> method returns empty object on empty query (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/167">#167</a>) (<a href="https://github.com/webpack/loader-utils/commit/b595cfba022d3f04f3d310dd570b0253e461605b">b595cfb</a>)</li>
<li>Use <code>md4</code> by default</li>
</ul>
<h2>v1.4.2</h2>
<h3><a href="https://github.com/webpack/loader-utils/compare/v1.4.1...v1.4.2">1.4.2</a> (2022-11-11)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>ReDoS problem (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/226">#226</a>) (<a href="https://github.com/webpack/loader-utils/commit/17cbf8fa8989c1cb45bdd2997aa524729475f1fa">17cbf8f</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/webpack/loader-utils/blob/v2.0.4/CHANGELOG.md">loader-utils's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/webpack/loader-utils/compare/v2.0.3...v2.0.4">2.0.4</a> (2022-11-11)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>ReDoS problem (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/225">#225</a>) (<a href="https://github.com/webpack/loader-utils/commit/ac09944dfacd7c4497ef692894b09e63e09a5eeb">ac09944</a>)</li>
</ul>
<h3><a href="https://github.com/webpack/loader-utils/compare/v2.0.1...v2.0.3">2.0.3</a> (2022-10-20)</h3>
<h3>Bug Fixes</h3>
<ul>
<li><strong>security:</strong> prototype pollution exploit (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/217">#217</a>) (<a href="https://github.com/webpack/loader-utils/commit/a93cf6f4702012030f6b5ee8340d5c95ec1c7d4c">a93cf6f</a>)</li>
</ul>
<h3><a href="https://github.com/webpack/loader-utils/compare/v2.0.1...v2.0.2">2.0.2</a> (2021-11-04)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>base64 generation and unicode characters (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/197">#197</a>) (<a href="https://github.com/webpack/loader-utils/commit/8c2d24ee400bc4567335e97ee6004c3baa6ef66f">8c2d24e</a>)</li>
</ul>
<h3><a href="https://github.com/webpack/loader-utils/compare/v2.0.0...v2.0.1">2.0.1</a> (2021-10-29)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>md4 support on Node.js v17 (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/193">#193</a>) (<a href="https://github.com/webpack/loader-utils/commit/1069f61284a571614ee4acdde6e6087174be118a">1069f61</a>)</li>
</ul>
<h2><a href="https://github.com/webpack/loader-utils/compare/v1.4.0...v2.0.0">2.0.0</a> (2020-03-17)</h2>
<h3>⚠ BREAKING CHANGES</h3>
<ul>
<li>minimum required <code>Node.js</code> version is <code>8.9.0</code> (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/166">#166</a>) (<a href="https://github.com/webpack/loader-utils/commit/c937e8c77231b42018be616b784a6b45eac86f8a">c937e8c</a>)</li>
<li>the <code>getOptions</code> method returns empty object on empty query (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/167">#167</a>) (<a href="https://github.com/webpack/loader-utils/commit/b595cfba022d3f04f3d310dd570b0253e461605b">b595cfb</a>)</li>
<li>Use <code>md4</code> by default</li>
</ul>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1><a href="https://github.com/webpack/loader-utils/compare/v1.3.0...v1.4.0">1.4.0</a> (2020-02-19)</h1>
<h3>Features</h3>
<ul>
<li>the <code>resourceQuery</code> is passed to the <code>interpolateName</code> method (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/163">#163</a>) (<a href="https://github.com/webpack/loader-utils/commit/cd0e428">cd0e428</a>)</li>
</ul>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1><a href="https://github.com/webpack/loader-utils/compare/v1.2.3...v1.3.0">1.3.0</a> (2020-02-19)</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/loader-utils/commit/6688b5028106f144ee9f543bebc8e6a87b57829f"><code>6688b50</code></a> chore(release): 2.0.4</li>
<li><a href="https://github.com/webpack/loader-utils/commit/ac09944dfacd7c4497ef692894b09e63e09a5eeb"><code>ac09944</code></a> fix: ReDoS problem (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/225">#225</a>)</li>
<li><a href="https://github.com/webpack/loader-utils/commit/7162619fb982c394ed75098a0a0ed7e7f3177c70"><code>7162619</code></a> chore(release): 2.0.3</li>
<li><a href="https://github.com/webpack/loader-utils/commit/a93cf6f4702012030f6b5ee8340d5c95ec1c7d4c"><code>a93cf6f</code></a> fix(security): prototype polution exploit (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/217">#217</a>)</li>
<li><a href="https://github.com/webpack/loader-utils/commit/90c7c4be17e3e0b2f6091a69c67db7a6df9fd044"><code>90c7c4b</code></a> chore(release): 2.0.2</li>
<li><a href="https://github.com/webpack/loader-utils/commit/8c2d24ee400bc4567335e97ee6004c3baa6ef66f"><code>8c2d24e</code></a> fix: base64 generation and unicode characters (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/197">#197</a>)</li>
<li><a href="https://github.com/webpack/loader-utils/commit/5fb556208426d281a18dfbf6f45dca24bfb24e96"><code>5fb5562</code></a> chore(release): 2.0.1</li>
<li><a href="https://github.com/webpack/loader-utils/commit/1069f61284a571614ee4acdde6e6087174be118a"><code>1069f61</code></a> fix: md4 support on Node.js v17 (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/193">#193</a>)</li>
<li><a href="https://github.com/webpack/loader-utils/commit/d9f4e23cf411d8556f8bac2d3bf05a6e0103b568"><code>d9f4e23</code></a> chore(release): 2.0.0</li>
<li><a href="https://github.com/webpack/loader-utils/commit/865dc03909bd0018c9d6a26ea65814faec8eb1e5"><code>865dc03</code></a> refactor: switch to <code>md4</code> by default (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/168">#168</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/loader-utils/compare/v1.2.3...v2.0.4">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-explorer/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-22 02:41:20 +0000 UTC
    </div>
</div>

