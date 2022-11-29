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
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/71" class=".btn">#71</a>
            </td>
            <td>
                <b>
                    Bump engine.io from 6.2.0 to 6.2.1 in /platform/backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [engine.io](https://github.com/socketio/engine.io) from 6.2.0 to 6.2.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/socketio/engine.io/releases">engine.io's releases</a>.</em></p>
<blockquote>
<h2>6.2.1</h2>
<p>:warning: This release contains an important security fix :warning:</p>
<p>A malicious client could send a specially crafted HTTP request, triggering an uncaught exception and killing the Node.js process:</p>
<pre><code>Error: read ECONNRESET
    at TCP.onStreamRead (internal/stream_base_commons.js:209:20)
Emitted 'error' event on Socket instance at:
    at emitErrorNT (internal/streams/destroy.js:106:8)
    at emitErrorCloseNT (internal/streams/destroy.js:74:3)
    at processTicksAndRejections (internal/process/task_queues.js:80:21) {
  errno: -104,
  code: 'ECONNRESET',
  syscall: 'read'
}
</code></pre>
<p>Please upgrade as soon as possible.</p>
<h3>Bug Fixes</h3>
<ul>
<li>catch errors when destroying invalid upgrades (<a href="https://github-redirect.dependabot.com/socketio/engine.io/issues/658">#658</a>) (<a href="https://github.com/socketio/engine.io/commit/425e833ab13373edf1dd5a0706f07100db14e3c6">425e833</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/socketio/engine.io/blob/main/CHANGELOG.md">engine.io's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/socketio/engine.io/compare/6.2.0...6.2.1">6.2.1</a> (2022-11-20)</h2>
<p>:warning: This release contains an important security fix :warning:</p>
<p>A malicious client could send a specially crafted HTTP request, triggering an uncaught exception and killing the Node.js process:</p>
<pre><code>Error: read ECONNRESET
    at TCP.onStreamRead (internal/stream_base_commons.js:209:20)
Emitted 'error' event on Socket instance at:
    at emitErrorNT (internal/streams/destroy.js:106:8)
    at emitErrorCloseNT (internal/streams/destroy.js:74:3)
    at processTicksAndRejections (internal/process/task_queues.js:80:21) {
  errno: -104,
  code: 'ECONNRESET',
  syscall: 'read'
}
</code></pre>
<p>Please upgrade as soon as possible.</p>
<h3>Bug Fixes</h3>
<ul>
<li>catch errors when destroying invalid upgrades (<a href="https://github-redirect.dependabot.com/socketio/engine.io/issues/658">#658</a>) (<a href="https://github.com/socketio/engine.io/commit/425e833ab13373edf1dd5a0706f07100db14e3c6">425e833</a>)</li>
</ul>
<h1><a href="https://github.com/socketio/engine.io/compare/3.5.0...3.6.0">3.6.0</a> (2022-06-06)</h1>
<h3>Bug Fixes</h3>
<ul>
<li>add extension in the package.json main entry (<a href="https://github-redirect.dependabot.com/socketio/engine.io/issues/608">#608</a>) (<a href="https://github.com/socketio/engine.io/commit/3ad0567dbd57cfb7c2ff4e8b7488d80f37022b4a">3ad0567</a>)</li>
<li>do not reset the ping timer after upgrade (<a href="https://github.com/socketio/engine.io/commit/1f5d4699862afee1e410fcb0e1f5e751ebcd2f9f">1f5d469</a>), closes <a href="https://github-redirect.dependabot.com//github-redirect.dependabot.com/socketio/socket.io-client-swift/pull/1309/issues/issuecomment-768475704">socketio/socket.io-client-swift#1309</a></li>
</ul>
<h3>Features</h3>
<ul>
<li>decrease the default value of maxHttpBufferSize (<a href="https://github.com/socketio/engine.io/commit/58e274c437e9cbcf69fd913c813aad8fbd253703">58e274c</a>)</li>
</ul>
<p>This change reduces the default value from 100 mb to a more sane 1 mb.</p>
<p>This helps protect the server against denial of service attacks by malicious clients sending huge amounts of data.</p>
<p>See also: <a href="https://github.com/advisories/GHSA-j4f2-536g-r55m">https://github.com/advisories/GHSA-j4f2-536g-r55m</a></p>
<ul>
<li>increase the default value of pingTimeout (<a href="https://github.com/socketio/engine.io/commit/f55a79a28a5fbc6c9edae876dd11308b89cc979e">f55a79a</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/socketio/engine.io/commit/24b847be6a61b64efc8c8c4d058a69259ad67693"><code>24b847b</code></a> chore(release): 6.2.1</li>
<li><a href="https://github.com/socketio/engine.io/commit/425e833ab13373edf1dd5a0706f07100db14e3c6"><code>425e833</code></a> fix: catch errors when destroying invalid upgrades (<a href="https://github-redirect.dependabot.com/socketio/engine.io/issues/658">#658</a>)</li>
<li><a href="https://github.com/socketio/engine.io/commit/99adb00ba11d80ab27a4a2f4afd0eebd8aa406c5"><code>99adb00</code></a> chore(deps): bump xmlhttprequest-ssl and engine.io-client in /examples/latenc...</li>
<li><a href="https://github.com/socketio/engine.io/commit/d196f6a6b746b5e362b131a1a16901a3db12cb21"><code>d196f6a</code></a> chore(deps): bump minimatch from 3.0.4 to 3.1.2 (<a href="https://github-redirect.dependabot.com/socketio/engine.io/issues/660">#660</a>)</li>
<li><a href="https://github.com/socketio/engine.io/commit/7c1270f98c51e51dfae1237492a56276070fd10e"><code>7c1270f</code></a> chore(deps): bump nanoid from 3.1.25 to 3.3.1 (<a href="https://github-redirect.dependabot.com/socketio/engine.io/issues/659">#659</a>)</li>
<li><a href="https://github.com/socketio/engine.io/commit/535a01d8898a5cc858c9d6031fc5ecda96ea4579"><code>535a01d</code></a> ci: add Node.js 18 in the test matrix</li>
<li><a href="https://github.com/socketio/engine.io/commit/1b71a6f5cb868c934696ae3cc1a92d1168ec8505"><code>1b71a6f</code></a> docs: remove &quot;Vanilla JS&quot; highlight from README (<a href="https://github-redirect.dependabot.com/socketio/engine.io/issues/656">#656</a>)</li>
<li><a href="https://github.com/socketio/engine.io/commit/917d1d29e13f2e8f523c3738f6413f67b587aebe"><code>917d1d2</code></a> refactor: replace deprecated <code>String.prototype.substr()</code> (<a href="https://github-redirect.dependabot.com/socketio/engine.io/issues/646">#646</a>)</li>
<li><a href="https://github.com/socketio/engine.io/commit/020801ab8ce2d4cba517fe04df89b39d403123a5"><code>020801a</code></a> chore: add changelog for version 3.6.0</li>
<li><a href="https://github.com/socketio/engine.io/commit/ed1d6f912ce61b13e2ae7ce7a1027b8c5fae2f15"><code>ed1d6f9</code></a> test: make test script work on Windows (<a href="https://github-redirect.dependabot.com/socketio/engine.io/issues/643">#643</a>)</li>
<li>See full diff in <a href="https://github.com/socketio/engine.io/compare/6.2.0...6.2.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=engine.io&package-manager=npm_and_yarn&previous-version=6.2.0&new-version=6.2.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-22 06:51:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/70" class=".btn">#70</a>
            </td>
            <td>
                <b>
                    Bump engine.io from 6.2.0 to 6.2.1 in /explorer/backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [engine.io](https://github.com/socketio/engine.io) from 6.2.0 to 6.2.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/socketio/engine.io/releases">engine.io's releases</a>.</em></p>
<blockquote>
<h2>6.2.1</h2>
<p>:warning: This release contains an important security fix :warning:</p>
<p>A malicious client could send a specially crafted HTTP request, triggering an uncaught exception and killing the Node.js process:</p>
<pre><code>Error: read ECONNRESET
    at TCP.onStreamRead (internal/stream_base_commons.js:209:20)
Emitted 'error' event on Socket instance at:
    at emitErrorNT (internal/streams/destroy.js:106:8)
    at emitErrorCloseNT (internal/streams/destroy.js:74:3)
    at processTicksAndRejections (internal/process/task_queues.js:80:21) {
  errno: -104,
  code: 'ECONNRESET',
  syscall: 'read'
}
</code></pre>
<p>Please upgrade as soon as possible.</p>
<h3>Bug Fixes</h3>
<ul>
<li>catch errors when destroying invalid upgrades (<a href="https://github-redirect.dependabot.com/socketio/engine.io/issues/658">#658</a>) (<a href="https://github.com/socketio/engine.io/commit/425e833ab13373edf1dd5a0706f07100db14e3c6">425e833</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/socketio/engine.io/blob/main/CHANGELOG.md">engine.io's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/socketio/engine.io/compare/6.2.0...6.2.1">6.2.1</a> (2022-11-20)</h2>
<p>:warning: This release contains an important security fix :warning:</p>
<p>A malicious client could send a specially crafted HTTP request, triggering an uncaught exception and killing the Node.js process:</p>
<pre><code>Error: read ECONNRESET
    at TCP.onStreamRead (internal/stream_base_commons.js:209:20)
Emitted 'error' event on Socket instance at:
    at emitErrorNT (internal/streams/destroy.js:106:8)
    at emitErrorCloseNT (internal/streams/destroy.js:74:3)
    at processTicksAndRejections (internal/process/task_queues.js:80:21) {
  errno: -104,
  code: 'ECONNRESET',
  syscall: 'read'
}
</code></pre>
<p>Please upgrade as soon as possible.</p>
<h3>Bug Fixes</h3>
<ul>
<li>catch errors when destroying invalid upgrades (<a href="https://github-redirect.dependabot.com/socketio/engine.io/issues/658">#658</a>) (<a href="https://github.com/socketio/engine.io/commit/425e833ab13373edf1dd5a0706f07100db14e3c6">425e833</a>)</li>
</ul>
<h1><a href="https://github.com/socketio/engine.io/compare/3.5.0...3.6.0">3.6.0</a> (2022-06-06)</h1>
<h3>Bug Fixes</h3>
<ul>
<li>add extension in the package.json main entry (<a href="https://github-redirect.dependabot.com/socketio/engine.io/issues/608">#608</a>) (<a href="https://github.com/socketio/engine.io/commit/3ad0567dbd57cfb7c2ff4e8b7488d80f37022b4a">3ad0567</a>)</li>
<li>do not reset the ping timer after upgrade (<a href="https://github.com/socketio/engine.io/commit/1f5d4699862afee1e410fcb0e1f5e751ebcd2f9f">1f5d469</a>), closes <a href="https://github-redirect.dependabot.com//github-redirect.dependabot.com/socketio/socket.io-client-swift/pull/1309/issues/issuecomment-768475704">socketio/socket.io-client-swift#1309</a></li>
</ul>
<h3>Features</h3>
<ul>
<li>decrease the default value of maxHttpBufferSize (<a href="https://github.com/socketio/engine.io/commit/58e274c437e9cbcf69fd913c813aad8fbd253703">58e274c</a>)</li>
</ul>
<p>This change reduces the default value from 100 mb to a more sane 1 mb.</p>
<p>This helps protect the server against denial of service attacks by malicious clients sending huge amounts of data.</p>
<p>See also: <a href="https://github.com/advisories/GHSA-j4f2-536g-r55m">https://github.com/advisories/GHSA-j4f2-536g-r55m</a></p>
<ul>
<li>increase the default value of pingTimeout (<a href="https://github.com/socketio/engine.io/commit/f55a79a28a5fbc6c9edae876dd11308b89cc979e">f55a79a</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/socketio/engine.io/commit/24b847be6a61b64efc8c8c4d058a69259ad67693"><code>24b847b</code></a> chore(release): 6.2.1</li>
<li><a href="https://github.com/socketio/engine.io/commit/425e833ab13373edf1dd5a0706f07100db14e3c6"><code>425e833</code></a> fix: catch errors when destroying invalid upgrades (<a href="https://github-redirect.dependabot.com/socketio/engine.io/issues/658">#658</a>)</li>
<li><a href="https://github.com/socketio/engine.io/commit/99adb00ba11d80ab27a4a2f4afd0eebd8aa406c5"><code>99adb00</code></a> chore(deps): bump xmlhttprequest-ssl and engine.io-client in /examples/latenc...</li>
<li><a href="https://github.com/socketio/engine.io/commit/d196f6a6b746b5e362b131a1a16901a3db12cb21"><code>d196f6a</code></a> chore(deps): bump minimatch from 3.0.4 to 3.1.2 (<a href="https://github-redirect.dependabot.com/socketio/engine.io/issues/660">#660</a>)</li>
<li><a href="https://github.com/socketio/engine.io/commit/7c1270f98c51e51dfae1237492a56276070fd10e"><code>7c1270f</code></a> chore(deps): bump nanoid from 3.1.25 to 3.3.1 (<a href="https://github-redirect.dependabot.com/socketio/engine.io/issues/659">#659</a>)</li>
<li><a href="https://github.com/socketio/engine.io/commit/535a01d8898a5cc858c9d6031fc5ecda96ea4579"><code>535a01d</code></a> ci: add Node.js 18 in the test matrix</li>
<li><a href="https://github.com/socketio/engine.io/commit/1b71a6f5cb868c934696ae3cc1a92d1168ec8505"><code>1b71a6f</code></a> docs: remove &quot;Vanilla JS&quot; highlight from README (<a href="https://github-redirect.dependabot.com/socketio/engine.io/issues/656">#656</a>)</li>
<li><a href="https://github.com/socketio/engine.io/commit/917d1d29e13f2e8f523c3738f6413f67b587aebe"><code>917d1d2</code></a> refactor: replace deprecated <code>String.prototype.substr()</code> (<a href="https://github-redirect.dependabot.com/socketio/engine.io/issues/646">#646</a>)</li>
<li><a href="https://github.com/socketio/engine.io/commit/020801ab8ce2d4cba517fe04df89b39d403123a5"><code>020801a</code></a> chore: add changelog for version 3.6.0</li>
<li><a href="https://github.com/socketio/engine.io/commit/ed1d6f912ce61b13e2ae7ce7a1027b8c5fae2f15"><code>ed1d6f9</code></a> test: make test script work on Windows (<a href="https://github-redirect.dependabot.com/socketio/engine.io/issues/643">#643</a>)</li>
<li>See full diff in <a href="https://github.com/socketio/engine.io/compare/6.2.0...6.2.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=engine.io&package-manager=npm_and_yarn&previous-version=6.2.0&new-version=6.2.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-22 06:50:52 +0000 UTC
    </div>
</div>

