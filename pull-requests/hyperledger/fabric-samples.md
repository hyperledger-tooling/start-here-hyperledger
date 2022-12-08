---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/882" class=".btn">#882</a>
            </td>
            <td>
                <b>
                    Update org1-peer2.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixing TLS issues while using org1-peer-gateway-svc.${DOMAIN}. This would be needed so there are no TLS issues when sending requests.

Signed-off-by: Deepak Singh <91736795+blockguardian@users.noreply.github.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-07 18:40:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/880" class=".btn">#880</a>
            </td>
            <td>
                <b>
                    Bump qs and express in /asset-transfer-basic/rest-api-typescript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [qs](https://github.com/ljharb/qs) to 6.11.0 and updates ancestor dependencies [qs](https://github.com/ljharb/qs), [qs](https://github.com/ljharb/qs) and [express](https://github.com/expressjs/express). These dependencies need to be updated together.

Updates `qs` from 6.10.2 to 6.11.0
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ljharb/qs/blob/main/CHANGELOG.md">qs's changelog</a>.</em></p>
<blockquote>
<h2><strong>6.11.0</strong></h2>
<ul>
<li>[New] [Fix] <code>stringify</code>: revert 0e903c0; add <code>commaRoundTrip</code> option (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/442">#442</a>)</li>
<li>[readme] fix version badge</li>
</ul>
<h2><strong>6.10.5</strong></h2>
<ul>
<li>[Fix] <code>stringify</code>: with <code>arrayFormat: comma</code>, properly include an explicit <code>[]</code> on a single-item array (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/434">#434</a>)</li>
</ul>
<h2><strong>6.10.4</strong></h2>
<ul>
<li>[Fix] <code>stringify</code>: with <code>arrayFormat: comma</code>, include an explicit <code>[]</code> on a single-item array (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/441">#441</a>)</li>
<li>[meta] use <code>npmignore</code> to autogenerate an npmignore file</li>
<li>[Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>aud</code>, <code>has-symbol</code>, <code>object-inspect</code>, <code>tape</code></li>
</ul>
<h2><strong>6.10.3</strong></h2>
<ul>
<li>[Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/428">#428</a>)</li>
<li>[Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/427">#427</a>)</li>
<li>[actions] reuse common workflows</li>
<li>[Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>object-inspect</code>, <code>tape</code></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ljharb/qs/commit/56763c12ec4fbf723333cbb32371cbd386c33cbb"><code>56763c1</code></a> v6.11.0</li>
<li><a href="https://github.com/ljharb/qs/commit/ddd3e293b801df7a06cb7f2746462a6ca1dd3fb2"><code>ddd3e29</code></a> [readme] fix version badge</li>
<li><a href="https://github.com/ljharb/qs/commit/c31347299f34afca90e8b5ff793eb4d0f77cfa56"><code>c313472</code></a> [New] [Fix] <code>stringify</code>: revert 0e903c0; add <code>commaRoundTrip</code> option</li>
<li><a href="https://github.com/ljharb/qs/commit/95bc0185e157d400da4f43f1fcf1c7f008fd847e"><code>95bc018</code></a> v6.10.5</li>
<li><a href="https://github.com/ljharb/qs/commit/0e903c0a9092618756b0962f1b80655ac0da436a"><code>0e903c0</code></a> [Fix] <code>stringify</code>: with <code>arrayFormat: comma</code>, properly include an explicit `[...</li>
<li><a href="https://github.com/ljharb/qs/commit/ba9703c0340dfdeb73cb4387d6ab32c37768aa5b"><code>ba9703c</code></a> v6.10.4</li>
<li><a href="https://github.com/ljharb/qs/commit/4e440195c7647f21c20bb76340774cb3a0cb6eac"><code>4e44019</code></a> [Fix] <code>stringify</code>: with <code>arrayFormat: comma</code>, include an explicit <code>[]</code> on a s...</li>
<li><a href="https://github.com/ljharb/qs/commit/113b990ed23ae8d6f670eb879e16ed105cd9081b"><code>113b990</code></a> [Dev Deps] update <code>object-inspect</code></li>
<li><a href="https://github.com/ljharb/qs/commit/c77f38f7174b9f10e8937e0f601fa1e6f0373b33"><code>c77f38f</code></a> [Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>aud</code>, <code>has-symbol</code>, <code>tape</code></li>
<li><a href="https://github.com/ljharb/qs/commit/2cf45b2dcd31a6d5c7fc16f33c7148fade0eef1e"><code>2cf45b2</code></a> [meta] use <code>npmignore</code> to autogenerate an npmignore file</li>
<li>Additional commits viewable in <a href="https://github.com/ljharb/qs/compare/v6.10.2...v6.11.0">compare view</a></li>
</ul>
</details>
<br />

Updates `qs` from 6.10.1 to 6.11.0
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ljharb/qs/blob/main/CHANGELOG.md">qs's changelog</a>.</em></p>
<blockquote>
<h2><strong>6.11.0</strong></h2>
<ul>
<li>[New] [Fix] <code>stringify</code>: revert 0e903c0; add <code>commaRoundTrip</code> option (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/442">#442</a>)</li>
<li>[readme] fix version badge</li>
</ul>
<h2><strong>6.10.5</strong></h2>
<ul>
<li>[Fix] <code>stringify</code>: with <code>arrayFormat: comma</code>, properly include an explicit <code>[]</code> on a single-item array (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/434">#434</a>)</li>
</ul>
<h2><strong>6.10.4</strong></h2>
<ul>
<li>[Fix] <code>stringify</code>: with <code>arrayFormat: comma</code>, include an explicit <code>[]</code> on a single-item array (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/441">#441</a>)</li>
<li>[meta] use <code>npmignore</code> to autogenerate an npmignore file</li>
<li>[Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>aud</code>, <code>has-symbol</code>, <code>object-inspect</code>, <code>tape</code></li>
</ul>
<h2><strong>6.10.3</strong></h2>
<ul>
<li>[Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/428">#428</a>)</li>
<li>[Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/427">#427</a>)</li>
<li>[actions] reuse common workflows</li>
<li>[Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>object-inspect</code>, <code>tape</code></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ljharb/qs/commit/56763c12ec4fbf723333cbb32371cbd386c33cbb"><code>56763c1</code></a> v6.11.0</li>
<li><a href="https://github.com/ljharb/qs/commit/ddd3e293b801df7a06cb7f2746462a6ca1dd3fb2"><code>ddd3e29</code></a> [readme] fix version badge</li>
<li><a href="https://github.com/ljharb/qs/commit/c31347299f34afca90e8b5ff793eb4d0f77cfa56"><code>c313472</code></a> [New] [Fix] <code>stringify</code>: revert 0e903c0; add <code>commaRoundTrip</code> option</li>
<li><a href="https://github.com/ljharb/qs/commit/95bc0185e157d400da4f43f1fcf1c7f008fd847e"><code>95bc018</code></a> v6.10.5</li>
<li><a href="https://github.com/ljharb/qs/commit/0e903c0a9092618756b0962f1b80655ac0da436a"><code>0e903c0</code></a> [Fix] <code>stringify</code>: with <code>arrayFormat: comma</code>, properly include an explicit `[...</li>
<li><a href="https://github.com/ljharb/qs/commit/ba9703c0340dfdeb73cb4387d6ab32c37768aa5b"><code>ba9703c</code></a> v6.10.4</li>
<li><a href="https://github.com/ljharb/qs/commit/4e440195c7647f21c20bb76340774cb3a0cb6eac"><code>4e44019</code></a> [Fix] <code>stringify</code>: with <code>arrayFormat: comma</code>, include an explicit <code>[]</code> on a s...</li>
<li><a href="https://github.com/ljharb/qs/commit/113b990ed23ae8d6f670eb879e16ed105cd9081b"><code>113b990</code></a> [Dev Deps] update <code>object-inspect</code></li>
<li><a href="https://github.com/ljharb/qs/commit/c77f38f7174b9f10e8937e0f601fa1e6f0373b33"><code>c77f38f</code></a> [Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>aud</code>, <code>has-symbol</code>, <code>tape</code></li>
<li><a href="https://github.com/ljharb/qs/commit/2cf45b2dcd31a6d5c7fc16f33c7148fade0eef1e"><code>2cf45b2</code></a> [meta] use <code>npmignore</code> to autogenerate an npmignore file</li>
<li>Additional commits viewable in <a href="https://github.com/ljharb/qs/compare/v6.10.2...v6.11.0">compare view</a></li>
</ul>
</details>
<br />

Updates `express` from 4.17.1 to 4.18.2
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-06 16:39:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/878" class=".btn">#878</a>
            </td>
            <td>
                <b>
                    Add in examples and notes on using PurgePrivateData
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Update the configtx.yaml to enable the 2.5 capabillity
- Added purge into the chancode
- Added pruge into the application client code.

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-05 11:00:47 +0000 UTC
    </div>
</div>

