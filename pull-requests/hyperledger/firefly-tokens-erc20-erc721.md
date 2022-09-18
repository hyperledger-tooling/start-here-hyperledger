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
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/92" class=".btn">#92</a>
            </td>
            <td>
                <b>
                    Bump undici, hardhat and @nomiclabs/hardhat-etherscan in /samples/solidity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [undici](https://github.com/nodejs/undici), [hardhat](https://github.com/nomiclabs/hardhat) and [@nomiclabs/hardhat-etherscan](https://github.com/nomiclabs/hardhat). These dependencies needed to be updated together.
Updates `undici` from 4.16.0 to 5.10.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nodejs/undici/releases">undici's releases</a>.</em></p>
<blockquote>
<h2>v5.10.0</h2>
<h2>What's Changed</h2>
<ul>
<li>fix(fetch): allow custom implementation of AbortSignal by <a href="https://github.com/SukkaW"><code>@​SukkaW</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1608">nodejs/undici#1608</a></li>
<li>fix: make mock intercept agnostic to query key ordering by <a href="https://github.com/James1x0"><code>@​James1x0</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1607">nodejs/undici#1607</a></li>
<li>fix: support <code>ArrayBufferView</code> and <code>ArrayBuffer</code> as body by <a href="https://github.com/LiviaMedeiros"><code>@​LiviaMedeiros</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1584">nodejs/undici#1584</a></li>
<li>fix: allow third party AbortControllers by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1609">nodejs/undici#1609</a></li>
<li>feat(fetch): implement spec compliant integrity checks by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1613">nodejs/undici#1613</a></li>
<li>avoid body reordering on really fast lines by <a href="https://github.com/mcollina"><code>@​mcollina</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1615">nodejs/undici#1615</a></li>
<li>fix: use FinalizationRegistry compat if global is missing by <a href="https://github.com/Kikobeats"><code>@​Kikobeats</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1545">nodejs/undici#1545</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/SukkaW"><code>@​SukkaW</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1608">nodejs/undici#1608</a></li>
<li><a href="https://github.com/James1x0"><code>@​James1x0</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1607">nodejs/undici#1607</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.9.1...v5.10.0">https://github.com/nodejs/undici/compare/v5.9.1...v5.10.0</a></p>
<h2>v5.9.1</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: don't timeout while waiting for client to send request (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1604">#1604</a>)</li>
<li>Fix array headers by <a href="https://github.com/mateonunez"><code>@​mateonunez</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1598">nodejs/undici#1598</a></li>
<li>fix(fetch): implement fully read body algorithm by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1597">nodejs/undici#1597</a></li>
<li>fix: add support for <code>integrity</code> option to Fetch by <a href="https://github.com/jelmervdl"><code>@​jelmervdl</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1596">nodejs/undici#1596</a></li>
<li>fix(File): respect typed array <code>byteOffset</code> and <code>byteLength</code> by <a href="https://github.com/mrbbot"><code>@​mrbbot</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1601">nodejs/undici#1601</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/mateonunez"><code>@​mateonunez</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1598">nodejs/undici#1598</a></li>
<li><a href="https://github.com/jelmervdl"><code>@​jelmervdl</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1596">nodejs/undici#1596</a></li>
<li><a href="https://github.com/mrbbot"><code>@​mrbbot</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1601">nodejs/undici#1601</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.8.2...v5.9.1">https://github.com/nodejs/undici/compare/v5.8.2...v5.9.1</a></p>
<h2>v5.8.2</h2>
<h2>⚠️ Security Release ⚠️</h2>
<ul>
<li>CRLF Injection in Nodejs ‘undici’ via Content-Type <a href="https://github.com/nodejs/undici/security/advisories/GHSA-f772-66g8-q5h3">GHSA-f772-66g8-q5h3</a> CVE-2022-35948</li>
<li><code>undici.request</code> vulnerable to SSRF using absolute URL on <code>pathname</code> <a href="https://github.com/nodejs/undici/security/advisories/GHSA-8qr4-xgw6-wmr3">GHSA-8qr4-xgw6-wmr3</a> CVE-2022-35949</li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>docs: mock different endpoints in a single file by <a href="https://github.com/ritvik130"><code>@​ritvik130</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1589">nodejs/undici#1589</a></li>
<li>feat(webidl): better error message for ByteString converter by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1591">nodejs/undici#1591</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/ritvik130"><code>@​ritvik130</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1589">nodejs/undici#1589</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.8.1...v5.8.2">https://github.com/nodejs/undici/compare/v5.8.1...v5.8.2</a></p>
<h2>v5.8.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Do not decode the body while we are following a redirect by <a href="https://github.com/mcollina"><code>@​mcollina</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1554">nodejs/undici#1554</a></li>
<li>docs: Fix spelling/grammar in &quot;Mocking Request&quot; by <a href="https://github.com/meyfa"><code>@​meyfa</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1555">nodejs/undici#1555</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nodejs/undici/commit/6a87bfb38b3f4a28be81d2cc44a80083a0e4f798"><code>6a87bfb</code></a> Bumped v5.10.0</li>
<li><a href="https://github.com/nodejs/undici/commit/b0f0f3112a243910b9093b7e9290bc3270cdf0bd"><code>b0f0f31</code></a> fix: use FinalizationRegistry compat if global is missing (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1545">#1545</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/5cb0bacef31ea3b7a3b2ff8586768844b500da99"><code>5cb0bac</code></a> avoid body reordering on really fast lines (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1615">#1615</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/21fdda54ca290456083874ab0727e3c343ee8e45"><code>21fdda5</code></a> feat(fetch): implement spec compliant integrity checks (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1613">#1613</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/417e7abdafed8b81fda7daf4ffcce77860e2c6dd"><code>417e7ab</code></a> fix: allow third party AbortControllers (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1609">#1609</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/8549a9402c46034d6d28b2f6f65d934736e51a59"><code>8549a94</code></a> fix: support <code>ArrayBufferView</code> and <code>ArrayBuffer</code> as body (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1584">#1584</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/e46d8bff81ccc1eaeffabc36a2f690c647ab4cd1"><code>e46d8bf</code></a> Add query key ordering fix (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1607">#1607</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/d83c1e2a9867023362f1322866784b9e332b22cf"><code>d83c1e2</code></a> fix(fetch): allow custom implementation of AbortSignal (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1608">#1608</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/5890e16ddd2703151ce0be0a468e13d685b89f60"><code>5890e16</code></a> 5.9.1</li>
<li><a href="https://github.com/nodejs/undici/commit/ecae314c90534d665b6a2b1da085cff80c138c1b"><code>ecae314</code></a> fix: don't timeout while waiting for client to send request (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1604">#1604</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/nodejs/undici/compare/v4.16.0...v5.10.0">compare view</a></li>
</ul>
</details>
<br />

Updates `hardhat` from 2.9.3 to 2.11.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nomiclabs/hardhat/releases">hardhat's releases</a>.</em></p>
<blockquote>
<h2>Hardhat v2.11.2</h2>
<p>This new version of Hardhat brings several fixes and improvements:</p>
<ul>
<li>Solidity 0.8.17 is now supported and used by default in the sample projects.</li>
<li>When forking a network, the disk cache is always used (thanks <a href="https://github.com/bernard-wagner"><code>@​bernard-wagner</code></a>!)</li>
<li>Stack traces are shown by default in CI servers</li>
<li>We fixed a problem related to the validation of the <code>eth_getStorageAt</code> being too restrictive (thanks <a href="https://github.com/aathan"><code>@​aathan</code></a>!)</li>
<li>Reverted an unintentional breaking change in the type of the resolved config</li>
<li>Improved the heuristic for detecting that a contract deployment failed because the code size was too large</li>
</ul>
<h2>Hardhat v2.11.1</h2>
<p>This release fixes a couple of bugs in v2.11.0:</p>
<ul>
<li>Some chains, like Polygon, were causing issues when they were forked</li>
<li>The WASM version of the solidity compiler, which is used in some machines, was not being correctly downloaded.</li>
</ul>
<h2>Hardhat v2.11.0 — The Merge support and <em>fast</em> compilation</h2>
<p>We are excited to release this new version of Hardhat, as it makes Hardhat Network compatible with The Merge and makes our compilation much faster. Read on to learn more about these and other improvements.</p>
<h2>Support for The Merge</h2>
<p>Hardhat Network now has support for The Merge. To try it out, use the new <code>merge</code> hardfork setting. This hardfork is not selected by default, but you can enable it in your config:</p>
<pre lang="jsx"><code>module.exports = {
  networks: {
    hardhat: {
      hardfork: &quot;merge&quot;
    }
  }  
};
</code></pre>
<p>Selecting this new hardfork will introduce a few changes to how Hardhat Network runs, but your contracts should still work without any modification. The rest of this section explains what these changes are.</p>
<p>The <code>DIFFICULTY</code> opcode (now renamed to <code>PREVRANDAO</code>) will return a pseudo-random value. This value is also exposed in the block header as <code>mixHash</code>.</p>
<p>You can use the new <code>hardhat_setPrevRandao</code> RPC method to modify the value returned by <code>DIFFICULTY</code>/<code>PREVRANDAO</code> in the next block. We recommend using the <a href="https://hardhat.org/hardhat-network-helpers/docs/reference#setprevrandao(prevrandao)"><code>setPrevRandao</code> network helper</a> for this.</p>
<p>Hardhat Network’s JSON-RPC now accepts the new <code>safe</code> and <code>finalized</code> block tags, which in Hardhat Network are just aliases for the <code>latest</code> block tag, and correspond to the latest block.</p>
<h2>Faster compilation</h2>
<p>We optimized Hardhat’s compilation pipeline, <strong>significantly</strong> reducing the overhead it adds on top of <code>solc</code>. Compilation takes 40% less in most workflows, with a few taking 90% less!</p>
<p>How much of an impact this has depends on the size of your project, setup, and workflow, so we’ll explore two examples here, running the same benchmarks on each.</p>
<p>We’ll focus on a few different workflows:</p>
<ul>
<li>Clean compilation: compiling the entire codebase from scratch</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/a3b4d9a67382d9a0e751fc3ac3abe61a0bc31321"><code>a3b4d9a</code></a> Run changesets version</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/b649a575b616484282c5d42c4889420f657e7acf"><code>b649a57</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/nomiclabs/hardhat/issues/3179">#3179</a> from NomicFoundation/upgrade-toolbox-sample-projects</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/59d262b8bbe7b80c120699e31ff461854bfd6883"><code>59d262b</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/nomiclabs/hardhat/issues/3169">#3169</a> from ololade97/patch-1</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/97b99e011d97db1fdc56d287319ee2ad46a4a148"><code>97b99e0</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/nomiclabs/hardhat/issues/3148">#3148</a> from NomicFoundation/fork-cache-not-working-for-opti...</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/7ca17a4097209620b592d2f3f653be917ae3f468"><code>7ca17a4</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/nomiclabs/hardhat/issues/3160">#3160</a> from NomicFoundation/ensure-support-for-solidity-081...</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/f7d38434542241c77d9997d203ef780c7c900e28"><code>f7d3843</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/nomiclabs/hardhat/issues/3177">#3177</a> from NomicFoundation/relax-eth-storage-at-validation</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/f4fd6a27ed6608c2b23d985bdb9725847caf63c8"><code>f4fd6a2</code></a> Create nervous-dolls-tell.md</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/7991b38053445e938643a3a6e2bab26327540c96"><code>7991b38</code></a> Make hardhat-ethers test more reliable</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/10f03fb99c59bacfcca6dea5dd0435bc8851b52e"><code>10f03fb</code></a> Add more test cases for storage slot</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/1cfee28db17df07184594a721b353a1480e8fc57"><code>1cfee28</code></a> Create big-cooks-decide.md</li>
<li>Additional commits viewable in <a href="https://github.com/nomiclabs/hardhat/compare/hardhat@2.9.3...hardhat@2.11.2">compare view</a></li>
</ul>
</details>
<br />

Updates `@nomiclabs/hardhat-etherscan` from 3.0.3 to 3.1.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nomiclabs/hardhat/releases"><code>@​nomiclabs/hardhat-etherscan</code>'s releases</a>.</em></p>
<blockquote>
<h2><code>@​nomiclabs/hardhat-etherscan</code> v3.1.0</h2>
<p>This release adds support for verifying contracts in chains that are not included by default in <code>hardhat-etherscan</code>.</p>
<p>To do this, you add the network you want to verify in the <code>customChains</code> entry of the Etherscan configuration:</p>
<pre lang="js"><code>etherscan: {
  apiKey: {
    customNetwork: &quot;&lt;custom-network-api-key&gt;&quot;
  },
  customChains: [
    {
      network: &quot;customNetwork&quot;,
      chainId: 12345,
      urls: {
        apiURL: &quot;https://api-custom-network.etherscan.io/api&quot;,
        browserURL: &quot;https://custom-network.etherscan.io&quot;
      }
    }
  ]
}
</code></pre>
<p>You can read more about this <a href="https://github.com/NomicFoundation/hardhat/tree/master/packages/hardhat-etherscan#adding-support-for-other-networks">here</a>.</p>
<p>Thanks to <a href="https://github.com/no2chem"><code>@​no2chem</code></a> for the initial implementation and to <a href="https://github.com/calvinaco"><code>@​calvinaco</code></a> who helped test this.</p>
<h2><code>@​nomiclabs/hardhat-etherscan</code> v3.0.4</h2>
<p>This release adds support for verifying contracts in the Sepolia testnet (thanks <a href="https://github.com/pcaversaccio"><code>@​pcaversaccio</code></a>!)</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/ebde4261403ddb84c85befa7248a1a3e51c3df4e"><code>ebde426</code></a> Version Packages</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/fb33e8b94690dab28c3e2279aacf0ef27e240b60"><code>fb33e8b</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/nomiclabs/hardhat/issues/2805">#2805</a> from NomicFoundation/export-missing-artifacts-method</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/3770a5bbc00f302ac0cfa66b0d3a7aea0df54c04"><code>3770a5b</code></a> Expose missing method in the artifacts interface</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/64456a03fcdd75cc7b22ca1d4085e72beab68e73"><code>64456a0</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/nomiclabs/hardhat/issues/2661">#2661</a> from NomicFoundation/hardhat-etherscan-custom-explorer</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/990b1f7773fd1760496f38a51c4e2c51acea5be7"><code>990b1f7</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/nomiclabs/hardhat/issues/2763">#2763</a> from NomicFoundation/francovictorio/hh-697/test-util...</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/50e29e471e8d87bba5ecfa74baabd38f2bd6177d"><code>50e29e4</code></a> Add warnings about beta version</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/bbe43b1c57727c996ab301675ad5bcdc322b5089"><code>bbe43b1</code></a> Add installation instructions</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/575239c0960cd0ef806d25f51e4bce733fa2c281"><code>575239c</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/nomiclabs/hardhat/issues/2793">#2793</a> from NomicFoundation/gene/hh-696</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/980f3a4492f53c89fff971a7d4d1138d45f4fe62"><code>980f3a4</code></a> Use multiple lines in example snippets</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/8dcddebfbda4654744bf9a6e058508126fb2318f"><code>8dcddeb</code></a> ran lint:fix</li>
<li>Additional commits viewable in <a href="https://github.com/nomiclabs/hardhat/compare/@nomiclabs/hardhat-etherscan@3.0.3...@nomiclabs/hardhat-etherscan@3.1.0">compare view</a></li>
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
        Created At 2022-09-16 16:03:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/91" class=".btn">#91</a>
            </td>
            <td>
                <b>
                    Bump @openzeppelin/contracts from 4.7.1 to 4.7.3 in /samples/solidity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) from 4.7.1 to 4.7.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/releases"><code>@​openzeppelin/contracts</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.7.3</h2>
<p>:warning: This is a patch for a high severity issue. For more information <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-4h98-2769-gh6h">visit the security advisory</a>.</p>
<h3>Breaking changes</h3>
<ul>
<li><code>ECDSA</code>: <code>recover(bytes32,bytes)</code> and <code>tryRecover(bytes32,bytes)</code> no longer accept compact signatures to prevent malleability. Compact signature support remains available using <code>recover(bytes32,bytes32,bytes32)</code> and <code>tryRecover(bytes32,bytes32,bytes32)</code>.</li>
</ul>
<h2>v4.7.2</h2>
<p>:warning: This is a patch for three issues, including a high severity issue in <code>GovernorVotesQuorumFraction</code>. For more information visit the security advisories (<a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-xrc4-737v-9q75">1</a>, <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-7grf-83vw-6f5x">2</a>, <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-9j3m-g383-29qr">3</a>).</p>
<ol>
<li><code>GovernorVotesQuorumFraction</code>: Fixed quorum updates so they do not affect past proposals that failed due to lack of quorum. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3561">#3561</a>)</li>
<li><code>ERC165Checker</code>: Added protection against large returndata. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3587">#3587</a>)</li>
<li><code>LibArbitrumL2</code>, <code>CrossChainEnabledArbitrumL2</code>: Fixed detection of cross-chain calls for EOAs. Previously, calls from EOAs would be classified as cross-chain calls. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3578">#3578</a>)</li>
</ol>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/CHANGELOG.md"><code>@​openzeppelin/contracts</code>'s changelog</a>.</em></p>
<blockquote>
<h2>4.7.3</h2>
<h3>Breaking changes</h3>
<ul>
<li><code>ECDSA</code>: <code>recover(bytes32,bytes)</code> and <code>tryRecover(bytes32,bytes)</code> no longer accept compact signatures to prevent malleability. Compact signature support remains available using <code>recover(bytes32,bytes32,bytes32)</code> and <code>tryRecover(bytes32,bytes32,bytes32)</code>.</li>
</ul>
<h2>4.7.2</h2>
<ul>
<li><code>LibArbitrumL2</code>, <code>CrossChainEnabledArbitrumL2</code>: Fixed detection of cross-chain calls for EOAs. Previously, calls from EOAs would be classified as cross-chain calls. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3578">#3578</a>)</li>
<li><code>GovernorVotesQuorumFraction</code>: Fixed quorum updates so they do not affect past proposals that failed due to lack of quorum. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3561">#3561</a>)</li>
<li><code>ERC165Checker</code>: Added protection against large returndata. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3587">#3587</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/ecd2ca2cd7cac116f7a37d0e474bbb3d7d5e1c4d"><code>ecd2ca2</code></a> 4.7.3</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/e1878ace8c2908b85d39f9925c68c6f738cf3325"><code>e1878ac</code></a> Fix ECDSA signature malleability (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3610">#3610</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/64e48203cecad94f02de9891ecdeed4d629c6dae"><code>64e4820</code></a> 4.7.2</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/b66fe1606a173f2b78694567b543d480cb39cfe4"><code>b66fe16</code></a> Update changelog</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/8fb5f5774e3e8cfc10699f58749d8a34ec9d3e86"><code>8fb5f57</code></a> Avoid returnbomb in ERC165Checker (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3587">#3587</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/67b2572c6a050563990637f5017af8eeda111b21"><code>67b2572</code></a> Keep track of historical quorum values (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3561">#3561</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/4337192dc02b64785885787e80126f93ee3f2659"><code>4337192</code></a> Fix arbitrum L1 to L2 crosschain call detection (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3578">#3578</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/41c7b25a65f636feaef7f0dc932ec4c44baa12f3"><code>41c7b25</code></a> Fix error in documentation and typo (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3567">#3567</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/e15862f2893f024e0872f0f1abcf275c4b436834"><code>e15862f</code></a> Remove test for feature not in 4.7</li>
<li>See full diff in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/compare/v4.7.1...v4.7.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts&package-manager=npm_and_yarn&previous-version=4.7.1&new-version=4.7.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-09-16 16:03:01 +0000 UTC
    </div>
</div>

