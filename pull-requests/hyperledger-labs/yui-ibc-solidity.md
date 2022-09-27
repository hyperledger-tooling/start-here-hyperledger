---
layout: default
title: yui-ibc-solidity
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/yui-ibc-solidity
---

# yui-ibc-solidity <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-ibc-solidity){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/114" class=".btn">#114</a>
            </td>
            <td>
                <b>
                    ci: remove unused patch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jun Kimura <jun.kimura@datachain.jp>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-27 16:04:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/113" class=".btn">#113</a>
            </td>
            <td>
                <b>
                    update README
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jun Kimura <jun.kimura@datachain.jp>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-27 14:35:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/112" class=".btn">#112</a>
            </td>
            <td>
                <b>
                    Bump underscore and web3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Removes [underscore](https://github.com/jashkenas/underscore). It's no longer used after updating ancestor dependency [web3](https://github.com/ethereum/web3.js). These dependencies need to be updated together.

Removes `underscore`

Updates `web3` from 1.3.4 to 1.8.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ethereum/web3.js/releases">web3's releases</a>.</em></p>
<blockquote>
<h2>web3-eth@4.0.0-alpha.0</h2>
<p>Initial alpha release</p>
<p>Install with <code>yarn add web3-eth@4.0.0-alpha.0</code></p>
<h2>web3-core-requestmanager@4.0.0-alpha.0</h2>
<p>Initial alpha release</p>
<p>Install with <code>yarn add web3-core-requestmanager@4.0.0-alpha.0</code></p>
<h2>web3-providers-http@4.0.0-alpha.0</h2>
<p>Initial alpha release</p>
<p>Install with <code>yarn add web3-providers-http@4.0.0-alpha.0</code></p>
<h2>web3-providers-base@1.0.0-alpha.1</h2>
<h3>Changed</h3>
<ul>
<li>Update version to <code>1.0.0-alpha.1</code> for <code>web3-providers-base</code></li>
<li>Update version to <code>4.0.0-alpha.0</code> for <code>web3-utils</code> in <code>web3-providers-base</code></li>
</ul>
<h2>web3-utils@4.0.0-alpha.0</h2>
<p>Initial alpha release</p>
<p>Install with <code>yarn add web3-utils@4.0.0-alpha.0</code></p>
<h2>web3-packagetemplate@1.0.0-alpha.0</h2>
<p>Initial alpha release</p>
<p>Install with <code>yarn add web3-packagetemplate@1.0.0-alpha.0</code></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/web3/web3.js/blob/1.x/CHANGELOG.md">web3's changelog</a>.</em></p>
<blockquote>
<h2>[1.3.4]</h2>
<h3>Changed</h3>
<ul>
<li>Fixed mutation of inputs to encoding and decoding functions (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3748">#3748</a>)</li>
<li>Fix default value for <code>fromBlock</code> option for <code>logs</code> subscriptions (defaults to <code>latest</code>) (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3883">#3883</a>)</li>
<li>ethjs-signer test (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3876">#3876</a>)</li>
<li>Rename <code>web3-eth2-base</code> to <code>web3-eth2-core</code> and <code>web3-eth2-beacon</code> to <code>web3-eth2-beaconchain</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3833">#3833</a>)</li>
<li>Bump <code>ts-node</code> from version <code>^8.10.2</code> to <code>^9.0.0</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3856">#3856</a>)</li>
<li>Ran <code>npm audit fix</code> which fixed 4 vulnerabilities (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3856">#3856</a>)</li>
<li>Correct <code>web3-eth2-beaconchain</code> type declarations (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3859">#3859</a>) and (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3865">#3865</a>)</li>
<li>Move interfaces <code>IBaseAPISchema</code> and <code>IBaseAPIMethodSchema</code> to <code>index.d.ts</code> for <code>web3-eth2-core</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3878">#3878</a>)</li>
<li>Update dependencies for <code>web3-eth2-core</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3878">#3878</a>)</li>
</ul>
<h3>Removed</h3>
<ul>
<li>Remove <code>notImplemented</code> flag from ETH2 Beacon Chain package methods schema (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3861">#3861</a>)</li>
<li>Removes <code>IETH2BeaconChain</code> interface in favor of exporting a class type: <code>ETH2BeaconChain</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3878">#3878</a>)</li>
<li>Remove <code>index.d.ts</code> files in favor of <code>types.ts</code> for <code>web3-eth2-core</code> and <code>web3-eth2-beaconchain</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3878">#3878</a>)</li>
<li><code>schema.ts</code> from <code>web3-eth2-core</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3878">#3878</a>)</li>
<li><code>dtslint</code> npm command from <code>web3-eth2-core</code> and <code>web3-eth2-beaconchain</code> as <code>index.d.ts</code> files were removed (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3878">#3878</a>)</li>
</ul>
<h3>Added</h3>
<ul>
<li>Add <code>ETH2Core</code> class export to <code>index.d.ts</code> for <code>web3-eth2-core</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3878">#3878</a>)</li>
<li>Deprecation of bzz warning (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3872">#3872</a>)</li>
<li>Deprecation of shh warning (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3888">#3888</a>)</li>
</ul>
<h2>[1.3.5]</h2>
<h3>Added</h3>
<ul>
<li>Github action for running tests for <code>web3-eth2-core</code> and <code>web3-eth2-beaconchain</code> packages (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3892">#3892</a>)</li>
<li>Added description to documentation on how to connect using a remote node provider (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3884">#3884</a>)</li>
<li>Added Security risk warning to docs for <code>web3.utils.soliditySha3</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3908">#3908</a>)</li>
<li><code>.nvmrc</code> file using Node.js version <code>v.14.15.1</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3817">#3817</a>)</li>
<li>Add commitment to semantic versioning since version <code>1.3.0</code> and onwards (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3961">#3961</a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Unified babel compiler for <code>web3-eth2-core</code> and <code>web3-eth2-beaconchain</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3892">#3892</a>)</li>
<li>Renamed the <code>tsc</code> script in all packages to <code>compile</code>; updates the corresponding <code>lerna run</code> usage in the main <code>package.json</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3894">#3894</a>)</li>
<li>moved deprecation warnings to postinstall scripts (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3917">#3917</a>)</li>
<li>Upgrade <code>@chainsafe/geth-dev-assistant</code> from <code>0.1.5</code> to <code>0.1.9</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3950">#3950</a>)</li>
<li>Replaced hardcoded infura link with Github Secret for some tests (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3943">#3943</a>)</li>
<li>Bump <code>elliptic</code> from <code>6.5.3</code> to <code>6.5.4</code> for <code>web3-eth-accounts</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3941">#3941</a>)</li>
<li>Bump <code>elliptic</code> from <code>6.5.3</code> to <code>6.5.4</code> for <code>web3-bzz</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3940">#3940</a>)</li>
<li>Bump <code>elliptic</code> from <code>6.5.3</code> to <code>6.5.4</code> for <code>web3-core-requestmanager</code> (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3945">#3945</a>)</li>
<li>Rewrite <code>web3-eth-iban</code> in ES6 (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/3955">#3955</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/web3/web3.js/commit/59b657b8c02af05575dc2d0ed321fa7d3aa8eaf6"><code>59b657b</code></a> Build for 1.8.0</li>
<li><a href="https://github.com/web3/web3.js/commit/e69ea861628f5bf17ed55d16051342644488b46e"><code>e69ea86</code></a> v1.8.0</li>
<li><a href="https://github.com/web3/web3.js/commit/09634f9ca4e5be7237fa968057bc60e657338f54"><code>09634f9</code></a> Manual build commit for 1.8.0-rc.0</li>
<li><a href="https://github.com/web3/web3.js/commit/81b06c91b674e85d0dbe762fac22b9355e7a030a"><code>81b06c9</code></a> v1.8.0-rc.0</li>
<li><a href="https://github.com/web3/web3.js/commit/a158594452cba79ae7c154b6f920715a938a6195"><code>a158594</code></a> npm i and CHANGELOG update for 1.8.0 release</li>
<li><a href="https://github.com/web3/web3.js/commit/f616e9f75b375ef5defdbb0ce44f11b9d14e1592"><code>f616e9f</code></a> docs: Fix example of tx usage (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/5402">#5402</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/1052540c3667b3cd009d842eba7db910970f11f5"><code>1052540</code></a> Adding Twitter button (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/5415">#5415</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/6311abe8cedd70a2863edee8adc381eb63515da4"><code>6311abe</code></a> Merge block tags support 5199 (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/5410">#5410</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/bd99127301ca2d427780125ecbfaabb38a4b53a0"><code>bd99127</code></a> 4.x info messages in 1.x (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/5412">#5412</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/a6ebb2ac9bd7cb45d4a3385fd7a760e1778292e6"><code>a6ebb2a</code></a> Nikos/5071/investigate signtransaction testcases (<a href="https://github-redirect.dependabot.com/ethereum/web3.js/issues/5377">#5377</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/ethereum/web3.js/compare/v1.3.4...v1.8.0">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~jdevcs">jdevcs</a>, a new releaser for web3 since your current version.</p>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-ibc-solidity/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-27 14:31:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/111" class=".btn">#111</a>
            </td>
            <td>
                <b>
                    Bump node-fetch and @truffle/hdwallet-provider
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [node-fetch](https://github.com/node-fetch/node-fetch) to 2.6.7 and updates ancestor dependency [@truffle/hdwallet-provider](https://github.com/trufflesuite/truffle/tree/HEAD/packages/hdwallet-provider). These dependencies need to be updated together.

Updates `node-fetch` from 1.7.3 to 2.6.7
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/node-fetch/node-fetch/releases">node-fetch's releases</a>.</em></p>
<blockquote>
<h2>v2.6.7</h2>
<h1>Security patch release</h1>
<p>Recommended to upgrade, to not leak sensitive cookie and authentication header information to 3th party host while a redirect occurred</p>
<h2>What's Changed</h2>
<ul>
<li>fix: don't forward secure headers to 3th party by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1453">node-fetch/node-fetch#1453</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/node-fetch/node-fetch/compare/v2.6.6...v2.6.7">https://github.com/node-fetch/node-fetch/compare/v2.6.6...v2.6.7</a></p>
<h2>v2.6.6</h2>
<h2>What's Changed</h2>
<ul>
<li>fix(URL): prefer built in URL version when available and fallback to whatwg by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1352">node-fetch/node-fetch#1352</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/node-fetch/node-fetch/compare/v2.6.5...v2.6.6">https://github.com/node-fetch/node-fetch/compare/v2.6.5...v2.6.6</a></p>
<h2>v2.6.2</h2>
<p>fixed main path in package.json</p>
<h2>v2.6.1</h2>
<p><strong>This is an important security release. It is strongly recommended to update as soon as possible.</strong></p>
<p>See <a href="https://github.com/node-fetch/node-fetch/blob/master/docs/CHANGELOG.md#v261">CHANGELOG</a> for details.</p>
<h2>v2.6.0</h2>
<p>See <a href="https://github.com/bitinn/node-fetch/blob/v2.6.0/CHANGELOG.md#v260">CHANGELOG</a>.</p>
<h2>v2.5.0</h2>
<p>See <a href="https://github.com/bitinn/node-fetch/blob/v2.5.0/CHANGELOG.md#v250">CHANGELOG</a>.</p>
<h2>v2.4.1</h2>
<p>See <a href="https://github.com/bitinn/node-fetch/blob/v2.4.1/CHANGELOG.md#v241">CHANGELOG</a>.</p>
<h2>v2.4.0</h2>
<p>See <a href="https://github.com/bitinn/node-fetch/blob/v2.4.0/CHANGELOG.md#v240">CHANGELOG</a>.</p>
<h2>v2.3.0</h2>
<p>See <a href="https://github.com/bitinn/node-fetch/blob/v2.3.0/CHANGELOG.md#v230">CHANGELOG</a>.</p>
<h2>v2.2.1</h2>
<p>See <a href="https://github.com/bitinn/node-fetch/blob/v2.2.1/CHANGELOG.md#v221">CHANGELOG</a>.</p>
<h2>Version 2.1.2</h2>
<ul>
<li>Fix: allow <code>Body</code> methods to work on ArrayBuffer<code>-backed </code>Body` objects</li>
<li>Fix: reject promise returned by <code>Body</code> methods when the accumulated <code>Buffer</code> exceeds the maximum size</li>
<li>Fix: support custom <code>Host</code> headers with any casing</li>
<li>Fix: support importing <code>fetch()</code> from TypeScript in <code>browser.js</code></li>
<li>Fix: handle the redirect response body properly</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/node-fetch/node-fetch/commit/1ef4b560a17e644a02a3bfdea7631ffeee578b35"><code>1ef4b56</code></a> backport of <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1449">#1449</a> (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1453">#1453</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/8fe5c4ea66b9b8187600e6d5ec9b1b6781f44009"><code>8fe5c4e</code></a> 2.x: Specify encoding as an optional peer dependency in package.json (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1310">#1310</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/f56b0c66d3dd2ef185436de1f2fd40f66bfea8f4"><code>f56b0c6</code></a> fix(URL): prefer built in URL version when available and fallback to whatwg (...</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/b5417aea6a3275932283a200214522e6ab53f1ea"><code>b5417ae</code></a> fix: import whatwg-url in a way compatible with ESM Node (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1303">#1303</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/18193c5922c64046b922e18faf41821290535f06"><code>18193c5</code></a> fix v2.6.3 that did not sending query params (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1301">#1301</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/ace7536c955556be742d9910566738630cc3c2a6"><code>ace7536</code></a> fix: properly encode url with unicode characters (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1291">#1291</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/152214ca2f6e2a5a17d71e4638114625d3be30c6"><code>152214c</code></a> Fix(package.json): Corrected main file path in package.json (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1274">#1274</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/b5e2e41b2b50bf2997720d6125accaf0dd68c0ab"><code>b5e2e41</code></a> update version number</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/2358a6c2563d1730a0cdaccc197c611949f6a334"><code>2358a6c</code></a> Honor the <code>size</code> option after following a redirect and revert data uri support</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/8c197f8982a238b3c345c64b17bfa92e16b4f7c4"><code>8c197f8</code></a> docs: Fix typos and grammatical errors in README.md (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/686">#686</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/node-fetch/node-fetch/compare/1.7.3...v2.6.7">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~endless">endless</a>, a new releaser for node-fetch since your current version.</p>
</details>
<br />

Updates `@truffle/hdwallet-provider` from 1.2.1 to 2.0.15
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/trufflesuite/truffle/releases"><code>@​truffle/hdwallet-provider</code>'s releases</a>.</em></p>
<blockquote>
<h2>v5.3.13 – Life is like...</h2>
<p>I guess it's true: you never know what you're going to get! 💝</p>
<p>This release fixes a bug to <code>truffle unbox</code> that caused community Truffle Boxes to fail to download. Thanks <a href="https://github.com/CaleTeeter"><code>@​CaleTeeter</code></a> and <a href="https://github.com/patrickalphac"><code>@​patrickalphac</code></a> for identifying this problem.</p>
<p>Apologies to anyone who ran into this bug... hope this fixes things for you! 🙇</p>
<h2>How to upgrade</h2>
<p>We recommend upgrading to the latest version of Truffle by running:</p>
<pre><code>npm uninstall -g truffle
npm install -g truffle
</code></pre>
<h2>Changelog</h2>
<h3>Bug fixes</h3>
<ul>
<li>Fix unbox to remove repo name restriction (<a href="https://github-redirect.dependabot.com/trufflesuite/truffle/pull/4145">#4145</a> by <a href="https://github.com/cds-amal"><code>@​cds-amal</code></a>)</li>
</ul>
<h3>Internal improvements</h3>
<ul>
<li>Allow a few missing values in artifactor/compile-common internals (<a href="https://github-redirect.dependabot.com/trufflesuite/truffle/pull/4126">#4126</a> by <a href="https://github.com/bergarces"><code>@​bergarces</code></a>)</li>
</ul>
<h2>v5.3.11 – Mrs. Malinda Russell's Rich Black Cake 🍰</h2>
<p>Salutations and happy Friday! 👋🏾</p>
<p>We have another release for you! This week offers a couple of bug fixes, internal improvements and version updates. <code>truffle unbox</code> will now recognize branches that have slashes, like <code>truffle unbox &lt;orgOrName&gt;/repo#branch/with/slashes</code>.  In case you didn't know you can <a href="https://www.trufflesuite.com/docs/truffle/advanced/creating-a-truffle-box">create your own Truffle boxes</a> which is a great way to bootstrap your Truffle project: hooray! :tada:</p>
<p>Enjoy, and as always please feel free to reach out through <a href="https://www.trufflesuite.com/community">one of these resources</a>.</p>
<h2>Changelog</h2>
<h3>Fixes</h3>
<ul>
<li>Handle unbox with slashes in branch name Fix/unbox 1676 (<a href="https://github-redirect.dependabot.com/trufflesuite/truffle/pull/4088">#4088</a> by <a href="https://github.com/cds-amal"><code>@​cds-amal</code></a>)</li>
<li>Remove --network option from <code>truffle compile</code> (<a href="https://github-redirect.dependabot.com/trufflesuite/truffle/pull/4116">#4116</a> by <a href="https://github.com/cds-amal"><code>@​cds-amal</code></a>)</li>
</ul>
<h3>Dependency updates</h3>
<ul>
<li>Update highlightjs-solidity to <code>v1.1.1</code> (<a href="https://github-redirect.dependabot.com/trufflesuite/truffle/pull/4111">#4111</a> by <a href="https://github.com/haltman-at"><code>@​haltman-at</code></a>)</li>
<li>Upgrade <code>@​truffle/codec</code>'s typedoc to <code>v0.20.36</code> (<a href="https://github-redirect.dependabot.com/trufflesuite/truffle/pull/4112">#4112</a> by <a href="https://github.com/gnidan"><code>@​gnidan</code></a>)</li>
</ul>
<h3>Internal improvements</h3>
<ul>
<li>Fix/testy rejections (<a href="https://github-redirect.dependabot.com/trufflesuite/truffle/pull/4118">#4118</a> by <a href="https://github.com/cds-amal"><code>@​cds-amal</code></a>)</li>
<li>Make consistent use of <code>import type</code> in most TS packages (<a href="https://github-redirect.dependabot.com/trufflesuite/truffle/pull/4110">#4110</a> by <a href="https://github.com/haltman-at"><code>@​haltman-at</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/trufflesuite/truffle/commit/1fbb6b1680b6c6eef5a98b7f21d7faae30c03994"><code>1fbb6b1</code></a> Publish</li>
<li><a href="https://github.com/trufflesuite/truffle/commit/778f348a6987abf4473a065cd02fb978619438ee"><code>778f348</code></a> bump to ganache@7.4.3</li>
<li><a href="https://github.com/trufflesuite/truffle/commit/0d96061f25e0927cd1d158b1636464ded86a57bb"><code>0d96061</code></a> Publish</li>
<li><a href="https://github.com/trufflesuite/truffle/commit/9c8eca99c541b135c659b483bc1c45593bdb93ef"><code>9c8eca9</code></a> Upgrade all packages to typescript@4.7.2</li>
<li><a href="https://github.com/trufflesuite/truffle/commit/2df562a36128b48cfbc022fecfde710c73561908"><code>2df562a</code></a> Standardize <code>@​types/node</code> for v12 LTS</li>
<li><a href="https://github.com/trufflesuite/truffle/commit/bc911496cdb3019a91398199dc9b260c6007df7f"><code>bc91149</code></a> Publish</li>
<li><a href="https://github.com/trufflesuite/truffle/commit/23610ab2848d8f4f627a15ad58040ef560273349"><code>23610ab</code></a> Revert &quot;Bump typescript to 4.7.2 and <code>@​types/node</code> to 18.6.1&quot;</li>
<li><a href="https://github.com/trufflesuite/truffle/commit/93f406b837d68b59c9b4abbb1d6f8b4d8642dd84"><code>93f406b</code></a> bump ganache to 7.4.0</li>
<li><a href="https://github.com/trufflesuite/truffle/commit/194ee5c077249e6c137c49018cfb2ce9be52a851"><code>194ee5c</code></a> Upgrade to typescript@4.7.2</li>
<li><a href="https://github.com/trufflesuite/truffle/commit/ba3f0164cd04f838b643f60f5aceecb5e303bd31"><code>ba3f016</code></a> Use latest node types, remove unused typeRoots</li>
<li>Additional commits viewable in <a href="https://github.com/trufflesuite/truffle/commits/@truffle/hdwallet-provider@2.0.15/packages/hdwallet-provider">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-ibc-solidity/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-27 14:31:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/109" class=".btn">#109</a>
            </td>
            <td>
                <b>
                    Bump elliptic and @ethersproject/signing-key
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [elliptic](https://github.com/indutny/elliptic) and [@ethersproject/signing-key](https://github.com/ethers-io/ethers.js/tree/HEAD/packages/signing-key). These dependencies needed to be updated together.
Updates `elliptic` from 6.5.3 to 6.5.4
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/indutny/elliptic/commit/43ac7f230069bd1575e1e4a58394a512303ba803"><code>43ac7f2</code></a> 6.5.4</li>
<li><a href="https://github.com/indutny/elliptic/commit/f4bc72be11b0a508fb790f445c43534307c9255b"><code>f4bc72b</code></a> package: bump deps</li>
<li><a href="https://github.com/indutny/elliptic/commit/441b7428b0e8f6636c42118ad2aaa186d3c34c3f"><code>441b742</code></a> ec: validate that a point before deriving keys</li>
<li><a href="https://github.com/indutny/elliptic/commit/e71b2d9359c5fe9437fbf46f1f05096de447de57"><code>e71b2d9</code></a> lib: relint using eslint</li>
<li><a href="https://github.com/indutny/elliptic/commit/8421a01aa3ff789c79f91eaf8845558a7be2b9fa"><code>8421a01</code></a> build(deps): bump elliptic from 6.4.1 to 6.5.3 (<a href="https://github-redirect.dependabot.com/indutny/elliptic/issues/231">#231</a>)</li>
<li>See full diff in <a href="https://github.com/indutny/elliptic/compare/v6.5.3...v6.5.4">compare view</a></li>
</ul>
</details>
<br />

Updates `@ethersproject/signing-key` from 5.0.9 to 5.7.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ethers-io/ethers.js/releases"><code>@​ethersproject/signing-key</code>'s releases</a>.</em></p>
<blockquote>
<h2>ethers/v5.7.0 (2022-08-18 16:17)</h2>
<ul>
<li>Update PocketProvider to newer URL format. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/2980">#2980</a>; <a href="https://github.com/ethers-io/ethers.js/commit/10d07ca6ec0622fb5a58b7e61b089166ebe8ea15">10d07ca</a>)</li>
<li>Add new ENS normalization specification for wider UTF-8 support. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/42">#42</a>, <a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/2376">#2376</a>, <a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/2754">#2754</a>; <a href="https://github.com/ethers-io/ethers.js/commit/14bf407bd948bb1bc91161032c93a67d81fb5a02">14bf407</a>, <a href="https://github.com/ethers-io/ethers.js/commit/fce9aaa7345a001a4a56bce66298ee23948d120c">fce9aaa</a>, <a href="https://github.com/ethers-io/ethers.js/commit/f274104865794f7f24db4244d591c39ad16f6688">f274104</a>)</li>
<li>Added ACTION_REJECTED error for UI-based Signers. (<a href="https://github.com/ethers-io/ethers.js/commit/d9897e0fdb5f9ca34822929c95a478634cc2a460">d9897e0</a>)</li>
<li>Include current baseFee in feeData for easier custom fee calculation. (<a href="https://github.com/ethers-io/ethers.js/commit/8314236143a300ae81c1dcc27a7a36640df22061">8314236</a>)</li>
<li>Add restrictions for new UTF-8 specification ENS names. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/42">#42</a>, <a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/2376">#2376</a>, <a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/2754">#2754</a>; <a href="https://github.com/ethers-io/ethers.js/commit/e52fbfbe70014e8033d3beed9c0dff2809eeef7f">e52fbfb</a>)</li>
<li>Expand the definition of a WebSocketLike. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/2843">#2843</a>; <a href="https://github.com/ethers-io/ethers.js/commit/00114d7b2f6e65a1cc974ea5b03abad568db4827">00114d7</a>)</li>
<li>Expanded type for queryFitler to allow string. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/2882">#2882</a>; <a href="https://github.com/ethers-io/ethers.js/commit/60da870cf2f8b71a4ec0c4bec67e28a11463038d">60da870</a>)</li>
<li>Added finalized and safe blockTags. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3091">#3091</a>; <a href="https://github.com/ethers-io/ethers.js/commit/549168cc4d0d3d18b12caa70bf5c58f4bcdc0175">549168c</a>)</li>
<li>Added arbitrum-goerli to Networks and AlchemyProvider. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3246">#3246</a>; <a href="https://github.com/ethers-io/ethers.js/commit/e72d13e651c236c0222265931285a466f1441134">e72d13e</a>)</li>
<li>Add EIP-712 type exports. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/221">#221</a>; <a href="https://github.com/ethers-io/ethers.js/commit/7ce41cdec706def0cd41f7f294c4d31bcb99a4ec">7ce41cd</a>)</li>
<li>Added optimism-goerli to AlchemyProvider. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3246">#3246</a>; <a href="https://github.com/ethers-io/ethers.js/commit/f1cb0d2dd654890836810e5c8d221e2664b2ae4a">f1cb0d2</a>)</li>
<li>Updated EtherscanProvider for new CommunityResource API throttling. (<a href="https://github.com/ethers-io/ethers.js/commit/6bd13c312fd53eaa78269d2c10e6bc373d67a2a9">6bd13c3</a>)</li>
<li>Fix old events from being emitted at the beginning of a filter. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3069">#3069</a>, <a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3094">#3094</a>; <a href="https://github.com/ethers-io/ethers.js/commit/ea2d2453a535a319ad55e7ca739ab1bcdb1432b7">ea2d245</a>)</li>
<li>Fixed Interface signautres missing strings as eventFragments. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3157">#3157</a>; <a href="https://github.com/ethers-io/ethers.js/commit/c004ae50f3df833380ca1540ef5024965ac8ef48">c004ae5</a>)</li>
<li>Fix bug in EIP1193Bridge forwarding to the wrong method. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3166">#3166</a>; <a href="https://github.com/ethers-io/ethers.js/commit/17676e9597ef7610443e3a7d7bb2967e7b509c26">17676e9</a>)</li>
<li>Use updated Web3 Secret Storage format for JSON wallets. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3075">#3075</a>; <a href="https://github.com/ethers-io/ethers.js/commit/6f57e8b1564a0b5c80b742775d02b9fad710c8e6">6f57e8b</a>)</li>
<li>Relaxed nameprep length requirement dropping RFC-5891 section 4.2.4. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3161">#3161</a>; <a href="https://github.com/ethers-io/ethers.js/commit/abdf2e30a5169d6ddd368f2bc3cdcd5feed25ae5">abdf2e3</a>)</li>
<li>Switch to hash.js for ripemd160 on node as it was removed from the default crypto provider in node 17. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3082">#3082</a>; <a href="https://github.com/ethers-io/ethers.js/commit/450694e25760d383f3fe3b299d181ebe5fd6ab06">450694e</a>)</li>
<li>Add optimism-kovan to EtherscanProvider. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3135">#3135</a>; <a href="https://github.com/ethers-io/ethers.js/commit/4d3e586701ca9ecd0ab63133d90185809d4f3811">4d3e586</a>)</li>
<li>Forward any blockTag along in the FallbackProvider during call. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3168">#3168</a>; <a href="https://github.com/ethers-io/ethers.js/commit/ab43e7d171b6191abc47318e76ddec4ee7156cdd">ab43e7d</a>)</li>
<li>Allow browser fetch option overrides. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3096">#3096</a>; <a href="https://github.com/ethers-io/ethers.js/commit/c309df8a3e988b00b4bc636622be78e246379f73">c309df8</a>)</li>
</ul>
<hr />
<p><strong>Embedding UMD with <a href="https://developer.mozilla.org/en-US/docs/Web/Security/Subresource_Integrity">SRI</a>:</strong></p>
<pre lang="html"><code>&lt;script type=&quot;text/javascript&quot;
        integrity=&quot;sha384-EQi5ynMqKKWGuwfjllsutXzvDo0ubfkYMhKrz5WJJB7PUXnkSo5qxWSy80hu/Zh9&quot;
        crossorigin=&quot;anonymous&quot;
        src=&quot;https://cdn-cors.ethers.io/lib/ethers-5.7.0.umd.min.js&quot;&gt;
&lt;/script&gt;
</code></pre>
<h2>ethers/v5.6.9 (2022-06-17 14:44)</h2>
<ul>
<li>Removed Ankr for Ropsten default provider; the merge seems to have broke it. (<a href="https://github.com/ethers-io/ethers.js/commit/3790671b424bfcfaaf27bab9f964c3ca407e8fea">3790671</a>)</li>
<li>Fix NonceManager for increment 0 and provided nonce. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3062">#3062</a>, <a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3085">#3085</a>; <a href="https://github.com/ethers-io/ethers.js/commit/0a28679994c844cef514f9e800c6cd8e1a21aa30">0a28679</a>)</li>
<li>Fixed topic filters for numeric types with string values. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3013">#3013</a>; <a href="https://github.com/ethers-io/ethers.js/commit/0078e026f1b438dd0976200ee16c38ec5a7788f6">0078e02</a>)</li>
</ul>
<hr />
<p><strong>Embedding UMD with <a href="https://developer.mozilla.org/en-US/docs/Web/Security/Subresource_Integrity">SRI</a>:</strong></p>
<pre lang="html"><code>&lt;script type=&quot;text/javascript&quot;
        integrity=&quot;sha384-qU3nvpskWirnJuSLmQWFfAFKbiN5+JKbAEEoTOcPYJu3s1xCe66b66sUER3x5wVF&quot;
        crossorigin=&quot;anonymous&quot;
        src=&quot;https://cdn-cors.ethers.io/lib/ethers-5.6.9.umd.min.js&quot;&gt;
&lt;/script&gt;
</code></pre>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ethers-io/ethers.js/blob/master/CHANGELOG.md"><code>@​ethersproject/signing-key</code>'s changelog</a>.</em></p>
<blockquote>
<h2>ethers/v5.7.0 (2022-08-18 16:17)</h2>
<ul>
<li>Update PocketProvider to newer URL format. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/2980">#2980</a>; <a href="https://github.com/ethers-io/ethers.js/commit/10d07ca6ec0622fb5a58b7e61b089166ebe8ea15">10d07ca</a>)</li>
<li>Add new ENS normalization specification for wider UTF-8 support. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/42">#42</a>, <a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/2376">#2376</a>, <a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/2754">#2754</a>; <a href="https://github.com/ethers-io/ethers.js/commit/14bf407bd948bb1bc91161032c93a67d81fb5a02">14bf407</a>, <a href="https://github.com/ethers-io/ethers.js/commit/fce9aaa7345a001a4a56bce66298ee23948d120c">fce9aaa</a>, <a href="https://github.com/ethers-io/ethers.js/commit/f274104865794f7f24db4244d591c39ad16f6688">f274104</a>)</li>
<li>Added ACTION_REJECTED error for UI-based Signers. (<a href="https://github.com/ethers-io/ethers.js/commit/d9897e0fdb5f9ca34822929c95a478634cc2a460">d9897e0</a>)</li>
<li>Include current baseFee in feeData for easier custom fee calculation. (<a href="https://github.com/ethers-io/ethers.js/commit/8314236143a300ae81c1dcc27a7a36640df22061">8314236</a>)</li>
<li>Add restrictions for new UTF-8 specification ENS names. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/42">#42</a>, <a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/2376">#2376</a>, <a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/2754">#2754</a>; <a href="https://github.com/ethers-io/ethers.js/commit/e52fbfbe70014e8033d3beed9c0dff2809eeef7f">e52fbfb</a>)</li>
<li>Expand the definition of a WebSocketLike. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/2843">#2843</a>; <a href="https://github.com/ethers-io/ethers.js/commit/00114d7b2f6e65a1cc974ea5b03abad568db4827">00114d7</a>)</li>
<li>Expanded type for queryFitler to allow string. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/2882">#2882</a>; <a href="https://github.com/ethers-io/ethers.js/commit/60da870cf2f8b71a4ec0c4bec67e28a11463038d">60da870</a>)</li>
<li>Added finalized and safe blockTags. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3091">#3091</a>; <a href="https://github.com/ethers-io/ethers.js/commit/549168cc4d0d3d18b12caa70bf5c58f4bcdc0175">549168c</a>)</li>
<li>Added arbitrum-goerli to Networks and AlchemyProvider. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3246">#3246</a>; <a href="https://github.com/ethers-io/ethers.js/commit/e72d13e651c236c0222265931285a466f1441134">e72d13e</a>)</li>
<li>Add EIP-712 type exports. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/221">#221</a>; <a href="https://github.com/ethers-io/ethers.js/commit/7ce41cdec706def0cd41f7f294c4d31bcb99a4ec">7ce41cd</a>)</li>
<li>Added optimism-goerli to AlchemyProvider. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3246">#3246</a>; <a href="https://github.com/ethers-io/ethers.js/commit/f1cb0d2dd654890836810e5c8d221e2664b2ae4a">f1cb0d2</a>)</li>
<li>Updated EtherscanProvider for new CommunityResource API throttling. (<a href="https://github.com/ethers-io/ethers.js/commit/6bd13c312fd53eaa78269d2c10e6bc373d67a2a9">6bd13c3</a>)</li>
<li>Fix old events from being emitted at the beginning of a filter. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3069">#3069</a>, <a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3094">#3094</a>; <a href="https://github.com/ethers-io/ethers.js/commit/ea2d2453a535a319ad55e7ca739ab1bcdb1432b7">ea2d245</a>)</li>
<li>Fixed Interface signautres missing strings as eventFragments. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3157">#3157</a>; <a href="https://github.com/ethers-io/ethers.js/commit/c004ae50f3df833380ca1540ef5024965ac8ef48">c004ae5</a>)</li>
<li>Fix bug in EIP1193Bridge forwarding to the wrong method. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3166">#3166</a>; <a href="https://github.com/ethers-io/ethers.js/commit/17676e9597ef7610443e3a7d7bb2967e7b509c26">17676e9</a>)</li>
<li>Use updated Web3 Secret Storage format for JSON wallets. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3075">#3075</a>; <a href="https://github.com/ethers-io/ethers.js/commit/6f57e8b1564a0b5c80b742775d02b9fad710c8e6">6f57e8b</a>)</li>
<li>Relaxed nameprep length requirement dropping RFC-5891 section 4.2.4. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3161">#3161</a>; <a href="https://github.com/ethers-io/ethers.js/commit/abdf2e30a5169d6ddd368f2bc3cdcd5feed25ae5">abdf2e3</a>)</li>
<li>Switch to hash.js for ripemd160 on node as it was removed from the default crypto provider in node 17. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3082">#3082</a>; <a href="https://github.com/ethers-io/ethers.js/commit/450694e25760d383f3fe3b299d181ebe5fd6ab06">450694e</a>)</li>
<li>Add optimism-kovan to EtherscanProvider. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3135">#3135</a>; <a href="https://github.com/ethers-io/ethers.js/commit/4d3e586701ca9ecd0ab63133d90185809d4f3811">4d3e586</a>)</li>
<li>Forward any blockTag along in the FallbackProvider during call. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3168">#3168</a>; <a href="https://github.com/ethers-io/ethers.js/commit/ab43e7d171b6191abc47318e76ddec4ee7156cdd">ab43e7d</a>)</li>
<li>Allow browser fetch option overrides. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3096">#3096</a>; <a href="https://github.com/ethers-io/ethers.js/commit/c309df8a3e988b00b4bc636622be78e246379f73">c309df8</a>)</li>
</ul>
<h2>ethers/v5.6.9 (2022-06-17 14:44)</h2>
<ul>
<li>Removed Ankr for Ropsten default provider; the merge seems to have broke it. (<a href="https://github.com/ethers-io/ethers.js/commit/3790671b424bfcfaaf27bab9f964c3ca407e8fea">3790671</a>)</li>
<li>Fix NonceManager for increment 0 and provided nonce. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3062">#3062</a>, <a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3085">#3085</a>; <a href="https://github.com/ethers-io/ethers.js/commit/0a28679994c844cef514f9e800c6cd8e1a21aa30">0a28679</a>)</li>
<li>Fixed topic filters for numeric types with string values. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3013">#3013</a>; <a href="https://github.com/ethers-io/ethers.js/commit/0078e026f1b438dd0976200ee16c38ec5a7788f6">0078e02</a>)</li>
</ul>
<h2>ethers/v5.6.8 (2022-05-24 11:50)</h2>
<ul>
<li>Update BN.js for hexstring bug fix. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/3017">#3017</a>; <a href="https://github.com/ethers-io/ethers.js/commit/30b716bf2cfd67ca38f76e344a26c0c2d5b75935">30b716b</a>, <a href="https://github.com/ethers-io/ethers.js/commit/a27ef825772f72071439c51e51180b6fcc64f03c">a27ef82</a>)</li>
</ul>
<h2>ethers/v5.6.7 (2022-05-20 19:11)</h2>
<ul>
<li>Add Skynet support. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/2853">#2853</a>, <a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/2866">#2866</a>; <a href="https://github.com/ethers-io/ethers.js/commit/13dd42c6c38d6977645555cdf7ab60354b0e2725">13dd42c</a>)</li>
<li>Fix WebWorker support in rollup files. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/2976">#2976</a>; <a href="https://github.com/ethers-io/ethers.js/commit/d06aa26d74eecd06149f908ce25dbaf867754c0e">d06aa26</a>)</li>
<li>Remove superfluous logging. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/2995">#2995</a>; <a href="https://github.com/ethers-io/ethers.js/commit/ed7e6a500e6087efcace8a5ff98997fbce2c6d6d">ed7e6a5</a>)</li>
<li>Add matic and optimism support to default provider. (<a href="https://github.com/ethers-io/ethers.js/commit/a3012977b1b10110ea15625754e8fc117e1ea147">a301297</a>)</li>
<li>Use case-insensitive schemes for getDefaultProvider. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/2320">#2320</a>; <a href="https://github.com/ethers-io/ethers.js/commit/8b62aeff9cce44cbd16ff41f8fc01ebb101f8265">8b62aef</a>)</li>
<li>Pad position in JSON-RPC getStorageAt calls. (<a href="https://github-redirect.dependabot.com/ethers-io/ethers.js/issues/2982">#2982</a>; <a href="https://github.com/ethers-io/ethers.js/commit/d5815cc4f1c13e5265c748d8afc4c085a97b1945">d5815cc</a>)</li>
</ul>
<h2>ethers/v5.6.6 (2022-05-12 17:29)</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ethers-io/ethers.js/commit/ec1b9583039a14a0e0fa15d0a2a6082a2f41cf5b"><code>ec1b958</code></a> admin: updated dist files</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/a71f51825571d1ea0fa997c1352d5b4d85643416"><code>a71f518</code></a> admin: update dist files</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/a27ef825772f72071439c51e51180b6fcc64f03c"><code>a27ef82</code></a> Lock versions for BigNumber fix (<a href="https://github.com/ethers-io/ethers.js/tree/HEAD/packages/signing-key/issues/3017">#3017</a>).</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/fc1e006575d59792fa97b4efb9ea2f8cca1944cf"><code>fc1e006</code></a> admin: update dist files</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/7b299dd9c97571b12916e3ae529540f3f2e5a367"><code>7b299dd</code></a> Enforce 32-byte private key length (2926).</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/b8cda5dffdcb688e38d7c6a0aec4c7b8b59c1af5"><code>b8cda5d</code></a> admin: updated dist files</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/73a46efea32c3f9a4833ed77896a216e3d3752a0"><code>73a46ef</code></a> admin: updated dist files</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/c2c0ce75039e7256b287f9a764188d08ed0b7296"><code>c2c0ce7</code></a> Updated dist files.</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/4e6d121fb8aa7327290afab7653364be8ddd8d81"><code>4e6d121</code></a> Updated dist files.</li>
<li><a href="https://github.com/ethers-io/ethers.js/commit/819b1ace5c9b16e29dc354ad80e0e5b71ac63c52"><code>819b1ac</code></a> Version bumps for bn.js and hash.js to match elliptic and fix some build tool...</li>
<li>Additional commits viewable in <a href="https://github.com/ethers-io/ethers.js/commits/v5.7.0/packages/signing-key">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-ibc-solidity/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-27 14:31:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/108" class=".btn">#108</a>
            </td>
            <td>
                <b>
                    Bump json-schema and jsprim
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [json-schema](https://github.com/kriszyp/json-schema) and [jsprim](https://github.com/joyent/node-jsprim). These dependencies needed to be updated together.
Updates `json-schema` from 0.2.3 to 0.4.0
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/kriszyp/json-schema/commit/f6f6a3b02d667aa4ba2d5d50cc19208c4462abfa"><code>f6f6a3b</code></a> Use a little more robust method of checking instances</li>
<li><a href="https://github.com/kriszyp/json-schema/commit/ef60987a9a14b9d9c739384460044ba53cd9b9a2"><code>ef60987</code></a> Update version</li>
<li><a href="https://github.com/kriszyp/json-schema/commit/b62f1da1ff5442f23443d6be6a92d00e65cba93a"><code>b62f1da</code></a> Protect against constructor modification, <a href="https://github-redirect.dependabot.com/kriszyp/json-schema/issues/84">#84</a></li>
<li><a href="https://github.com/kriszyp/json-schema/commit/fb427cd4d175684786e4b2538718e72453e825e9"><code>fb427cd</code></a> Link to json-schema-org repository in addition to site, fixes <a href="https://github-redirect.dependabot.com/kriszyp/json-schema/issues/54">#54</a></li>
<li><a href="https://github.com/kriszyp/json-schema/commit/22f146111f541d9737e832823699ad3528ca7741"><code>22f1461</code></a> Don't allow <strong>proto</strong> property to be used for schema default/coerce, fixes <a href="https://github-redirect.dependabot.com/kriszyp/json-schema/issues/84">#84</a></li>
<li><a href="https://github.com/kriszyp/json-schema/commit/c52a27c653428149e4f9fb776d5e110d04639a9c"><code>c52a27c</code></a> Get basic test to pass</li>
<li><a href="https://github.com/kriszyp/json-schema/commit/b3f42b3331608fe83b6cc267c5fc513ec1b839ed"><code>b3f42b3</code></a> Add security policy</li>
<li><a href="https://github.com/kriszyp/json-schema/commit/3b0cec3042a5aac5c967fd43475f5edc4c5b6eff"><code>3b0cec3</code></a> Update version</li>
<li><a href="https://github.com/kriszyp/json-schema/commit/c28470f2d64bace29c73d140f9c6876e3c3a9fef"><code>c28470f</code></a> Update readme to acknowledge the state of the package</li>
<li><a href="https://github.com/kriszyp/json-schema/commit/7dff9cd2c35c31ff3c43fa4e38737c94283dd3d3"><code>7dff9cd</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/kriszyp/json-schema/issues/81">#81</a> from hodovani/patch-1</li>
<li>Additional commits viewable in <a href="https://github.com/kriszyp/json-schema/compare/v0.2.3...v0.4.0">compare view</a></li>
</ul>
</details>
<br />

Updates `jsprim` from 1.4.1 to 1.4.2
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/TritonDataCenter/node-jsprim/blob/v1.4.2/CHANGES.md">jsprim's changelog</a>.</em></p>
<blockquote>
<h2>v1.4.2 (2021-11-29)</h2>
<ul>
<li><a href="https://github-redirect.dependabot.com/joyent/node-jsprim/issues/35">#35</a> Backport json-schema 0.4.0 to version 1.4.x</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/TritonDataCenter/node-jsprim/commit/5c8475fd44567e459b1b73b82f2669c39a0642b8"><code>5c8475f</code></a> <a href="https://github-redirect.dependabot.com/joyent/node-jsprim/issues/35">joyent/node-jsprim#35</a> Backport json-schema 0.4.0 to version 1.4.x</li>
<li>See full diff in <a href="https://github.com/joyent/node-jsprim/compare/v1.4.1...v1.4.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~bahamat">bahamat</a>, a new releaser for jsprim since your current version.</p>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-ibc-solidity/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-27 14:31:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/107" class=".btn">#107</a>
            </td>
            <td>
                <b>
                    Add relayer address to IBC module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix #70 

Signed-off-by: Jun Kimura <jun.kimura@datachain.jp>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-27 14:10:20 +0000 UTC
    </div>
</div>

