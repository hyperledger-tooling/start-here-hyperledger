---
layout: default
title: yui-docs
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/yui-docs
---

# yui-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-docs/pull/47" class=".btn">#47</a>
            </td>
            <td>
                <b>
                    Bump express from 4.17.1 to 4.18.2 in /docsrcs/yui-ibc-solidity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-docs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-14 22:58:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-docs/pull/46" class=".btn">#46</a>
            </td>
            <td>
                <b>
                    Bump express from 4.17.1 to 4.18.2 in /samples/minitoken-besu-ethereum
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-docs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-14 22:52:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-docs/pull/45" class=".btn">#45</a>
            </td>
            <td>
                <b>
                    Bump express from 4.17.1 to 4.18.2 in /contracts/minitoken/solidity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-docs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-14 22:52:12 +0000 UTC
    </div>
</div>

