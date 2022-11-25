---
layout: default
title: fabric-operations-console
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operations-console
---

# fabric-operations-console <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operations-console){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/342" class=".btn">#342</a>
            </td>
            <td>
                <b>
                    Welcome page links update to hlf from cloud
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: selvaprakash92 <selvaprakash92@gmail.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
<!--- Describe your changes in detail, including motivation. -->

 Welcome page links update to hlf from cloud
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-22 14:34:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/341" class=".btn">#341</a>
            </td>
            <td>
                <b>
                    Bump engine.io and socket.io in /packages/stitch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [engine.io](https://github.com/socketio/engine.io) and [socket.io](https://github.com/socketio/socket.io). These dependencies needed to be updated together.
Updates `engine.io` from 6.1.3 to 6.2.1
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
<h2>6.2.0</h2>
<h2>Features</h2>
<ul>
<li>add the &quot;maxPayload&quot; field in the handshake details (<a href="https://github.com/socketio/engine.io/commit/088dcb4dff60df39785df13d0a33d3ceaa1dff38">088dcb4</a>)</li>
</ul>
<p>So that clients in HTTP long-polling can decide how many packets they have to send to stay under the maxHttpBufferSize
value.</p>
<p>This is a backward compatible change which should not mandate a new major revision of the protocol (we stay in v4), as
we only add a field in the JSON-encoded handshake data:</p>
<pre><code>0{&quot;sid&quot;:&quot;lv_VI97HAXpY6yYWAAAC&quot;,&quot;upgrades&quot;:[&quot;websocket&quot;],&quot;pingInterval&quot;:25000,&quot;pingTimeout&quot;:5000,&quot;maxPayload&quot;:1000000}
</code></pre>
<h4>Links</h4>
<ul>
<li>Diff: <a href="https://github.com/socketio/engine.io/compare/6.1.3...6.2.0">https://github.com/socketio/engine.io/compare/6.1.3...6.2.0</a></li>
<li>Client release: <a href="https://github.com/socketio/engine.io-client/releases/tag/6.2.0">6.2.0</a></li>
<li>ws version: <a href="https://github.com/websockets/ws/releases/tag/8.2.3">~8.2.3</a></li>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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
<li>Additional commits viewable in <a href="https://github.com/socketio/engine.io/compare/6.1.3...6.2.1">compare view</a></li>
</ul>
</details>
<br />

Updates `socket.io` from 4.4.1 to 4.5.3
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/socketio/socket.io/releases">socket.io's releases</a>.</em></p>
<blockquote>
<h2>4.5.3</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>typings:</strong> accept an HTTP2 server in the constructor (<a href="https://github.com/socketio/socket.io/commit/d3d0a2d5beaff51fd145f810bcaf6914213f8a06">d3d0a2d</a>)</li>
<li><strong>typings:</strong> apply types to &quot;io.timeout(...).emit()&quot; calls (<a href="https://github.com/socketio/socket.io/commit/e357daf5858560bc84e7e50cd36f0278d6721ea1">e357daf</a>)</li>
</ul>
<h4>Links:</h4>
<ul>
<li>Diff: <a href="https://github.com/socketio/socket.io/compare/4.5.2...4.5.3">https://github.com/socketio/socket.io/compare/4.5.2...4.5.3</a></li>
<li>Client release: <a href="https://github.com/socketio/socket.io-client/releases/tag/4.5.3">4.5.3</a></li>
<li>engine.io version:  <code>~6.2.0</code></li>
<li>ws version: <code>~8.2.3</code></li>
</ul>
<h2>4.5.2</h2>
<h3>Bug Fixes</h3>
<ul>
<li>prevent the socket from joining a room after disconnection (<a href="https://github.com/socketio/socket.io/commit/18f3fdab12947a9fee3e9c37cfc1da97027d1473">18f3fda</a>)</li>
<li><strong>uws:</strong> prevent the server from crashing after upgrade (<a href="https://github.com/socketio/socket.io/commit/ba497ee3eb52c4abf1464380d015d8c788714364">ba497ee</a>)</li>
</ul>
<h4>Links:</h4>
<ul>
<li>Diff: <a href="https://github.com/socketio/socket.io/compare/4.5.1...4.5.2">https://github.com/socketio/socket.io/compare/4.5.1...4.5.2</a></li>
<li>Client release: <a href="https://github.com/socketio/socket.io-client/releases/tag/4.5.2">4.5.2</a></li>
<li>engine.io version:  <code>~6.2.0</code></li>
<li>ws version: <code>~8.2.3</code></li>
</ul>
<h2>4.5.1</h2>
<h3>Bug Fixes</h3>
<ul>
<li>forward the local flag to the adapter when using fetchSockets() (<a href="https://github.com/socketio/socket.io/commit/30430f0985f8e7c49394543d4c84913b6a15df60">30430f0</a>)</li>
<li><strong>typings:</strong> add HTTPS server to accepted types (<a href="https://github-redirect.dependabot.com/socketio/socket.io/issues/4351">#4351</a>) (<a href="https://github.com/socketio/socket.io/commit/9b43c9167cff817c60fa29dbda2ef7cd938aff51">9b43c91</a>)</li>
</ul>
<h4>Links:</h4>
<ul>
<li>Diff: <a href="https://github.com/socketio/socket.io/compare/4.5.0...4.5.1">https://github.com/socketio/socket.io/compare/4.5.0...4.5.1</a></li>
<li>Client release: <a href="https://github.com/socketio/socket.io-client/releases/tag/4.5.1">4.5.1</a></li>
<li>engine.io version:  <code>~6.2.0</code></li>
<li>ws version: <code>~8.2.3</code></li>
</ul>
<h2>4.5.0</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>typings:</strong> ensure compatibility with TypeScript 3.x (<a href="https://github-redirect.dependabot.com/socketio/socket.io/issues/4259">#4259</a>) (<a href="https://github.com/socketio/socket.io/commit/02c87a85614e217b8e7b93753f315790ae9d99f6">02c87a8</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>add support for catch-all listeners for outgoing packets (<a href="https://github.com/socketio/socket.io/commit/531104d332690138b7aab84d5583d6204132c8b4">531104d</a>)</li>
</ul>
<p>This is similar to <code>onAny()</code>, but for outgoing packets.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/socketio/socket.io/blob/main/CHANGELOG.md">socket.io's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/socketio/socket.io/compare/4.5.2...4.5.3">4.5.3</a> (2022-10-15)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>typings:</strong> accept an HTTP2 server in the constructor (<a href="https://github.com/socketio/socket.io/commit/d3d0a2d5beaff51fd145f810bcaf6914213f8a06">d3d0a2d</a>)</li>
<li><strong>typings:</strong> apply types to &quot;io.timeout(...).emit()&quot; calls (<a href="https://github.com/socketio/socket.io/commit/e357daf5858560bc84e7e50cd36f0278d6721ea1">e357daf</a>)</li>
</ul>
<h2><a href="https://github.com/socketio/socket.io/compare/4.5.1...4.5.2">4.5.2</a> (2022-09-02)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>prevent the socket from joining a room after disconnection (<a href="https://github.com/socketio/socket.io/commit/18f3fdab12947a9fee3e9c37cfc1da97027d1473">18f3fda</a>)</li>
<li><strong>uws:</strong> prevent the server from crashing after upgrade (<a href="https://github.com/socketio/socket.io/commit/ba497ee3eb52c4abf1464380d015d8c788714364">ba497ee</a>)</li>
</ul>
<h1><a href="https://github.com/socketio/socket.io/compare/2.4.1...2.5.0">2.5.0</a> (2022-06-26)</h1>
<h3>Bug Fixes</h3>
<ul>
<li>fix race condition in dynamic namespaces (<a href="https://github.com/socketio/socket.io/commit/05e1278cfa99f3ecf3f8f0531ffe57d850e9a05b">05e1278</a>)</li>
<li>ignore packet received after disconnection (<a href="https://github.com/socketio/socket.io/commit/22d4bdf00d1a03885dc0171125faddfaef730066">22d4bdf</a>)</li>
<li>only set 'connected' to true after middleware execution (<a href="https://github.com/socketio/socket.io/commit/226cc16165f9fe60f16ff4d295fb91c8971cde35">226cc16</a>)</li>
<li>prevent the socket from joining a room after disconnection (<a href="https://github.com/socketio/socket.io/commit/f223178eb655a7713303b21a78f9ef9e161d6458">f223178</a>)</li>
</ul>
<h2><a href="https://github.com/socketio/socket.io/compare/4.5.0...4.5.1">4.5.1</a> (2022-05-17)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>forward the local flag to the adapter when using fetchSockets() (<a href="https://github.com/socketio/socket.io/commit/30430f0985f8e7c49394543d4c84913b6a15df60">30430f0</a>)</li>
<li><strong>typings:</strong> add HTTPS server to accepted types (<a href="https://github-redirect.dependabot.com/socketio/socket.io/issues/4351">#4351</a>) (<a href="https://github.com/socketio/socket.io/commit/9b43c9167cff817c60fa29dbda2ef7cd938aff51">9b43c91</a>)</li>
</ul>
<h1><a href="https://github.com/socketio/socket.io/compare/4.4.1...4.5.0">4.5.0</a> (2022-04-23)</h1>
<h3>Bug Fixes</h3>
<ul>
<li><strong>typings:</strong> ensure compatibility with TypeScript 3.x (<a href="https://github-redirect.dependabot.com/socketio/socket.io/issues/4259">#4259</a>) (<a href="https://github.com/socketio/socket.io/commit/02c87a85614e217b8e7b93753f315790ae9d99f6">02c87a8</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/socketio/socket.io/commit/945c84be47d2923a9132786c9fd11dd90fa2c6db"><code>945c84b</code></a> chore(release): 4.5.3</li>
<li><a href="https://github.com/socketio/socket.io/commit/d3d0a2d5beaff51fd145f810bcaf6914213f8a06"><code>d3d0a2d</code></a> fix(typings): accept an HTTP2 server in the constructor</li>
<li><a href="https://github.com/socketio/socket.io/commit/19b225b0c8a093d7f54ccf1b9d3765bc8f463a65"><code>19b225b</code></a> docs(examples): update dependencies of the basic CRUD example</li>
<li><a href="https://github.com/socketio/socket.io/commit/8fae95dd182ee1fdd033f7646eacc6beca6f456a"><code>8fae95d</code></a> docs: add jsdoc for each public method</li>
<li><a href="https://github.com/socketio/socket.io/commit/e6f6b906db8209996b1adb564332cb443df38fc6"><code>e6f6b90</code></a> docs: add deprecation notice for the allSockets() method</li>
<li><a href="https://github.com/socketio/socket.io/commit/596eb88af7fcd41e9d7c0abca4d1305a7e2c2fea"><code>596eb88</code></a> ci: upgrade to actions/checkout@3 and actions/setup-node@3</li>
<li><a href="https://github.com/socketio/socket.io/commit/e357daf5858560bc84e7e50cd36f0278d6721ea1"><code>e357daf</code></a> fix(typings): apply types to &quot;io.timeout(...).emit()&quot; calls</li>
<li><a href="https://github.com/socketio/socket.io/commit/10fa4a2690fafcf9415e49aad507394e0b9a9ab0"><code>10fa4a2</code></a> refactor: add list of possible disconnection reasons</li>
<li><a href="https://github.com/socketio/socket.io/commit/8be95b3bd323f83b9bc5d7b0292abc2dbea9ce56"><code>8be95b3</code></a> chore(release): 4.5.2</li>
<li><a href="https://github.com/socketio/socket.io/commit/ba497ee3eb52c4abf1464380d015d8c788714364"><code>ba497ee</code></a> fix(uws): prevent the server from crashing after upgrade</li>
<li>Additional commits viewable in <a href="https://github.com/socketio/socket.io/compare/4.4.1...4.5.3">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-operations-console/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-22 03:49:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/340" class=".btn">#340</a>
            </td>
            <td>
                <b>
                    Bump loader-utils from 1.4.1 to 1.4.2 in /packages/stitch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [loader-utils](https://github.com/webpack/loader-utils) from 1.4.1 to 1.4.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/loader-utils/releases">loader-utils's releases</a>.</em></p>
<blockquote>
<h2>v1.4.2</h2>
<h3><a href="https://github.com/webpack/loader-utils/compare/v1.4.1...v1.4.2">1.4.2</a> (2022-11-11)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>ReDoS problem (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/226">#226</a>) (<a href="https://github.com/webpack/loader-utils/commit/17cbf8fa8989c1cb45bdd2997aa524729475f1fa">17cbf8f</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/webpack/loader-utils/blob/v1.4.2/CHANGELOG.md">loader-utils's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/webpack/loader-utils/compare/v1.4.1...v1.4.2">1.4.2</a> (2022-11-11)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>ReDoS problem (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/226">#226</a>) (<a href="https://github.com/webpack/loader-utils/commit/17cbf8fa8989c1cb45bdd2997aa524729475f1fa">17cbf8f</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/loader-utils/commit/331ad5067d9a1a7b8d646692e6959639969210d1"><code>331ad50</code></a> chore(release): 1.4.2</li>
<li><a href="https://github.com/webpack/loader-utils/commit/17cbf8fa8989c1cb45bdd2997aa524729475f1fa"><code>17cbf8f</code></a> fix: ReDoS problem (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/226">#226</a>)</li>
<li>See full diff in <a href="https://github.com/webpack/loader-utils/compare/v1.4.1...v1.4.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=loader-utils&package-manager=npm_and_yarn&previous-version=1.4.1&new-version=1.4.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-operations-console/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-21 14:09:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/339" class=".btn">#339</a>
            </td>
            <td>
                <b>
                    Welcome page launch icon added
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: selvaprakash92 <selvaprakash92@gmail.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix


#### Description
<!--- Describe your changes in detail, including motivation. -->

Welcome page launch icon added

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-21 13:33:16 +0000 UTC
    </div>
</div>

