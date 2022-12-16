---
layout: default
title: university-course
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/university-course
---

# university-course <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/university-course){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/university-course/pull/95" class=".btn">#95</a>
            </td>
            <td>
                <b>
                    chore(deps): bump express from 4.17.1 to 4.18.2 in /support/Lab06/b4s/organization/university/user-interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [express](https://github.com/expressjs/express) from 4.17.1 to 4.18.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/express/releases">express's releases</a>.</em></p>
<blockquote>
<h2>4.18.2</h2>
<ul>
<li>Fix regression routing a large stack in a single route</li>
<li>deps: body-parser@1.20.1
<ul>
<li>deps: qs@6.11.0</li>
<li>perf: remove unnecessary object clone</li>
</ul>
</li>
<li>deps: qs@6.11.0</li>
</ul>
<h2>4.18.1</h2>
<ul>
<li>Fix hanging on large stack of sync routes</li>
</ul>
<h2>4.18.0</h2>
<ul>
<li>Add &quot;root&quot; option to <code>res.download</code></li>
<li>Allow <code>options</code> without <code>filename</code> in <code>res.download</code></li>
<li>Deprecate string and non-integer arguments to <code>res.status</code></li>
<li>Fix behavior of <code>null</code>/<code>undefined</code> as <code>maxAge</code> in <code>res.cookie</code></li>
<li>Fix handling very large stacks of sync middleware</li>
<li>Ignore <code>Object.prototype</code> values in settings through <code>app.set</code>/<code>app.get</code></li>
<li>Invoke <code>default</code> with same arguments as types in <code>res.format</code></li>
<li>Support proper 205 responses using <code>res.send</code></li>
<li>Use <code>http-errors</code> for <code>res.format</code> error</li>
<li>deps: body-parser@1.20.0
<ul>
<li>Fix error message for json parse whitespace in <code>strict</code></li>
<li>Fix internal error when inflated body exceeds limit</li>
<li>Prevent loss of async hooks context</li>
<li>Prevent hanging when request already read</li>
<li>deps: depd@2.0.0</li>
<li>deps: http-errors@2.0.0</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: qs@6.10.3</li>
<li>deps: raw-body@2.5.1</li>
</ul>
</li>
<li>deps: cookie@0.5.0
<ul>
<li>Add <code>priority</code> option</li>
<li>Fix <code>expires</code> option to reject invalid dates</li>
</ul>
</li>
<li>deps: depd@2.0.0
<ul>
<li>Replace internal <code>eval</code> usage with <code>Function</code> constructor</li>
<li>Use instance methods on <code>process</code> to check for listeners</li>
</ul>
</li>
<li>deps: finalhandler@1.2.0
<ul>
<li>Remove set content headers that break response</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: statuses@2.0.1</li>
</ul>
</li>
<li>deps: on-finished@2.4.1
<ul>
<li>Prevent loss of async hooks context</li>
</ul>
</li>
<li>deps: qs@6.10.3</li>
<li>deps: send@0.18.0
<ul>
<li>Fix emitted 416 error missing headers property</li>
<li>Limit the headers removed for 304 response</li>
<li>deps: depd@2.0.0</li>
<li>deps: destroy@1.2.0</li>
<li>deps: http-errors@2.0.0</li>
<li>deps: on-finished@2.4.1</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/express/blob/master/History.md">express's changelog</a>.</em></p>
<blockquote>
<h1>4.18.2 / 2022-10-08</h1>
<ul>
<li>Fix regression routing a large stack in a single route</li>
<li>deps: body-parser@1.20.1
<ul>
<li>deps: qs@6.11.0</li>
<li>perf: remove unnecessary object clone</li>
</ul>
</li>
<li>deps: qs@6.11.0</li>
</ul>
<h1>4.18.1 / 2022-04-29</h1>
<ul>
<li>Fix hanging on large stack of sync routes</li>
</ul>
<h1>4.18.0 / 2022-04-25</h1>
<ul>
<li>Add &quot;root&quot; option to <code>res.download</code></li>
<li>Allow <code>options</code> without <code>filename</code> in <code>res.download</code></li>
<li>Deprecate string and non-integer arguments to <code>res.status</code></li>
<li>Fix behavior of <code>null</code>/<code>undefined</code> as <code>maxAge</code> in <code>res.cookie</code></li>
<li>Fix handling very large stacks of sync middleware</li>
<li>Ignore <code>Object.prototype</code> values in settings through <code>app.set</code>/<code>app.get</code></li>
<li>Invoke <code>default</code> with same arguments as types in <code>res.format</code></li>
<li>Support proper 205 responses using <code>res.send</code></li>
<li>Use <code>http-errors</code> for <code>res.format</code> error</li>
<li>deps: body-parser@1.20.0
<ul>
<li>Fix error message for json parse whitespace in <code>strict</code></li>
<li>Fix internal error when inflated body exceeds limit</li>
<li>Prevent loss of async hooks context</li>
<li>Prevent hanging when request already read</li>
<li>deps: depd@2.0.0</li>
<li>deps: http-errors@2.0.0</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: qs@6.10.3</li>
<li>deps: raw-body@2.5.1</li>
</ul>
</li>
<li>deps: cookie@0.5.0
<ul>
<li>Add <code>priority</code> option</li>
<li>Fix <code>expires</code> option to reject invalid dates</li>
</ul>
</li>
<li>deps: depd@2.0.0
<ul>
<li>Replace internal <code>eval</code> usage with <code>Function</code> constructor</li>
<li>Use instance methods on <code>process</code> to check for listeners</li>
</ul>
</li>
<li>deps: finalhandler@1.2.0
<ul>
<li>Remove set content headers that break response</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: statuses@2.0.1</li>
</ul>
</li>
<li>deps: on-finished@2.4.1
<ul>
<li>Prevent loss of async hooks context</li>
</ul>
</li>
<li>deps: qs@6.10.3</li>
<li>deps: send@0.18.0</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/expressjs/express/commit/8368dc178af16b91b576c4c1d135f701a0007e5d"><code>8368dc1</code></a> 4.18.2</li>
<li><a href="https://github.com/expressjs/express/commit/61f40491222dbede653b9938e6a4676f187aab44"><code>61f4049</code></a> docs: replace Freenode with Libera Chat</li>
<li><a href="https://github.com/expressjs/express/commit/bb7907b932afe3a19236a642f6054b6c8f7349a0"><code>bb7907b</code></a> build: Node.js@18.10</li>
<li><a href="https://github.com/expressjs/express/commit/f56ce73186e885a938bfdb3d3d1005a58e6ae12b"><code>f56ce73</code></a> build: supertest@6.3.0</li>
<li><a href="https://github.com/expressjs/express/commit/24b3dc551670ac4fb0cd5a2bd5ef643c9525e60f"><code>24b3dc5</code></a> deps: qs@6.11.0</li>
<li><a href="https://github.com/expressjs/express/commit/689d175b8b39d8860b81d723233fb83d15201827"><code>689d175</code></a> deps: body-parser@1.20.1</li>
<li><a href="https://github.com/expressjs/express/commit/340be0f79afb9b3176afb76235aa7f92acbd5050"><code>340be0f</code></a> build: eslint@8.24.0</li>
<li><a href="https://github.com/expressjs/express/commit/33e8dc303af9277f8a7e4f46abfdcb5e72f6797b"><code>33e8dc3</code></a> docs: use Node.js name style</li>
<li><a href="https://github.com/expressjs/express/commit/644f6464b9f61cbafa8f880636b1aa5237d95bad"><code>644f646</code></a> build: supertest@6.2.4</li>
<li><a href="https://github.com/expressjs/express/commit/ecd7572f1e920b7a512452b8d9806ae617a99c54"><code>ecd7572</code></a> build: Node.js@14.20</li>
<li>Additional commits viewable in <a href="https://github.com/expressjs/express/compare/4.17.1...4.18.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=express&package-manager=npm_and_yarn&previous-version=4.17.1&new-version=4.18.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/university-course/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-13 14:13:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/university-course/pull/94" class=".btn">#94</a>
            </td>
            <td>
                <b>
                    chore(deps): bump qs from 6.5.2 to 6.5.3 in /support/Lab02
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [qs](https://github.com/ljharb/qs) from 6.5.2 to 6.5.3.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ljharb/qs/blob/main/CHANGELOG.md">qs's changelog</a>.</em></p>
<blockquote>
<h2><strong>6.5.3</strong></h2>
<ul>
<li>[Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/428">#428</a>)</li>
<li>[Fix] <code>utils.merge</code>: avoid a crash with a null target and a truthy non-array source</li>
<li>[Fix] correctly parse nested arrays</li>
<li>[Fix] <code>stringify</code>: fix a crash with <code>strictNullHandling</code> and a custom <code>filter</code>/<code>serializeDate</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/279">#279</a>)</li>
<li>[Fix] <code>utils</code>: <code>merge</code>: fix crash when <code>source</code> is a truthy primitive &amp; no options are provided</li>
<li>[Fix] when <code>parseArrays</code> is false, properly handle keys ending in <code>[]</code></li>
<li>[Fix] fix for an impossible situation: when the formatter is called with a non-string value</li>
<li>[Fix] <code>utils.merge</code>: avoid a crash with a null target and an array source</li>
<li>[Refactor] <code>utils</code>: reduce observable [[Get]]s</li>
<li>[Refactor] use cached <code>Array.isArray</code></li>
<li>[Refactor] <code>stringify</code>: Avoid arr = arr.concat(...), push to the existing instance (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/269">#269</a>)</li>
<li>[Refactor] <code>parse</code>: only need to reassign the var once</li>
<li>[Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/427">#427</a>)</li>
<li>[readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li>[Docs] Clean up license text so it’s properly detected as BSD-3-Clause</li>
<li>[Docs] Clarify the need for &quot;arrayLimit&quot; option</li>
<li>[meta] fix README.md (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/399">#399</a>)</li>
<li>[meta] add FUNDING.yml</li>
<li>[actions] backport actions from main</li>
<li>[Tests] always use <code>String(x)</code> over <code>x.toString()</code></li>
<li>[Tests] remove nonexistent tape option</li>
<li>[Dev Deps] backport from main</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ljharb/qs/commit/298bfa55d6db00ddea78dd0333509aadf9bb3077"><code>298bfa5</code></a> v6.5.3</li>
<li><a href="https://github.com/ljharb/qs/commit/ed0f5dcbef4b168a8ae299d78b1e4a2e9b1baf1f"><code>ed0f5dc</code></a> [Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/428">#428</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/691e739cfa40cd42604dc05a54e6154371a429ab"><code>691e739</code></a> [Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/427">#427</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/1072d57d38a690e1ad7616dced44390bffedcbb2"><code>1072d57</code></a> [readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li><a href="https://github.com/ljharb/qs/commit/12ac1c403aaa04d1a34844f514ed9f9abfb76e64"><code>12ac1c4</code></a> [meta] fix README.md (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/399">#399</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/0338716b09fdbd4711823eeb0a14e556a2498e7a"><code>0338716</code></a> [actions] backport actions from main</li>
<li><a href="https://github.com/ljharb/qs/commit/5639c20ce0a7c1332200a3181339331483e5a3a1"><code>5639c20</code></a> Clean up license text so it’s properly detected as BSD-3-Clause</li>
<li><a href="https://github.com/ljharb/qs/commit/51b8a0b1b213596dd1702b837f5e7dec2229793d"><code>51b8a0b</code></a> add FUNDING.yml</li>
<li><a href="https://github.com/ljharb/qs/commit/45f675936e742d92fac8d4dae5cfc385c576a977"><code>45f6759</code></a> [Fix] fix for an impossible situation: when the formatter is called with a no...</li>
<li><a href="https://github.com/ljharb/qs/commit/f814a7f8f2af059f8158f7e4b2bf8b46aeb62cd3"><code>f814a7f</code></a> [Dev Deps] backport from main</li>
<li>Additional commits viewable in <a href="https://github.com/ljharb/qs/compare/v6.5.2...v6.5.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=qs&package-manager=npm_and_yarn&previous-version=6.5.2&new-version=6.5.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/university-course/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-11 20:09:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/university-course/pull/93" class=".btn">#93</a>
            </td>
            <td>
                <b>
                    chore(deps): bump qs, body-parser and express in /support/Lab06/b4s/organization/students-union/b4s_client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [qs](https://github.com/ljharb/qs) to 6.5.3 and updates ancestor dependencies [qs](https://github.com/ljharb/qs), [body-parser](https://github.com/expressjs/body-parser) and [express](https://github.com/expressjs/express). These dependencies need to be updated together.

Updates `qs` from 6.5.2 to 6.5.3
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ljharb/qs/blob/main/CHANGELOG.md">qs's changelog</a>.</em></p>
<blockquote>
<h2><strong>6.5.3</strong></h2>
<ul>
<li>[Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/428">#428</a>)</li>
<li>[Fix] <code>utils.merge</code>: avoid a crash with a null target and a truthy non-array source</li>
<li>[Fix] correctly parse nested arrays</li>
<li>[Fix] <code>stringify</code>: fix a crash with <code>strictNullHandling</code> and a custom <code>filter</code>/<code>serializeDate</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/279">#279</a>)</li>
<li>[Fix] <code>utils</code>: <code>merge</code>: fix crash when <code>source</code> is a truthy primitive &amp; no options are provided</li>
<li>[Fix] when <code>parseArrays</code> is false, properly handle keys ending in <code>[]</code></li>
<li>[Fix] fix for an impossible situation: when the formatter is called with a non-string value</li>
<li>[Fix] <code>utils.merge</code>: avoid a crash with a null target and an array source</li>
<li>[Refactor] <code>utils</code>: reduce observable [[Get]]s</li>
<li>[Refactor] use cached <code>Array.isArray</code></li>
<li>[Refactor] <code>stringify</code>: Avoid arr = arr.concat(...), push to the existing instance (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/269">#269</a>)</li>
<li>[Refactor] <code>parse</code>: only need to reassign the var once</li>
<li>[Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/427">#427</a>)</li>
<li>[readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li>[Docs] Clean up license text so it’s properly detected as BSD-3-Clause</li>
<li>[Docs] Clarify the need for &quot;arrayLimit&quot; option</li>
<li>[meta] fix README.md (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/399">#399</a>)</li>
<li>[meta] add FUNDING.yml</li>
<li>[actions] backport actions from main</li>
<li>[Tests] always use <code>String(x)</code> over <code>x.toString()</code></li>
<li>[Tests] remove nonexistent tape option</li>
<li>[Dev Deps] backport from main</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ljharb/qs/commit/298bfa55d6db00ddea78dd0333509aadf9bb3077"><code>298bfa5</code></a> v6.5.3</li>
<li><a href="https://github.com/ljharb/qs/commit/ed0f5dcbef4b168a8ae299d78b1e4a2e9b1baf1f"><code>ed0f5dc</code></a> [Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/428">#428</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/691e739cfa40cd42604dc05a54e6154371a429ab"><code>691e739</code></a> [Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/427">#427</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/1072d57d38a690e1ad7616dced44390bffedcbb2"><code>1072d57</code></a> [readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li><a href="https://github.com/ljharb/qs/commit/12ac1c403aaa04d1a34844f514ed9f9abfb76e64"><code>12ac1c4</code></a> [meta] fix README.md (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/399">#399</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/0338716b09fdbd4711823eeb0a14e556a2498e7a"><code>0338716</code></a> [actions] backport actions from main</li>
<li><a href="https://github.com/ljharb/qs/commit/5639c20ce0a7c1332200a3181339331483e5a3a1"><code>5639c20</code></a> Clean up license text so it’s properly detected as BSD-3-Clause</li>
<li><a href="https://github.com/ljharb/qs/commit/51b8a0b1b213596dd1702b837f5e7dec2229793d"><code>51b8a0b</code></a> add FUNDING.yml</li>
<li><a href="https://github.com/ljharb/qs/commit/45f675936e742d92fac8d4dae5cfc385c576a977"><code>45f6759</code></a> [Fix] fix for an impossible situation: when the formatter is called with a no...</li>
<li><a href="https://github.com/ljharb/qs/commit/f814a7f8f2af059f8158f7e4b2bf8b46aeb62cd3"><code>f814a7f</code></a> [Dev Deps] backport from main</li>
<li>Additional commits viewable in <a href="https://github.com/ljharb/qs/compare/v6.5.2...v6.5.3">compare view</a></li>
</ul>
</details>
<br />

Updates `body-parser` from 1.19.0 to 1.20.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/body-parser/releases">body-parser's releases</a>.</em></p>
<blockquote>
<h2>1.20.0</h2>
<ul>
<li>Fix error message for json parse whitespace in <code>strict</code></li>
<li>Fix internal error when inflated body exceeds limit</li>
<li>Prevent loss of async hooks context</li>
<li>Prevent hanging when request already read</li>
<li>deps: depd@2.0.0
<ul>
<li>Replace internal <code>eval</code> usage with <code>Function</code> constructor</li>
<li>Use instance methods on <code>process</code> to check for listeners</li>
</ul>
</li>
<li>deps: http-errors@2.0.0
<ul>
<li>deps: depd@2.0.0</li>
<li>deps: statuses@2.0.1</li>
</ul>
</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: qs@6.10.3</li>
<li>deps: raw-body@2.5.1
<ul>
<li>deps: http-errors@2.0.0</li>
</ul>
</li>
</ul>
<h2>1.19.2</h2>
<ul>
<li>deps: bytes@3.1.2</li>
<li>deps: qs@6.9.7
<ul>
<li>Fix handling of <code>__proto__</code> keys</li>
</ul>
</li>
<li>deps: raw-body@2.4.3
<ul>
<li>deps: bytes@3.1.2</li>
</ul>
</li>
</ul>
<h2>1.19.1</h2>
<ul>
<li>deps: bytes@3.1.1</li>
<li>deps: http-errors@1.8.1
<ul>
<li>deps: inherits@2.0.4</li>
<li>deps: toidentifier@1.0.1</li>
<li>deps: setprototypeof@1.2.0</li>
</ul>
</li>
<li>deps: qs@6.9.6</li>
<li>deps: raw-body@2.4.2
<ul>
<li>deps: bytes@3.1.1</li>
<li>deps: http-errors@1.8.1</li>
</ul>
</li>
<li>deps: safe-buffer@5.2.1</li>
<li>deps: type-is@~1.6.18</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/body-parser/blob/master/HISTORY.md">body-parser's changelog</a>.</em></p>
<blockquote>
<h1>1.20.1 / 2022-10-06</h1>
<ul>
<li>deps: qs@6.11.0</li>
<li>perf: remove unnecessary object clone</li>
</ul>
<h1>1.20.0 / 2022-04-02</h1>
<ul>
<li>Fix error message for json parse whitespace in <code>strict</code></li>
<li>Fix internal error when inflated body exceeds limit</li>
<li>Prevent loss of async hooks context</li>
<li>Prevent hanging when request already read</li>
<li>deps: depd@2.0.0
<ul>
<li>Replace internal <code>eval</code> usage with <code>Function</code> constructor</li>
<li>Use instance methods on <code>process</code> to check for listeners</li>
</ul>
</li>
<li>deps: http-errors@2.0.0
<ul>
<li>deps: depd@2.0.0</li>
<li>deps: statuses@2.0.1</li>
</ul>
</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: qs@6.10.3</li>
<li>deps: raw-body@2.5.1
<ul>
<li>deps: http-errors@2.0.0</li>
</ul>
</li>
</ul>
<h1>1.19.2 / 2022-02-15</h1>
<ul>
<li>deps: bytes@3.1.2</li>
<li>deps: qs@6.9.7
<ul>
<li>Fix handling of <code>__proto__</code> keys</li>
</ul>
</li>
<li>deps: raw-body@2.4.3
<ul>
<li>deps: bytes@3.1.2</li>
</ul>
</li>
</ul>
<h1>1.19.1 / 2021-12-10</h1>
<ul>
<li>deps: bytes@3.1.1</li>
<li>deps: http-errors@1.8.1
<ul>
<li>deps: inherits@2.0.4</li>
<li>deps: toidentifier@1.0.1</li>
<li>deps: setprototypeof@1.2.0</li>
</ul>
</li>
<li>deps: qs@6.9.6</li>
<li>deps: raw-body@2.4.2
<ul>
<li>deps: bytes@3.1.1</li>
<li>deps: http-errors@1.8.1</li>
</ul>
</li>
<li>deps: safe-buffer@5.2.1</li>
<li>deps: type-is@~1.6.18</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/expressjs/body-parser/commit/830bdfbee021d540a742de857dcbd43f40563a02"><code>830bdfb</code></a> 1.20.1</li>
<li><a href="https://github.com/expressjs/body-parser/commit/ecad1ccf9eefe61a4ba5b8354d914e262eba7648"><code>ecad1cc</code></a> build: eslint@8.24.0</li>
<li><a href="https://github.com/expressjs/body-parser/commit/03b93cf9f11c201631a8cefa09df08feb6f2bb00"><code>03b93cf</code></a> build: supertest@6.3.0</li>
<li><a href="https://github.com/expressjs/body-parser/commit/2c611fcda0fe54043eb8c914f1fde412ba9432c0"><code>2c611fc</code></a> build: Node.js@18.10</li>
<li><a href="https://github.com/expressjs/body-parser/commit/f199e94b115de00feae7ae5559638c0c52019b2e"><code>f199e94</code></a> perf: remove unnecessary object clone</li>
<li><a href="https://github.com/expressjs/body-parser/commit/0123e12d6b6db1bdb66b271b2822b5070096dc32"><code>0123e12</code></a> build: Node.js@18.9</li>
<li><a href="https://github.com/expressjs/body-parser/commit/de1e6c2b390244e486f235151d8e6b9646f2122f"><code>de1e6c2</code></a> build: Node.js@16.17</li>
<li><a href="https://github.com/expressjs/body-parser/commit/477ff13b9c608800cc25331e0de6da6cd4970ee3"><code>477ff13</code></a> build: eslint-plugin-import@2.26.0</li>
<li><a href="https://github.com/expressjs/body-parser/commit/40c3fff30b0d88763e89f1a41ed76d2cf8aa1b14"><code>40c3fff</code></a> deps: qs@6.11.0</li>
<li><a href="https://github.com/expressjs/body-parser/commit/4aa84b70c298354e902edfc4a85ddfdc9fa905c8"><code>4aa84b7</code></a> build: supertest@6.2.4</li>
<li>Additional commits viewable in <a href="https://github.com/expressjs/body-parser/compare/1.19.0...1.20.1">compare view</a></li>
</ul>
</details>
<br />

Updates `express` from 4.16.4 to 4.18.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/express/releases">express's releases</a>.</em></p>
<blockquote>
<h2>4.18.2</h2>
<ul>
<li>Fix regression routing a large stack in a single route</li>
<li>deps: body-parser@1.20.1
<ul>
<li>deps: qs@6.11.0</li>
<li>perf: remove unnecessary object clone</li>
</ul>
</li>
<li>deps: qs@6.11.0</li>
</ul>
<h2>4.18.1</h2>
<ul>
<li>Fix hanging on large stack of sync routes</li>
</ul>
<h2>4.18.0</h2>
<ul>
<li>Add &quot;root&quot; option to <code>res.download</code></li>
<li>Allow <code>options</code> without <code>filename</code> in <code>res.download</code></li>
<li>Deprecate string and non-integer arguments to <code>res.status</code></li>
<li>Fix behavior of <code>null</code>/<code>undefined</code> as <code>maxAge</code> in <code>res.cookie</code></li>
<li>Fix handling very large stacks of sync middleware</li>
<li>Ignore <code>Object.prototype</code> values in settings through <code>app.set</code>/<code>app.get</code></li>
<li>Invoke <code>default</code> with same arguments as types in <code>res.format</code></li>
<li>Support proper 205 responses using <code>res.send</code></li>
<li>Use <code>http-errors</code> for <code>res.format</code> error</li>
<li>deps: body-parser@1.20.0
<ul>
<li>Fix error message for json parse whitespace in <code>strict</code></li>
<li>Fix internal error when inflated body exceeds limit</li>
<li>Prevent loss of async hooks context</li>
<li>Prevent hanging when request already read</li>
<li>deps: depd@2.0.0</li>
<li>deps: http-errors@2.0.0</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: qs@6.10.3</li>
<li>deps: raw-body@2.5.1</li>
</ul>
</li>
<li>deps: cookie@0.5.0
<ul>
<li>Add <code>priority</code> option</li>
<li>Fix <code>expires</code> option to reject invalid dates</li>
</ul>
</li>
<li>deps: depd@2.0.0
<ul>
<li>Replace internal <code>eval</code> usage with <code>Function</code> constructor</li>
<li>Use instance methods on <code>process</code> to check for listeners</li>
</ul>
</li>
<li>deps: finalhandler@1.2.0
<ul>
<li>Remove set content headers that break response</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: statuses@2.0.1</li>
</ul>
</li>
<li>deps: on-finished@2.4.1
<ul>
<li>Prevent loss of async hooks context</li>
</ul>
</li>
<li>deps: qs@6.10.3</li>
<li>deps: send@0.18.0
<ul>
<li>Fix emitted 416 error missing headers property</li>
<li>Limit the headers removed for 304 response</li>
<li>deps: depd@2.0.0</li>
<li>deps: destroy@1.2.0</li>
<li>deps: http-errors@2.0.0</li>
<li>deps: on-finished@2.4.1</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/express/blob/master/History.md">express's changelog</a>.</em></p>
<blockquote>
<h1>4.18.2 / 2022-10-08</h1>
<ul>
<li>Fix regression routing a large stack in a single route</li>
<li>deps: body-parser@1.20.1
<ul>
<li>deps: qs@6.11.0</li>
<li>perf: remove unnecessary object clone</li>
</ul>
</li>
<li>deps: qs@6.11.0</li>
</ul>
<h1>4.18.1 / 2022-04-29</h1>
<ul>
<li>Fix hanging on large stack of sync routes</li>
</ul>
<h1>4.18.0 / 2022-04-25</h1>
<ul>
<li>Add &quot;root&quot; option to <code>res.download</code></li>
<li>Allow <code>options</code> without <code>filename</code> in <code>res.download</code></li>
<li>Deprecate string and non-integer arguments to <code>res.status</code></li>
<li>Fix behavior of <code>null</code>/<code>undefined</code> as <code>maxAge</code> in <code>res.cookie</code></li>
<li>Fix handling very large stacks of sync middleware</li>
<li>Ignore <code>Object.prototype</code> values in settings through <code>app.set</code>/<code>app.get</code></li>
<li>Invoke <code>default</code> with same arguments as types in <code>res.format</code></li>
<li>Support proper 205 responses using <code>res.send</code></li>
<li>Use <code>http-errors</code> for <code>res.format</code> error</li>
<li>deps: body-parser@1.20.0
<ul>
<li>Fix error message for json parse whitespace in <code>strict</code></li>
<li>Fix internal error when inflated body exceeds limit</li>
<li>Prevent loss of async hooks context</li>
<li>Prevent hanging when request already read</li>
<li>deps: depd@2.0.0</li>
<li>deps: http-errors@2.0.0</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: qs@6.10.3</li>
<li>deps: raw-body@2.5.1</li>
</ul>
</li>
<li>deps: cookie@0.5.0
<ul>
<li>Add <code>priority</code> option</li>
<li>Fix <code>expires</code> option to reject invalid dates</li>
</ul>
</li>
<li>deps: depd@2.0.0
<ul>
<li>Replace internal <code>eval</code> usage with <code>Function</code> constructor</li>
<li>Use instance methods on <code>process</code> to check for listeners</li>
</ul>
</li>
<li>deps: finalhandler@1.2.0
<ul>
<li>Remove set content headers that break response</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: statuses@2.0.1</li>
</ul>
</li>
<li>deps: on-finished@2.4.1
<ul>
<li>Prevent loss of async hooks context</li>
</ul>
</li>
<li>deps: qs@6.10.3</li>
<li>deps: send@0.18.0</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/expressjs/express/commit/8368dc178af16b91b576c4c1d135f701a0007e5d"><code>8368dc1</code></a> 4.18.2</li>
<li><a href="https://github.com/expressjs/express/commit/61f40491222dbede653b9938e6a4676f187aab44"><code>61f4049</code></a> docs: replace Freenode with Libera Chat</li>
<li><a href="https://github.com/expressjs/express/commit/bb7907b932afe3a19236a642f6054b6c8f7349a0"><code>bb7907b</code></a> build: Node.js@18.10</li>
<li><a href="https://github.com/expressjs/express/commit/f56ce73186e885a938bfdb3d3d1005a58e6ae12b"><code>f56ce73</code></a> build: supertest@6.3.0</li>
<li><a href="https://github.com/expressjs/express/commit/24b3dc551670ac4fb0cd5a2bd5ef643c9525e60f"><code>24b3dc5</code></a> deps: qs@6.11.0</li>
<li><a href="https://github.com/expressjs/express/commit/689d175b8b39d8860b81d723233fb83d15201827"><code>689d175</code></a> deps: body-parser@1.20.1</li>
<li><a href="https://github.com/expressjs/express/commit/340be0f79afb9b3176afb76235aa7f92acbd5050"><code>340be0f</code></a> build: eslint@8.24.0</li>
<li><a href="https://github.com/expressjs/express/commit/33e8dc303af9277f8a7e4f46abfdcb5e72f6797b"><code>33e8dc3</code></a> docs: use Node.js name style</li>
<li><a href="https://github.com/expressjs/express/commit/644f6464b9f61cbafa8f880636b1aa5237d95bad"><code>644f646</code></a> build: supertest@6.2.4</li>
<li><a href="https://github.com/expressjs/express/commit/ecd7572f1e920b7a512452b8d9806ae617a99c54"><code>ecd7572</code></a> build: Node.js@14.20</li>
<li>Additional commits viewable in <a href="https://github.com/expressjs/express/compare/4.16.4...4.18.2">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/university-course/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-11 18:34:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/university-course/pull/92" class=".btn">#92</a>
            </td>
            <td>
                <b>
                    chore(deps): bump qs, body-parser and express in /support/Lab06/b4s/organization/university/b4s_client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [qs](https://github.com/ljharb/qs) to 6.5.3 and updates ancestor dependencies [qs](https://github.com/ljharb/qs), [body-parser](https://github.com/expressjs/body-parser) and [express](https://github.com/expressjs/express). These dependencies need to be updated together.

Updates `qs` from 6.5.2 to 6.5.3
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ljharb/qs/blob/main/CHANGELOG.md">qs's changelog</a>.</em></p>
<blockquote>
<h2><strong>6.5.3</strong></h2>
<ul>
<li>[Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/428">#428</a>)</li>
<li>[Fix] <code>utils.merge</code>: avoid a crash with a null target and a truthy non-array source</li>
<li>[Fix] correctly parse nested arrays</li>
<li>[Fix] <code>stringify</code>: fix a crash with <code>strictNullHandling</code> and a custom <code>filter</code>/<code>serializeDate</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/279">#279</a>)</li>
<li>[Fix] <code>utils</code>: <code>merge</code>: fix crash when <code>source</code> is a truthy primitive &amp; no options are provided</li>
<li>[Fix] when <code>parseArrays</code> is false, properly handle keys ending in <code>[]</code></li>
<li>[Fix] fix for an impossible situation: when the formatter is called with a non-string value</li>
<li>[Fix] <code>utils.merge</code>: avoid a crash with a null target and an array source</li>
<li>[Refactor] <code>utils</code>: reduce observable [[Get]]s</li>
<li>[Refactor] use cached <code>Array.isArray</code></li>
<li>[Refactor] <code>stringify</code>: Avoid arr = arr.concat(...), push to the existing instance (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/269">#269</a>)</li>
<li>[Refactor] <code>parse</code>: only need to reassign the var once</li>
<li>[Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/427">#427</a>)</li>
<li>[readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li>[Docs] Clean up license text so it’s properly detected as BSD-3-Clause</li>
<li>[Docs] Clarify the need for &quot;arrayLimit&quot; option</li>
<li>[meta] fix README.md (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/399">#399</a>)</li>
<li>[meta] add FUNDING.yml</li>
<li>[actions] backport actions from main</li>
<li>[Tests] always use <code>String(x)</code> over <code>x.toString()</code></li>
<li>[Tests] remove nonexistent tape option</li>
<li>[Dev Deps] backport from main</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ljharb/qs/commit/298bfa55d6db00ddea78dd0333509aadf9bb3077"><code>298bfa5</code></a> v6.5.3</li>
<li><a href="https://github.com/ljharb/qs/commit/ed0f5dcbef4b168a8ae299d78b1e4a2e9b1baf1f"><code>ed0f5dc</code></a> [Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/428">#428</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/691e739cfa40cd42604dc05a54e6154371a429ab"><code>691e739</code></a> [Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/427">#427</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/1072d57d38a690e1ad7616dced44390bffedcbb2"><code>1072d57</code></a> [readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li><a href="https://github.com/ljharb/qs/commit/12ac1c403aaa04d1a34844f514ed9f9abfb76e64"><code>12ac1c4</code></a> [meta] fix README.md (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/399">#399</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/0338716b09fdbd4711823eeb0a14e556a2498e7a"><code>0338716</code></a> [actions] backport actions from main</li>
<li><a href="https://github.com/ljharb/qs/commit/5639c20ce0a7c1332200a3181339331483e5a3a1"><code>5639c20</code></a> Clean up license text so it’s properly detected as BSD-3-Clause</li>
<li><a href="https://github.com/ljharb/qs/commit/51b8a0b1b213596dd1702b837f5e7dec2229793d"><code>51b8a0b</code></a> add FUNDING.yml</li>
<li><a href="https://github.com/ljharb/qs/commit/45f675936e742d92fac8d4dae5cfc385c576a977"><code>45f6759</code></a> [Fix] fix for an impossible situation: when the formatter is called with a no...</li>
<li><a href="https://github.com/ljharb/qs/commit/f814a7f8f2af059f8158f7e4b2bf8b46aeb62cd3"><code>f814a7f</code></a> [Dev Deps] backport from main</li>
<li>Additional commits viewable in <a href="https://github.com/ljharb/qs/compare/v6.5.2...v6.5.3">compare view</a></li>
</ul>
</details>
<br />

Updates `body-parser` from 1.19.0 to 1.20.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/body-parser/releases">body-parser's releases</a>.</em></p>
<blockquote>
<h2>1.20.0</h2>
<ul>
<li>Fix error message for json parse whitespace in <code>strict</code></li>
<li>Fix internal error when inflated body exceeds limit</li>
<li>Prevent loss of async hooks context</li>
<li>Prevent hanging when request already read</li>
<li>deps: depd@2.0.0
<ul>
<li>Replace internal <code>eval</code> usage with <code>Function</code> constructor</li>
<li>Use instance methods on <code>process</code> to check for listeners</li>
</ul>
</li>
<li>deps: http-errors@2.0.0
<ul>
<li>deps: depd@2.0.0</li>
<li>deps: statuses@2.0.1</li>
</ul>
</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: qs@6.10.3</li>
<li>deps: raw-body@2.5.1
<ul>
<li>deps: http-errors@2.0.0</li>
</ul>
</li>
</ul>
<h2>1.19.2</h2>
<ul>
<li>deps: bytes@3.1.2</li>
<li>deps: qs@6.9.7
<ul>
<li>Fix handling of <code>__proto__</code> keys</li>
</ul>
</li>
<li>deps: raw-body@2.4.3
<ul>
<li>deps: bytes@3.1.2</li>
</ul>
</li>
</ul>
<h2>1.19.1</h2>
<ul>
<li>deps: bytes@3.1.1</li>
<li>deps: http-errors@1.8.1
<ul>
<li>deps: inherits@2.0.4</li>
<li>deps: toidentifier@1.0.1</li>
<li>deps: setprototypeof@1.2.0</li>
</ul>
</li>
<li>deps: qs@6.9.6</li>
<li>deps: raw-body@2.4.2
<ul>
<li>deps: bytes@3.1.1</li>
<li>deps: http-errors@1.8.1</li>
</ul>
</li>
<li>deps: safe-buffer@5.2.1</li>
<li>deps: type-is@~1.6.18</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/body-parser/blob/master/HISTORY.md">body-parser's changelog</a>.</em></p>
<blockquote>
<h1>1.20.1 / 2022-10-06</h1>
<ul>
<li>deps: qs@6.11.0</li>
<li>perf: remove unnecessary object clone</li>
</ul>
<h1>1.20.0 / 2022-04-02</h1>
<ul>
<li>Fix error message for json parse whitespace in <code>strict</code></li>
<li>Fix internal error when inflated body exceeds limit</li>
<li>Prevent loss of async hooks context</li>
<li>Prevent hanging when request already read</li>
<li>deps: depd@2.0.0
<ul>
<li>Replace internal <code>eval</code> usage with <code>Function</code> constructor</li>
<li>Use instance methods on <code>process</code> to check for listeners</li>
</ul>
</li>
<li>deps: http-errors@2.0.0
<ul>
<li>deps: depd@2.0.0</li>
<li>deps: statuses@2.0.1</li>
</ul>
</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: qs@6.10.3</li>
<li>deps: raw-body@2.5.1
<ul>
<li>deps: http-errors@2.0.0</li>
</ul>
</li>
</ul>
<h1>1.19.2 / 2022-02-15</h1>
<ul>
<li>deps: bytes@3.1.2</li>
<li>deps: qs@6.9.7
<ul>
<li>Fix handling of <code>__proto__</code> keys</li>
</ul>
</li>
<li>deps: raw-body@2.4.3
<ul>
<li>deps: bytes@3.1.2</li>
</ul>
</li>
</ul>
<h1>1.19.1 / 2021-12-10</h1>
<ul>
<li>deps: bytes@3.1.1</li>
<li>deps: http-errors@1.8.1
<ul>
<li>deps: inherits@2.0.4</li>
<li>deps: toidentifier@1.0.1</li>
<li>deps: setprototypeof@1.2.0</li>
</ul>
</li>
<li>deps: qs@6.9.6</li>
<li>deps: raw-body@2.4.2
<ul>
<li>deps: bytes@3.1.1</li>
<li>deps: http-errors@1.8.1</li>
</ul>
</li>
<li>deps: safe-buffer@5.2.1</li>
<li>deps: type-is@~1.6.18</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/expressjs/body-parser/commit/830bdfbee021d540a742de857dcbd43f40563a02"><code>830bdfb</code></a> 1.20.1</li>
<li><a href="https://github.com/expressjs/body-parser/commit/ecad1ccf9eefe61a4ba5b8354d914e262eba7648"><code>ecad1cc</code></a> build: eslint@8.24.0</li>
<li><a href="https://github.com/expressjs/body-parser/commit/03b93cf9f11c201631a8cefa09df08feb6f2bb00"><code>03b93cf</code></a> build: supertest@6.3.0</li>
<li><a href="https://github.com/expressjs/body-parser/commit/2c611fcda0fe54043eb8c914f1fde412ba9432c0"><code>2c611fc</code></a> build: Node.js@18.10</li>
<li><a href="https://github.com/expressjs/body-parser/commit/f199e94b115de00feae7ae5559638c0c52019b2e"><code>f199e94</code></a> perf: remove unnecessary object clone</li>
<li><a href="https://github.com/expressjs/body-parser/commit/0123e12d6b6db1bdb66b271b2822b5070096dc32"><code>0123e12</code></a> build: Node.js@18.9</li>
<li><a href="https://github.com/expressjs/body-parser/commit/de1e6c2b390244e486f235151d8e6b9646f2122f"><code>de1e6c2</code></a> build: Node.js@16.17</li>
<li><a href="https://github.com/expressjs/body-parser/commit/477ff13b9c608800cc25331e0de6da6cd4970ee3"><code>477ff13</code></a> build: eslint-plugin-import@2.26.0</li>
<li><a href="https://github.com/expressjs/body-parser/commit/40c3fff30b0d88763e89f1a41ed76d2cf8aa1b14"><code>40c3fff</code></a> deps: qs@6.11.0</li>
<li><a href="https://github.com/expressjs/body-parser/commit/4aa84b70c298354e902edfc4a85ddfdc9fa905c8"><code>4aa84b7</code></a> build: supertest@6.2.4</li>
<li>Additional commits viewable in <a href="https://github.com/expressjs/body-parser/compare/1.19.0...1.20.1">compare view</a></li>
</ul>
</details>
<br />

Updates `express` from 4.16.4 to 4.18.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/express/releases">express's releases</a>.</em></p>
<blockquote>
<h2>4.18.2</h2>
<ul>
<li>Fix regression routing a large stack in a single route</li>
<li>deps: body-parser@1.20.1
<ul>
<li>deps: qs@6.11.0</li>
<li>perf: remove unnecessary object clone</li>
</ul>
</li>
<li>deps: qs@6.11.0</li>
</ul>
<h2>4.18.1</h2>
<ul>
<li>Fix hanging on large stack of sync routes</li>
</ul>
<h2>4.18.0</h2>
<ul>
<li>Add &quot;root&quot; option to <code>res.download</code></li>
<li>Allow <code>options</code> without <code>filename</code> in <code>res.download</code></li>
<li>Deprecate string and non-integer arguments to <code>res.status</code></li>
<li>Fix behavior of <code>null</code>/<code>undefined</code> as <code>maxAge</code> in <code>res.cookie</code></li>
<li>Fix handling very large stacks of sync middleware</li>
<li>Ignore <code>Object.prototype</code> values in settings through <code>app.set</code>/<code>app.get</code></li>
<li>Invoke <code>default</code> with same arguments as types in <code>res.format</code></li>
<li>Support proper 205 responses using <code>res.send</code></li>
<li>Use <code>http-errors</code> for <code>res.format</code> error</li>
<li>deps: body-parser@1.20.0
<ul>
<li>Fix error message for json parse whitespace in <code>strict</code></li>
<li>Fix internal error when inflated body exceeds limit</li>
<li>Prevent loss of async hooks context</li>
<li>Prevent hanging when request already read</li>
<li>deps: depd@2.0.0</li>
<li>deps: http-errors@2.0.0</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: qs@6.10.3</li>
<li>deps: raw-body@2.5.1</li>
</ul>
</li>
<li>deps: cookie@0.5.0
<ul>
<li>Add <code>priority</code> option</li>
<li>Fix <code>expires</code> option to reject invalid dates</li>
</ul>
</li>
<li>deps: depd@2.0.0
<ul>
<li>Replace internal <code>eval</code> usage with <code>Function</code> constructor</li>
<li>Use instance methods on <code>process</code> to check for listeners</li>
</ul>
</li>
<li>deps: finalhandler@1.2.0
<ul>
<li>Remove set content headers that break response</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: statuses@2.0.1</li>
</ul>
</li>
<li>deps: on-finished@2.4.1
<ul>
<li>Prevent loss of async hooks context</li>
</ul>
</li>
<li>deps: qs@6.10.3</li>
<li>deps: send@0.18.0
<ul>
<li>Fix emitted 416 error missing headers property</li>
<li>Limit the headers removed for 304 response</li>
<li>deps: depd@2.0.0</li>
<li>deps: destroy@1.2.0</li>
<li>deps: http-errors@2.0.0</li>
<li>deps: on-finished@2.4.1</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/express/blob/master/History.md">express's changelog</a>.</em></p>
<blockquote>
<h1>4.18.2 / 2022-10-08</h1>
<ul>
<li>Fix regression routing a large stack in a single route</li>
<li>deps: body-parser@1.20.1
<ul>
<li>deps: qs@6.11.0</li>
<li>perf: remove unnecessary object clone</li>
</ul>
</li>
<li>deps: qs@6.11.0</li>
</ul>
<h1>4.18.1 / 2022-04-29</h1>
<ul>
<li>Fix hanging on large stack of sync routes</li>
</ul>
<h1>4.18.0 / 2022-04-25</h1>
<ul>
<li>Add &quot;root&quot; option to <code>res.download</code></li>
<li>Allow <code>options</code> without <code>filename</code> in <code>res.download</code></li>
<li>Deprecate string and non-integer arguments to <code>res.status</code></li>
<li>Fix behavior of <code>null</code>/<code>undefined</code> as <code>maxAge</code> in <code>res.cookie</code></li>
<li>Fix handling very large stacks of sync middleware</li>
<li>Ignore <code>Object.prototype</code> values in settings through <code>app.set</code>/<code>app.get</code></li>
<li>Invoke <code>default</code> with same arguments as types in <code>res.format</code></li>
<li>Support proper 205 responses using <code>res.send</code></li>
<li>Use <code>http-errors</code> for <code>res.format</code> error</li>
<li>deps: body-parser@1.20.0
<ul>
<li>Fix error message for json parse whitespace in <code>strict</code></li>
<li>Fix internal error when inflated body exceeds limit</li>
<li>Prevent loss of async hooks context</li>
<li>Prevent hanging when request already read</li>
<li>deps: depd@2.0.0</li>
<li>deps: http-errors@2.0.0</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: qs@6.10.3</li>
<li>deps: raw-body@2.5.1</li>
</ul>
</li>
<li>deps: cookie@0.5.0
<ul>
<li>Add <code>priority</code> option</li>
<li>Fix <code>expires</code> option to reject invalid dates</li>
</ul>
</li>
<li>deps: depd@2.0.0
<ul>
<li>Replace internal <code>eval</code> usage with <code>Function</code> constructor</li>
<li>Use instance methods on <code>process</code> to check for listeners</li>
</ul>
</li>
<li>deps: finalhandler@1.2.0
<ul>
<li>Remove set content headers that break response</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: statuses@2.0.1</li>
</ul>
</li>
<li>deps: on-finished@2.4.1
<ul>
<li>Prevent loss of async hooks context</li>
</ul>
</li>
<li>deps: qs@6.10.3</li>
<li>deps: send@0.18.0</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/expressjs/express/commit/8368dc178af16b91b576c4c1d135f701a0007e5d"><code>8368dc1</code></a> 4.18.2</li>
<li><a href="https://github.com/expressjs/express/commit/61f40491222dbede653b9938e6a4676f187aab44"><code>61f4049</code></a> docs: replace Freenode with Libera Chat</li>
<li><a href="https://github.com/expressjs/express/commit/bb7907b932afe3a19236a642f6054b6c8f7349a0"><code>bb7907b</code></a> build: Node.js@18.10</li>
<li><a href="https://github.com/expressjs/express/commit/f56ce73186e885a938bfdb3d3d1005a58e6ae12b"><code>f56ce73</code></a> build: supertest@6.3.0</li>
<li><a href="https://github.com/expressjs/express/commit/24b3dc551670ac4fb0cd5a2bd5ef643c9525e60f"><code>24b3dc5</code></a> deps: qs@6.11.0</li>
<li><a href="https://github.com/expressjs/express/commit/689d175b8b39d8860b81d723233fb83d15201827"><code>689d175</code></a> deps: body-parser@1.20.1</li>
<li><a href="https://github.com/expressjs/express/commit/340be0f79afb9b3176afb76235aa7f92acbd5050"><code>340be0f</code></a> build: eslint@8.24.0</li>
<li><a href="https://github.com/expressjs/express/commit/33e8dc303af9277f8a7e4f46abfdcb5e72f6797b"><code>33e8dc3</code></a> docs: use Node.js name style</li>
<li><a href="https://github.com/expressjs/express/commit/644f6464b9f61cbafa8f880636b1aa5237d95bad"><code>644f646</code></a> build: supertest@6.2.4</li>
<li><a href="https://github.com/expressjs/express/commit/ecd7572f1e920b7a512452b8d9806ae617a99c54"><code>ecd7572</code></a> build: Node.js@14.20</li>
<li>Additional commits viewable in <a href="https://github.com/expressjs/express/compare/4.16.4...4.18.2">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/university-course/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-11 18:34:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/university-course/pull/91" class=".btn">#91</a>
            </td>
            <td>
                <b>
                    chore(deps): bump qs from 6.5.2 to 6.5.3 in /support/Lab06/b4s/organization/students-union/utils
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [qs](https://github.com/ljharb/qs) from 6.5.2 to 6.5.3.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ljharb/qs/blob/main/CHANGELOG.md">qs's changelog</a>.</em></p>
<blockquote>
<h2><strong>6.5.3</strong></h2>
<ul>
<li>[Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/428">#428</a>)</li>
<li>[Fix] <code>utils.merge</code>: avoid a crash with a null target and a truthy non-array source</li>
<li>[Fix] correctly parse nested arrays</li>
<li>[Fix] <code>stringify</code>: fix a crash with <code>strictNullHandling</code> and a custom <code>filter</code>/<code>serializeDate</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/279">#279</a>)</li>
<li>[Fix] <code>utils</code>: <code>merge</code>: fix crash when <code>source</code> is a truthy primitive &amp; no options are provided</li>
<li>[Fix] when <code>parseArrays</code> is false, properly handle keys ending in <code>[]</code></li>
<li>[Fix] fix for an impossible situation: when the formatter is called with a non-string value</li>
<li>[Fix] <code>utils.merge</code>: avoid a crash with a null target and an array source</li>
<li>[Refactor] <code>utils</code>: reduce observable [[Get]]s</li>
<li>[Refactor] use cached <code>Array.isArray</code></li>
<li>[Refactor] <code>stringify</code>: Avoid arr = arr.concat(...), push to the existing instance (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/269">#269</a>)</li>
<li>[Refactor] <code>parse</code>: only need to reassign the var once</li>
<li>[Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/427">#427</a>)</li>
<li>[readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li>[Docs] Clean up license text so it’s properly detected as BSD-3-Clause</li>
<li>[Docs] Clarify the need for &quot;arrayLimit&quot; option</li>
<li>[meta] fix README.md (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/399">#399</a>)</li>
<li>[meta] add FUNDING.yml</li>
<li>[actions] backport actions from main</li>
<li>[Tests] always use <code>String(x)</code> over <code>x.toString()</code></li>
<li>[Tests] remove nonexistent tape option</li>
<li>[Dev Deps] backport from main</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ljharb/qs/commit/298bfa55d6db00ddea78dd0333509aadf9bb3077"><code>298bfa5</code></a> v6.5.3</li>
<li><a href="https://github.com/ljharb/qs/commit/ed0f5dcbef4b168a8ae299d78b1e4a2e9b1baf1f"><code>ed0f5dc</code></a> [Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/428">#428</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/691e739cfa40cd42604dc05a54e6154371a429ab"><code>691e739</code></a> [Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/427">#427</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/1072d57d38a690e1ad7616dced44390bffedcbb2"><code>1072d57</code></a> [readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li><a href="https://github.com/ljharb/qs/commit/12ac1c403aaa04d1a34844f514ed9f9abfb76e64"><code>12ac1c4</code></a> [meta] fix README.md (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/399">#399</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/0338716b09fdbd4711823eeb0a14e556a2498e7a"><code>0338716</code></a> [actions] backport actions from main</li>
<li><a href="https://github.com/ljharb/qs/commit/5639c20ce0a7c1332200a3181339331483e5a3a1"><code>5639c20</code></a> Clean up license text so it’s properly detected as BSD-3-Clause</li>
<li><a href="https://github.com/ljharb/qs/commit/51b8a0b1b213596dd1702b837f5e7dec2229793d"><code>51b8a0b</code></a> add FUNDING.yml</li>
<li><a href="https://github.com/ljharb/qs/commit/45f675936e742d92fac8d4dae5cfc385c576a977"><code>45f6759</code></a> [Fix] fix for an impossible situation: when the formatter is called with a no...</li>
<li><a href="https://github.com/ljharb/qs/commit/f814a7f8f2af059f8158f7e4b2bf8b46aeb62cd3"><code>f814a7f</code></a> [Dev Deps] backport from main</li>
<li>Additional commits viewable in <a href="https://github.com/ljharb/qs/compare/v6.5.2...v6.5.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=qs&package-manager=npm_and_yarn&previous-version=6.5.2&new-version=6.5.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/university-course/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-11 18:33:44 +0000 UTC
    </div>
</div>

