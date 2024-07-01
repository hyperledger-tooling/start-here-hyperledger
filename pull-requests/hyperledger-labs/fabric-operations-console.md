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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/766" class=".btn">#766</a>
            </td>
            <td>
                <b>
                    renamed the misc cases file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                renamed the misc cases file as file name was having space in word and failing in firefox

#### Type of change
- Test update

#### Description
renamed the misc cases file as file name was having space in word

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-01 05:11:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/765" class=".btn">#765</a>
            </td>
            <td>
                <b>
                    Bump ws and cypress-watch-and-reload in /packages/apollo/test/cypress
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [ws](https://github.com/websockets/ws) to 8.17.1 and updates ancestor dependency [cypress-watch-and-reload](https://github.com/bahmutov/cypress-watch-and-reload). These dependencies need to be updated together.

Updates `ws` from 8.14.2 to 8.17.1
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
<li>Additional commits viewable in <a href="https://github.com/websockets/ws/compare/8.14.2...8.17.1">compare view</a></li>
</ul>
</details>
<br />

Updates `cypress-watch-and-reload` from 1.10.9 to 1.10.15
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/bahmutov/cypress-watch-and-reload/releases">cypress-watch-and-reload's releases</a>.</em></p>
<blockquote>
<h2>v1.10.15</h2>
<h2><a href="https://github.com/bahmutov/cypress-watch-and-reload/compare/v1.10.14...v1.10.15">1.10.15</a> (2024-06-16)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>deps:</strong> update dependency ws to v8.17.1 (<a href="https://github.com/bahmutov/cypress-watch-and-reload/commit/e99941b15f6f5e614db39fad082c31e78d61030c">e99941b</a>)</li>
</ul>
<h2>v1.10.14</h2>
<h2><a href="https://github.com/bahmutov/cypress-watch-and-reload/compare/v1.10.13...v1.10.14">1.10.14</a> (2024-04-28)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>deps:</strong> update dependency ws to v8.17.0 (<a href="https://github.com/bahmutov/cypress-watch-and-reload/commit/a0d8888bf4c5960ce1384a904c4b01a659f51239">a0d8888</a>)</li>
</ul>
<h2>v1.10.13</h2>
<h2><a href="https://github.com/bahmutov/cypress-watch-and-reload/compare/v1.10.12...v1.10.13">1.10.13</a> (2024-02-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>deps:</strong> update dependency chokidar to v3.6.0 (<a href="https://github.com/bahmutov/cypress-watch-and-reload/commit/6ecdc1c848ec38ab0886956aec9badf19fb37259">6ecdc1c</a>)</li>
</ul>
<h2>v1.10.12</h2>
<h2><a href="https://github.com/bahmutov/cypress-watch-and-reload/compare/v1.10.11...v1.10.12">1.10.12</a> (2023-12-26)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>deps:</strong> update dependency ws to v8.16.0 (<a href="https://github.com/bahmutov/cypress-watch-and-reload/commit/a89be7e87570089c8d2efe620686bb2262140c38">a89be7e</a>)</li>
</ul>
<h2>v1.10.11</h2>
<h2><a href="https://github.com/bahmutov/cypress-watch-and-reload/compare/v1.10.10...v1.10.11">1.10.11</a> (2023-12-13)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>deps:</strong> update dependency ws to v8.15.1 (<a href="https://github.com/bahmutov/cypress-watch-and-reload/commit/2b4cba3c26cca99df17b743bc83af5c74aac9046">2b4cba3</a>)</li>
</ul>
<h2>v1.10.10</h2>
<h2><a href="https://github.com/bahmutov/cypress-watch-and-reload/compare/v1.10.9...v1.10.10">1.10.10</a> (2023-12-09)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>deps:</strong> update dependency ws to v8.15.0 (<a href="https://github.com/bahmutov/cypress-watch-and-reload/commit/91c5bc330323512b4039b16f1b56602c01da52d3">91c5bc3</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/bahmutov/cypress-watch-and-reload/commit/e99941b15f6f5e614db39fad082c31e78d61030c"><code>e99941b</code></a> fix(deps): update dependency ws to v8.17.1</li>
<li><a href="https://github.com/bahmutov/cypress-watch-and-reload/commit/a0d8888bf4c5960ce1384a904c4b01a659f51239"><code>a0d8888</code></a> fix(deps): update dependency ws to v8.17.0</li>
<li><a href="https://github.com/bahmutov/cypress-watch-and-reload/commit/6ecdc1c848ec38ab0886956aec9badf19fb37259"><code>6ecdc1c</code></a> fix(deps): update dependency chokidar to v3.6.0</li>
<li><a href="https://github.com/bahmutov/cypress-watch-and-reload/commit/a89be7e87570089c8d2efe620686bb2262140c38"><code>a89be7e</code></a> fix(deps): update dependency ws to v8.16.0</li>
<li><a href="https://github.com/bahmutov/cypress-watch-and-reload/commit/2b4cba3c26cca99df17b743bc83af5c74aac9046"><code>2b4cba3</code></a> fix(deps): update dependency ws to v8.15.1</li>
<li><a href="https://github.com/bahmutov/cypress-watch-and-reload/commit/91c5bc330323512b4039b16f1b56602c01da52d3"><code>91c5bc3</code></a> fix(deps): update dependency ws to v8.15.0</li>
<li>See full diff in <a href="https://github.com/bahmutov/cypress-watch-and-reload/compare/v1.10.9...v1.10.15">compare view</a></li>
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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-operations-console/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-28 12:35:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/764" class=".btn">#764</a>
            </td>
            <td>
                <b>
                    UI automation test update as per carbon library update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Test update

#### Description
UI automation test update as per carbon library update
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-28 12:09:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/763" class=".btn">#763</a>
            </td>
            <td>
                <b>
                    Detect secret
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
<!--- Describe your changes in detail, including motivation. -->


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-27 06:34:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/761" class=".btn">#761</a>
            </td>
            <td>
                <b>
                    updated tab ui as per previous console
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvement (improvement to code, performance, etc)

#### Description
<!--- Describe your changes in detail, including motivation. -->
- Update tab ui as per previous console 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-26 13:21:55 +0000 UTC
    </div>
</div>

