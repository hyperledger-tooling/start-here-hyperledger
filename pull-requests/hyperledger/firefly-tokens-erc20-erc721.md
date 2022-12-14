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
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/99" class=".btn">#99</a>
            </td>
            <td>
                <b>
                    Bump qs, body-parser and express in /samples/solidity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [qs](https://github.com/ljharb/qs), [body-parser](https://github.com/expressjs/body-parser) and [express](https://github.com/expressjs/express). These dependencies needed to be updated together.
Updates `qs` from 6.5.2 to 6.10.3
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ljharb/qs/blob/main/CHANGELOG.md">qs's changelog</a>.</em></p>
<blockquote>
<h2><strong>6.10.3</strong></h2>
<ul>
<li>[Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/428">#428</a>)</li>
<li>[Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/427">#427</a>)</li>
<li>[actions] reuse common workflows</li>
<li>[Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>object-inspect</code>, <code>tape</code></li>
</ul>
<h2><strong>6.10.2</strong></h2>
<ul>
<li>[Fix] <code>stringify</code>: actually fix cyclic references (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/426">#426</a>)</li>
<li>[Fix] <code>stringify</code>: avoid encoding arrayformat comma when <code>encodeValuesOnly = true</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/424">#424</a>)</li>
<li>[readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li>[Docs] add note and links for coercing primitive values (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/408">#408</a>)</li>
<li>[actions] update codecov uploader</li>
<li>[actions] update workflows</li>
<li>[Tests] clean up stringify tests slightly</li>
<li>[Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>aud</code>, <code>object-inspect</code>, <code>safe-publish-latest</code>, <code>tape</code></li>
</ul>
<h2><strong>6.10.1</strong></h2>
<ul>
<li>[Fix] <code>stringify</code>: avoid exception on repeated object values (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/402">#402</a>)</li>
</ul>
<h2><strong>6.10.0</strong></h2>
<ul>
<li>[New] <code>stringify</code>: throw on cycles, instead of an infinite loop (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/395">#395</a>, <a href="https://github-redirect.dependabot.com/ljharb/qs/issues/394">#394</a>, <a href="https://github-redirect.dependabot.com/ljharb/qs/issues/393">#393</a>)</li>
<li>[New] <code>parse</code>: add <code>allowSparse</code> option for collapsing arrays with missing indices (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/312">#312</a>)</li>
<li>[meta] fix README.md (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/399">#399</a>)</li>
<li>[meta] only run <code>npm run dist</code> in publish, not install</li>
<li>[Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>aud</code>, <code>has-symbols</code>, <code>tape</code></li>
<li>[Tests] fix tests on node v0.6</li>
<li>[Tests] use <code>ljharb/actions/node/install</code> instead of <code>ljharb/actions/node/run</code></li>
<li>[Tests] Revert &quot;[meta] ignore eclint transitive audit warning&quot;</li>
</ul>
<h2><strong>6.9.7</strong></h2>
<ul>
<li>[Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/428">#428</a>)</li>
<li>[Fix] <code>stringify</code>: avoid encoding arrayformat comma when <code>encodeValuesOnly = true</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/424">#424</a>)</li>
<li>[Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/427">#427</a>)</li>
<li>[readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li>[Docs] add note and links for coercing primitive values (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/408">#408</a>)</li>
<li>[Tests] clean up stringify tests slightly</li>
<li>[meta] fix README.md (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/399">#399</a>)</li>
<li>Revert &quot;[meta] ignore eclint transitive audit warning&quot;</li>
<li>[actions] backport actions from main</li>
<li>[Dev Deps] backport updates from main</li>
</ul>
<h2><strong>6.9.6</strong></h2>
<ul>
<li>[Fix] restore <code>dist</code> dir; mistakenly removed in d4f6c32</li>
</ul>
<h2><strong>6.9.5</strong></h2>
<ul>
<li>[Fix] <code>stringify</code>: do not encode parens for RFC1738</li>
<li>[Fix] <code>stringify</code>: fix arrayFormat comma with empty array/objects (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/350">#350</a>)</li>
<li>[Refactor] <code>format</code>: remove <code>util.assign</code> call</li>
<li>[meta] add &quot;Allow Edits&quot; workflow; update rebase workflow</li>
<li>[actions] switch Automatic Rebase workflow to <code>pull_request_target</code> event</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ljharb/qs/commit/f92ddb56089ae2c74f5ca7b0447fef3a97e8c9bc"><code>f92ddb5</code></a> v6.10.3</li>
<li><a href="https://github.com/ljharb/qs/commit/d9e95298c88ef52d1ca3b3b5d227f02420e02a01"><code>d9e9529</code></a> [Dev Deps] update <code>eslint</code></li>
<li><a href="https://github.com/ljharb/qs/commit/8b4cc14cda94a5c89341b77e5fe435ec6c41be2d"><code>8b4cc14</code></a> [Fix] <code>parse</code>: ignore <code>__proto__</code> keys</li>
<li><a href="https://github.com/ljharb/qs/commit/ad63d36ce18cd2c315899ac1e8193de22be08cd8"><code>ad63d36</code></a> [actions] reuse common workflows</li>
<li><a href="https://github.com/ljharb/qs/commit/c028385f6543e3148f243e2768e487c63b7e60b7"><code>c028385</code></a> [Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>object-inspect</code>, <code>tape</code></li>
<li><a href="https://github.com/ljharb/qs/commit/0a1d3e806e6c7d9d640d46df7b1d27e6e44125f8"><code>0a1d3e8</code></a> [Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code></li>
<li><a href="https://github.com/ljharb/qs/commit/408ff95f1ab94ea73027bc8a7443afb62d41a72d"><code>408ff95</code></a> v6.10.2</li>
<li><a href="https://github.com/ljharb/qs/commit/3cea04d889db3953e408554012f0ff44571eeb99"><code>3cea04d</code></a> [Dev Deps] update <code>@ljharb/eslint-config</code></li>
<li><a href="https://github.com/ljharb/qs/commit/28fba8fd928ee14c758c7f55cbce9d8730443dd4"><code>28fba8f</code></a> [Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>tape</code></li>
<li><a href="https://github.com/ljharb/qs/commit/9aee773432b80bd50441f7ac1b64a86a7e00ccca"><code>9aee773</code></a> [Fix] <code>stringify</code>: actually fix cyclic references</li>
<li>Additional commits viewable in <a href="https://github.com/ljharb/qs/compare/v6.5.2...v6.10.3">compare view</a></li>
</ul>
</details>
<br />

Updates `body-parser` from 1.19.0 to 1.20.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/body-parser/releases">body-parser's releases</a>.</em></p>
<blockquote>
<h2>1.20.0</h2>
<ul>
<li>Fix error message for json parse whitespace in <code>strict</code></li>
<li>Fix internal error when inflated body exceeds limit</li>
<li>Prevent loss of async hooks context</li>
<li>Prevent hanging when request already read</li>
<li>deps: depd@2.0.0
<ul>
<li>Replace internal <code>eval</code> usage with <code>Function</code> constructor</li>
<li>Use instance methods on <code>process</code> to check for listeners</li>
</ul>
</li>
<li>deps: http-errors@2.0.0
<ul>
<li>deps: depd@2.0.0</li>
<li>deps: statuses@2.0.1</li>
</ul>
</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: qs@6.10.3</li>
<li>deps: raw-body@2.5.1
<ul>
<li>deps: http-errors@2.0.0</li>
</ul>
</li>
</ul>
<h2>1.19.2</h2>
<ul>
<li>deps: bytes@3.1.2</li>
<li>deps: qs@6.9.7
<ul>
<li>Fix handling of <code>__proto__</code> keys</li>
</ul>
</li>
<li>deps: raw-body@2.4.3
<ul>
<li>deps: bytes@3.1.2</li>
</ul>
</li>
</ul>
<h2>1.19.1</h2>
<ul>
<li>deps: bytes@3.1.1</li>
<li>deps: http-errors@1.8.1
<ul>
<li>deps: inherits@2.0.4</li>
<li>deps: toidentifier@1.0.1</li>
<li>deps: setprototypeof@1.2.0</li>
</ul>
</li>
<li>deps: qs@6.9.6</li>
<li>deps: raw-body@2.4.2
<ul>
<li>deps: bytes@3.1.1</li>
<li>deps: http-errors@1.8.1</li>
</ul>
</li>
<li>deps: safe-buffer@5.2.1</li>
<li>deps: type-is@~1.6.18</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/body-parser/blob/master/HISTORY.md">body-parser's changelog</a>.</em></p>
<blockquote>
<h1>1.20.0 / 2022-04-02</h1>
<ul>
<li>Fix error message for json parse whitespace in <code>strict</code></li>
<li>Fix internal error when inflated body exceeds limit</li>
<li>Prevent loss of async hooks context</li>
<li>Prevent hanging when request already read</li>
<li>deps: depd@2.0.0
<ul>
<li>Replace internal <code>eval</code> usage with <code>Function</code> constructor</li>
<li>Use instance methods on <code>process</code> to check for listeners</li>
</ul>
</li>
<li>deps: http-errors@2.0.0
<ul>
<li>deps: depd@2.0.0</li>
<li>deps: statuses@2.0.1</li>
</ul>
</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: qs@6.10.3</li>
<li>deps: raw-body@2.5.1
<ul>
<li>deps: http-errors@2.0.0</li>
</ul>
</li>
</ul>
<h1>1.19.2 / 2022-02-15</h1>
<ul>
<li>deps: bytes@3.1.2</li>
<li>deps: qs@6.9.7
<ul>
<li>Fix handling of <code>__proto__</code> keys</li>
</ul>
</li>
<li>deps: raw-body@2.4.3
<ul>
<li>deps: bytes@3.1.2</li>
</ul>
</li>
</ul>
<h1>1.19.1 / 2021-12-10</h1>
<ul>
<li>deps: bytes@3.1.1</li>
<li>deps: http-errors@1.8.1
<ul>
<li>deps: inherits@2.0.4</li>
<li>deps: toidentifier@1.0.1</li>
<li>deps: setprototypeof@1.2.0</li>
</ul>
</li>
<li>deps: qs@6.9.6</li>
<li>deps: raw-body@2.4.2
<ul>
<li>deps: bytes@3.1.1</li>
<li>deps: http-errors@1.8.1</li>
</ul>
</li>
<li>deps: safe-buffer@5.2.1</li>
<li>deps: type-is@~1.6.18</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/expressjs/body-parser/commit/1f6f58e1f8dc222f2b6cfc7eb3a3bf5145ff2b56"><code>1f6f58e</code></a> 1.20.0</li>
<li><a href="https://github.com/expressjs/body-parser/commit/7861a0055df9f3171732adf99fb2814dcf6a36e2"><code>7861a00</code></a> docs: update CI badge link</li>
<li><a href="https://github.com/expressjs/body-parser/commit/601a076ddc66dc0b2cf909df14120b3adbaea91a"><code>601a076</code></a> docs: add security policy</li>
<li><a href="https://github.com/expressjs/body-parser/commit/77bcc0e44dd9be1b0a60b647fd23faac9b72c8be"><code>77bcc0e</code></a> deps: qs@6.10.3</li>
<li><a href="https://github.com/expressjs/body-parser/commit/eac5f22952ce8e6ec33315a3a16226b102591764"><code>eac5f22</code></a> build: Node.js@17.8</li>
<li><a href="https://github.com/expressjs/body-parser/commit/86115397674d19449473f74206e4b168a51e245e"><code>8611539</code></a> build: mocha@9.2.2</li>
<li><a href="https://github.com/expressjs/body-parser/commit/2a2f47199b443c56b6ebb74cac7acdeb63fac61f"><code>2a2f471</code></a> Fix internal error when inflated body exceeds limit</li>
<li><a href="https://github.com/expressjs/body-parser/commit/9db582d2af35936f0347572163a17aeaef290aaf"><code>9db582d</code></a> Fix error message for json parse whitespace in strict</li>
<li><a href="https://github.com/expressjs/body-parser/commit/bd702d2f007332dedcd4a1db0a7f21843ed537d7"><code>bd702d2</code></a> lint: remove deprecated String.prototype.substr</li>
<li><a href="https://github.com/expressjs/body-parser/commit/96df60f9d0d60c88cce33cd79c513e81d11c5162"><code>96df60f</code></a> deps: depd@2.0.0</li>
<li>Additional commits viewable in <a href="https://github.com/expressjs/body-parser/compare/1.19.0...1.20.0">compare view</a></li>
</ul>
</details>
<br />

Updates `express` from 4.17.1 to 4.18.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/express/releases">express's releases</a>.</em></p>
<blockquote>
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
<li>deps: statuses@2.0.1</li>
</ul>
</li>
<li>deps: serve-static@1.15.0
<ul>
<li>deps: send@0.18.0</li>
</ul>
</li>
<li>deps: statuses@2.0.1
<ul>
<li>Remove code 306</li>
<li>Rename <code>425 Unordered Collection</code> to standard <code>425 Too Early</code></li>
</ul>
</li>
</ul>
<h2>4.17.3</h2>
<ul>
<li>deps: accepts@~1.3.8
<ul>
<li>deps: mime-types@~2.1.34</li>
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
<li>deps: send@0.18.0
<ul>
<li>Fix emitted 416 error missing headers property</li>
<li>Limit the headers removed for 304 response</li>
<li>deps: depd@2.0.0</li>
<li>deps: destroy@1.2.0</li>
<li>deps: http-errors@2.0.0</li>
<li>deps: on-finished@2.4.1</li>
<li>deps: statuses@2.0.1</li>
</ul>
</li>
<li>deps: serve-static@1.15.0
<ul>
<li>deps: send@0.18.0</li>
</ul>
</li>
<li>deps: statuses@2.0.1
<ul>
<li>Remove code 306</li>
<li>Rename <code>425 Unordered Collection</code> to standard <code>425 Too Early</code></li>
</ul>
</li>
</ul>
<p>4.17.3 / 2022-02-16</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/expressjs/express/commit/547fdd41dca9ae9c49956748cc0bd1f011310fb6"><code>547fdd4</code></a> 4.18.0</li>
<li><a href="https://github.com/expressjs/express/commit/0b330ef57c0801313251c95a461d93f8d3afa7f7"><code>0b330ef</code></a> bench: print latency and vary connections</li>
<li><a href="https://github.com/expressjs/express/commit/158a17031a2668269aedb31ea07b58d6b700272b"><code>158a170</code></a> build: support Node.js 18.x</li>
<li><a href="https://github.com/expressjs/express/commit/29ea1b2f74c5e76e79e329ef425e5fbbcd6a71c3"><code>29ea1b2</code></a> build: use 64-bit Node.js in AppVeyor</li>
<li><a href="https://github.com/expressjs/express/commit/11a209e4b7e229bf5041e1ab76ba0ac4e0cad324"><code>11a209e</code></a> build: support Node.js 17.x</li>
<li><a href="https://github.com/expressjs/express/commit/fd8e45c344325a4a91c1b916f3617a3574018976"><code>fd8e45c</code></a> tests: mark stack overflow as long running</li>
<li><a href="https://github.com/expressjs/express/commit/708ac4cdf5cd0a658d62490a9f4d78d3e1ec6612"><code>708ac4c</code></a> Fix handling very large stacks of sync middleware</li>
<li><a href="https://github.com/expressjs/express/commit/92c5ce59f51cce4b3598fd040117772fac42dce8"><code>92c5ce5</code></a> deps: cookie@0.5.0</li>
<li><a href="https://github.com/expressjs/express/commit/8880ddad1c0f00612b53f5f686f55e7566b16562"><code>8880dda</code></a> examples: add missing html label associations</li>
<li><a href="https://github.com/expressjs/express/commit/b91c7ffb289af1753b9d1d84e16fbfcd34954124"><code>b91c7ff</code></a> examples: use http-errors to create errors</li>
<li>Additional commits viewable in <a href="https://github.com/expressjs/express/compare/4.17.1...4.18.0">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/firefly-tokens-erc20-erc721/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-09 09:01:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/98" class=".btn">#98</a>
            </td>
            <td>
                <b>
                    Bump decode-uri-component from 0.2.0 to 0.2.2 in /samples/solidity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [decode-uri-component](https://github.com/SamVerschueren/decode-uri-component) from 0.2.0 to 0.2.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/SamVerschueren/decode-uri-component/releases">decode-uri-component's releases</a>.</em></p>
<blockquote>
<h2>v0.2.2</h2>
<ul>
<li>Prevent overwriting previously decoded tokens  980e0bf</li>
</ul>
<p><a href="https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.1...v0.2.2">https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.1...v0.2.2</a></p>
<h2>v0.2.1</h2>
<ul>
<li>Switch to GitHub workflows  76abc93</li>
<li>Fix issue where decode throws - fixes <a href="https://github-redirect.dependabot.com/SamVerschueren/decode-uri-component/issues/6">#6</a>  746ca5d</li>
<li>Update license (<a href="https://github-redirect.dependabot.com/SamVerschueren/decode-uri-component/issues/1">#1</a>)  486d7e2</li>
<li>Tidelift tasks  a650457</li>
<li>Meta tweaks  66e1c28</li>
</ul>
<p><a href="https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.0...v0.2.1">https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.0...v0.2.1</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/a0eea469d26eb0df668b081672cdb9581feb78eb"><code>a0eea46</code></a> 0.2.2</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/980e0bf09b64d94f1aa79012f895816c30ffd152"><code>980e0bf</code></a> Prevent overwriting previously decoded tokens</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/3c8a373dd4837e89b3f970e01295dd03e1405a33"><code>3c8a373</code></a> 0.2.1</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/76abc939783fe3900fadb7d384a74d324d5557f3"><code>76abc93</code></a> Switch to GitHub workflows</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/746ca5dcb6667c5d364e782d53c542830e4c10b9"><code>746ca5d</code></a> Fix issue where decode throws - fixes <a href="https://github-redirect.dependabot.com/SamVerschueren/decode-uri-component/issues/6">#6</a></li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/486d7e26d3a8c0fbe860fb651fe1bc98c2f2be30"><code>486d7e2</code></a> Update license (<a href="https://github-redirect.dependabot.com/SamVerschueren/decode-uri-component/issues/1">#1</a>)</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/a65045724e6234acef87f31da499d4807b20b134"><code>a650457</code></a> Tidelift tasks</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/66e1c2834c0e189201cb65196ec3101372459b02"><code>66e1c28</code></a> Meta tweaks</li>
<li>See full diff in <a href="https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.0...v0.2.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=decode-uri-component&package-manager=npm_and_yarn&previous-version=0.2.0&new-version=0.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/firefly-tokens-erc20-erc721/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-08 23:36:26 +0000 UTC
    </div>
</div>

