---
layout: default
title: firefly-tokens-erc20-erc721
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-tokens-erc20-erc721
---

# firefly-tokens-erc20-erc721 <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-tokens-erc20-erc721){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/164" class=".btn">#164</a>
            </td>
            <td>
                <b>
                    Bump the npm_and_yarn group across 2 directories with 3 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps the npm_and_yarn group with 2 updates in the / directory: [ws](https://github.com/websockets/ws) and [braces](https://github.com/micromatch/braces).
Bumps the npm_and_yarn group with 3 updates in the /samples/solidity directory: [ws](https://github.com/websockets/ws), [ethers](https://github.com/ethers-io/ethers.js) and [braces](https://github.com/micromatch/braces).

Updates `ws` from 8.16.0 to 8.17.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/websockets/ws/releases">ws's releases</a>.</em></p>
<blockquote>
<h2>8.17.1</h2>
<h1>Bug fixes</h1>
<ul>
<li>Fixed a DoS vulnerability (<a href="https://redirect.github.com/websockets/ws/issues/2231">#2231</a>).</li>
</ul>
<p>A request with a number of headers exceeding the[<code>server.maxHeadersCount</code>][]
threshold could be used to crash a ws server.</p>
<pre lang="js"><code>const http = require('http');
const WebSocket = require('ws');
<p>const wss = new WebSocket.Server({ port: 0 }, function () {
const chars = &quot;!#$%&amp;'*+-.0123456789abcdefghijklmnopqrstuvwxyz^_`|~&quot;.split('');
const headers = {};
let count = 0;</p>
<p>for (let i = 0; i &lt; chars.length; i++) {
if (count === 2000) break;</p>
<pre><code>for (let j = 0; j &amp;lt; chars.length; j++) {
  const key = chars[i] + chars[j];
  headers[key] = 'x';

  if (++count === 2000) break;
}
</code></pre>
<p>}</p>
<p>headers.Connection = 'Upgrade';
headers.Upgrade = 'websocket';
headers['Sec-WebSocket-Key'] = 'dGhlIHNhbXBsZSBub25jZQ==';
headers['Sec-WebSocket-Version'] = '13';</p>
<p>const request = http.request({
headers: headers,
host: '127.0.0.1',
port: wss.address().port
});</p>
<p>request.end();
});
</code></pre></p>
<p>The vulnerability was reported by <a href="https://github.com/rrlapointe">Ryan LaPointe</a> in <a href="https://redirect.github.com/websockets/ws/issues/2230">websockets/ws#2230</a>.</p>
<p>In vulnerable versions of ws, the issue can be mitigated in the following ways:</p>
<ol>
<li>Reduce the maximum allowed length of the request headers using the
[<code>--max-http-header-size=size</code>][] and/or the [<code>maxHeaderSize</code>][] options so
that no more headers than the <code>server.maxHeadersCount</code> limit can be sent.</li>
</ol>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/websockets/ws/commit/3c56601092872f7d7566989f0e379271afd0e4a1"><code>3c56601</code></a> [dist] 8.17.1</li>
<li><a href="https://github.com/websockets/ws/commit/e55e5106f10fcbaac37cfa89759e4cc0d073a52c"><code>e55e510</code></a> [security] Fix crash when the Upgrade header cannot be read (<a href="https://redirect.github.com/websockets/ws/issues/2231">#2231</a>)</li>
<li><a href="https://github.com/websockets/ws/commit/6a00029edd924499f892aed8003cef1fa724cfe5"><code>6a00029</code></a> [test] Increase code coverage</li>
<li><a href="https://github.com/websockets/ws/commit/ddfe4a804d79e7788ab136290e609f91cf68423f"><code>ddfe4a8</code></a> [perf] Reduce the amount of <code>crypto.randomFillSync()</code> calls</li>
<li><a href="https://github.com/websockets/ws/commit/b73b11828d166e9692a9bffe9c01a7e93bab04a8"><code>b73b118</code></a> [dist] 8.17.0</li>
<li><a href="https://github.com/websockets/ws/commit/29694a5905fa703e86667928e6bacac397469471"><code>29694a5</code></a> [test] Use the <code>highWaterMark</code> variable</li>
<li><a href="https://github.com/websockets/ws/commit/934c9d6b938b93c045cb13e5f7c19c27a8dd925a"><code>934c9d6</code></a> [ci] Test on node 22</li>
<li><a href="https://github.com/websockets/ws/commit/1817bac06e1204bfb578b8b3f4bafd0fa09623d0"><code>1817bac</code></a> [ci] Do not test on node 21</li>
<li><a href="https://github.com/websockets/ws/commit/96c9b3deddf56cacb2d756aaa918071e03cdbc42"><code>96c9b3d</code></a> [major] Flip the default value of <code>allowSynchronousEvents</code> (<a href="https://redirect.github.com/websockets/ws/issues/2221">#2221</a>)</li>
<li><a href="https://github.com/websockets/ws/commit/e5f32c7e1e6d3d19cd4a1fdec84890e154db30c1"><code>e5f32c7</code></a> [fix] Emit at most one event per event loop iteration (<a href="https://redirect.github.com/websockets/ws/issues/2218">#2218</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/websockets/ws/compare/8.16.0...8.17.1">compare view</a></li>
</ul>
</details>
<br />

Updates `braces` from 3.0.2 to 3.0.3
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/micromatch/braces/commit/74b2db2938fad48a2ea54a9c8bf27a37a62c350d"><code>74b2db2</code></a> 3.0.3</li>
<li><a href="https://github.com/micromatch/braces/commit/88f1429a0f47e1dd3813de35211fc97ffda27f9e"><code>88f1429</code></a> update eslint. lint, fix unit tests.</li>
<li><a href="https://github.com/micromatch/braces/commit/415d660c3002d1ab7e63dbf490c9851da80596ff"><code>415d660</code></a> Snyk js braces 6838727 (<a href="https://redirect.github.com/micromatch/braces/issues/40">#40</a>)</li>
<li><a href="https://github.com/micromatch/braces/commit/190510f79db1adf21d92798b0bb6fccc1f72c9d6"><code>190510f</code></a> fix tests, skip 1 test in test/braces.expand</li>
<li><a href="https://github.com/micromatch/braces/commit/716eb9f12d820b145a831ad678618731927e8856"><code>716eb9f</code></a> readme bump</li>
<li><a href="https://github.com/micromatch/braces/commit/a5851e57f45c3431a94d83fc565754bc10f5bbc3"><code>a5851e5</code></a> Merge pull request <a href="https://redirect.github.com/micromatch/braces/issues/37">#37</a> from coderaiser/fix/vulnerability</li>
<li><a href="https://github.com/micromatch/braces/commit/2092bd1fb108d2c59bd62e243b70ad98db961538"><code>2092bd1</code></a> feature: braces: add maxSymbols (<a href="https://github.com/micromatch/braces/issues/">https://github.com/micromatch/braces/issues/</a>...</li>
<li><a href="https://github.com/micromatch/braces/commit/9f5b4cf47329351bcb64287223ffb6ecc9a5e6d3"><code>9f5b4cf</code></a> fix: vulnerability (<a href="https://security.snyk.io/vuln/SNYK-JS-BRACES-6838727">https://security.snyk.io/vuln/SNYK-JS-BRACES-6838727</a>)</li>
<li><a href="https://github.com/micromatch/braces/commit/98414f9f1fabe021736e26836d8306d5de747e0d"><code>98414f9</code></a> remove funding file</li>
<li><a href="https://github.com/micromatch/braces/commit/665ab5d561c017a38ba7aafd92cc6655b91d8c14"><code>665ab5d</code></a> update keepEscaping doc (<a href="https://redirect.github.com/micromatch/braces/issues/27">#27</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/micromatch/braces/compare/3.0.2...3.0.3">compare view</a></li>
</ul>
</details>
<br />

Updates `ws` from 7.5.9 to 8.17.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/websockets/ws/releases">ws's releases</a>.</em></p>
<blockquote>
<h2>8.17.1</h2>
<h1>Bug fixes</h1>
<ul>
<li>Fixed a DoS vulnerability (<a href="https://redirect.github.com/websockets/ws/issues/2231">#2231</a>).</li>
</ul>
<p>A request with a number of headers exceeding the[<code>server.maxHeadersCount</code>][]
threshold could be used to crash a ws server.</p>
<pre lang="js"><code>const http = require('http');
const WebSocket = require('ws');
<p>const wss = new WebSocket.Server({ port: 0 }, function () {
const chars = &quot;!#$%&amp;'*+-.0123456789abcdefghijklmnopqrstuvwxyz^_`|~&quot;.split('');
const headers = {};
let count = 0;</p>
<p>for (let i = 0; i &lt; chars.length; i++) {
if (count === 2000) break;</p>
<pre><code>for (let j = 0; j &amp;lt; chars.length; j++) {
  const key = chars[i] + chars[j];
  headers[key] = 'x';

  if (++count === 2000) break;
}
</code></pre>
<p>}</p>
<p>headers.Connection = 'Upgrade';
headers.Upgrade = 'websocket';
headers['Sec-WebSocket-Key'] = 'dGhlIHNhbXBsZSBub25jZQ==';
headers['Sec-WebSocket-Version'] = '13';</p>
<p>const request = http.request({
headers: headers,
host: '127.0.0.1',
port: wss.address().port
});</p>
<p>request.end();
});
</code></pre></p>
<p>The vulnerability was reported by <a href="https://github.com/rrlapointe">Ryan LaPointe</a> in <a href="https://redirect.github.com/websockets/ws/issues/2230">websockets/ws#2230</a>.</p>
<p>In vulnerable versions of ws, the issue can be mitigated in the following ways:</p>
<ol>
<li>Reduce the maximum allowed length of the request headers using the
[<code>--max-http-header-size=size</code>][] and/or the [<code>maxHeaderSize</code>][] options so
that no more headers than the <code>server.maxHeadersCount</code> limit can be sent.</li>
</ol>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/websockets/ws/commit/3c56601092872f7d7566989f0e379271afd0e4a1"><code>3c56601</code></a> [dist] 8.17.1</li>
<li><a href="https://github.com/websockets/ws/commit/e55e5106f10fcbaac37cfa89759e4cc0d073a52c"><code>e55e510</code></a> [security] Fix crash when the Upgrade header cannot be read (<a href="https://redirect.github.com/websockets/ws/issues/2231">#2231</a>)</li>
<li><a href="https://github.com/websockets/ws/commit/6a00029edd924499f892aed8003cef1fa724cfe5"><code>6a00029</code></a> [test] Increase code coverage</li>
<li><a href="https://github.com/websockets/ws/commit/ddfe4a804d79e7788ab136290e609f91cf68423f"><code>ddfe4a8</code></a> [perf] Reduce the amount of <code>crypto.randomFillSync()</code> calls</li>
<li><a href="https://github.com/websockets/ws/commit/b73b11828d166e9692a9bffe9c01a7e93bab04a8"><code>b73b118</code></a> [dist] 8.17.0</li>
<li><a href="https://github.com/websockets/ws/commit/29694a5905fa703e86667928e6bacac397469471"><code>29694a5</code></a> [test] Use the <code>highWaterMark</code> variable</li>
<li><a href="https://github.com/websockets/ws/commit/934c9d6b938b93c045cb13e5f7c19c27a8dd925a"><code>934c9d6</code></a> [ci] Test on node 22</li>
<li><a href="https://github.com/websockets/ws/commit/1817bac06e1204bfb578b8b3f4bafd0fa09623d0"><code>1817bac</code></a> [ci] Do not test on node 21</li>
<li><a href="https://github.com/websockets/ws/commit/96c9b3deddf56cacb2d756aaa918071e03cdbc42"><code>96c9b3d</code></a> [major] Flip the default value of <code>allowSynchronousEvents</code> (<a href="https://redirect.github.com/websockets/ws/issues/2221">#2221</a>)</li>
<li><a href="https://github.com/websockets/ws/commit/e5f32c7e1e6d3d19cd4a1fdec84890e154db30c1"><code>e5f32c7</code></a> [fix] Emit at most one event per event loop iteration (<a href="https://redirect.github.com/websockets/ws/issues/2218">#2218</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/websockets/ws/compare/8.16.0...8.17.1">compare view</a></li>
</ul>
</details>
<br />

Updates `ethers` from 6.11.1 to 6.13.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ethers-io/ethers.js/releases">ethers's releases</a>.</em></p>
<blockquote>
<h2>ethers/v6.13.1 (2024-06-18 02:37)</h2>
<ul>
<li>Update ws package to address possible DoS vulnerability (<a href="https://github.com/ethers-io/ethers.js/commit/a4b1d1f43fca14f2e826e3c60e0d45f5b6ef3ec4">a4b1d1f</a>).</li>
</ul>
<h2>ethers/v6.13.0 (2024-06-04 01:38)</h2>
<ul>
<li>Added Options for BrowserProvider (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4707">#4707</a>; <a href="https://github.com/ethers-io/ethers.js/commit/33bb0bf30e1e6a699c24415a1edf0fa4ed28b6aa">33bb0bf</a>).</li>
<li>Fix Result deep toObject when a parent is an Array (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4681">#4681</a>; <a href="https://github.com/ethers-io/ethers.js/commit/d8cb84957078985f5449fa26c6fd8087dbd17aec">d8cb849</a>).</li>
<li>Added consistent timeout and cancel behaviour to FetchRequest (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4122">#4122</a>; <a href="https://github.com/ethers-io/ethers.js/commit/a12a7391fba39b5c114fa658590fae305dcedd17">a12a739</a>).</li>
</ul>
<h2>ethers/v6.12.2 (2024-05-30 17:24)</h2>
<ul>
<li>Copy EIP-4844 properties during estimateGas and call (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4728">#4728</a>; <a href="https://github.com/ethers-io/ethers.js/commit/cebe5eed91de0db5931b7847e76ee27cb2ce9219">cebe5ee</a>).</li>
<li>Use non-capturing regex for data to prevent memory exhaustion for long strings (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4741">#4741</a>; <a href="https://github.com/ethers-io/ethers.js/commit/5463aa03eacde45322a1e05693ce90e4d7abcaa7">5463aa0</a>).</li>
<li>Added Base endpointsto EtherscanProvider (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4729">#4729</a>; <a href="https://github.com/ethers-io/ethers.js/commit/7e1dc95ea2564c1eb0a9452b9a16002f3696765c">7e1dc95</a>).</li>
</ul>
<h2>ethers/v6.12.1 (2024-04-30 23:23)</h2>
<ul>
<li>Prevent bad Interface clone when using two different versions of v6 (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4689">#4689</a>; <a href="https://github.com/ethers-io/ethers.js/commit/4d2d90f5cea2eb2f9559e490a34aa1567c8c4c14">4d2d90f</a>).</li>
<li>Fixed typo in error message for invalid quorum weight (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4149">#4149</a>; <a href="https://github.com/ethers-io/ethers.js/commit/45b9b9c9322bf20feaf892d948bcfb8db8932877">45b9b9c</a>).</li>
<li>Added matic-amoy to EtherescanProvider (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4711">#4711</a>; <a href="https://github.com/ethers-io/ethers.js/commit/5c8d17a61825fe002bd45ee5b2239bfd8c8ae189">5c8d17a</a>).</li>
<li>Fix JsonRpcProvider ignoring pollingInterval in options (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4644">#4644</a>; <a href="https://github.com/ethers-io/ethers.js/commit/7b7be0d1ef637f073b28bce54f4ecdfb8c88d09c">7b7be0d</a>).</li>
</ul>
<h2>ethers/v6.12.0 (2024-04-17 02:09)</h2>
<ul>
<li>Added Linea Sepolia network and Infura endpoint (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4655">#4655</a>; <a href="https://github.com/ethers-io/ethers.js/commit/b4aaab8d39fe47f8a1a296fa442f0856f84faf03">b4aaab8</a>).</li>
<li>Do not send unsubscribe messages to destroyed Providers (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4678">#4678</a>; <a href="https://github.com/ethers-io/ethers.js/commit/c45935e29ca0dd1ecdf1277fa1107246041be580">c45935e</a>).</li>
<li>Get definitive network from InfuraProvider when using InfuraWebSocketProvider (<a href="https://github.com/ethers-io/ethers.js/commit/38e32d82145eb289e5179f9b6b11f4a9225a7022">38e32d8</a>).</li>
<li>Better error messages for transaction field mismatch (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4659">#4659</a>; <a href="https://github.com/ethers-io/ethers.js/commit/9230aa0b9a88b5241915a8d6afa8a522d35abd5d">9230aa0</a>).</li>
<li>Added prevRandao to block (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/3372">#3372</a>; <a href="https://github.com/ethers-io/ethers.js/commit/ec6a754f0c8647dae59c73b2589225cb200d83dd">ec6a754</a>).</li>
<li>Added Polygon Amoy testnet (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4645">#4645</a>; <a href="https://github.com/ethers-io/ethers.js/commit/1717abbf29a14a6f6b106e479fe9a5b1f8768dc4">1717abb</a>).</li>
<li>Added Chainstack provider (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/2741">#2741</a>; <a href="https://github.com/ethers-io/ethers.js/commit/014004d9402d7fd8c15553792cfb7a8a84ed327a">014004d</a>).</li>
<li>Added deep convertion to Result for toObject and toArray (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4681">#4681</a>; <a href="https://github.com/ethers-io/ethers.js/commit/03bfe2a4f7b29b15cd90127974b7fc1d8b03edf9">03bfe2a</a>).</li>
<li>Added EIP-4844 broadcast support (<a href="https://github.com/ethers-io/ethers.js/commit/92bad88261a5d8a538535a7d5528162fe5010527">92bad88</a>).</li>
<li>Fix ignored throttle parameters (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4663">#4663</a>; <a href="https://github.com/ethers-io/ethers.js/commit/12772e9498b70f8538838f30e16f3792ea90e173">12772e9</a>).</li>
</ul>
<h2>ethers/v6.12.0-beta.1 (2024-03-27 14:47)</h2>
<ul>
<li>Added EIP-4844 broadcast support.</li>
<li>Fix ignored throttle parameters (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4663">#4663</a>; <a href="https://github.com/ethers-io/ethers.js/commit/12772e9498b70f8538838f30e16f3792ea90e173">12772e9</a>).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ethers-io/ethers.js/blob/main/CHANGELOG.md">ethers's changelog</a>.</em></p>
<blockquote>
<h2>ethers/v6.13.1 (2024-06-18 02:09)</h2>
<ul>
<li>Update ws package to address possible DoS vulnerability (<a href="https://github.com/ethers-io/ethers.js/commit/a4b1d1f43fca14f2e826e3c60e0d45f5b6ef3ec4">a4b1d1f</a>).</li>
</ul>
<h2>ethers/v6.13.0 (2024-06-04 01:01)</h2>
<ul>
<li>Added Options for BrowserProvider (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4707">#4707</a>; <a href="https://github.com/ethers-io/ethers.js/commit/33bb0bf30e1e6a699c24415a1edf0fa4ed28b6aa">33bb0bf</a>).</li>
<li>Fix Result deep toObject when a parent is an Array (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4681">#4681</a>; <a href="https://github.com/ethers-io/ethers.js/commit/d8cb84957078985f5449fa26c6fd8087dbd17aec">d8cb849</a>).</li>
<li>Added consistent timeout and cancel behaviour to FetchRequest (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4122">#4122</a>; <a href="https://github.com/ethers-io/ethers.js/commit/a12a7391fba39b5c114fa658590fae305dcedd17">a12a739</a>).</li>
</ul>
<h2>ethers/v6.12.2 (2024-05-30 17:24)</h2>
<ul>
<li>Copy EIP-4844 properties during estimateGas and call (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4728">#4728</a>; <a href="https://github.com/ethers-io/ethers.js/commit/cebe5eed91de0db5931b7847e76ee27cb2ce9219">cebe5ee</a>).</li>
<li>Use non-capturing regex for data to prevent memory exhaustion for long strings (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4741">#4741</a>; <a href="https://github.com/ethers-io/ethers.js/commit/5463aa03eacde45322a1e05693ce90e4d7abcaa7">5463aa0</a>).</li>
<li>Added Base endpointsto EtherscanProvider (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4729">#4729</a>; <a href="https://github.com/ethers-io/ethers.js/commit/7e1dc95ea2564c1eb0a9452b9a16002f3696765c">7e1dc95</a>).</li>
</ul>
<h2>ethers/v6.12.1 (2024-04-30 22:46)</h2>
<ul>
<li>Prevent bad Interface clone when using two different versions of v6 (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4689">#4689</a>; <a href="https://github.com/ethers-io/ethers.js/commit/4d2d90f5cea2eb2f9559e490a34aa1567c8c4c14">4d2d90f</a>).</li>
<li>Fixed typo in error message for invalid quorum weight (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4149">#4149</a>; <a href="https://github.com/ethers-io/ethers.js/commit/45b9b9c9322bf20feaf892d948bcfb8db8932877">45b9b9c</a>).</li>
<li>Added matic-amoy to EtherescanProvider (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4711">#4711</a>; <a href="https://github.com/ethers-io/ethers.js/commit/5c8d17a61825fe002bd45ee5b2239bfd8c8ae189">5c8d17a</a>).</li>
<li>Fix JsonRpcProvider ignoring pollingInterval in options (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4644">#4644</a>; <a href="https://github.com/ethers-io/ethers.js/commit/7b7be0d1ef637f073b28bce54f4ecdfb8c88d09c">7b7be0d</a>).</li>
</ul>
<h2>ethers/v6.12.0 (2024-04-17 01:09)</h2>
<ul>
<li>Added Linea Sepolia network and Infura endpoint (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4655">#4655</a>; <a href="https://github.com/ethers-io/ethers.js/commit/b4aaab8d39fe47f8a1a296fa442f0856f84faf03">b4aaab8</a>).</li>
<li>Do not send unsubscribe messages to destroyed Providers (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4678">#4678</a>; <a href="https://github.com/ethers-io/ethers.js/commit/c45935e29ca0dd1ecdf1277fa1107246041be580">c45935e</a>).</li>
<li>Get definitive network from InfuraProvider when using InfuraWebSocketProvider (<a href="https://github.com/ethers-io/ethers.js/commit/38e32d82145eb289e5179f9b6b11f4a9225a7022">38e32d8</a>).</li>
<li>Better error messages for transaction field mismatch (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4659">#4659</a>; <a href="https://github.com/ethers-io/ethers.js/commit/9230aa0b9a88b5241915a8d6afa8a522d35abd5d">9230aa0</a>).</li>
<li>Added prevRandao to block (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/3372">#3372</a>; <a href="https://github.com/ethers-io/ethers.js/commit/ec6a754f0c8647dae59c73b2589225cb200d83dd">ec6a754</a>).</li>
<li>Added Polygon Amoy testnet (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4645">#4645</a>; <a href="https://github.com/ethers-io/ethers.js/commit/1717abbf29a14a6f6b106e479fe9a5b1f8768dc4">1717abb</a>).</li>
<li>Added Chainstack provider (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/2741">#2741</a>; <a href="https://github.com/ethers-io/ethers.js/commit/014004d9402d7fd8c15553792cfb7a8a84ed327a">014004d</a>).</li>
<li>Added deep convertion to Result for toObject and toArray (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4681">#4681</a>; <a href="https://github.com/ethers-io/ethers.js/commit/03bfe2a4f7b29b15cd90127974b7fc1d8b03edf9">03bfe2a</a>).</li>
<li>Added EIP-4844 broadcast support (<a href="https://github.com/ethers-io/ethers.js/commit/92bad88261a5d8a538535a7d5528162fe5010527">92bad88</a>).</li>
<li>Fix ignored throttle parameters (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4663">#4663</a>; <a href="https://github.com/ethers-io/ethers.js/commit/12772e9498b70f8538838f30e16f3792ea90e173">12772e9</a>).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ethers-io/ethers.js/commit/a4b1d1f43fca14f2e826e3c60e0d45f5b6ef3ec4"><code>a4b1d1f</code></a> Update ws package to address possible DoS vulnerability.</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/16b8e18a42d91a174637a493ea9732521a53251f"><code>16b8e18</code></a> docs: fixed paragraph leaking into code in migration docs</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/92761872198cf6c9334570da3d110bca2bafa641"><code>9276187</code></a> admin: updated dist files</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/90c196a749a1eb0a8fae336301a490e30d8e0166"><code>90c196a</code></a> Fix missing return for Result proxy (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4681">#4681</a>).</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/5b8781d2bbe9adec908d5c57a95be3fbfe382ac1"><code>5b8781d</code></a> admin: updated dist files</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/e97ca3b8d494b86839956ca353c2526101b9cbb4"><code>e97ca3b</code></a> Merge branch 'wip-6.13'</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/c2d5346a0558ed49f6db094ef81bd38a8303caa1"><code>c2d5346</code></a> tests: added gasless testcase for RicMoo-controlled domain</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/0f1434b85ef5b53c1167730abad3ccc6be02e42e"><code>0f1434b</code></a> admin: remove deprecated mumbai network from tests.</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/33bb0bf30e1e6a699c24415a1edf0fa4ed28b6aa"><code>33bb0bf</code></a> Added Options for BrowserProvider (<a href="https://redirect.github.com/ethers-io/ethers.js/issues/4707">#4707</a>).</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/2d2572a498cc1d9b6653b14823c279d873838f32"><code>2d2572a</code></a> admin: update dist files</li>
<li>Additional commits viewable in <a href="https://github.com/ethers-io/ethers.js/compare/v6.11.1...v6.13.1">compare view</a></li>
</ul>
</details>
<br />

Updates `braces` from 3.0.2 to 3.0.3
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/micromatch/braces/commit/74b2db2938fad48a2ea54a9c8bf27a37a62c350d"><code>74b2db2</code></a> 3.0.3</li>
<li><a href="https://github.com/micromatch/braces/commit/88f1429a0f47e1dd3813de35211fc97ffda27f9e"><code>88f1429</code></a> update eslint. lint, fix unit tests.</li>
<li><a href="https://github.com/micromatch/braces/commit/415d660c3002d1ab7e63dbf490c9851da80596ff"><code>415d660</code></a> Snyk js braces 6838727 (<a href="https://redirect.github.com/micromatch/braces/issues/40">#40</a>)</li>
<li><a href="https://github.com/micromatch/braces/commit/190510f79db1adf21d92798b0bb6fccc1f72c9d6"><code>190510f</code></a> fix tests, skip 1 test in test/braces.expand</li>
<li><a href="https://github.com/micromatch/braces/commit/716eb9f12d820b145a831ad678618731927e8856"><code>716eb9f</code></a> readme bump</li>
<li><a href="https://github.com/micromatch/braces/commit/a5851e57f45c3431a94d83fc565754bc10f5bbc3"><code>a5851e5</code></a> Merge pull request <a href="https://redirect.github.com/micromatch/braces/issues/37">#37</a> from coderaiser/fix/vulnerability</li>
<li><a href="https://github.com/micromatch/braces/commit/2092bd1fb108d2c59bd62e243b70ad98db961538"><code>2092bd1</code></a> feature: braces: add maxSymbols (<a href="https://github.com/micromatch/braces/issues/">https://github.com/micromatch/braces/issues/</a>...</li>
<li><a href="https://github.com/micromatch/braces/commit/9f5b4cf47329351bcb64287223ffb6ecc9a5e6d3"><code>9f5b4cf</code></a> fix: vulnerability (<a href="https://security.snyk.io/vuln/SNYK-JS-BRACES-6838727">https://security.snyk.io/vuln/SNYK-JS-BRACES-6838727</a>)</li>
<li><a href="https://github.com/micromatch/braces/commit/98414f9f1fabe021736e26836d8306d5de747e0d"><code>98414f9</code></a> remove funding file</li>
<li><a href="https://github.com/micromatch/braces/commit/665ab5d561c017a38ba7aafd92cc6655b91d8c14"><code>665ab5d</code></a> update keepEscaping doc (<a href="https://redirect.github.com/micromatch/braces/issues/27">#27</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/micromatch/braces/compare/3.0.2...3.0.3">compare view</a></li>
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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore <dependency name> major version` will close this group update PR and stop Dependabot creating any more for the specific dependency's major version (unless you unignore this specific dependency's major version or upgrade to it yourself)
- `@dependabot ignore <dependency name> minor version` will close this group update PR and stop Dependabot creating any more for the specific dependency's minor version (unless you unignore this specific dependency's minor version or upgrade to it yourself)
- `@dependabot ignore <dependency name>` will close this group update PR and stop Dependabot creating any more for the specific dependency (unless you unignore this specific dependency or upgrade to it yourself)
- `@dependabot unignore <dependency name>` will remove all of the ignore conditions of the specified dependency
- `@dependabot unignore <dependency name> <ignore condition>` will remove the ignore condition of the specified dependency and ignore conditions
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/firefly-tokens-erc20-erc721/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-18 23:20:20 +0000 UTC
    </div>
</div>

