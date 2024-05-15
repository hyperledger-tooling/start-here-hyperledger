---
layout: default
title: indy-besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-besu
---

# indy-besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-besu/pull/48" class=".btn">#48</a>
            </td>
            <td>
                <b>
                    Bump the npm_and_yarn group across 1 directory with 5 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps the npm_and_yarn group with 5 updates in the /smart_contracts directory:

| Package | From | To |
| --- | --- | --- |
| [@openzeppelin/contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) | `5.0.0` | `5.0.2` |
| [es5-ext](https://github.com/medikoo/es5-ext) | `0.10.62` | `0.10.64` |
| [express](https://github.com/expressjs/express) | `4.18.2` | `4.19.2` |
| [follow-redirects](https://github.com/follow-redirects/follow-redirects) | `1.15.5` | `1.15.6` |
| [undici](https://github.com/nodejs/undici) | `5.28.3` | `5.28.4` |


Updates `@openzeppelin/contracts` from 5.0.0 to 5.0.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/releases"><code>@​openzeppelin/contracts</code>'s releases</a>.</em></p>
<blockquote>
<h2>v5.0.2</h2>
<ul>
<li><code>Base64</code>: Fix issue where dirty memory located just after the input buffer is affecting the result. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4926">#4926</a>)</li>
</ul>
<h2>v5.0.1</h2>
<ul>
<li><code>ERC2771Context</code> and <code>Context</code>: Introduce a <code>_contextPrefixLength()</code> getter, used to trim extra information appended to <code>msg.data</code>.</li>
<li><code>Multicall</code>: Make aware of non-canonical context (i.e. <code>msg.sender</code> is not <code>_msgSender()</code>), allowing compatibility with <code>ERC2771Context</code>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/CHANGELOG.md"><code>@​openzeppelin/contracts</code>'s changelog</a>.</em></p>
<blockquote>
<h2>5.0.2 (2024-02-29)</h2>
<ul>
<li><code>Base64</code>: Fix issue where dirty memory located just after the input buffer is affecting the result. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4926">#4926</a>)</li>
</ul>
<h2>5.0.1 (2023-12-07)</h2>
<ul>
<li><code>ERC2771Context</code> and <code>Context</code>: Introduce a <code>_contextPrefixLength()</code> getter, used to trim extra information appended to <code>msg.data</code>.</li>
<li><code>Multicall</code>: Make aware of non-canonical context (i.e. <code>msg.sender</code> is not <code>_msgSender()</code>), allowing compatibility with <code>ERC2771Context</code>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/dbb6104ce834628e473d2173bbc9d47f81a9eec3"><code>dbb6104</code></a> Release v5.0.2 (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4928">#4928</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/26b4b6099936fc785309f3da118ec8607b6716ed"><code>26b4b60</code></a> Port Base64 tests to truffle (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4926">#4926</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/d4ec2782b724be9e56bf33aa91ff599df185c0b0"><code>d4ec278</code></a> List every contract in each API doc section (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4848">#4848</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/f7bb9881a8d5119b7a1aaf8dc8a589b48bca64dd"><code>f7bb988</code></a> Replace Defender Admin with Transaction Proposals (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4804">#4804</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/e53f81b7044657e4e14e85a587e92a995e2c266b"><code>e53f81b</code></a> Remove Governor's guide ERC6372 disclaimer for Tally (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4801">#4801</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/01ef448981be9d20ca85f2faf6ebdf591ce409f3"><code>01ef448</code></a> Release v5.0.1 (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4785">#4785</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/9ce0340466bb125d6bb9f22bfcb5e37e062e26e2"><code>9ce0340</code></a> Make Multicall context-aware</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/4eb67a408c13e8c67f7b99a9d618aa442ad53a84"><code>4eb67a4</code></a> Close <code>access-control.adoc</code> code block (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4726">#4726</a>) (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4727">#4727</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/83330a6e4c8efeded3ea2b8d6aae5ac2ffc18555"><code>83330a6</code></a> Add <code>AccessManager</code> guide (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4691">#4691</a>) (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4724">#4724</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/ab967b863964b5de4a8be5c30796180a78fb3b6e"><code>ab967b8</code></a> Update the &quot;utilities&quot; documentation page (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4678">#4678</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/compare/v5.0.0...v5.0.2">compare view</a></li>
</ul>
</details>
<br />

Updates `es5-ext` from 0.10.62 to 0.10.64
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/medikoo/es5-ext/releases">es5-ext's releases</a>.</em></p>
<blockquote>
<h2>0.10.64 (2024-02-27)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>Revert update to postinstall script meant to fix Powershell issue, as it's a regression for some Linux terminals (<a href="https://github.com/medikoo/es5-ext/commit/c2e2bb90c295c4c582445a6f03b2a3ad0b22550a">c2e2bb9</a>)</li>
</ul>
<hr />
<p><a href="https://github.com/medikoo/es5-ext/compare/v0.10.63...v0.10.64">Comparison since last release</a></p>
<h2>0.10.63 (2024-02-23)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>Do not rely on problematic regex (<a href="https://github.com/medikoo/es5-ext/commit/3551cdd7b2db08b1632841f819d008757d28e8e2">3551cdd</a>), addresses <a href="https://redirect.github.com/medikoo/es5-ext/issues/201">#201</a></li>
<li>Support ES2015+ function definitions in <code>function#toStringTokens()</code> (<a href="https://github.com/medikoo/es5-ext/commit/a52e95736690ad1d465ebcd9791d54570e294602">a52e957</a>), addresses <a href="https://redirect.github.com/medikoo/es5-ext/issues/021">#021</a></li>
<li>Ensure postinstall script does not crash on Windows, fixes <a href="https://redirect.github.com/medikoo/es5-ext/issues/181">#181</a> (<a href="https://github.com/medikoo/es5-ext/commit/bf8ed799d57df53096da9d908ff577f305e1366f">bf8ed79</a>)</li>
</ul>
<h3>Maintenance Improvements</h3>
<ul>
<li>Simplify the manifest message (<a href="https://github.com/medikoo/es5-ext/commit/7855319f41b9736639cf4555bd2c419f17addf55">7855319</a>)</li>
</ul>
<hr />
<p><a href="https://github.com/medikoo/es5-ext/compare/v0.10.62...v0.10.63">Comparison since last release</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/medikoo/es5-ext/blob/main/CHANGELOG.md">es5-ext's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/medikoo/es5-ext/compare/v0.10.63...v0.10.64">0.10.64</a> (2024-02-27)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>Revert update to postinstall script meant to fix Powershell issue, as it's a regression for some Linux terminals (<a href="https://github.com/medikoo/es5-ext/commit/c2e2bb90c295c4c582445a6f03b2a3ad0b22550a">c2e2bb9</a>)</li>
</ul>
<h3><a href="https://github.com/medikoo/es5-ext/compare/v0.10.62...v0.10.63">0.10.63</a> (2024-02-23)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>Do not rely on problematic regex (<a href="https://github.com/medikoo/es5-ext/commit/3551cdd7b2db08b1632841f819d008757d28e8e2">3551cdd</a>), addresses <a href="https://redirect.github.com/medikoo/es5-ext/issues/201">#201</a></li>
<li>Support ES2015+ function definitions in <code>function#toStringTokens()</code> (<a href="https://github.com/medikoo/es5-ext/commit/a52e95736690ad1d465ebcd9791d54570e294602">a52e957</a>), addresses <a href="https://redirect.github.com/medikoo/es5-ext/issues/021">#021</a></li>
<li>Ensure postinstall script does not crash on Windows, fixes <a href="https://redirect.github.com/medikoo/es5-ext/issues/181">#181</a> (<a href="https://github.com/medikoo/es5-ext/commit/bf8ed799d57df53096da9d908ff577f305e1366f">bf8ed79</a>)</li>
</ul>
<h3>Maintenance Improvements</h3>
<ul>
<li>Simplify the manifest message (<a href="https://github.com/medikoo/es5-ext/commit/7855319f41b9736639cf4555bd2c419f17addf55">7855319</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/medikoo/es5-ext/commit/f76b03d8c49ce4871f37f428c0e1d3ee6637fcc4"><code>f76b03d</code></a> chore: Release v0.10.64</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/2881acda50de0848b456690769919ed4b86be489"><code>2881acd</code></a> chore: Bump dependencies</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/c2e2bb90c295c4c582445a6f03b2a3ad0b22550a"><code>c2e2bb9</code></a> fix: Revert update meant to fix Powershell issue, as it's a regression</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/16f2b7253d3d8d499d8cf1d3ca76c585da7f08d3"><code>16f2b72</code></a> docs: Fix date in the changelog</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/de4e03c4776a303284142f73f3f181a070615817"><code>de4e03c</code></a> chore: Release v0.10.63</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/3fd53b755ec883be8f119c747f0b04130741e456"><code>3fd53b7</code></a> chore: Upgrade<code> lint-staged</code> to v13</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/bf8ed799d57df53096da9d908ff577f305e1366f"><code>bf8ed79</code></a> chore: Ensure postinstall script does not crash on Windows</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/2cbbb0717bd8de6e38fcba1f0d45bc876e7a1951"><code>2cbbb07</code></a> chore: Bump dependencies</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/22d0416ea170000a115609f22a560dfa9193ebb0"><code>22d0416</code></a> chore: Bump LICENSE year</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/a52e95736690ad1d465ebcd9791d54570e294602"><code>a52e957</code></a> fix: Support ES2015+ function definitions in <code>function#toStringTokens()</code></li>
<li>Additional commits viewable in <a href="https://github.com/medikoo/es5-ext/compare/v0.10.62...v0.10.64">compare view</a></li>
</ul>
</details>
<br />

Updates `express` from 4.18.2 to 4.19.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/express/releases">express's releases</a>.</em></p>
<blockquote>
<h2>4.19.2</h2>
<h2>What's Changed</h2>
<ul>
<li><a href="https://github.com/expressjs/express/commit/0b746953c4bd8e377123527db11f9cd866e39f94">Improved fix for open redirect allow list bypass</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/expressjs/express/compare/4.19.1...4.19.2">https://github.com/expressjs/express/compare/4.19.1...4.19.2</a></p>
<h2>4.19.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix ci after location patch by <a href="https://github.com/wesleytodd"><code>@​wesleytodd</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5552">expressjs/express#5552</a></li>
<li>fixed un-edited version in history.md for 4.19.0 by <a href="https://github.com/wesleytodd"><code>@​wesleytodd</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5556">expressjs/express#5556</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/expressjs/express/compare/4.19.0...4.19.1">https://github.com/expressjs/express/compare/4.19.0...4.19.1</a></p>
<h2>4.19.0</h2>
<h2>What's Changed</h2>
<ul>
<li>fix typo in release date by <a href="https://github.com/UlisesGascon"><code>@​UlisesGascon</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5527">expressjs/express#5527</a></li>
<li>docs: nominating <a href="https://github.com/wesleytodd"><code>@​wesleytodd</code></a> to be project captian by <a href="https://github.com/wesleytodd"><code>@​wesleytodd</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5511">expressjs/express#5511</a></li>
<li>docs: loosen TC activity rules by <a href="https://github.com/wesleytodd"><code>@​wesleytodd</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5510">expressjs/express#5510</a></li>
<li>Add note on how to update docs for new release by <a href="https://github.com/crandmck"><code>@​crandmck</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5541">expressjs/express#5541</a></li>
<li><a href="https://redirect.github.com/expressjs/express/pull/5551/commits/660ccf5fa33dd0baab069e5c8ddd9ffe7d8bbff1">Prevent open redirect allow list bypass due to encodeurl</a></li>
<li>Release 4.19.0 by <a href="https://github.com/wesleytodd"><code>@​wesleytodd</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5551">expressjs/express#5551</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/crandmck"><code>@​crandmck</code></a> made their first contribution in <a href="https://redirect.github.com/expressjs/express/pull/5541">expressjs/express#5541</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/expressjs/express/compare/4.18.3...4.19.0">https://github.com/expressjs/express/compare/4.18.3...4.19.0</a></p>
<h2>4.18.3</h2>
<h2>Main Changes</h2>
<ul>
<li>Fix routing requests without method</li>
<li>deps: body-parser@1.20.2
<ul>
<li>Fix strict json error message on Node.js 19+</li>
<li>deps: content-type@~1.0.5</li>
<li>deps: raw-body@2.5.2</li>
</ul>
</li>
</ul>
<h2>Other Changes</h2>
<ul>
<li>Use https: protocol instead of deprecated git: protocol by <a href="https://github.com/vcsjones"><code>@​vcsjones</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5032">expressjs/express#5032</a></li>
<li>build: Node.js@16.18 and Node.js@18.12 by <a href="https://github.com/abenhamdine"><code>@​abenhamdine</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5034">expressjs/express#5034</a></li>
<li>ci: update actions/checkout to v3 by <a href="https://github.com/armujahid"><code>@​armujahid</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5027">expressjs/express#5027</a></li>
<li>test: remove unused function arguments in params by <a href="https://github.com/raksbisht"><code>@​raksbisht</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5124">expressjs/express#5124</a></li>
<li>Remove unused originalIndex from acceptParams by <a href="https://github.com/raksbisht"><code>@​raksbisht</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5119">expressjs/express#5119</a></li>
<li>Fixed typos by <a href="https://github.com/raksbisht"><code>@​raksbisht</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5117">expressjs/express#5117</a></li>
<li>examples: remove unused params by <a href="https://github.com/raksbisht"><code>@​raksbisht</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5113">expressjs/express#5113</a></li>
<li>fix: parameter str is not described in JSDoc by <a href="https://github.com/raksbisht"><code>@​raksbisht</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5130">expressjs/express#5130</a></li>
<li>fix: typos in History.md by <a href="https://github.com/raksbisht"><code>@​raksbisht</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5131">expressjs/express#5131</a></li>
<li>build : add Node.js@19.7 by <a href="https://github.com/abenhamdine"><code>@​abenhamdine</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5028">expressjs/express#5028</a></li>
<li>test: remove unused function arguments in params by <a href="https://github.com/raksbisht"><code>@​raksbisht</code></a> in <a href="https://redirect.github.com/expressjs/express/pull/5137">expressjs/express#5137</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/expressjs/express/blob/master/History.md">express's changelog</a>.</em></p>
<blockquote>
<h1>4.19.2 / 2024-03-25</h1>
<ul>
<li>Improved fix for open redirect allow list bypass</li>
</ul>
<h1>4.19.1 / 2024-03-20</h1>
<ul>
<li>Allow passing non-strings to res.location with new encoding handling checks</li>
</ul>
<h1>4.19.0 / 2024-03-20</h1>
<ul>
<li>Prevent open redirect allow list bypass due to encodeurl</li>
<li>deps: cookie@0.6.0</li>
</ul>
<h1>4.18.3 / 2024-02-29</h1>
<ul>
<li>Fix routing requests without method</li>
<li>deps: body-parser@1.20.2
<ul>
<li>Fix strict json error message on Node.js 19+</li>
<li>deps: content-type@~1.0.5</li>
<li>deps: raw-body@2.5.2</li>
</ul>
</li>
<li>deps: cookie@0.6.0
<ul>
<li>Add <code>partitioned</code> option</li>
</ul>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/expressjs/express/commit/04bc62787be974874bc1467b23606c36bc9779ba"><code>04bc627</code></a> 4.19.2</li>
<li><a href="https://github.com/expressjs/express/commit/da4d763ff6ba9df6dbd8f1f0b1d05412dda934d5"><code>da4d763</code></a> Improved fix for open redirect allow list bypass</li>
<li><a href="https://github.com/expressjs/express/commit/4f0f6cc67d531431c096ea006c2191b92931bbc3"><code>4f0f6cc</code></a> 4.19.1</li>
<li><a href="https://github.com/expressjs/express/commit/a003cfab034fbadb1c78ae337ee8ab389adda217"><code>a003cfa</code></a> Allow passing non-strings to res.location with new encoding handling checks f...</li>
<li><a href="https://github.com/expressjs/express/commit/a1fa90fcea7d8e844e1c9938ad095d62669c3abd"><code>a1fa90f</code></a> fixed un-edited version in history.md for 4.19.0</li>
<li><a href="https://github.com/expressjs/express/commit/11f2b1db227fd42c2508c427032c1ec671b306be"><code>11f2b1d</code></a> build: fix build due to inconsistent supertest behavior in older versions</li>
<li><a href="https://github.com/expressjs/express/commit/084e36506a18774f85206a65d8da04dc1107fc1b"><code>084e365</code></a> 4.19.0</li>
<li><a href="https://github.com/expressjs/express/commit/0867302ddbde0e9463d0564fea5861feb708c2dd"><code>0867302</code></a> Prevent open redirect allow list bypass due to encodeurl</li>
<li><a href="https://github.com/expressjs/express/commit/567c9c665d0de4c344b8e160146050770233783c"><code>567c9c6</code></a> Add note on how to update docs for new release (<a href="https://redirect.github.com/expressjs/express/issues/5541">#5541</a>)</li>
<li><a href="https://github.com/expressjs/express/commit/69a4cf2819c4449ec6ea45649691fb43a528d5d1"><code>69a4cf2</code></a> deps: cookie@0.6.0</li>
<li>Additional commits viewable in <a href="https://github.com/expressjs/express/compare/4.18.2...4.19.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~wesleytodd">wesleytodd</a>, a new releaser for express since your current version.</p>
</details>
<br />

Updates `follow-redirects` from 1.15.5 to 1.15.6
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/35a517c5861d79dc8bff7db8626013d20b711b06"><code>35a517c</code></a> Release version 1.15.6 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/c4f847f85176991f95ab9c88af63b1294de8649b"><code>c4f847f</code></a> Drop Proxy-Authorization across hosts.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/8526b4a1b2ab3a2e4044299377df623a661caa76"><code>8526b4a</code></a> Use GitHub for disclosure.</li>
<li>See full diff in <a href="https://github.com/follow-redirects/follow-redirects/compare/v1.15.5...v1.15.6">compare view</a></li>
</ul>
</details>
<br />

Updates `undici` from 5.28.3 to 5.28.4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nodejs/undici/releases">undici's releases</a>.</em></p>
<blockquote>
<h2>v5.28.4</h2>
<h2>:warning: Security Release :warning:</h2>
<ul>
<li>Fixes <a href="https://github.com/nodejs/undici/security/advisories/GHSA-m4v8-wqvr-p9f7">https://github.com/nodejs/undici/security/advisories/GHSA-m4v8-wqvr-p9f7</a> CVE-2024-30260</li>
<li>Fixes <a href="https://github.com/nodejs/undici/security/advisories/GHSA-9qxr-qj54-h672">https://github.com/nodejs/undici/security/advisories/GHSA-9qxr-qj54-h672</a> CVE-2024-30261</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.28.3...v5.28.4">https://github.com/nodejs/undici/compare/v5.28.3...v5.28.4</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nodejs/undici/commit/fb983069071f52e0a7ea0e71078459c765aae172"><code>fb98306</code></a> Bumped v5.28.4</li>
<li><a href="https://github.com/nodejs/undici/commit/2b39440bd9ded841c93dd72138f3b1763ae26055"><code>2b39440</code></a> Merge pull request from GHSA-9qxr-qj54-h672</li>
<li><a href="https://github.com/nodejs/undici/commit/64e3402da4e032e68de46acb52800c9a06aaea3f"><code>64e3402</code></a> Merge pull request from GHSA-m4v8-wqvr-p9f7</li>
<li><a href="https://github.com/nodejs/undici/commit/723c4e728051aefd5eb5ae7193dfb18046009f83"><code>723c4e7</code></a> Revert &quot;build(deps-dev): bump formdata-node from 4.4.1 to 6.0.3 (<a href="https://redirect.github.com/nodejs/undici/issues/2389">#2389</a>)&quot;</li>
<li><a href="https://github.com/nodejs/undici/commit/0e9d54b2c2a5ec0b58937114c857a9ed9fe22d5b"><code>0e9d54b</code></a> skip failing test due to Node.js changes</li>
<li>See full diff in <a href="https://github.com/nodejs/undici/compare/v5.28.3...v5.28.4">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-besu/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 11:48:17 +0000 UTC
    </div>
</div>

