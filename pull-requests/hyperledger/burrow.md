---
layout: default
title: burrow
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/burrow
---

# burrow <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/burrow){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/burrow/pull/1539" class=".btn">#1539</a>
            </td>
            <td>
                <b>
                    Bump simple-get from 2.8.1 to 2.8.2 in /vent/test/eth
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [simple-get](https://github.com/feross/simple-get) from 2.8.1 to 2.8.2.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/feross/simple-get/commit/4e156b6bb19e11ccfad05fad310ea799d63f890d"><code>4e156b6</code></a> 2.8.2</li>
<li><a href="https://github.com/feross/simple-get/commit/43c272db3e4b1383cb03d80338dba3e08c451641"><code>43c272d</code></a> Bug fix: Thirdparty cookie leak</li>
<li>See full diff in <a href="https://github.com/feross/simple-get/compare/v2.8.1...v2.8.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~linusu">linusu</a>, a new releaser for simple-get since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=simple-get&package-manager=npm_and_yarn&previous-version=2.8.1&new-version=2.8.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/burrow/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-12 16:53:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/burrow/pull/1538" class=".btn">#1538</a>
            </td>
            <td>
                <b>
                    Bump node-fetch from 2.6.1 to 2.6.7 in /docs/example/basic-app
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [node-fetch](https://github.com/node-fetch/node-fetch) from 2.6.1 to 2.6.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/node-fetch/node-fetch/releases">node-fetch's releases</a>.</em></p>
<blockquote>
<h2>v2.6.7</h2>
<h1>Security patch release</h1>
<p>Recommended to upgrade, to not leak sensitive cookie and authentication header information to 3th party host while a redirect occurred</p>
<h2>What's Changed</h2>
<ul>
<li>fix: don't forward secure headers to 3th party by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1453">node-fetch/node-fetch#1453</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/node-fetch/node-fetch/compare/v2.6.6...v2.6.7">https://github.com/node-fetch/node-fetch/compare/v2.6.6...v2.6.7</a></p>
<h2>v2.6.6</h2>
<h2>What's Changed</h2>
<ul>
<li>fix(URL): prefer built in URL version when available and fallback to whatwg by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1352">node-fetch/node-fetch#1352</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/node-fetch/node-fetch/compare/v2.6.5...v2.6.6">https://github.com/node-fetch/node-fetch/compare/v2.6.5...v2.6.6</a></p>
<h2>v2.6.2</h2>
<p>fixed main path in package.json</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/node-fetch/node-fetch/commit/1ef4b560a17e644a02a3bfdea7631ffeee578b35"><code>1ef4b56</code></a> backport of <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1449">#1449</a> (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1453">#1453</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/8fe5c4ea66b9b8187600e6d5ec9b1b6781f44009"><code>8fe5c4e</code></a> 2.x: Specify encoding as an optional peer dependency in package.json (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1310">#1310</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/f56b0c66d3dd2ef185436de1f2fd40f66bfea8f4"><code>f56b0c6</code></a> fix(URL): prefer built in URL version when available and fallback to whatwg (...</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/b5417aea6a3275932283a200214522e6ab53f1ea"><code>b5417ae</code></a> fix: import whatwg-url in a way compatible with ESM Node (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1303">#1303</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/18193c5922c64046b922e18faf41821290535f06"><code>18193c5</code></a> fix v2.6.3 that did not sending query params (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1301">#1301</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/ace7536c955556be742d9910566738630cc3c2a6"><code>ace7536</code></a> fix: properly encode url with unicode characters (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1291">#1291</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/152214ca2f6e2a5a17d71e4638114625d3be30c6"><code>152214c</code></a> Fix(package.json): Corrected main file path in package.json (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1274">#1274</a>)</li>
<li>See full diff in <a href="https://github.com/node-fetch/node-fetch/compare/v2.6.1...v2.6.7">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~endless">endless</a>, a new releaser for node-fetch since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=node-fetch&package-manager=npm_and_yarn&previous-version=2.6.1&new-version=2.6.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/burrow/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-12 16:53:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/burrow/pull/1537" class=".btn">#1537</a>
            </td>
            <td>
                <b>
                    Bump node-fetch from 2.6.1 to 2.6.7 in /docs/example/basic-app-website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [node-fetch](https://github.com/node-fetch/node-fetch) from 2.6.1 to 2.6.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/node-fetch/node-fetch/releases">node-fetch's releases</a>.</em></p>
<blockquote>
<h2>v2.6.7</h2>
<h1>Security patch release</h1>
<p>Recommended to upgrade, to not leak sensitive cookie and authentication header information to 3th party host while a redirect occurred</p>
<h2>What's Changed</h2>
<ul>
<li>fix: don't forward secure headers to 3th party by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1453">node-fetch/node-fetch#1453</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/node-fetch/node-fetch/compare/v2.6.6...v2.6.7">https://github.com/node-fetch/node-fetch/compare/v2.6.6...v2.6.7</a></p>
<h2>v2.6.6</h2>
<h2>What's Changed</h2>
<ul>
<li>fix(URL): prefer built in URL version when available and fallback to whatwg by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1352">node-fetch/node-fetch#1352</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/node-fetch/node-fetch/compare/v2.6.5...v2.6.6">https://github.com/node-fetch/node-fetch/compare/v2.6.5...v2.6.6</a></p>
<h2>v2.6.2</h2>
<p>fixed main path in package.json</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/node-fetch/node-fetch/commit/1ef4b560a17e644a02a3bfdea7631ffeee578b35"><code>1ef4b56</code></a> backport of <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1449">#1449</a> (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1453">#1453</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/8fe5c4ea66b9b8187600e6d5ec9b1b6781f44009"><code>8fe5c4e</code></a> 2.x: Specify encoding as an optional peer dependency in package.json (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1310">#1310</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/f56b0c66d3dd2ef185436de1f2fd40f66bfea8f4"><code>f56b0c6</code></a> fix(URL): prefer built in URL version when available and fallback to whatwg (...</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/b5417aea6a3275932283a200214522e6ab53f1ea"><code>b5417ae</code></a> fix: import whatwg-url in a way compatible with ESM Node (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1303">#1303</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/18193c5922c64046b922e18faf41821290535f06"><code>18193c5</code></a> fix v2.6.3 that did not sending query params (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1301">#1301</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/ace7536c955556be742d9910566738630cc3c2a6"><code>ace7536</code></a> fix: properly encode url with unicode characters (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1291">#1291</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/152214ca2f6e2a5a17d71e4638114625d3be30c6"><code>152214c</code></a> Fix(package.json): Corrected main file path in package.json (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1274">#1274</a>)</li>
<li>See full diff in <a href="https://github.com/node-fetch/node-fetch/compare/v2.6.1...v2.6.7">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~endless">endless</a>, a new releaser for node-fetch since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=node-fetch&package-manager=npm_and_yarn&previous-version=2.6.1&new-version=2.6.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/burrow/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-12 16:53:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/burrow/pull/1536" class=".btn">#1536</a>
            </td>
            <td>
                <b>
                    Bump ejs from 2.6.2 to 3.1.7 in /docs/example/basic-app-website
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [ejs](https://github.com/mde/ejs) from 2.6.2 to 3.1.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/mde/ejs/releases">ejs's releases</a>.</em></p>
<blockquote>
<h2>v3.1.7</h2>
<p>Version 3.1.7</p>
<h2>v3.1.6</h2>
<p>Version 3.1.6</p>
<h2>v3.1.5</h2>
<p>Version 3.1.5</p>
<h2>v3.0.2</h2>
<p>No release notes provided.</p>
<h2>v2.7.4</h2>
<h3>Bug fixes</h3>
<ul>
<li>Fixed Node 4 support, which broke in v2.7.3 (<a href="https://github.com/mde/ejs/commit/5e42d6cef15ae6f2c7d29ef55a455e8e49b5e76e">https://github.com/mde/ejs/commit/5e42d6cef15ae6f2c7d29ef55a455e8e49b5e76e</a>, <a href="https://github.com/mde"><code>@​mde</code></a>)</li>
</ul>
<h2>v2.7.3</h2>
<h3>Bug fixes</h3>
<ul>
<li>Made the post-install message more discreet by following the example of <a href="https://github.com/opencollective/opencollective-postinstall">opencollective-postinstall</a> (<a href="https://github.com/mde/ejs/commit/228d8e45b7ced2afd3e596c13d44aed464e57e43">https://github.com/mde/ejs/commit/228d8e45b7ced2afd3e596c13d44aed464e57e43</a>, <a href="https://github.com/mde"><code>@​mde</code></a>)</li>
</ul>
<h2>v2.7.2</h2>
<h3>Features</h3>
<ul>
<li>Added support for destructuring locals (<a href="https://github-redirect.dependabot.com/mde/ejs/issues/452">#452</a>, <a href="https://github.com/ExE-Boss"><code>@​ExE-Boss</code></a>)</li>
<li>Added support for disabling legacy <code>include</code> directives (<a href="https://github-redirect.dependabot.com/mde/ejs/issues/458">#458</a>, <a href="https://github-redirect.dependabot.com/mde/ejs/issues/459">#459</a>, <a href="https://github.com/ExE-Boss"><code>@​ExE-Boss</code></a>)</li>
<li>Compiled functions are now shown in the debugger (<a href="https://github-redirect.dependabot.com/mde/ejs/issues/456">#456</a>, <a href="https://github.com/S2"><code>@​S2</code></a>-)</li>
<li><code>function.name</code> is now set to the file base name in environments that support this (<a href="https://github-redirect.dependabot.com/mde/ejs/issues/466">#466</a>, <a href="https://github.com/ExE-Boss"><code>@​ExE-Boss</code></a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>The error message when <code>async != true</code> now correctly mention the existence of the <code>async</code> option (<a href="https://github-redirect.dependabot.com/mde/ejs/issues/460">#460</a>, <a href="https://github.com/ExE-Boss"><code>@​ExE-Boss</code></a>)</li>
<li>Improved performance of HTML output generation (<a href="https://github-redirect.dependabot.com/mde/ejs/issues/470">#470</a>, <a href="https://github.com/nwoltman"><code>@​nwoltman</code></a>)</li>
</ul>
<h2>v2.7.1</h2>
<h3>Deprecated:</h3>
<ul>
<li>Added deprecation notice for use of <code>require.extensions</code> (<a href="https://github.com/mde"><code>@​mde</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/mde/ejs/blob/main/CHANGELOG.md">ejs's changelog</a>.</em></p>
<blockquote>
<h2>v3.0.1: 2019-11-23</h2>
<ul>
<li>Removed require.extensions (<a href="https://github.com/mde"><code>@​mde</code></a>)</li>
<li>Removed legacy preprocessor include (<a href="https://github.com/mde"><code>@​mde</code></a>)</li>
<li>Removed support for EOL Nodes 4 and 6 (<a href="https://github.com/mde"><code>@​mde</code></a>)</li>
</ul>
<h2>v2.7.4: 2019-11-19</h2>
<h3>Bug fixes</h3>
<ul>
<li>Fixed Node 4 support, which broke in v2.7.3 (<a href="https://github.com/mde/ejs/commit/5e42d6cef15ae6f2c7d29ef55a455e8e49b5e76e"><code>5e42d6c</code></a>, <a href="https://github.com/mde"><code>@​mde</code></a>)</li>
</ul>
<h2>v2.7.3: 2019-11-19</h2>
<h3>Bug fixes</h3>
<ul>
<li>Made the post-install message more discreet by following the example of <a href="https://github.com/opencollective/opencollective-postinstall">opencollective-postinstall</a> (<a href="https://github.com/mde/ejs/commit/228d8e45b7ced2afd3e596c13d44aed464e57e43"><code>228d8e4</code></a>, <a href="https://github.com/mde"><code>@​mde</code></a>)</li>
</ul>
<h2>v2.7.2: 2019-11-13</h2>
<h3>Features</h3>
<ul>
<li>Added support for destructuring locals (<a href="https://github-redirect.dependabot.com/mde/ejs/pull/452">#452</a>, <a href="https://github.com/ExE-Boss"><code>@​ExE-Boss</code></a>)</li>
<li>Added support for disabling legacy <code>include</code> directives (<a href="https://github-redirect.dependabot.com/mde/ejs/pull/458">#458</a>, <a href="https://github-redirect.dependabot.com/mde/ejs/pull/459">#459</a>, <a href="https://github.com/ExE-Boss"><code>@​ExE-Boss</code></a>)</li>
<li>Compiled functions are now shown in the debugger (<a href="https://github-redirect.dependabot.com/mde/ejs/pull/456">#456</a>, <a href="https://github.com/S2-"><code>@​S2-</code></a>)</li>
<li><code>function.name</code> is now set to the file base name in environments that support this (<a href="https://github-redirect.dependabot.com/mde/ejs/pull/466">#466</a>, <a href="https://github.com/ExE-Boss"><code>@​ExE-Boss</code></a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>The error message when <code>async != true</code> now correctly mention the existence of the <code>async</code> option (<a href="https://github-redirect.dependabot.com/mde/ejs/pull/460">#460</a>, <a href="https://github.com/ExE-Boss"><code>@​ExE-Boss</code></a>)</li>
<li>Improved performance of HTML output generation (<a href="https://github-redirect.dependabot.com/mde/ejs/pull/470">#470</a>, <a href="https://github.com/nwoltman"><code>@​nwoltman</code></a>)</li>
</ul>
<h2>v2.7.1: 2019-09-02</h2>
<ul>
<li>Added deprecation notice for use of require.extensions (<a href="https://github.com/mde"><code>@​mde</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/mde/ejs/commit/820855ad75034e303be82c482c5eb8c6616da5c5"><code>820855a</code></a> Version 3.1.7</li>
<li><a href="https://github.com/mde/ejs/commit/076dcb643c5aed2e10c2847639c98fd923b72854"><code>076dcb6</code></a> Don't use template literal</li>
<li><a href="https://github.com/mde/ejs/commit/faf8b849a4e46db21fa813a08a7cbe00256a188a"><code>faf8b84</code></a> Skip test -- error message vary depending on JS runtime</li>
<li><a href="https://github.com/mde/ejs/commit/c028c343c127859f7189c3feee1e5239c199fec9"><code>c028c34</code></a> Update packages</li>
<li><a href="https://github.com/mde/ejs/commit/e4180b4fa2dd0e06d811f2c155f9d993ee9d8edd"><code>e4180b4</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/mde/ejs/issues/629">#629</a> from markbrouwer96/main</li>
<li><a href="https://github.com/mde/ejs/commit/d5404d6e68d64c165580d238e7562ea6532c2541"><code>d5404d6</code></a> Updated jsdoc to 3.6.7</li>
<li><a href="https://github.com/mde/ejs/commit/7b0845d6aab044d244e8ec3818f0f70d05ef13c1"><code>7b0845d</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/mde/ejs/issues/609">#609</a> from mde/dependabot/npm_and_yarn/glob-parent-5.1.2</li>
<li><a href="https://github.com/mde/ejs/commit/32fb8ee387383c67eaa5feff05347ef0504f3b15"><code>32fb8ee</code></a> Bump glob-parent from 5.1.1 to 5.1.2</li>
<li><a href="https://github.com/mde/ejs/commit/f21a9e464337032af5e61352c54b9dd8dae8fd1b"><code>f21a9e4</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/mde/ejs/issues/603">#603</a> from mde/mde-null-proto-where-possible</li>
<li><a href="https://github.com/mde/ejs/commit/a50e46f002a78544e10982a037742cfb67fc7b80"><code>a50e46f</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/mde/ejs/issues/606">#606</a> from akash-55/main</li>
<li>Additional commits viewable in <a href="https://github.com/mde/ejs/compare/v2.6.2...v3.1.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ejs&package-manager=npm_and_yarn&previous-version=2.6.2&new-version=3.1.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/burrow/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-12 16:53:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/burrow/pull/1535" class=".btn">#1535</a>
            </td>
            <td>
                <b>
                    Archive Burrow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hyperledger Burrow has been moved to End of Life.

Fixes: https://github.com/hyperledger/tsc/issues/34
https://tsc.hyperledger.org/project-lifecycle.html

Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-11 19:36:38 +0000 UTC
    </div>
</div>

