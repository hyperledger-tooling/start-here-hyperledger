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
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/102" class=".btn">#102</a>
            </td>
            <td>
                <b>
                    Bump socket.io-parser from 4.2.1 to 4.2.3 in /explorer/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [socket.io-parser](https://github.com/socketio/socket.io-parser) from 4.2.1 to 4.2.3.
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
<h2>4.2.2</h2>
<h3>Bug Fixes</h3>
<ul>
<li>calling destroy() should clear all internal state (<a href="https://github.com/socketio/socket.io-parser/commit/22c42e3545e4adbc5931276c378f5d62c8b3854a">22c42e3</a>)</li>
<li>do not modify the input packet upon encoding (<a href="https://github.com/socketio/socket.io-parser/commit/ae8dd88995dbd7f89c97e5cc15e5b489fa0efece">ae8dd88</a>)</li>
</ul>
<h4>Links</h4>
<ul>
<li>Diff: <a href="https://github.com/socketio/socket.io-parser/compare/4.2.1...4.2.2">https://github.com/socketio/socket.io-parser/compare/4.2.1...4.2.2</a></li>
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
<h2><a href="https://github.com/socketio/socket.io-parser/compare/4.2.1...4.2.2">4.2.2</a> (2023-01-19)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>calling destroy() should clear all internal state (<a href="https://github.com/socketio/socket.io-parser/commit/22c42e3545e4adbc5931276c378f5d62c8b3854a">22c42e3</a>)</li>
<li>do not modify the input packet upon encoding (<a href="https://github.com/socketio/socket.io-parser/commit/ae8dd88995dbd7f89c97e5cc15e5b489fa0efece">ae8dd88</a>)</li>
</ul>
<h2><a href="https://github.com/Automattic/socket.io-parser/compare/3.3.2...3.3.3">3.3.3</a> (2022-11-09)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>check the format of the index of each attachment (<a href="https://github.com/Automattic/socket.io-parser/commit/fb21e422fc193b34347395a33e0f625bebc09983">fb21e42</a>)</li>
</ul>
<h2><a href="https://github.com/socketio/socket.io-parser/compare/3.4.1...3.4.2">3.4.2</a> (2022-11-09)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>check the format of the index of each attachment (<a href="https://github.com/socketio/socket.io-parser/commit/04d23cecafe1b859fb03e0cbf6ba3b74dff56d14">04d23ce</a>)</li>
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
<li><a href="https://github.com/socketio/socket.io-parser/commit/28dd6685021353b26a4b022e25b453c627d0a7e8"><code>28dd668</code></a> chore(release): 4.2.2</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/22c42e3545e4adbc5931276c378f5d62c8b3854a"><code>22c42e3</code></a> fix: calling destroy() should clear all internal state</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/ae8dd88995dbd7f89c97e5cc15e5b489fa0efece"><code>ae8dd88</code></a> fix: do not modify the input packet upon encoding</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/9143aa4c8e911a8e3044a0f47fde8f98a9a86974"><code>9143aa4</code></a> chore: update browserslist</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/194a9b762e65d655d93897866f1568ed185b19ae"><code>194a9b7</code></a> ci: migrate from zuul to webdriver.io</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/a9758da4be988419a1c17ddd2299833993712d5f"><code>a9758da</code></a> ci: update actions in GitHub Actions workflows (<a href="https://redirect.github.com/socketio/socket.io-parser/issues/117">#117</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/socketio/socket.io-parser/compare/4.2.1...4.2.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=socket.io-parser&package-manager=npm_and_yarn&previous-version=4.2.1&new-version=4.2.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-05-24 00:48:29 +0000 UTC
    </div>
</div>

