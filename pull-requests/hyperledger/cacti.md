---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3153" class=".btn">#3153</a>
            </td>
            <td>
                <b>
                    build(plugin-persistence-ethereum): bump web3-utils to v4.2.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [web3-utils](https://github.com/ChainSafe/web3.js) from 4.0.6 to 4.2.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ChainSafe/web3.js/releases">web3-utils's releases</a>.</em></p>
<blockquote>
<h2>web3-utils@4.0.0-alpha.0</h2>
<p>Initial alpha release</p>
<p>Install with <code>yarn add web3-utils@4.0.0-alpha.0</code></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/web3/web3.js/blob/4.x/CHANGELOG.md">web3-utils's changelog</a>.</em></p>
<blockquote>
<h2>[4.2.1]</h2>
<h3>Fixed</h3>
<h4>web3-eth-abi</h4>
<ul>
<li>Bug fix of <code>ERR_UNSUPPORTED_DIR_IMPORT</code> in ABI (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6535">#6535</a>)</li>
</ul>
<h3>Changed</h3>
<h4>web3-eth-contract</h4>
<ul>
<li>Dependencies updated</li>
</ul>
<h4>web3-eth</h4>
<ul>
<li>Dependencies updated</li>
</ul>
<h4>web3-eth-ens</h4>
<ul>
<li>Dependencies updated</li>
</ul>
<h4>web3-eth-personal</h4>
<ul>
<li>Dependencies updated</li>
</ul>
<h2>[4.2.2]</h2>
<h3>Added</h3>
<h4>web3-core</h4>
<ul>
<li>Added <code>isMetaMaskProvider</code> function to check if provider is metamask (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6534">#6534</a>)</li>
</ul>
<h4>web3-types</h4>
<ul>
<li>Interface <code>MetaMaskProvider</code> added and is part of <code>SupportedProviders</code> (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6534">#6534</a>)</li>
<li><code>gasPrice</code> was added to <code>Transaction1559UnsignedAPI</code> type. (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6539">#6539</a>)</li>
</ul>
<h3>Changed</h3>
<h4>web3</h4>
<ul>
<li>Dependencies updated</li>
</ul>
<h3>Fixed</h3>
<h4>web3-errors</h4>
<ul>
<li>Fixed grammar and spelling in <code>transactionTimeoutHint</code> (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6559">#6559</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/ChainSafe/web3.js/commits/v4.2.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=web3-utils&package-manager=npm_and_yarn&previous-version=4.0.6&new-version=4.2.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-28 16:37:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3152" class=".btn">#3152</a>
            </td>
            <td>
                <b>
                    build(deps): bump express from 4.18.2 to 4.19.2 in /examples/test-run-transaction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [express](https://github.com/expressjs/express) from 4.18.2 to 4.19.2.
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


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=express&package-manager=npm_and_yarn&previous-version=4.18.2&new-version=4.19.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-28 16:37:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3151" class=".btn">#3151</a>
            </td>
            <td>
                <b>
                    build(deps): bump web3-utils from 4.0.3 to 4.2.1 in /packages/cactus-test-plugin-htlc-eth-besu-erc20
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [web3-utils](https://github.com/ChainSafe/web3.js) from 4.0.3 to 4.2.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ChainSafe/web3.js/releases">web3-utils's releases</a>.</em></p>
<blockquote>
<h2>web3-utils@4.0.0-alpha.0</h2>
<p>Initial alpha release</p>
<p>Install with <code>yarn add web3-utils@4.0.0-alpha.0</code></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/web3/web3.js/blob/4.x/CHANGELOG.md">web3-utils's changelog</a>.</em></p>
<blockquote>
<h2>[4.0.3]</h2>
<h3>Fixed</h3>
<h4>web3</h4>
<ul>
<li>Fixed bug <a href="https://redirect.github.com/ChainSafe/web3.js/issues/6236">#6236</a> by adding personal type in web3.eth (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6245">#6245</a>)</li>
</ul>
<h4>web3-rpc-methods</h4>
<ul>
<li>Rpc method <code>getPastLogs</code> accept blockHash as a parameter <a href="https://ethereum.org/en/developers/docs/apis/json-rpc/#eth_getlogs">https://ethereum.org/en/developers/docs/apis/json-rpc/#eth_getlogs</a> (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6181">#6181</a>)</li>
</ul>
<h4>web3-types</h4>
<ul>
<li>type <code>Filter</code> includes <code>blockHash</code> (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6206">#6206</a>)</li>
</ul>
<h4>web3-utils</h4>
<ul>
<li>BigInts pass validation within the method <code>numberToHex</code> (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6206">#6206</a>)</li>
</ul>
<h3>Changed</h3>
<h4>web3-core</h4>
<ul>
<li>Dependencies updated</li>
</ul>
<h4>web3-errors</h4>
<ul>
<li>Dependencies updated</li>
</ul>
<h4>web3-eth</h4>
<ul>
<li>Dependencies updated</li>
</ul>
<h4>web3-eth-abi</h4>
<ul>
<li>Dependencies updated</li>
</ul>
<h4>web3-eth-accounts</h4>
<ul>
<li>Dependencies updated</li>
</ul>
<h4>web3-eth-contract</h4>
<ul>
<li>Dependencies updated</li>
</ul>
<h4>web3-eth-ens</h4>
<ul>
<li>Dependencies updated</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/web3/web3.js/commit/a6c6dec9fef078ced630677de67dc379b4fd5b81"><code>a6c6dec</code></a> version and changelog bump</li>
<li><a href="https://github.com/web3/web3.js/commit/f860b0481d7c1ef09ddaeb33098b2253ca694150"><code>f860b04</code></a> Bump <code>@​babel/traverse</code> from 7.22.4 to 7.23.2 in /docs (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6514">#6514</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/a0d6730e317ab97fa4983c09880a0a1d01af9b74"><code>a0d6730</code></a> Bug Fixing ERR_UNSUPPORTED_DIR_IMPORT in web3-eth-abi/lib/esm/coders/encode.j...</li>
<li><a href="https://github.com/web3/web3.js/commit/90b8581630ba8c15acca259179d1de69d7d1aab5"><code>90b8581</code></a> Bump <code>@​babel/traverse</code> from 7.18.11 to 7.23.2 (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6513">#6513</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/6791e60ee3d66feab782e1ee79713f7baa5655c1"><code>6791e60</code></a> Bump undici from 5.22.0 to 5.26.3 (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6511">#6511</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/7bee9bc7706f9c16757b464553fb7234fc8e4491"><code>7bee9bc</code></a> fix CI/CD Firefox tests (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6516">#6516</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/bd3b9a0dacc6f15a406dd660ec7add3c2765b600"><code>bd3b9a0</code></a> Release/4.2.0 (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6517">#6517</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/09f4c8b077c06322855a99c722fd87aadee2feac"><code>09f4c8b</code></a> Fix validation uint int sizes (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6434">#6434</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/226b3ba9c1ece0a399d120b83229582ea20b6c95"><code>226b3ba</code></a> 6508 fix (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6509">#6509</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/70d1957e0a8642d1e5dba47c39ea65504689b6ec"><code>70d1957</code></a> Add functionality to extend tx types (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6493">#6493</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/ChainSafe/web3.js/compare/v4.0.3...v4.2.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=web3-utils&package-manager=npm_and_yarn&previous-version=4.0.3&new-version=4.2.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-28 16:36:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3150" class=".btn">#3150</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump web3-utils from 4.0.3 to 4.2.1 in /extensions/cactus-plugin-htlc-coordinator-besu
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [web3-utils](https://github.com/ChainSafe/web3.js) from 4.0.3 to 4.2.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ChainSafe/web3.js/releases">web3-utils's releases</a>.</em></p>
<blockquote>
<h2>web3-utils@4.0.0-alpha.0</h2>
<p>Initial alpha release</p>
<p>Install with <code>yarn add web3-utils@4.0.0-alpha.0</code></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/web3/web3.js/blob/4.x/CHANGELOG.md">web3-utils's changelog</a>.</em></p>
<blockquote>
<h2>[4.0.3]</h2>
<h3>Fixed</h3>
<h4>web3</h4>
<ul>
<li>Fixed bug <a href="https://redirect.github.com/ChainSafe/web3.js/issues/6236">#6236</a> by adding personal type in web3.eth (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6245">#6245</a>)</li>
</ul>
<h4>web3-rpc-methods</h4>
<ul>
<li>Rpc method <code>getPastLogs</code> accept blockHash as a parameter <a href="https://ethereum.org/en/developers/docs/apis/json-rpc/#eth_getlogs">https://ethereum.org/en/developers/docs/apis/json-rpc/#eth_getlogs</a> (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6181">#6181</a>)</li>
</ul>
<h4>web3-types</h4>
<ul>
<li>type <code>Filter</code> includes <code>blockHash</code> (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6206">#6206</a>)</li>
</ul>
<h4>web3-utils</h4>
<ul>
<li>BigInts pass validation within the method <code>numberToHex</code> (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6206">#6206</a>)</li>
</ul>
<h3>Changed</h3>
<h4>web3-core</h4>
<ul>
<li>Dependencies updated</li>
</ul>
<h4>web3-errors</h4>
<ul>
<li>Dependencies updated</li>
</ul>
<h4>web3-eth</h4>
<ul>
<li>Dependencies updated</li>
</ul>
<h4>web3-eth-abi</h4>
<ul>
<li>Dependencies updated</li>
</ul>
<h4>web3-eth-accounts</h4>
<ul>
<li>Dependencies updated</li>
</ul>
<h4>web3-eth-contract</h4>
<ul>
<li>Dependencies updated</li>
</ul>
<h4>web3-eth-ens</h4>
<ul>
<li>Dependencies updated</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/web3/web3.js/commit/a6c6dec9fef078ced630677de67dc379b4fd5b81"><code>a6c6dec</code></a> version and changelog bump</li>
<li><a href="https://github.com/web3/web3.js/commit/f860b0481d7c1ef09ddaeb33098b2253ca694150"><code>f860b04</code></a> Bump <code>@​babel/traverse</code> from 7.22.4 to 7.23.2 in /docs (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6514">#6514</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/a0d6730e317ab97fa4983c09880a0a1d01af9b74"><code>a0d6730</code></a> Bug Fixing ERR_UNSUPPORTED_DIR_IMPORT in web3-eth-abi/lib/esm/coders/encode.j...</li>
<li><a href="https://github.com/web3/web3.js/commit/90b8581630ba8c15acca259179d1de69d7d1aab5"><code>90b8581</code></a> Bump <code>@​babel/traverse</code> from 7.18.11 to 7.23.2 (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6513">#6513</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/6791e60ee3d66feab782e1ee79713f7baa5655c1"><code>6791e60</code></a> Bump undici from 5.22.0 to 5.26.3 (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6511">#6511</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/7bee9bc7706f9c16757b464553fb7234fc8e4491"><code>7bee9bc</code></a> fix CI/CD Firefox tests (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6516">#6516</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/bd3b9a0dacc6f15a406dd660ec7add3c2765b600"><code>bd3b9a0</code></a> Release/4.2.0 (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6517">#6517</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/09f4c8b077c06322855a99c722fd87aadee2feac"><code>09f4c8b</code></a> Fix validation uint int sizes (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6434">#6434</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/226b3ba9c1ece0a399d120b83229582ea20b6c95"><code>226b3ba</code></a> 6508 fix (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6509">#6509</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/70d1957e0a8642d1e5dba47c39ea65504689b6ec"><code>70d1957</code></a> Add functionality to extend tx types (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6493">#6493</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/ChainSafe/web3.js/compare/v4.0.3...v4.2.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=web3-utils&package-manager=npm_and_yarn&previous-version=4.0.3&new-version=4.2.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-28 16:36:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3149" class=".btn">#3149</a>
            </td>
            <td>
                <b>
                    build(deps): bump express from 4.18.2 to 4.19.2 in /examples/test-run-transaction/supply-chain-app-stub
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [express](https://github.com/expressjs/express) from 4.18.2 to 4.19.2.
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


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=express&package-manager=npm_and_yarn&previous-version=4.18.2&new-version=4.19.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-28 16:36:53 +0000 UTC
    </div>
</div>

