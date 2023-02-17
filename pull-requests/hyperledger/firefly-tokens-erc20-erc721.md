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
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/123" class=".btn">#123</a>
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
                Bumps [undici](https://github.com/nodejs/undici) to 5.19.1 and updates ancestor dependencies [undici](https://github.com/nodejs/undici), [hardhat](https://github.com/nomiclabs/hardhat) and [@nomiclabs/hardhat-etherscan](https://github.com/nomiclabs/hardhat). These dependencies need to be updated together.

Updates `undici` from 4.16.0 to 5.19.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nodejs/undici/releases">undici's releases</a>.</em></p>
<blockquote>
<h2>v5.19.1</h2>
<h2>⚠️ Security Release ⚠️</h2>
<ul>
<li><a href="https://github.com/nodejs/undici/security/advisories/GHSA-r6ch-mqf9-qc9w">Regular Expression Denial of Service in Headers</a> with CVE-2023-24807</li>
<li><a href="https://github.com/nodejs/undici/security/advisories/GHSA-5r9g-qh6m-jxff">CRLF Injection in Nodejs ‘undici’ via host</a> with CVE-2023-23936</li>
</ul>
<p>This release is part of the Node.js security release train: <a href="https://nodejs.org/en/blog/vulnerability/february-2023-security-releases/">https://nodejs.org/en/blog/vulnerability/february-2023-security-releases/</a></p>
<h2>v5.19.0</h2>
<h2>What's Changed</h2>
<ul>
<li>fix(fetch): raise AbortSignal max event listeners by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1910">nodejs/undici#1910</a></li>
<li>fix: content-disposition header parsing by <a href="https://github.com/climba03003"><code>@​climba03003</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1911">nodejs/undici#1911</a></li>
<li>fix: remove test by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1916">nodejs/undici#1916</a></li>
<li>feat: add Headers.prototype.getSetCookie by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1915">nodejs/undici#1915</a></li>
<li>fix(headers): clone getSetCookie list &amp; add getSetCookie type by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1917">nodejs/undici#1917</a></li>
<li>doc(mock): update out-of-date reply documentation by <a href="https://github.com/p9f"><code>@​p9f</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1913">nodejs/undici#1913</a></li>
<li>fix(types): add missing keepAlive params by <a href="https://github.com/SkeLLLa"><code>@​SkeLLLa</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1918">nodejs/undici#1918</a></li>
<li>Make the fetch() abort test pass locally, on Linux and Mac, Node 18/19. by <a href="https://github.com/mcollina"><code>@​mcollina</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1927">nodejs/undici#1927</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/climba03003"><code>@​climba03003</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1911">nodejs/undici#1911</a></li>
<li><a href="https://github.com/p9f"><code>@​p9f</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1913">nodejs/undici#1913</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.18.0...v5.19.0">https://github.com/nodejs/undici/compare/v5.18.0...v5.19.0</a></p>
<h2>v5.18.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Add ability to set TCP keepalive by <a href="https://github.com/xconverge"><code>@​xconverge</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1904">nodejs/undici#1904</a></li>
<li>use faster timers by <a href="https://github.com/ronag"><code>@​ronag</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1908">nodejs/undici#1908</a></li>
<li>fix: ensure header value is a string by <a href="https://github.com/ronag"><code>@​ronag</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1899">nodejs/undici#1899</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.17.1...v5.18.0">https://github.com/nodejs/undici/compare/v5.17.1...v5.18.0</a></p>
<h2>v5.17.1</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: bad buffer slice (<a href="https://github.com/nodejs/undici/commit/d2be675575512794dcd41b9683b209fc15368154">https://github.com/nodejs/undici/commit/d2be675575512794dcd41b9683b209fc15368154</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.17.0...v5.17.1">https://github.com/nodejs/undici/compare/v5.17.0...v5.17.1</a></p>
<h2>v5.17.0</h2>
<h2>What's Changed</h2>
<ul>
<li>fix(wpts): Blob is a global getter in &gt;=v19.x.x by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1880">nodejs/undici#1880</a></li>
<li>doc: fix anchor links dispatcher.stream by <a href="https://github.com/RafaelGSS"><code>@​RafaelGSS</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1881">nodejs/undici#1881</a></li>
<li>wpt: make runner more resilient by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1884">nodejs/undici#1884</a></li>
<li>Make test pass in v19.x by <a href="https://github.com/mcollina"><code>@​mcollina</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1879">nodejs/undici#1879</a></li>
<li>Correct the type of DispatchOptions[&quot;headers&quot;] by <a href="https://github.com/pan93412"><code>@​pan93412</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1896">nodejs/undici#1896</a></li>
<li>perf(content-type parser): faster string collector by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1894">nodejs/undici#1894</a></li>
<li>feat: expose content-type parser by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1895">nodejs/undici#1895</a></li>
<li>fix(types): Update DispatchOptions type for missing &quot;blocking&quot; by <a href="https://github.com/xconverge"><code>@​xconverge</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1889">nodejs/undici#1889</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nodejs/undici/commit/984d53bad97c98529424a7f3bef6be1d0e76d039"><code>984d53b</code></a> Bumped v5.19.1</li>
<li><a href="https://github.com/nodejs/undici/commit/6c32c0fd5b874328e5e1f635e2cc431aa21cddab"><code>6c32c0f</code></a> lint fixes</li>
<li><a href="https://github.com/nodejs/undici/commit/f2324e549943f0b0937b09fb1c0c16cc7c93abdf"><code>f2324e5</code></a> Merge pull request from GHSA-r6ch-mqf9-qc9w</li>
<li><a href="https://github.com/nodejs/undici/commit/a2eff05401358f6595138df963837c24348f2034"><code>a2eff05</code></a> Merge pull request from GHSA-5r9g-qh6m-jxff</li>
<li><a href="https://github.com/nodejs/undici/commit/f5c89e5c87c7d702996b152c4ad86302b60c4181"><code>f5c89e5</code></a> Bumped v5.19.0</li>
<li><a href="https://github.com/nodejs/undici/commit/f7c6c6a4a2aef7ee3b8207c4eeab700cb0cfc7dc"><code>f7c6c6a</code></a> Make the fetch() abort test pass locally, on Linux and Mac, Node 18 and 19 (#...</li>
<li><a href="https://github.com/nodejs/undici/commit/aebb232d22e9adafce015b985093114a95b560f0"><code>aebb232</code></a> fix(types): add missing keepAlive params (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1918">#1918</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/e155c6db5cec9bc577d548fa7c7378013631c79c"><code>e155c6d</code></a> doc(mock): update out-of-date reply documentation (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1913">#1913</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/87fa73498d6014a33989179cfaa4347dcb29600f"><code>87fa734</code></a> fix(headers): clone getSetCookie list &amp; add getSetCookie type (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1917">#1917</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/ba5ef44b71eff5a86a8473850a326ff7392664d3"><code>ba5ef44</code></a> feat: add Headers.prototype.getSetCookie (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1915">#1915</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/nodejs/undici/compare/v4.16.0...v5.19.1">compare view</a></li>
</ul>
</details>
<br />

Updates `hardhat` from 2.9.3 to 2.12.7
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nomiclabs/hardhat/releases">hardhat's releases</a>.</em></p>
<blockquote>
<h2>hardhat@2.12.7</h2>
<h1>Changes</h1>
<ul>
<li>
<p>e443b3667: Added an option in Hardhat Network to allow mining blocks with the same timestamp</p>
</li>
<li>
<p>c23a1cac4: Added support for the <code>http_proxy</code> environment variable. When this variable is set, Hardhat will send its requests through the given proxy for things like JSON-RPC requests, mainnet forking and downloading compilers.</p>
<p>We also removed support for the <code>HTTP_PROXY</code> and <code>HTTPS_PROXY</code> environment variables, since <code>http_proxy</code> is the most commonly used environment variable for this kind of thing. Those variables could only be used for downloading compilers.</p>
<p>Finally, we also added support for <code>no_proxy</code>, which accepts a comma separated list of hosts or <code>&quot;*&quot;</code>. Any host included in this list will not be proxied.</p>
<p>Note that requests to <code>&quot;localhost&quot;</code> or <code>&quot;127.0.0.1&quot;</code> are never proxied.</p>
</li>
<li>
<p>69546655e: Added support for sending batch requests through WebSocket to the Hardhat node (thanks <a href="https://github.com/tenbits"><code>@​tenbits</code></a>!)</p>
</li>
<li>
<p>6bf1673bb: Added a config validation for the number of optimizer runs used (thanks <a href="https://github.com/konarshankar07"><code>@​konarshankar07</code></a>!)</p>
</li>
</ul>
<h2>Hardhat v2.12.6</h2>
<h3>Features</h3>
<ul>
<li>Added support for pnpm during project creation (thanks <a href="https://github.com/Hopsken"><code>@​Hopsken</code></a>!)</li>
<li>Added a <code>version</code> field to the Hardhat Runtime Environment (thanks <a href="https://github.com/konarshankar07"><code>@​konarshankar07</code></a>!)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Fixed a problem with impersonated-sender transactions sometimes resulting in duplicate transaction hashes (issue <a href="https://github-redirect.dependabot.com/nomiclabs/hardhat/issues/1963">#1963</a>)</li>
</ul>
<h3>Other changes</h3>
<ul>
<li>Added a minor clarification to the help output of the <code>flatten</code> task</li>
<li>Upgraded the versions of <code>mocha</code> and <code>@types/mocha</code> used by Hardhat</li>
<li>Upgraded the version of <a href="http://undici.nodejs.org/">undici</a> used by Hardhat.</li>
<li>Removed the message linking to the 2022 Solidity Survey</li>
<li>Added a new subtask to the <code>compile</code> task that will be used by the <code>hardhat-foundry</code> plugin.</li>
</ul>
<h2>Hardhat v2.12.5</h2>
<ul>
<li>The full return data of unrecognized custom errors is now shown in error messages</li>
<li>Fixed a bug that was causing the flatten task to produce non-deterministic results</li>
<li>Fixed a bug when <code>gasPrice</code> was set to <code>&quot;auto&quot;</code>, which is the default configuration when connecting to a JSON-RPC network. This bug was preventing the results from <code>eth_feeHistory</code> from being used when they should.</li>
<li>Added an experimental environment variable flag to disable the local installation check (thanks <a href="https://github.com/arijoon"><code>@​arijoon</code></a>!)</li>
</ul>
<h2>Hardhat v2.12.4</h2>
<p>This release fixes a small issue that was affecting <a href="https://marketplace.visualstudio.com/items?itemName=NomicFoundation.hardhat-solidity">our VSCode extension</a> in some edge cases.</p>
<p>It also includes a non-intrusive message promoting this year's <a href="https://cryptpad.fr/form/#/2/form/view/HuPIRv4gvziSV0dPV1SJncKzYJXTVc8LGCaMfLUoj2c/">Solidity Developer Survey</a>.</p>
<h2>Hardhat v2.12.3</h2>
<ul>
<li>Added a new <code>hardhat_metadata</code> RPC method</li>
<li>Trim leading and trailing spaces in mnemonics (thanks <a href="https://github.com/winor30"><code>@​winor30</code></a>!)</li>
<li>Pending blocks now include the <code>bloom</code> field (thanks <a href="https://github.com/InoMurko"><code>@​InoMurko</code></a>!)</li>
<li>A better error is shown if a Solidity file makes an import through its own package name (thanks <a href="https://github.com/KaanKC"><code>@​KaanKC</code></a>!)</li>
<li>Added a <code>getBuildInfoSync</code> function to the <code>hre.artifacts</code> object (thanks <a href="https://github.com/emretepedev"><code>@​emretepedev</code></a>!)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/6baf30a296db6f0a4981660aed25753839e75675"><code>6baf30a</code></a> Version Packages</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/ccf8841f7efb0949179553b7b6d91b6e13fd99da"><code>ccf8841</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/nomiclabs/hardhat/issues/3658">#3658</a> from NomicFoundation/plugin-error-eslint</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/5a9b9a33b00844ec4957b851c1f7ef47bf61cedc"><code>5a9b9a3</code></a> remove unnecessary line</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/471a70f2b31bb7813cd3825b1fc5b10fdb31fff0"><code>471a70f</code></a> Update packages/eslint-plugin/onlyHardhatErrorRule.js</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/0edcf75ef7d6f06add958ce82e74d60fadfaa6df"><code>0edcf75</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/nomiclabs/hardhat/issues/2976">#2976</a> from NomicFoundation/francovictorio/hh-937/improve-w...</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/337456b8a0adb837a4da50fbcdec015251e67328"><code>337456b</code></a> Create cyan-knives-study.md</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/42560688fefe5b13bd3797e4ec9ed59bef704018"><code>4256068</code></a> add eslint rule for hardhat plugin errors</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/95328cc25c3ca84ecdf4d36c36acbf6583f7de11"><code>95328cc</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/nomiclabs/hardhat/issues/3432">#3432</a> from NomicFoundation/improve-proxy-support</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/6a3c6eccba831dcaa006f52f94f07399fbd5b93a"><code>6a3c6ec</code></a> Add docs about http_proxy</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/42d848121ed3804e2aea6e1440dbabb5b8132874"><code>42d8481</code></a> Update .changeset/few-flies-drum.md</li>
<li>Additional commits viewable in <a href="https://github.com/nomiclabs/hardhat/compare/hardhat@2.9.3...hardhat@2.12.7">compare view</a></li>
</ul>
</details>
<br />

Updates `@nomiclabs/hardhat-etherscan` from 3.0.3 to 3.1.6
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nomiclabs/hardhat/releases"><code>@​nomiclabs/hardhat-etherscan</code>'s releases</a>.</em></p>
<blockquote>
<h2><code>@​nomiclabs/hardhat-etherscan</code><a href="https://github.com/3"><code>@​3</code></a>.1.6</h2>
<h1>Changes</h1>
<ul>
<li>070abb7f5: Added support for the <code>http_proxy</code> environment variable. When this variable is set, <code>hardhat-etherscan</code> will use the given proxy to send the verification requests.</li>
</ul>
<h2><code>@​nomiclabs/hardhat-etherscan</code> v3.1.5</h2>
<p>This release upgrades the version of <a href="http://undici.nodejs.org/">undici</a> used by the hardhat-etherscan plugin.</p>
<h2><code>@​nomiclabs/hardhat-etherscan</code> v3.1.4</h2>
<p>Added a warning when the <code>etherscan</code> config is mistakenly included in the <code>networks</code> object instead of being at the root of the config.</p>
<h2><code>@​nomiclabs/hardhat-etherscan</code> v3.1.3</h2>
<p>Added a <code>--no-compile</code> flag to the <code>verify</code> task (thanks <a href="https://github.com/spalladino"><code>@​spalladino</code></a>!)</p>
<h2><code>@​nomiclabs/hardhat-etherscan</code> v3.1.2</h2>
<ul>
<li>Added Arbitrum Goerli to the list of supported networks.</li>
<li>Fixed an issue with the URLs used for Optimism Goerli.</li>
</ul>
<h2><code>@​nomiclabs/hardhat-etherscan</code> v3.1.1</h2>
<p>This version makes two changes to the networks supported by default:</p>
<ul>
<li>A new <code>gnosis</code> network was added, that works as an alias for xdai (thanks <a href="https://github.com/alebanzas"><code>@​alebanzas</code></a>!)</li>
<li>The deprecated Optimism Kovan network was removed in favor of the Optimism Goerli network (thanks <a href="https://github.com/shanefontaine"><code>@​shanefontaine</code></a>)</li>
</ul>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/6baf30a296db6f0a4981660aed25753839e75675"><code>6baf30a</code></a> Version Packages</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/ccf8841f7efb0949179553b7b6d91b6e13fd99da"><code>ccf8841</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/nomiclabs/hardhat/issues/3658">#3658</a> from NomicFoundation/plugin-error-eslint</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/5a9b9a33b00844ec4957b851c1f7ef47bf61cedc"><code>5a9b9a3</code></a> remove unnecessary line</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/471a70f2b31bb7813cd3825b1fc5b10fdb31fff0"><code>471a70f</code></a> Update packages/eslint-plugin/onlyHardhatErrorRule.js</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/0edcf75ef7d6f06add958ce82e74d60fadfaa6df"><code>0edcf75</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/nomiclabs/hardhat/issues/2976">#2976</a> from NomicFoundation/francovictorio/hh-937/improve-w...</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/337456b8a0adb837a4da50fbcdec015251e67328"><code>337456b</code></a> Create cyan-knives-study.md</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/42560688fefe5b13bd3797e4ec9ed59bef704018"><code>4256068</code></a> add eslint rule for hardhat plugin errors</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/95328cc25c3ca84ecdf4d36c36acbf6583f7de11"><code>95328cc</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/nomiclabs/hardhat/issues/3432">#3432</a> from NomicFoundation/improve-proxy-support</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/6a3c6eccba831dcaa006f52f94f07399fbd5b93a"><code>6a3c6ec</code></a> Add docs about http_proxy</li>
<li><a href="https://github.com/NomicFoundation/hardhat/commit/42d848121ed3804e2aea6e1440dbabb5b8132874"><code>42d8481</code></a> Update .changeset/few-flies-drum.md</li>
<li>Additional commits viewable in <a href="https://github.com/nomiclabs/hardhat/compare/@nomiclabs/hardhat-etherscan@3.0.3...@nomiclabs/hardhat-etherscan@3.1.6">compare view</a></li>
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
        Created At 2023-02-16 21:18:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/122" class=".btn">#122</a>
            </td>
            <td>
                <b>
                    Support "config.factoryAddress" to create tokens using a custom factory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Support "config.factoryAddress" to create tokens using a custom factory
* Mark token contract methods as virtual (to allow overriding in a child contract)
* ~~Retry indefinitely for errors during event processing (particularly to solve transient failures in retrieving ERC721 token URI)~~

The URI issue was called out here: https://github.com/hyperledger/firefly-tokens-erc1155/issues/114 (but no separate issue filed in this repository)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 18:25:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/121" class=".btn">#121</a>
            </td>
            <td>
                <b>
                    Bump cacheable-request, @nomiclabs/hardhat-waffle, ethereum-waffle and solidity-coverage in /samples/solidity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Removes [cacheable-request](https://github.com/jaredwray/cacheable-request). It's no longer used after updating ancestor dependencies [cacheable-request](https://github.com/jaredwray/cacheable-request), [@nomiclabs/hardhat-waffle](https://github.com/NomicFoundation/hardhat-waffle), [ethereum-waffle](https://github.com/EthWorks/Waffle) and [solidity-coverage](https://github.com/sc-forks/solidity-coverage). These dependencies need to be updated together.

Removes `cacheable-request`

Updates `@nomiclabs/hardhat-waffle` from 2.0.3 to 2.0.5
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/NomicFoundation/hardhat-waffle/releases"><code>@​nomiclabs/hardhat-waffle</code>'s releases</a>.</em></p>
<blockquote>
<h2><code>@​nomiclabs/hardaht-waffle</code> v2.0.5 released</h2>
<p>This is the first version of the plugin published in collaboration with the <a href="https://truefi.io/">TrueFi</a> team, the maintainers of Waffle 🚀</p>
<p>We moved this plugin to its own repository, cleaned it up in the process, and implemented some small improvements.</p>
<h2>Changes</h2>
<ul>
<li>c5b5c29: Introduce skipEstimateGas and injectCallHistory fields to hardhat config</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/NomicFoundation/hardhat-waffle/blob/main/CHANGELOG.md"><code>@​nomiclabs/hardhat-waffle</code>'s changelog</a>.</em></p>
<blockquote>
<h2>2.0.5</h2>
<h3>Patch Changes</h3>
<ul>
<li>36441d8: Add hardhat chai matchers incompatibility check</li>
<li>c5b5c29: Introduce skipEstimateGas and injectCallHistory fields to hardhat config</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/NomicFoundation/hardhat-waffle/commits/v2.0.5">compare view</a></li>
</ul>
</details>
<br />

Updates `ethereum-waffle` from 3.4.4 to 4.0.9
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/EthWorks/Waffle/releases">ethereum-waffle's releases</a>.</em></p>
<blockquote>
<h2><code>@​ethereum-waffle/chai</code><a href="https://github.com/4"><code>@​4</code></a>.0.9</h2>
<h3>Patch Changes</h3>
<ul>
<li>216f1d8: Switch hardhat error priority</li>
</ul>
<h2>ethereum-waffle@4.0.9</h2>
<h3>Patch Changes</h3>
<ul>
<li>Updated dependencies [216f1d8]
<ul>
<li><code>@​ethereum-waffle/chai</code><a href="https://github.com/4"><code>@​4</code></a>.0.9</li>
<li><code>@​ethereum-waffle/compiler</code><a href="https://github.com/4"><code>@​4</code></a>.0.3</li>
<li><code>@​ethereum-waffle/mock-contract</code><a href="https://github.com/4"><code>@​4</code></a>.0.3</li>
</ul>
</li>
</ul>
<h2><code>@​ethereum-waffle/chai</code><a href="https://github.com/4"><code>@​4</code></a>.0.8</h2>
<h3>Patch Changes</h3>
<ul>
<li>f93abe9: Move call history injection logic to hardhat plugin</li>
<li>9602243: 👔 revertedWith().withArgs no longer fails for uint values exceeding JavaScript's max int limit</li>
<li>b54c6b9: Add delta to balance changing matchers</li>
<li>64707ae: Allow special characters in revertedWith regex</li>
<li>702c6ab: 🗾 Extend matching of Hardhat revert reasons</li>
<li>a0f721a: Move ethers to peer deps</li>
<li>f6d240e: 🛶 Updates for hardhat v2.11</li>
<li>Updated dependencies [ee1d1b8]</li>
<li>Updated dependencies [a0f721a]
<ul>
<li><code>@​ethereum-waffle/provider</code><a href="https://github.com/4"><code>@​4</code></a>.0.5</li>
</ul>
</li>
</ul>
<h2>ethereum-waffle@4.0.8</h2>
<h3>Patch Changes</h3>
<ul>
<li>f93abe9: Move call history injection logic to hardhat plugin</li>
<li>a0f721a: Move ethers to peer deps</li>
<li>Updated dependencies [da92375]</li>
<li>Updated dependencies [f93abe9]</li>
<li>Updated dependencies [46b954e]</li>
<li>Updated dependencies [9602243]</li>
<li>Updated dependencies [fb6863d]</li>
<li>Updated dependencies [b54c6b9]</li>
<li>Updated dependencies [64707ae]</li>
<li>Updated dependencies [1fa1312]</li>
<li>Updated dependencies [ee1d1b8]</li>
<li>Updated dependencies [702c6ab]</li>
<li>Updated dependencies [a0f721a]</li>
<li>Updated dependencies [f6d240e]
<ul>
<li><code>@​ethereum-waffle/mock-contract</code><a href="https://github.com/4"><code>@​4</code></a>.0.3</li>
<li><code>@​ethereum-waffle/chai</code><a href="https://github.com/4"><code>@​4</code></a>.0.8</li>
<li><code>@​ethereum-waffle/provider</code><a href="https://github.com/4"><code>@​4</code></a>.0.5</li>
<li><code>@​ethereum-waffle/compiler</code><a href="https://github.com/4"><code>@​4</code></a>.0.3</li>
</ul>
</li>
</ul>
<h2><code>@​ethereum-waffle/chai</code><a href="https://github.com/4"><code>@​4</code></a>.0.7</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/TrueFiEng/Waffle/commit/a1d89d0063c7cc3d9d2e9b23cb17d9590fa1b7fd"><code>a1d89d0</code></a> 🎉 Release new version (<a href="https://github-redirect.dependabot.com/EthWorks/Waffle/issues/821">#821</a>)</li>
<li><a href="https://github.com/TrueFiEng/Waffle/commit/216f1d8cdfd98d02c6a335d7789831559aecf955"><code>216f1d8</code></a> 🌏 Switch hardhat errors priority (<a href="https://github-redirect.dependabot.com/EthWorks/Waffle/issues/820">#820</a>)</li>
<li><a href="https://github.com/TrueFiEng/Waffle/commit/13d1af063fe5d78a84aafeb549b2e3073f2e57c1"><code>13d1af0</code></a> 🎉 Release new version (<a href="https://github-redirect.dependabot.com/EthWorks/Waffle/issues/796">#796</a>)</li>
<li><a href="https://github.com/TrueFiEng/Waffle/commit/5637cc55a81ede4976ab5863c3a04840fff395eb"><code>5637cc5</code></a> 🦉 Optimism tests use latest commit (<a href="https://github-redirect.dependabot.com/EthWorks/Waffle/issues/819">#819</a>)</li>
<li><a href="https://github.com/TrueFiEng/Waffle/commit/1fa13127d199e43226178ffc45a661fddd657045"><code>1fa1312</code></a> 🥑 Add mock contract typing (<a href="https://github-redirect.dependabot.com/EthWorks/Waffle/issues/818">#818</a>)</li>
<li><a href="https://github.com/TrueFiEng/Waffle/commit/702c6ab299d78c1dbbb42ea72aa8bfbfce0c8390"><code>702c6ab</code></a> 🗾 Extend matching of Hardhat revert reasons (<a href="https://github-redirect.dependabot.com/EthWorks/Waffle/issues/802">#802</a>)</li>
<li><a href="https://github.com/TrueFiEng/Waffle/commit/46b954e1f9cbf9036ece5837c574ce800e6cdacc"><code>46b954e</code></a> 🖼 Mock contract chaining behaviour (<a href="https://github-redirect.dependabot.com/EthWorks/Waffle/issues/816">#816</a>)</li>
<li><a href="https://github.com/TrueFiEng/Waffle/commit/fb6863d0a795db091b925385e1c1c670aa53eedd"><code>fb6863d</code></a> 🍶 Implement mocking receive function to revert (<a href="https://github-redirect.dependabot.com/EthWorks/Waffle/issues/807">#807</a>)</li>
<li><a href="https://github.com/TrueFiEng/Waffle/commit/da9237577597618afa306161edfbdcad7a426542"><code>da92375</code></a> 🗽 Add address parameter to the mock contract (<a href="https://github-redirect.dependabot.com/EthWorks/Waffle/issues/815">#815</a>)</li>
<li><a href="https://github.com/TrueFiEng/Waffle/commit/b54c6b93dee70dd54f831b2b6af60b11e4f8c827"><code>b54c6b9</code></a> 🗿 Add error to balance changing matchers (<a href="https://github-redirect.dependabot.com/EthWorks/Waffle/issues/814">#814</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/EthWorks/Waffle/compare/ethereum-waffle@3.4.4...ethereum-waffle@4.0.9">compare view</a></li>
</ul>
</details>
<br />

Updates `solidity-coverage` from 0.7.21 to 0.8.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sc-forks/solidity-coverage/releases">solidity-coverage's releases</a>.</em></p>
<blockquote>
<h2>0.8.2</h2>
<h2>What's Changed</h2>
<ul>
<li>Set web3-utils dep to ^1.3.6 by <a href="https://github.com/MarkuSchick"><code>@​MarkuSchick</code></a> in <a href="https://github-redirect.dependabot.com/sc-forks/solidity-coverage/pull/744">sc-forks/solidity-coverage#744</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/MarkuSchick"><code>@​MarkuSchick</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/sc-forks/solidity-coverage/pull/744">sc-forks/solidity-coverage#744</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sc-forks/solidity-coverage/compare/v0.8.1...v0.8.2">https://github.com/sc-forks/solidity-coverage/compare/v0.8.1...v0.8.2</a></p>
<h2>0.8.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Bug fix: restore missing web3-utils dependency by <a href="https://github.com/cgewecke"><code>@​cgewecke</code></a> in <a href="https://github-redirect.dependabot.com/sc-forks/solidity-coverage/pull/743">sc-forks/solidity-coverage#743</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sc-forks/solidity-coverage/compare/v0.8.0...v0.8.1">https://github.com/sc-forks/solidity-coverage/compare/v0.8.0...v0.8.1</a></p>
<h2>0.8.0</h2>
<p>Hi!</p>
<h4>⚠️ This version requires Hardhat &gt;= 2.11.0 (Ethereum Merge)</h4>
<h2>New Features</h2>
<p>A central focus of the 0.8.0 release is improving the coverage tool's branch detection.</p>
<p>Beginning with this version the following syntax is measured as a branch:</p>
<h3>OR conditions</h3>
<p>When a logical expression is composed with the <code>||</code> operator, both sides can be considered branches. To test the entire expression</p>
<pre lang="solidity"><code>if (a == 1 || a == 2)
</code></pre>
<p>... <code>a</code> must equal 1, 2 <em>and</em> neither of those values. (Thanks to Gnosis engineer <a href="https://github.com/rmeissner"><code>@​rmeissner</code></a> for proposing this in <a href="https://github-redirect.dependabot.com/sc-forks/solidity-coverage/issues/175">#175</a>)</p>
<p><img src="https://user-images.githubusercontent.com/7332026/104411309-fd2e9380-551e-11eb-8502-85cc72033b26.png" alt="Screen Shot 2021-01-12 at 9 41 09 PM" /></p>
<h3>Ternary Conditionals</h3>
<p>Long ago, when Solidity was 0.4, solidity-coverage treated ternary conditionals like regular if/else statements. Some language improvements v0.5 subsequently made this impossible. Now it's back...</p>
<p><img src="https://user-images.githubusercontent.com/7332026/104411766-db81dc00-551f-11eb-88a2-fd3e3867909e.png" alt="Screen Shot 2021-01-12 at 9 47 43 PM" /></p>
<h3>Modifier Invocations</h3>
<p>Solidity-coverage already covers the code within modifier definitions. However, each modifier invocation at the function level should really be considered its own branch. Some of the most critical logic in Solidity contracts is handled this way (ex: <code>onlyOwner</code>). Testing the pass/fail cases for each occurrence of these gates protects you from accidentally removing them during a refactor.</p>
<p>Because it's possible to write a modifier which performs a preparatory task and never reverts, there's a new option (<code>modifierWhitelist</code>) which allows you to exclude specific modifiers from branch measurement.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/sc-forks/solidity-coverage/blob/master/CHANGELOG.md">solidity-coverage's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<h1>0.8.1 / 2022-09-06</h1>
<ul>
<li>Restore web3-utils (<a href="https://github-redirect.dependabot.com/sc-forks/solidity-coverage/issues/743">sc-forks/solidity-coverage#743</a>)</li>
</ul>
<h1>0.8.0 / 2022-09-05</h1>
<ul>
<li>See release notes at: <a href="https://github.com/sc-forks/solidity-coverage/releases/tag/v0.8.0">https://github.com/sc-forks/solidity-coverage/releases/tag/v0.8.0</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/sc-forks/solidity-coverage/commits/v0.8.2">compare view</a></li>
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
        Created At 2023-02-12 03:42:31 +0000 UTC
    </div>
</div>

