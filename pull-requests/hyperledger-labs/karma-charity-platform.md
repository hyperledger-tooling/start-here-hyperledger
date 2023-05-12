---
layout: default
title: karma-charity-platform
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/karma-charity-platform
---

# karma-charity-platform <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/karma-charity-platform){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/101" class=".btn">#101</a>
            </td>
            <td>
                <b>
                    Bump engine.io from 6.4.1 to 6.4.2 in /platform/backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [engine.io](https://github.com/socketio/engine.io) from 6.4.1 to 6.4.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/socketio/engine.io/releases">engine.io's releases</a>.</em></p>
<blockquote>
<h2>6.4.2</h2>
<p>:warning: This release contains an important security fix :warning:</p>
<p>A malicious client could send a specially crafted HTTP request, triggering an uncaught exception and killing the Node.js process:</p>
<pre><code>TypeError: Cannot read properties of undefined (reading 'handlesUpgrades')
  at Server.onWebSocket (build/server.js:515:67)
</code></pre>
<p>Please upgrade as soon as possible.</p>
<h3>Bug Fixes</h3>
<ul>
<li>include error handling for Express middlewares (<a href="https://redirect.github.com/socketio/engine.io/issues/674">#674</a>) (<a href="https://github.com/socketio/engine.io/commit/93957828be1252c83275b56f0c7c0bd145a0ceb9">9395782</a>)</li>
<li>prevent crash when provided with an invalid query param (<a href="https://github.com/socketio/engine.io/commit/fc480b4f305e16fe5972cf337d055e598372dc44">fc480b4</a>)</li>
<li><strong>typings:</strong> make clientsCount public (<a href="https://redirect.github.com/socketio/engine.io/issues/675">#675</a>) (<a href="https://github.com/socketio/engine.io/commit/bd6d4713b02ff646c581872cd9ffe753acff0d73">bd6d471</a>)</li>
<li><strong>uws:</strong> prevent crash when using with middlewares (<a href="https://github.com/socketio/engine.io/commit/8b2216290330b174c9e67be32765bec0c74769f9">8b22162</a>)</li>
</ul>
<h3>Credits</h3>
<p>Huge thanks to <a href="https://github.com/tyilo"><code>@​tyilo</code></a> and <a href="https://github.com/cieldeville"><code>@​cieldeville</code></a> for helping!</p>
<h4>Links</h4>
<ul>
<li>Diff: <a href="https://github.com/socketio/engine.io/compare/6.4.1...6.4.2">https://github.com/socketio/engine.io/compare/6.4.1...6.4.2</a></li>
<li>Client release: -</li>
<li>ws version: <a href="https://github.com/websockets/ws/releases/tag/8.11.0">~8.11.0</a> (no change)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/socketio/engine.io/blob/main/CHANGELOG.md">engine.io's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/socketio/engine.io/compare/6.4.1...6.4.2">6.4.2</a> (2023-05-02)</h2>
<p>:warning: This release contains an important security fix :warning:</p>
<p>A malicious client could send a specially crafted HTTP request, triggering an uncaught exception and killing the Node.js process:</p>
<pre><code>TypeError: Cannot read properties of undefined (reading 'handlesUpgrades')
  at Server.onWebSocket (build/server.js:515:67)
</code></pre>
<p>Please upgrade as soon as possible.</p>
<h3>Bug Fixes</h3>
<ul>
<li>include error handling for Express middlewares (<a href="https://redirect.github.com/socketio/engine.io/issues/674">#674</a>) (<a href="https://github.com/socketio/engine.io/commit/93957828be1252c83275b56f0c7c0bd145a0ceb9">9395782</a>)</li>
<li>prevent crash when provided with an invalid query param (<a href="https://github.com/socketio/engine.io/commit/fc480b4f305e16fe5972cf337d055e598372dc44">fc480b4</a>)</li>
<li><strong>typings:</strong> make clientsCount public (<a href="https://redirect.github.com/socketio/engine.io/issues/675">#675</a>) (<a href="https://github.com/socketio/engine.io/commit/bd6d4713b02ff646c581872cd9ffe753acff0d73">bd6d471</a>)</li>
<li><strong>uws:</strong> prevent crash when using with middlewares (<a href="https://github.com/socketio/engine.io/commit/8b2216290330b174c9e67be32765bec0c74769f9">8b22162</a>)</li>
</ul>
<h3>Credits</h3>
<p>Huge thanks to <a href="https://github.com/tyilo"><code>@​tyilo</code></a> and <a href="https://github.com/cieldeville"><code>@​cieldeville</code></a> for helping!</p>
<h3>Dependencies</h3>
<ul>
<li><a href="https://github.com/websockets/ws/releases/tag/8.11.0"><code>ws@~8.11.0</code></a> (no change)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/socketio/engine.io/commit/95e215387c589025dde3982865bf8c862d049469"><code>95e2153</code></a> chore(release): 6.4.2</li>
<li><a href="https://github.com/socketio/engine.io/commit/fc480b4f305e16fe5972cf337d055e598372dc44"><code>fc480b4</code></a> fix: prevent crash when provided with an invalid query param</li>
<li><a href="https://github.com/socketio/engine.io/commit/014195118535669af0ad3bde38a76601dafa4d81"><code>0141951</code></a> refactor(types): ensure compatibility with Express middlewares</li>
<li><a href="https://github.com/socketio/engine.io/commit/8b2216290330b174c9e67be32765bec0c74769f9"><code>8b22162</code></a> fix(uws): prevent crash when using with middlewares</li>
<li><a href="https://github.com/socketio/engine.io/commit/93957828be1252c83275b56f0c7c0bd145a0ceb9"><code>9395782</code></a> fix: include error handling for Express middlewares (<a href="https://redirect.github.com/socketio/engine.io/issues/674">#674</a>)</li>
<li><a href="https://github.com/socketio/engine.io/commit/911d0e35757ea9ee93d1807c401c734661615e96"><code>911d0e3</code></a> refactor: return HTTP 400 upon invalid request overlap</li>
<li><a href="https://github.com/socketio/engine.io/commit/bd6d4713b02ff646c581872cd9ffe753acff0d73"><code>bd6d471</code></a> fix(typings): make clientsCount public (<a href="https://redirect.github.com/socketio/engine.io/issues/675">#675</a>)</li>
<li>See full diff in <a href="https://github.com/socketio/engine.io/compare/6.4.1...6.4.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=engine.io&package-manager=npm_and_yarn&previous-version=6.4.1&new-version=6.4.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-12 13:26:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/100" class=".btn">#100</a>
            </td>
            <td>
                <b>
                    Bump engine.io from 6.4.1 to 6.4.2 in /explorer/backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [engine.io](https://github.com/socketio/engine.io) from 6.4.1 to 6.4.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/socketio/engine.io/releases">engine.io's releases</a>.</em></p>
<blockquote>
<h2>6.4.2</h2>
<p>:warning: This release contains an important security fix :warning:</p>
<p>A malicious client could send a specially crafted HTTP request, triggering an uncaught exception and killing the Node.js process:</p>
<pre><code>TypeError: Cannot read properties of undefined (reading 'handlesUpgrades')
  at Server.onWebSocket (build/server.js:515:67)
</code></pre>
<p>Please upgrade as soon as possible.</p>
<h3>Bug Fixes</h3>
<ul>
<li>include error handling for Express middlewares (<a href="https://redirect.github.com/socketio/engine.io/issues/674">#674</a>) (<a href="https://github.com/socketio/engine.io/commit/93957828be1252c83275b56f0c7c0bd145a0ceb9">9395782</a>)</li>
<li>prevent crash when provided with an invalid query param (<a href="https://github.com/socketio/engine.io/commit/fc480b4f305e16fe5972cf337d055e598372dc44">fc480b4</a>)</li>
<li><strong>typings:</strong> make clientsCount public (<a href="https://redirect.github.com/socketio/engine.io/issues/675">#675</a>) (<a href="https://github.com/socketio/engine.io/commit/bd6d4713b02ff646c581872cd9ffe753acff0d73">bd6d471</a>)</li>
<li><strong>uws:</strong> prevent crash when using with middlewares (<a href="https://github.com/socketio/engine.io/commit/8b2216290330b174c9e67be32765bec0c74769f9">8b22162</a>)</li>
</ul>
<h3>Credits</h3>
<p>Huge thanks to <a href="https://github.com/tyilo"><code>@​tyilo</code></a> and <a href="https://github.com/cieldeville"><code>@​cieldeville</code></a> for helping!</p>
<h4>Links</h4>
<ul>
<li>Diff: <a href="https://github.com/socketio/engine.io/compare/6.4.1...6.4.2">https://github.com/socketio/engine.io/compare/6.4.1...6.4.2</a></li>
<li>Client release: -</li>
<li>ws version: <a href="https://github.com/websockets/ws/releases/tag/8.11.0">~8.11.0</a> (no change)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/socketio/engine.io/blob/main/CHANGELOG.md">engine.io's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/socketio/engine.io/compare/6.4.1...6.4.2">6.4.2</a> (2023-05-02)</h2>
<p>:warning: This release contains an important security fix :warning:</p>
<p>A malicious client could send a specially crafted HTTP request, triggering an uncaught exception and killing the Node.js process:</p>
<pre><code>TypeError: Cannot read properties of undefined (reading 'handlesUpgrades')
  at Server.onWebSocket (build/server.js:515:67)
</code></pre>
<p>Please upgrade as soon as possible.</p>
<h3>Bug Fixes</h3>
<ul>
<li>include error handling for Express middlewares (<a href="https://redirect.github.com/socketio/engine.io/issues/674">#674</a>) (<a href="https://github.com/socketio/engine.io/commit/93957828be1252c83275b56f0c7c0bd145a0ceb9">9395782</a>)</li>
<li>prevent crash when provided with an invalid query param (<a href="https://github.com/socketio/engine.io/commit/fc480b4f305e16fe5972cf337d055e598372dc44">fc480b4</a>)</li>
<li><strong>typings:</strong> make clientsCount public (<a href="https://redirect.github.com/socketio/engine.io/issues/675">#675</a>) (<a href="https://github.com/socketio/engine.io/commit/bd6d4713b02ff646c581872cd9ffe753acff0d73">bd6d471</a>)</li>
<li><strong>uws:</strong> prevent crash when using with middlewares (<a href="https://github.com/socketio/engine.io/commit/8b2216290330b174c9e67be32765bec0c74769f9">8b22162</a>)</li>
</ul>
<h3>Credits</h3>
<p>Huge thanks to <a href="https://github.com/tyilo"><code>@​tyilo</code></a> and <a href="https://github.com/cieldeville"><code>@​cieldeville</code></a> for helping!</p>
<h3>Dependencies</h3>
<ul>
<li><a href="https://github.com/websockets/ws/releases/tag/8.11.0"><code>ws@~8.11.0</code></a> (no change)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/socketio/engine.io/commit/95e215387c589025dde3982865bf8c862d049469"><code>95e2153</code></a> chore(release): 6.4.2</li>
<li><a href="https://github.com/socketio/engine.io/commit/fc480b4f305e16fe5972cf337d055e598372dc44"><code>fc480b4</code></a> fix: prevent crash when provided with an invalid query param</li>
<li><a href="https://github.com/socketio/engine.io/commit/014195118535669af0ad3bde38a76601dafa4d81"><code>0141951</code></a> refactor(types): ensure compatibility with Express middlewares</li>
<li><a href="https://github.com/socketio/engine.io/commit/8b2216290330b174c9e67be32765bec0c74769f9"><code>8b22162</code></a> fix(uws): prevent crash when using with middlewares</li>
<li><a href="https://github.com/socketio/engine.io/commit/93957828be1252c83275b56f0c7c0bd145a0ceb9"><code>9395782</code></a> fix: include error handling for Express middlewares (<a href="https://redirect.github.com/socketio/engine.io/issues/674">#674</a>)</li>
<li><a href="https://github.com/socketio/engine.io/commit/911d0e35757ea9ee93d1807c401c734661615e96"><code>911d0e3</code></a> refactor: return HTTP 400 upon invalid request overlap</li>
<li><a href="https://github.com/socketio/engine.io/commit/bd6d4713b02ff646c581872cd9ffe753acff0d73"><code>bd6d471</code></a> fix(typings): make clientsCount public (<a href="https://redirect.github.com/socketio/engine.io/issues/675">#675</a>)</li>
<li>See full diff in <a href="https://github.com/socketio/engine.io/compare/6.4.1...6.4.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=engine.io&package-manager=npm_and_yarn&previous-version=6.4.1&new-version=6.4.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-12 13:26:26 +0000 UTC
    </div>
</div>

