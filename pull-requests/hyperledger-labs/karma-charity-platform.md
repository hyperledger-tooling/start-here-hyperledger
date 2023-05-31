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
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/105" class=".btn">#105</a>
            </td>
            <td>
                <b>
                    Bump socket.io-parser from 4.2.2 to 4.2.3 in /platform/backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [socket.io-parser](https://github.com/socketio/socket.io-parser) from 4.2.2 to 4.2.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/socketio/socket.io-parser/releases">socket.io-parser's releases</a>.</em></p>
<blockquote>
<h2>4.2.3</h2>
<p>:warning: This release contains an important security fix :warning:</p>
<p>A malicious client could send a specially crafted HTTP request, triggering an uncaught exception and killing the Node.js process:</p>
<pre><code>TypeError: Cannot convert object to primitive value
       at Socket.emit (node:events:507:25)
       at .../node_modules/socket.io/lib/socket.js:531:14
</code></pre>
<p>Please upgrade as soon as possible.</p>
<h3>Bug Fixes</h3>
<ul>
<li>check the format of the event name (<a href="https://github.com/socketio/socket.io-parser/commit/3b78117bf6ba7e99d7a5cfc1ba54d0477554a7f3">3b78117</a>)</li>
</ul>
<h4>Links</h4>
<ul>
<li>Diff: <a href="https://github.com/socketio/socket.io-parser/compare/4.2.2...4.2.3">https://github.com/socketio/socket.io-parser/compare/4.2.2...4.2.3</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/socketio/socket.io-parser/blob/main/CHANGELOG.md">socket.io-parser's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/socketio/socket.io-parser/compare/4.2.2...4.2.3">4.2.3</a> (2023-05-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>check the format of the event name (<a href="https://github.com/socketio/socket.io-parser/commit/3b78117bf6ba7e99d7a5cfc1ba54d0477554a7f3">3b78117</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/socketio/socket.io-parser/commit/b6c824f82421aa44dfd5ef395f5132866543de59"><code>b6c824f</code></a> chore(release): 4.2.3</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/dcc70d9678ac896de08294d6e8d668be6a68680a"><code>dcc70d9</code></a> refactor: export typescript declarations for the commonjs build</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/3b78117bf6ba7e99d7a5cfc1ba54d0477554a7f3"><code>3b78117</code></a> fix: check the format of the event name</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/0841bd562351c3d45a5288e2adf9707cc8a3131d"><code>0841bd5</code></a> chore: bump ua-parser-js from 1.0.32 to 1.0.33 (<a href="https://redirect.github.com/socketio/socket.io-parser/issues/121">#121</a>)</li>
<li>See full diff in <a href="https://github.com/socketio/socket.io-parser/compare/4.2.2...4.2.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=socket.io-parser&package-manager=npm_and_yarn&previous-version=4.2.2&new-version=4.2.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-05-24 02:11:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/104" class=".btn">#104</a>
            </td>
            <td>
                <b>
                    Bump socket.io-parser from 4.2.2 to 4.2.3 in /explorer/backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [socket.io-parser](https://github.com/socketio/socket.io-parser) from 4.2.2 to 4.2.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/socketio/socket.io-parser/releases">socket.io-parser's releases</a>.</em></p>
<blockquote>
<h2>4.2.3</h2>
<p>:warning: This release contains an important security fix :warning:</p>
<p>A malicious client could send a specially crafted HTTP request, triggering an uncaught exception and killing the Node.js process:</p>
<pre><code>TypeError: Cannot convert object to primitive value
       at Socket.emit (node:events:507:25)
       at .../node_modules/socket.io/lib/socket.js:531:14
</code></pre>
<p>Please upgrade as soon as possible.</p>
<h3>Bug Fixes</h3>
<ul>
<li>check the format of the event name (<a href="https://github.com/socketio/socket.io-parser/commit/3b78117bf6ba7e99d7a5cfc1ba54d0477554a7f3">3b78117</a>)</li>
</ul>
<h4>Links</h4>
<ul>
<li>Diff: <a href="https://github.com/socketio/socket.io-parser/compare/4.2.2...4.2.3">https://github.com/socketio/socket.io-parser/compare/4.2.2...4.2.3</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/socketio/socket.io-parser/blob/main/CHANGELOG.md">socket.io-parser's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/socketio/socket.io-parser/compare/4.2.2...4.2.3">4.2.3</a> (2023-05-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>check the format of the event name (<a href="https://github.com/socketio/socket.io-parser/commit/3b78117bf6ba7e99d7a5cfc1ba54d0477554a7f3">3b78117</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/socketio/socket.io-parser/commit/b6c824f82421aa44dfd5ef395f5132866543de59"><code>b6c824f</code></a> chore(release): 4.2.3</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/dcc70d9678ac896de08294d6e8d668be6a68680a"><code>dcc70d9</code></a> refactor: export typescript declarations for the commonjs build</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/3b78117bf6ba7e99d7a5cfc1ba54d0477554a7f3"><code>3b78117</code></a> fix: check the format of the event name</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/0841bd562351c3d45a5288e2adf9707cc8a3131d"><code>0841bd5</code></a> chore: bump ua-parser-js from 1.0.32 to 1.0.33 (<a href="https://redirect.github.com/socketio/socket.io-parser/issues/121">#121</a>)</li>
<li>See full diff in <a href="https://github.com/socketio/socket.io-parser/compare/4.2.2...4.2.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=socket.io-parser&package-manager=npm_and_yarn&previous-version=4.2.2&new-version=4.2.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-05-24 02:11:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/103" class=".btn">#103</a>
            </td>
            <td>
                <b>
                    Bump socket.io-parser from 4.2.2 to 4.2.3 in /chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [socket.io-parser](https://github.com/socketio/socket.io-parser) from 4.2.2 to 4.2.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/socketio/socket.io-parser/releases">socket.io-parser's releases</a>.</em></p>
<blockquote>
<h2>4.2.3</h2>
<p>:warning: This release contains an important security fix :warning:</p>
<p>A malicious client could send a specially crafted HTTP request, triggering an uncaught exception and killing the Node.js process:</p>
<pre><code>TypeError: Cannot convert object to primitive value
       at Socket.emit (node:events:507:25)
       at .../node_modules/socket.io/lib/socket.js:531:14
</code></pre>
<p>Please upgrade as soon as possible.</p>
<h3>Bug Fixes</h3>
<ul>
<li>check the format of the event name (<a href="https://github.com/socketio/socket.io-parser/commit/3b78117bf6ba7e99d7a5cfc1ba54d0477554a7f3">3b78117</a>)</li>
</ul>
<h4>Links</h4>
<ul>
<li>Diff: <a href="https://github.com/socketio/socket.io-parser/compare/4.2.2...4.2.3">https://github.com/socketio/socket.io-parser/compare/4.2.2...4.2.3</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/socketio/socket.io-parser/blob/main/CHANGELOG.md">socket.io-parser's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/socketio/socket.io-parser/compare/4.2.2...4.2.3">4.2.3</a> (2023-05-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>check the format of the event name (<a href="https://github.com/socketio/socket.io-parser/commit/3b78117bf6ba7e99d7a5cfc1ba54d0477554a7f3">3b78117</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/socketio/socket.io-parser/commit/b6c824f82421aa44dfd5ef395f5132866543de59"><code>b6c824f</code></a> chore(release): 4.2.3</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/dcc70d9678ac896de08294d6e8d668be6a68680a"><code>dcc70d9</code></a> refactor: export typescript declarations for the commonjs build</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/3b78117bf6ba7e99d7a5cfc1ba54d0477554a7f3"><code>3b78117</code></a> fix: check the format of the event name</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/0841bd562351c3d45a5288e2adf9707cc8a3131d"><code>0841bd5</code></a> chore: bump ua-parser-js from 1.0.32 to 1.0.33 (<a href="https://redirect.github.com/socketio/socket.io-parser/issues/121">#121</a>)</li>
<li>See full diff in <a href="https://github.com/socketio/socket.io-parser/compare/4.2.2...4.2.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=socket.io-parser&package-manager=npm_and_yarn&previous-version=4.2.2&new-version=4.2.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-05-24 02:11:29 +0000 UTC
    </div>
</div>

