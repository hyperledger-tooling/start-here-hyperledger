---
layout: default
title: aries-acapy-controllers
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-controllers
---

# aries-acapy-controllers <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-controllers){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-controllers/pull/91" class=".btn">#91</a>
            </td>
            <td>
                <b>
                    Bump socket.io-parser from 4.2.1 to 4.2.4 in /AliceFaberAcmeDemo/controllers/alice-controller
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [socket.io-parser](https://github.com/socketio/socket.io-parser) from 4.2.1 to 4.2.4.
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
<h2><a href="https://github.com/socketio/socket.io-parser/compare/4.2.3...4.2.4">4.2.4</a> (2023-05-31)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>ensure reserved events cannot be used as event names (<a href="https://github.com/socketio/socket.io-parser/commit/d9db4737a3c8ce5f1f49ecc8d928a74f3da591f7">d9db473</a>)</li>
<li>properly detect plain objects (<a href="https://github.com/socketio/socket.io-parser/commit/b0e6400c93b5c4aa25e6a629d6448b8627275213">b0e6400</a>)</li>
</ul>
<h2><a href="https://github.com/socketio/socket.io-parser/compare/3.4.2...3.4.3">3.4.3</a> (2023-05-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>check the format of the event name (<a href="https://github.com/socketio/socket.io-parser/commit/2dc3c92622dad113b8676be06f23b1ed46b02ced">2dc3c92</a>)</li>
</ul>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/socketio/socket.io-parser/commit/164ba2a11edc34c2f363401e9768f9a8541a8b89"><code>164ba2a</code></a> chore(release): 4.2.4</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/b0e6400c93b5c4aa25e6a629d6448b8627275213"><code>b0e6400</code></a> fix: properly detect plain objects</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/d9db4737a3c8ce5f1f49ecc8d928a74f3da591f7"><code>d9db473</code></a> fix: ensure reserved events cannot be used as event names</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/6a5a004d1e1fd7b7250fdc6fb148e0d9015f8368"><code>6a5a004</code></a> docs(changelog): include changelog for release 3.4.3</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/b6c824f82421aa44dfd5ef395f5132866543de59"><code>b6c824f</code></a> chore(release): 4.2.3</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/dcc70d9678ac896de08294d6e8d668be6a68680a"><code>dcc70d9</code></a> refactor: export typescript declarations for the commonjs build</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/3b78117bf6ba7e99d7a5cfc1ba54d0477554a7f3"><code>3b78117</code></a> fix: check the format of the event name</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/0841bd562351c3d45a5288e2adf9707cc8a3131d"><code>0841bd5</code></a> chore: bump ua-parser-js from 1.0.32 to 1.0.33 (<a href="https://redirect.github.com/socketio/socket.io-parser/issues/121">#121</a>)</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/28dd6685021353b26a4b022e25b453c627d0a7e8"><code>28dd668</code></a> chore(release): 4.2.2</li>
<li><a href="https://github.com/socketio/socket.io-parser/commit/22c42e3545e4adbc5931276c378f5d62c8b3854a"><code>22c42e3</code></a> fix: calling destroy() should clear all internal state</li>
<li>Additional commits viewable in <a href="https://github.com/socketio/socket.io-parser/compare/4.2.1...4.2.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=socket.io-parser&package-manager=npm_and_yarn&previous-version=4.2.1&new-version=4.2.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-controllers/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-01 10:43:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-controllers/pull/90" class=".btn">#90</a>
            </td>
            <td>
                <b>
                    Add QR code to new connection page on faber and acme controller
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Related to : https://github.com/hyperledger/aries-acapy-controllers/issues/88#issue-1728720771 and https://github.com/hyperledger/aries-acapy-controllers/issues/89

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-31 16:25:38 +0000 UTC
    </div>
</div>

