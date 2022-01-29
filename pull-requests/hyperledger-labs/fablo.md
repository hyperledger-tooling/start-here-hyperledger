---
layout: default
title: fablo
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fablo
---

# fablo <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fablo){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/280" class=".btn">#280</a>
            </td>
            <td>
                <b>
                    Bump node-fetch from 2.6.1 to 2.6.7
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
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/node-fetch/node-fetch/blob/main/docs/CHANGELOG.md">node-fetch's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<p>All notable changes will be recorded here.</p>
<p>The format is based on <a href="https://keepachangelog.com/en/1.0.0/">Keep a Changelog</a>,
and this project adheres to <a href="https://semver.org/spec/v2.0.0.html">Semantic Versioning</a>.</p>
<h2>What's Changed</h2>
<ul>
<li>core: update fetch-blob by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1371">node-fetch/node-fetch#1371</a></li>
<li>docs: Fix typo around sending a file by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1381">node-fetch/node-fetch#1381</a></li>
<li>core: (http.request): Cast URL to string before sending it to NodeJS core by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1378">node-fetch/node-fetch#1378</a></li>
<li>core: handle errors from the request body stream by <a href="https://github.com/mdmitry01"><code>@​mdmitry01</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1392">node-fetch/node-fetch#1392</a></li>
<li>core: Better handle wrong redirect header in a response by <a href="https://github.com/tasinet"><code>@​tasinet</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1387">node-fetch/node-fetch#1387</a></li>
<li>core: Don't use buffer to make a blob by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1402">node-fetch/node-fetch#1402</a></li>
<li>docs: update readme for TS <code>@​types/node-fetch</code> by <a href="https://github.com/adamellsworth"><code>@​adamellsworth</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1405">node-fetch/node-fetch#1405</a></li>
<li>core: Fix logical operator priority to disallow GET/HEAD with non-empty body by <a href="https://github.com/maxshirshin"><code>@​maxshirshin</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1369">node-fetch/node-fetch#1369</a></li>
<li>core: Don't use global buffer by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1422">node-fetch/node-fetch#1422</a></li>
<li>ci: fix main branch by <a href="https://github.com/dnalborczyk"><code>@​dnalborczyk</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1429">node-fetch/node-fetch#1429</a></li>
<li>core: use more node: protocol imports by <a href="https://github.com/dnalborczyk"><code>@​dnalborczyk</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1428">node-fetch/node-fetch#1428</a></li>
<li>core: Warn when using data by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1421">node-fetch/node-fetch#1421</a></li>
<li>docs: Create SECURITY.md by <a href="https://github.com/JamieSlome"><code>@​JamieSlome</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1445">node-fetch/node-fetch#1445</a></li>
<li>core: don't forward secure headers to 3th party by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1449">node-fetch/node-fetch#1449</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/mdmitry01"><code>@​mdmitry01</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1392">node-fetch/node-fetch#1392</a></li>
<li><a href="https://github.com/tasinet"><code>@​tasinet</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1387">node-fetch/node-fetch#1387</a></li>
<li><a href="https://github.com/adamellsworth"><code>@​adamellsworth</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1405">node-fetch/node-fetch#1405</a></li>
<li><a href="https://github.com/maxshirshin"><code>@​maxshirshin</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1369">node-fetch/node-fetch#1369</a></li>
<li><a href="https://github.com/JamieSlome"><code>@​JamieSlome</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1445">node-fetch/node-fetch#1445</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/node-fetch/node-fetch/compare/v3.1.0...v3.1.2">https://github.com/node-fetch/node-fetch/compare/v3.1.0...v3.1.2</a></p>
<h2>3.1.0</h2>
<h2>What's Changed</h2>
<ul>
<li>fix(Body): Discourage form-data and buffer() by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1212">node-fetch/node-fetch#1212</a></li>
<li>fix: Pass url string to http.request by <a href="https://github.com/serverwentdown"><code>@​serverwentdown</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1268">node-fetch/node-fetch#1268</a></li>
<li>Fix octocat image link by <a href="https://github.com/lakuapik"><code>@​lakuapik</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1281">node-fetch/node-fetch#1281</a></li>
<li>fix(Body.body): Normalize <code>Body.body</code> into a <code>node:stream</code> by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/924">node-fetch/node-fetch#924</a></li>
<li>docs(Headers): Add default Host request header to README.md file by <a href="https://github.com/robertoaceves"><code>@​robertoaceves</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1316">node-fetch/node-fetch#1316</a></li>
<li>Update CHANGELOG.md by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1292">node-fetch/node-fetch#1292</a></li>
<li>Add highWaterMark to cloned properties by <a href="https://github.com/davesidious"><code>@​davesidious</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1162">node-fetch/node-fetch#1162</a></li>
<li>Update README.md to fix HTTPResponseError by <a href="https://github.com/thedanfernandez"><code>@​thedanfernandez</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1135">node-fetch/node-fetch#1135</a></li>
<li>docs: switch <code>url</code> to <code>URL</code> by <a href="https://github.com/dhritzkiv"><code>@​dhritzkiv</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1318">node-fetch/node-fetch#1318</a></li>
<li>fix(types): declare buffer() deprecated by <a href="https://github.com/dnalborczyk"><code>@​dnalborczyk</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1345">node-fetch/node-fetch#1345</a></li>
<li>chore: fix lint by <a href="https://github.com/dnalborczyk"><code>@​dnalborczyk</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1348">node-fetch/node-fetch#1348</a></li>
<li>refactor: use node: prefix for imports by <a href="https://github.com/dnalborczyk"><code>@​dnalborczyk</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1346">node-fetch/node-fetch#1346</a></li>
<li>Bump data-uri-to-buffer from 3.0.1 to 4.0.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1319">node-fetch/node-fetch#1319</a></li>
<li>Bump mocha from 8.4.0 to 9.1.3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1339">node-fetch/node-fetch#1339</a></li>
<li>Referrer and Referrer Policy by <a href="https://github.com/tekwiz"><code>@​tekwiz</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1057">node-fetch/node-fetch#1057</a></li>
<li>Add typing for Response.redirect(url, status) by <a href="https://github.com/c-w"><code>@​c-w</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1169">node-fetch/node-fetch#1169</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fablo/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-23 19:09:53 +0000 UTC
    </div>
</div>

