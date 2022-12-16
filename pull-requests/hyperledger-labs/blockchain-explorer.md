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
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/318" class=".btn">#318</a>
            </td>
            <td>
                <b>
                    Bump express from 4.17.2 to 4.18.2 in /client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [express](https://github.com/expressjs/express) from 4.17.2 to 4.18.2.
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
<li>Additional commits viewable in <a href="https://github.com/expressjs/express/compare/4.17.2...4.18.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=express&package-manager=npm_and_yarn&previous-version=4.17.2&new-version=4.18.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-12-15 22:35:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/317" class=".btn">#317</a>
            </td>
            <td>
                <b>
                    Bump express from 4.17.1 to 4.17.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [express](https://github.com/expressjs/express) from 4.17.1 to 4.17.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/express/releases">express's releases</a>.</em></p>
<blockquote>
<h2>4.17.3</h2>
<ul>
<li>deps: accepts@~1.3.8
<ul>
<li>deps: mime-types@~2.1.34</li>
<li>deps: negotiator@0.6.3</li>
</ul>
</li>
<li>deps: body-parser@1.19.2
<ul>
<li>deps: bytes@3.1.2</li>
<li>deps: qs@6.9.7</li>
<li>deps: raw-body@2.4.3</li>
</ul>
</li>
<li>deps: cookie@0.4.2</li>
<li>deps: qs@6.9.7
<ul>
<li>Fix handling of <code>__proto__</code> keys</li>
</ul>
</li>
<li>pref: remove unnecessary regexp for trust proxy</li>
</ul>
<h2>4.17.2</h2>
<ul>
<li>Fix handling of <code>undefined</code> in <code>res.jsonp</code></li>
<li>Fix handling of <code>undefined</code> when <code>&quot;json escape&quot;</code> is enabled</li>
<li>Fix incorrect middleware execution with unanchored <code>RegExp</code>s</li>
<li>Fix <code>res.jsonp(obj, status)</code> deprecation message</li>
<li>Fix typo in <code>res.is</code> JSDoc</li>
<li>deps: body-parser@1.19.1
<ul>
<li>deps: bytes@3.1.1</li>
<li>deps: http-errors@1.8.1</li>
<li>deps: qs@6.9.6</li>
<li>deps: raw-body@2.4.2</li>
<li>deps: safe-buffer@5.2.1</li>
<li>deps: type-is@~1.6.18</li>
</ul>
</li>
<li>deps: content-disposition@0.5.4
<ul>
<li>deps: safe-buffer@5.2.1</li>
</ul>
</li>
<li>deps: cookie@0.4.1
<ul>
<li>Fix <code>maxAge</code> option to reject invalid values</li>
</ul>
</li>
<li>deps: proxy-addr@~2.0.7
<ul>
<li>Use <code>req.socket</code> over deprecated <code>req.connection</code></li>
<li>deps: forwarded@0.2.0</li>
<li>deps: ipaddr.js@1.9.1</li>
</ul>
</li>
<li>deps: qs@6.9.6</li>
<li>deps: safe-buffer@5.2.1</li>
<li>deps: send@0.17.2
<ul>
<li>deps: http-errors@1.8.1</li>
<li>deps: ms@2.1.3</li>
<li>pref: ignore empty http tokens</li>
</ul>
</li>
<li>deps: serve-static@1.14.2
<ul>
<li>deps: send@0.17.2</li>
</ul>
</li>
<li>deps: setprototypeof@1.2.0</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/express/blob/master/History.md">express's changelog</a>.</em></p>
<blockquote>
<h1>4.17.3 / 2022-02-16</h1>
<ul>
<li>deps: accepts@~1.3.8
<ul>
<li>deps: mime-types@~2.1.34</li>
<li>deps: negotiator@0.6.3</li>
</ul>
</li>
<li>deps: body-parser@1.19.2
<ul>
<li>deps: bytes@3.1.2</li>
<li>deps: qs@6.9.7</li>
<li>deps: raw-body@2.4.3</li>
</ul>
</li>
<li>deps: cookie@0.4.2</li>
<li>deps: qs@6.9.7
<ul>
<li>Fix handling of <code>__proto__</code> keys</li>
</ul>
</li>
<li>pref: remove unnecessary regexp for trust proxy</li>
</ul>
<h1>4.17.2 / 2021-12-16</h1>
<ul>
<li>Fix handling of <code>undefined</code> in <code>res.jsonp</code></li>
<li>Fix handling of <code>undefined</code> when <code>&quot;json escape&quot;</code> is enabled</li>
<li>Fix incorrect middleware execution with unanchored <code>RegExp</code>s</li>
<li>Fix <code>res.jsonp(obj, status)</code> deprecation message</li>
<li>Fix typo in <code>res.is</code> JSDoc</li>
<li>deps: body-parser@1.19.1
<ul>
<li>deps: bytes@3.1.1</li>
<li>deps: http-errors@1.8.1</li>
<li>deps: qs@6.9.6</li>
<li>deps: raw-body@2.4.2</li>
<li>deps: safe-buffer@5.2.1</li>
<li>deps: type-is@~1.6.18</li>
</ul>
</li>
<li>deps: content-disposition@0.5.4
<ul>
<li>deps: safe-buffer@5.2.1</li>
</ul>
</li>
<li>deps: cookie@0.4.1
<ul>
<li>Fix <code>maxAge</code> option to reject invalid values</li>
</ul>
</li>
<li>deps: proxy-addr@~2.0.7
<ul>
<li>Use <code>req.socket</code> over deprecated <code>req.connection</code></li>
<li>deps: forwarded@0.2.0</li>
<li>deps: ipaddr.js@1.9.1</li>
</ul>
</li>
<li>deps: qs@6.9.6</li>
<li>deps: safe-buffer@5.2.1</li>
<li>deps: send@0.17.2
<ul>
<li>deps: http-errors@1.8.1</li>
<li>deps: ms@2.1.3</li>
<li>pref: ignore empty http tokens</li>
</ul>
</li>
<li>deps: serve-static@1.14.2
<ul>
<li>deps: send@0.17.2</li>
</ul>
</li>
<li>deps: setprototypeof@1.2.0</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/expressjs/express/commit/3d7fce56a35f4f73fa437866cd1401587a212334"><code>3d7fce5</code></a> 4.17.3</li>
<li><a href="https://github.com/expressjs/express/commit/f9063712e01979588818b0756851053b5ee43d09"><code>f906371</code></a> build: update example dependencies</li>
<li><a href="https://github.com/expressjs/express/commit/6381bc6317ec8ffbf830e2d16677e4b5af37cc08"><code>6381bc6</code></a> deps: qs@6.9.7</li>
<li><a href="https://github.com/expressjs/express/commit/a00786309641731661edb4d826a6919330887ca7"><code>a007863</code></a> deps: body-parser@1.19.2</li>
<li><a href="https://github.com/expressjs/express/commit/e98f5848a0a496c0977a2d1734067b77f69de360"><code>e98f584</code></a> Revert &quot;build: use minimatch@3.0.4 for Node.js &lt; 4&quot;</li>
<li><a href="https://github.com/expressjs/express/commit/a65913776d0b16837364ee66caa1a7f38a9997c0"><code>a659137</code></a> tests: use strict mode</li>
<li><a href="https://github.com/expressjs/express/commit/a39e409cf3739ef9c9b597a9680813a34c3931c2"><code>a39e409</code></a> tests: prevent leaking changes to NODE_ENV</li>
<li><a href="https://github.com/expressjs/express/commit/82de4de5ab92e8237d713285104e4b8452927352"><code>82de4de</code></a> examples: fix path traversal in downloads example</li>
<li><a href="https://github.com/expressjs/express/commit/12310c52947ee159f7ecd63d125243cdca891135"><code>12310c5</code></a> build: use nyc for test coverage</li>
<li><a href="https://github.com/expressjs/express/commit/884657d54665f323c236055d6e3d3e85d96e5f08"><code>884657d</code></a> examples: remove bitwise syntax for includes check</li>
<li>Additional commits viewable in <a href="https://github.com/expressjs/express/compare/4.17.1...4.17.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=express&package-manager=npm_and_yarn&previous-version=4.17.1&new-version=4.17.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-12-15 09:15:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/315" class=".btn">#315</a>
            </td>
            <td>
                <b>
                    Bump decode-uri-component from 0.2.0 to 0.2.2 in /client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [decode-uri-component](https://github.com/SamVerschueren/decode-uri-component) from 0.2.0 to 0.2.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/SamVerschueren/decode-uri-component/releases">decode-uri-component's releases</a>.</em></p>
<blockquote>
<h2>v0.2.2</h2>
<ul>
<li>Prevent overwriting previously decoded tokens  980e0bf</li>
</ul>
<p><a href="https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.1...v0.2.2">https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.1...v0.2.2</a></p>
<h2>v0.2.1</h2>
<ul>
<li>Switch to GitHub workflows  76abc93</li>
<li>Fix issue where decode throws - fixes <a href="https://github-redirect.dependabot.com/SamVerschueren/decode-uri-component/issues/6">#6</a>  746ca5d</li>
<li>Update license (<a href="https://github-redirect.dependabot.com/SamVerschueren/decode-uri-component/issues/1">#1</a>)  486d7e2</li>
<li>Tidelift tasks  a650457</li>
<li>Meta tweaks  66e1c28</li>
</ul>
<p><a href="https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.0...v0.2.1">https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.0...v0.2.1</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/a0eea469d26eb0df668b081672cdb9581feb78eb"><code>a0eea46</code></a> 0.2.2</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/980e0bf09b64d94f1aa79012f895816c30ffd152"><code>980e0bf</code></a> Prevent overwriting previously decoded tokens</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/3c8a373dd4837e89b3f970e01295dd03e1405a33"><code>3c8a373</code></a> 0.2.1</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/76abc939783fe3900fadb7d384a74d324d5557f3"><code>76abc93</code></a> Switch to GitHub workflows</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/746ca5dcb6667c5d364e782d53c542830e4c10b9"><code>746ca5d</code></a> Fix issue where decode throws - fixes <a href="https://github-redirect.dependabot.com/SamVerschueren/decode-uri-component/issues/6">#6</a></li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/486d7e26d3a8c0fbe860fb651fe1bc98c2f2be30"><code>486d7e2</code></a> Update license (<a href="https://github-redirect.dependabot.com/SamVerschueren/decode-uri-component/issues/1">#1</a>)</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/a65045724e6234acef87f31da499d4807b20b134"><code>a650457</code></a> Tidelift tasks</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/66e1c2834c0e189201cb65196ec3101372459b02"><code>66e1c28</code></a> Meta tweaks</li>
<li>See full diff in <a href="https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.0...v0.2.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=decode-uri-component&package-manager=npm_and_yarn&previous-version=0.2.0&new-version=0.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-12-09 07:01:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/314" class=".btn">#314</a>
            </td>
            <td>
                <b>
                    Bump decode-uri-component from 0.2.0 to 0.2.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [decode-uri-component](https://github.com/SamVerschueren/decode-uri-component) from 0.2.0 to 0.2.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/SamVerschueren/decode-uri-component/releases">decode-uri-component's releases</a>.</em></p>
<blockquote>
<h2>v0.2.2</h2>
<ul>
<li>Prevent overwriting previously decoded tokens  980e0bf</li>
</ul>
<p><a href="https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.1...v0.2.2">https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.1...v0.2.2</a></p>
<h2>v0.2.1</h2>
<ul>
<li>Switch to GitHub workflows  76abc93</li>
<li>Fix issue where decode throws - fixes <a href="https://github-redirect.dependabot.com/SamVerschueren/decode-uri-component/issues/6">#6</a>  746ca5d</li>
<li>Update license (<a href="https://github-redirect.dependabot.com/SamVerschueren/decode-uri-component/issues/1">#1</a>)  486d7e2</li>
<li>Tidelift tasks  a650457</li>
<li>Meta tweaks  66e1c28</li>
</ul>
<p><a href="https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.0...v0.2.1">https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.0...v0.2.1</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/a0eea469d26eb0df668b081672cdb9581feb78eb"><code>a0eea46</code></a> 0.2.2</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/980e0bf09b64d94f1aa79012f895816c30ffd152"><code>980e0bf</code></a> Prevent overwriting previously decoded tokens</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/3c8a373dd4837e89b3f970e01295dd03e1405a33"><code>3c8a373</code></a> 0.2.1</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/76abc939783fe3900fadb7d384a74d324d5557f3"><code>76abc93</code></a> Switch to GitHub workflows</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/746ca5dcb6667c5d364e782d53c542830e4c10b9"><code>746ca5d</code></a> Fix issue where decode throws - fixes <a href="https://github-redirect.dependabot.com/SamVerschueren/decode-uri-component/issues/6">#6</a></li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/486d7e26d3a8c0fbe860fb651fe1bc98c2f2be30"><code>486d7e2</code></a> Update license (<a href="https://github-redirect.dependabot.com/SamVerschueren/decode-uri-component/issues/1">#1</a>)</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/a65045724e6234acef87f31da499d4807b20b134"><code>a650457</code></a> Tidelift tasks</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/66e1c2834c0e189201cb65196ec3101372459b02"><code>66e1c28</code></a> Meta tweaks</li>
<li>See full diff in <a href="https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.0...v0.2.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=decode-uri-component&package-manager=npm_and_yarn&previous-version=0.2.0&new-version=0.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-12-09 07:01:11 +0000 UTC
    </div>
</div>

