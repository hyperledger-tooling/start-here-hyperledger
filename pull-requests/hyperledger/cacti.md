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
                PR <a href="https://github.com/hyperledger/cacti/pull/3265" class=".btn">#3265</a>
            </td>
            <td>
                <b>
                    fix(cactus-example-cbdc-bridging-backend): add missing CRPC port conf…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …ig option

**Pull Request Requirements**
- [ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-15 11:25:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3264" class=".btn">#3264</a>
            </td>
            <td>
                <b>
                    build: bump the npm_and_yarn group across 7 directories with 17 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps the npm_and_yarn group with 15 updates in the / directory:

| Package | From | To |
| --- | --- | --- |
| [web3-utils](https://github.com/ChainSafe/web3.js) | `1.6.1` | `1.7.0` |
| [axios](https://github.com/axios/axios) | `1.5.1` | `1.6.0` |
| [express](https://github.com/expressjs/express) | `4.18.2` | `4.19.2` |
| [bl](https://github.com/rvagg/bl) | `5.0.0` | `5.1.0` |
| [undici](https://github.com/nodejs/undici) | `6.11.1` | `6.12.0` |
| [qs](https://github.com/ljharb/qs) | `6.7.3` | `6.8.3` |
| [vite](https://github.com/vitejs/vite/tree/HEAD/packages/vite) | `5.0.13` | `5.1.7` |
| [pkg](https://github.com/vercel/pkg) | `4.5.1` | `5.8.1` |
| [@adobe/css-tools](https://github.com/adobe/css-tools) | `4.2.0` | `4.3.3` |
| [apollo-server-core](https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core) | `3.12.0` | `3.13.0` |
| [browserify-sign](https://github.com/crypto-browserify/browserify-sign) | `4.2.1` | `4.2.3` |
| [es5-ext](https://github.com/medikoo/es5-ext) | `0.10.53` | `0.10.64` |
| [ip](https://github.com/indutny/node-ip) | `1.1.5` | `1.1.9` |
| [react-devtools-core](https://github.com/facebook/react/tree/HEAD/packages/react-devtools-core) | `4.27.8` | `4.28.5` |
| [word-wrap](https://github.com/jonschlinkert/word-wrap) | `1.2.3` | `1.2.5` |

Bumps the npm_and_yarn group with 1 update in the /examples/cactus-example-tcs-huawei directory: [jsonwebtoken](https://github.com/auth0/node-jsonwebtoken).
Bumps the npm_and_yarn group with 1 update in the /examples/test-run-transaction directory: [jsonwebtoken](https://github.com/auth0/node-jsonwebtoken).
Bumps the npm_and_yarn group with 1 update in the /packages/cactus-plugin-ledger-connector-tcs-huawei-socketio directory: [jsonwebtoken](https://github.com/auth0/node-jsonwebtoken).
Bumps the npm_and_yarn group with 1 update in the /packages/cactus-test-plugin-keychain-memory directory: [express](https://github.com/expressjs/express).
Bumps the npm_and_yarn group with 1 update in the /weaver/docs directory: [gh-pages](https://github.com/tschaub/gh-pages).
Bumps the npm_and_yarn group with 1 update in the /weaver/samples/fabric/fabric-cli directory: [pkg](https://github.com/vercel/pkg).

Updates `web3-utils` from 1.6.1 to 1.7.0
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
<h2>[1.6.1]</h2>
<h3>Added</h3>
<ul>
<li>Support for <code>eth_createAccessList</code> as both an rpc call (<code>web3.eth.createAccessList</code>) and property of contract method wrappers (<code>contractInstance.methods.getValue().createAccessList</code>) (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4332">#4332</a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Not considering <code>tx.chainId</code> if <code>tx.common.customChain.chainId</code> is provided for <code>web3.eth.accounts.signTransaction</code> function (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4293">#4293</a>)</li>
<li>Added missing PromiEvent handler types (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4194">#4194</a>)</li>
<li>Updated README to include webpack 5 angular support instructions (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4174">#4174</a>)</li>
<li>Updated the documentation for the <code>Web3.utils</code>, removed context for <code>_</code> (underscore lib) (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4403">#4403</a>)</li>
<li>Emit subscription id with connect event when creating a subscription (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4300">#4300</a>)</li>
<li>Introduced new configuration &quot;blockHeaderTimeout&quot; for waiting of block headers for transaction receipt (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/3891">#3891</a>)</li>
<li>Format <code>block.baseFeePerGas</code> to number (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4330">#4330</a>)</li>
<li>Correct <code>web3-eth-personal.sendTransaction</code> example in documentation (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4409">#4409</a>)</li>
<li>Updated README to include webpack 5 angular support instructions (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4174">#4174</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Fix 1.6.1 build size issue with removing static asset files (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4506">#4506</a>)</li>
<li>Correct <code>web3.rst</code> example in documentation (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4511">#4511</a>)</li>
<li>Correct <code>BlockHeader</code> typing (<code>receiptRoot</code> -&gt; <code>receiptsRoot</code>) (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4452">#4452</a>)</li>
</ul>
<h2>[1.7.0]</h2>
<h3>Added</h3>
<ul>
<li><code>maxPriorityFeePerGas</code> and <code>maxFeePerGas</code> added to <code>Transaction</code> and <code>TransactionConfig</code> interfaces (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4232">#4232</a>) (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4585">#4585</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Fix readthedoc's build for web3js documentation (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4425">#4425</a>)</li>
<li>Fix response sorting for batch requests (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4250">#4250</a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Changed getFeeHistory first parameter type from <code>number</code> to <code>hex</code> according to the <a href="https://playground.open-rpc.org/?schemaUrl=https://raw.githubusercontent.com/ethereum/eth1.0-apis/assembled-spec/openrpc.json&amp;uiSchema%5BappBar%5D%5Bui:splitView%5D=false&amp;uiSchema%5BappBar%5D%5Bui:input%5D=false&amp;uiSchema%5BappBar%5D%5Bui:examplesDropdown%5D=false">spec</a> (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4529">#4529</a>)</li>
</ul>
<h2>[1.7.1]</h2>
<h3>Added</h3>
<ul>
<li><code>transactionPollingInterval</code> added to web3, contract and method constructor options. defaults to 1 second. (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4584">#4584</a>)</li>
<li>Add example import for package level types (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4611">#4611</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Fix a typo in the documentation for <code>methods.myMethod.send</code> (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4599">#4599</a>)</li>
<li>Use globalThis to locate global object if possible (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4613">#4613</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/web3/web3.js/commit/cd4b4d13e7e1d973ceee29c118798d4931860a2b"><code>cd4b4d1</code></a> Build for v1.7.0</li>
<li><a href="https://github.com/web3/web3.js/commit/d30033f966c47ce291da992cb80b59dc16868ea7"><code>d30033f</code></a> v1.7.0</li>
<li><a href="https://github.com/web3/web3.js/commit/c191d9a30f97b6dc2c22d09882e41f009fa01a10"><code>c191d9a</code></a> Merge branch '1.x' into release/1.7.0</li>
<li><a href="https://github.com/web3/web3.js/commit/b32555cfeedde128c657dabbba201102f691f955"><code>b32555c</code></a> add: custom transaction polling interval (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4584">#4584</a>) (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4672">#4672</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/0b890b70b977451836dc693614960256bcbcb6d8"><code>0b890b7</code></a> adding effective gas price to transactionreceipt (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4694">#4694</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/9c9417a21dc6b51fda4d68090fa81ae9388226db"><code>9c9417a</code></a> correction in documentation for signtransaction accounts (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4674">#4674</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/9b19af853087fc3a217907e337cae95700309d62"><code>9b19af8</code></a> added webpack 5 create-react-app instructions (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4670">#4670</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/8783f4d64e424456bdc53b34ef1142d0a7cee4d7"><code>8783f4d</code></a> Fix a typo in docs <a href="https://redirect.github.com/ChainSafe/web3.js/issues/4616">#4616</a> (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/4640">#4640</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/bbb9cdf178a769565329ccabafb9ea1937a899c0"><code>bbb9cdf</code></a> Manual build commit for 1.7.0-rc.0</li>
<li><a href="https://github.com/web3/web3.js/commit/e76d9dca2c8df2a766789b8da860ca5840e976f6"><code>e76d9dc</code></a> v1.7.0-rc.0</li>
<li>Additional commits viewable in <a href="https://github.com/ChainSafe/web3.js/compare/v1.6.1...v1.7.0">compare view</a></li>
</ul>
</details>
<br />

Updates `axios` from 1.5.1 to 1.6.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/releases">axios's releases</a>.</em></p>
<blockquote>
<h2>Release v1.6.0</h2>
<h2>Release notes:</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>CSRF:</strong> fixed CSRF vulnerability CVE-2023-45857 (<a href="https://redirect.github.com/axios/axios/issues/6028">#6028</a>) (<a href="https://github.com/axios/axios/commit/96ee232bd3ee4de2e657333d4d2191cd389e14d0">96ee232</a>)</li>
<li><strong>dns:</strong> fixed lookup function decorator to work properly in node v20; (<a href="https://redirect.github.com/axios/axios/issues/6011">#6011</a>) (<a href="https://github.com/axios/axios/commit/5aaff532a6b820bb9ab6a8cd0f77131b47e2adb8">5aaff53</a>)</li>
<li><strong>types:</strong> fix AxiosHeaders types; (<a href="https://redirect.github.com/axios/axios/issues/5931">#5931</a>) (<a href="https://github.com/axios/axios/commit/a1c8ad008b3c13d53e135bbd0862587fb9d3fc09">a1c8ad0</a>)</li>
</ul>
<h3>PRs</h3>
<ul>
<li>CVE 2023 45857 ( <a href="https://api.github.com/repos/axios/axios/pulls/6028">#6028</a> )</li>
</ul>
<pre><code>
⚠️ Critical vulnerability fix. See https://security.snyk.io/vuln/SNYK-JS-AXIOS-6032459
</code></pre>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+449/-114 ([#6032](https://github.com/axios/axios/issues/6032) [#6021](https://github.com/axios/axios/issues/6021) [#6011](https://github.com/axios/axios/issues/6011) [#5932](https://github.com/axios/axios/issues/5932) [#5931](https://github.com/axios/axios/issues/5931) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/valentin-panov" title="+4/-4 ([#6028](https://github.com/axios/axios/issues/6028) )">Valentin Panov</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/therealrinku" title="+1/-1 ([#5889](https://github.com/axios/axios/issues/5889) )">Rinku Chaudhari</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/blob/v1.x/CHANGELOG.md">axios's changelog</a>.</em></p>
<blockquote>
<h1><a href="https://github.com/axios/axios/compare/v1.5.1...v1.6.0">1.6.0</a> (2023-10-26)</h1>
<h3>Bug Fixes</h3>
<ul>
<li><strong>CSRF:</strong> fixed CSRF vulnerability CVE-2023-45857 (<a href="https://redirect.github.com/axios/axios/issues/6028">#6028</a>) (<a href="https://github.com/axios/axios/commit/96ee232bd3ee4de2e657333d4d2191cd389e14d0">96ee232</a>)</li>
<li><strong>dns:</strong> fixed lookup function decorator to work properly in node v20; (<a href="https://redirect.github.com/axios/axios/issues/6011">#6011</a>) (<a href="https://github.com/axios/axios/commit/5aaff532a6b820bb9ab6a8cd0f77131b47e2adb8">5aaff53</a>)</li>
<li><strong>types:</strong> fix AxiosHeaders types; (<a href="https://redirect.github.com/axios/axios/issues/5931">#5931</a>) (<a href="https://github.com/axios/axios/commit/a1c8ad008b3c13d53e135bbd0862587fb9d3fc09">a1c8ad0</a>)</li>
</ul>
<h3>PRs</h3>
<ul>
<li>CVE 2023 45857 ( <a href="https://api.github.com/repos/axios/axios/pulls/6028">#6028</a> )</li>
</ul>
<pre><code>
⚠️ Critical vulnerability fix. See https://security.snyk.io/vuln/SNYK-JS-AXIOS-6032459
</code></pre>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+449/-114 ([#6032](https://github.com/axios/axios/issues/6032) [#6021](https://github.com/axios/axios/issues/6021) [#6011](https://github.com/axios/axios/issues/6011) [#5932](https://github.com/axios/axios/issues/5932) [#5931](https://github.com/axios/axios/issues/5931) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/valentin-panov" title="+4/-4 ([#6028](https://github.com/axios/axios/issues/6028) )">Valentin Panov</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/therealrinku" title="+1/-1 ([#5889](https://github.com/axios/axios/issues/5889) )">Rinku Chaudhari</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/axios/axios/commit/f7adacdbaa569281253c8cfc623ad3f4dc909c60"><code>f7adacd</code></a> chore(release): v1.6.0 (<a href="https://redirect.github.com/axios/axios/issues/6031">#6031</a>)</li>
<li><a href="https://github.com/axios/axios/commit/9917e67cbb6c157382863bad8c741de58e3f3c2b"><code>9917e67</code></a> chore(ci): fix release-it arg; (<a href="https://redirect.github.com/axios/axios/issues/6032">#6032</a>)</li>
<li><a href="https://github.com/axios/axios/commit/96ee232bd3ee4de2e657333d4d2191cd389e14d0"><code>96ee232</code></a> fix(CSRF): fixed CSRF vulnerability CVE-2023-45857 (<a href="https://redirect.github.com/axios/axios/issues/6028">#6028</a>)</li>
<li><a href="https://github.com/axios/axios/commit/7d45ab2e2ad6e59f5475e39afd4b286b1f393fc0"><code>7d45ab2</code></a> chore(tests): fixed tests to pass in node v19 and v20 with <code>keep-alive</code> enabl...</li>
<li><a href="https://github.com/axios/axios/commit/5aaff532a6b820bb9ab6a8cd0f77131b47e2adb8"><code>5aaff53</code></a> fix(dns): fixed lookup function decorator to work properly in node v20; (<a href="https://redirect.github.com/axios/axios/issues/6011">#6011</a>)</li>
<li><a href="https://github.com/axios/axios/commit/a48a63ad823fc20e5a6a705f05f09842ca49f48c"><code>a48a63a</code></a> chore(docs): added AxiosHeaders docs; (<a href="https://redirect.github.com/axios/axios/issues/5932">#5932</a>)</li>
<li><a href="https://github.com/axios/axios/commit/a1c8ad008b3c13d53e135bbd0862587fb9d3fc09"><code>a1c8ad0</code></a> fix(types): fix AxiosHeaders types; (<a href="https://redirect.github.com/axios/axios/issues/5931">#5931</a>)</li>
<li><a href="https://github.com/axios/axios/commit/2ac731d60545ba5c4202c25fd2e732ddd8297d82"><code>2ac731d</code></a> chore(docs): update readme.md (<a href="https://redirect.github.com/axios/axios/issues/5889">#5889</a>)</li>
<li>See full diff in <a href="https://github.com/axios/axios/compare/v1.5.1...v1.6.0">compare view</a></li>
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

Updates `bl` from 5.0.0 to 5.1.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/rvagg/bl/releases">bl's releases</a>.</em></p>
<blockquote>
<h2>v5.1.0</h2>
<h2><a href="https://github.com/rvagg/bl/compare/v5.0.0...v5.1.0">5.1.0</a> (2022-10-18)</h2>
<h3>Features</h3>
<ul>
<li>added integrated TypeScript typings (<a href="https://redirect.github.com/rvagg/bl/issues/108">#108</a>) (<a href="https://github.com/rvagg/bl/commit/433ff8942f47fab8a5c9d13b2c00989ccf8d0710">433ff89</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>windows support in tests (<a href="https://github.com/rvagg/bl/commit/387dfaf9b2bca7849f12785436ceb01e42adac2c">387dfaf</a>)</li>
</ul>
<h3>Trivial Changes</h3>
<ul>
<li>GH Actions, Dependabot, auto-release, remove Travis (<a href="https://github.com/rvagg/bl/commit/997f058357de8f2a7f66998e80a72b491835573f">997f058</a>)</li>
<li><strong>no-release:</strong> bump standard from 16.0.4 to 17.0.0 (<a href="https://redirect.github.com/rvagg/bl/issues/112">#112</a>) (<a href="https://github.com/rvagg/bl/commit/078bfe33390d125297b1c946e5989c4aa9228961">078bfe3</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/rvagg/bl/blob/master/CHANGELOG.md">bl's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/rvagg/bl/compare/v5.0.0...v5.1.0">5.1.0</a> (2022-10-18)</h2>
<h3>Features</h3>
<ul>
<li>added integrated TypeScript typings (<a href="https://redirect.github.com/rvagg/bl/issues/108">#108</a>) (<a href="https://github.com/rvagg/bl/commit/433ff8942f47fab8a5c9d13b2c00989ccf8d0710">433ff89</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>windows support in tests (<a href="https://github.com/rvagg/bl/commit/387dfaf9b2bca7849f12785436ceb01e42adac2c">387dfaf</a>)</li>
</ul>
<h3>Trivial Changes</h3>
<ul>
<li>GH Actions, Dependabot, auto-release, remove Travis (<a href="https://github.com/rvagg/bl/commit/997f058357de8f2a7f66998e80a72b491835573f">997f058</a>)</li>
<li><strong>no-release:</strong> bump standard from 16.0.4 to 17.0.0 (<a href="https://redirect.github.com/rvagg/bl/issues/112">#112</a>) (<a href="https://github.com/rvagg/bl/commit/078bfe33390d125297b1c946e5989c4aa9228961">078bfe3</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rvagg/bl/commit/3af8c54d33433c4683be4a74588a9739270ca4d4"><code>3af8c54</code></a> chore(release): 5.1.0 [skip ci]</li>
<li><a href="https://github.com/rvagg/bl/commit/433ff8942f47fab8a5c9d13b2c00989ccf8d0710"><code>433ff89</code></a> feat: added integrated TypeScript typings (<a href="https://redirect.github.com/rvagg/bl/issues/108">#108</a>)</li>
<li><a href="https://github.com/rvagg/bl/commit/078bfe33390d125297b1c946e5989c4aa9228961"><code>078bfe3</code></a> chore(no-release): bump standard from 16.0.4 to 17.0.0 (<a href="https://redirect.github.com/rvagg/bl/issues/112">#112</a>)</li>
<li><a href="https://github.com/rvagg/bl/commit/387dfaf9b2bca7849f12785436ceb01e42adac2c"><code>387dfaf</code></a> fix: windows support in tests</li>
<li><a href="https://github.com/rvagg/bl/commit/997f058357de8f2a7f66998e80a72b491835573f"><code>997f058</code></a> chore: GH Actions, Dependabot, auto-release, remove Travis</li>
<li>See full diff in <a href="https://github.com/rvagg/bl/compare/v5.0.0...v5.1.0">compare view</a></li>
</ul>
</details>
<br />

Updates `undici` from 6.11.1 to 6.12.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nodejs/undici/releases">undici's releases</a>.</em></p>
<blockquote>
<h2>v6.12.0</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: broken test by <a href="https://github.com/tsctx"><code>@​tsctx</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3045">nodejs/undici#3045</a></li>
<li>fix: http2 header parsing by <a href="https://github.com/climba03003"><code>@​climba03003</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3047">nodejs/undici#3047</a></li>
<li>types: fix Request.refererPolicy and RequestInit.refererPolicy are incompatible by <a href="https://github.com/zbinlin"><code>@​zbinlin</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3039">nodejs/undici#3039</a></li>
<li>fix(types): onHeaders always takes headers as an array of buffer by <a href="https://github.com/ronag"><code>@​ronag</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3050">nodejs/undici#3050</a></li>
<li>fix: ProxyAgent causes request.headers.host to be forcibly reset by <a href="https://github.com/1zilc"><code>@​1zilc</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3026">nodejs/undici#3026</a></li>
<li>fallback to Buffer.isUtf8 on platforms without icu by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3006">nodejs/undici#3006</a></li>
<li>build(deps): bump github/codeql-action from 3.24.6 to 3.24.9 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3037">nodejs/undici#3037</a></li>
<li>build(deps): bump actions/dependency-review-action from 4.1.3 to 4.2.5 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3035">nodejs/undici#3035</a></li>
<li>build(deps): bump node from <code>577f8eb</code> to <code>87524df</code> in /build by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3055">nodejs/undici#3055</a></li>
<li>build(deps): bump node from <code>87524df</code> to <code>9696b26</code> in /build by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3058">nodejs/undici#3058</a></li>
<li>fetch: Block ports 4190 &amp; 6679 by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3059">nodejs/undici#3059</a></li>
<li>test: activate testing for interceptors and cache by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3061">nodejs/undici#3061</a></li>
<li>cache: improve test coverage by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3063">nodejs/undici#3063</a></li>
<li>feat: modernize fuzzing by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3060">nodejs/undici#3060</a></li>
<li>fix: request abort by <a href="https://github.com/ronag"><code>@​ronag</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3056">nodejs/undici#3056</a></li>
<li>fix: signal handling by <a href="https://github.com/ronag"><code>@​ronag</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3053">nodejs/undici#3053</a></li>
<li>fix(H2): handle goaway properly by <a href="https://github.com/metcoder95"><code>@​metcoder95</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3057">nodejs/undici#3057</a></li>
<li>test: client, set body to null if bigger than CHUNK_LIMIT by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3064">nodejs/undici#3064</a></li>
<li>mock: improve mock interceptor by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3062">nodejs/undici#3062</a></li>
<li>fix: bad client destroy on servername change by <a href="https://github.com/ronag"><code>@​ronag</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3066">nodejs/undici#3066</a></li>
<li>perf: improve isBlobLike by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3070">nodejs/undici#3070</a></li>
<li>test: add sanity check for llhttp wasm files by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3068">nodejs/undici#3068</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/zbinlin"><code>@​zbinlin</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/3039">nodejs/undici#3039</a></li>
<li><a href="https://github.com/1zilc"><code>@​1zilc</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/3026">nodejs/undici#3026</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v6.11.1...v6.12.0">https://github.com/nodejs/undici/compare/v6.11.1...v6.12.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nodejs/undici/commit/7751d9bcd5bbba45b60c90183aeab450b60c0831"><code>7751d9b</code></a> Bumped v6.12.0</li>
<li><a href="https://github.com/nodejs/undici/commit/e9c3b22c97b5bf2113057ea2cf1c6dec8868e9fb"><code>e9c3b22</code></a> Revert &quot;automate releases (<a href="https://redirect.github.com/nodejs/undici/issues/3052">#3052</a>)&quot;</li>
<li><a href="https://github.com/nodejs/undici/commit/f51f226522ec75a0613a07a4efc8f78938030c45"><code>f51f226</code></a> automate releases (<a href="https://redirect.github.com/nodejs/undici/issues/3052">#3052</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/502e13472d4bcebbf4669c2a91a7ef97705a0fd7"><code>502e134</code></a> test: add test for llhttp wasm (<a href="https://redirect.github.com/nodejs/undici/issues/3068">#3068</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/413fd4de5b161c1e9a539089a4d51965abd5018d"><code>413fd4d</code></a> perf: improve isBlobLike (<a href="https://redirect.github.com/nodejs/undici/issues/3070">#3070</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/7ae20e6070fa7de2831a907c92fa44268003c145"><code>7ae20e6</code></a> fix: bad client destroy on servername change (<a href="https://redirect.github.com/nodejs/undici/issues/3066">#3066</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/ad3fac577cca737976ed82cd9d55027eb8af654c"><code>ad3fac5</code></a> mock: improve mock interceptor (<a href="https://redirect.github.com/nodejs/undici/issues/3062">#3062</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/d399b3db9e16b25e9ed0f07c0e067fe99fa8c409"><code>d399b3d</code></a> test: client, set body to null if bigger than CHUNK_LIMIT (<a href="https://redirect.github.com/nodejs/undici/issues/3064">#3064</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/bc4b20698f38b4f43f0eb4091dad28c83844f3ef"><code>bc4b206</code></a> fix(H2): handle goaway properly (<a href="https://redirect.github.com/nodejs/undici/issues/3057">#3057</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/b6aa794e2db44f20adc4c9cc99009e72048f4fed"><code>b6aa794</code></a> fix: signal handling (<a href="https://redirect.github.com/nodejs/undici/issues/3053">#3053</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/nodejs/undici/compare/v6.11.1...v6.12.0">compare view</a></li>
</ul>
</details>
<br />

Updates `qs` from 6.7.3 to 6.8.3
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ljharb/qs/blob/main/CHANGELOG.md">qs's changelog</a>.</em></p>
<blockquote>
<h2><strong>6.8.3</strong></h2>
<ul>
<li>[Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://redirect.github.com/ljharb/qs/issues/428">#428</a>)</li>
<li>[Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://redirect.github.com/ljharb/qs/issues/427">#427</a>)</li>
<li>[Fix] <code>stringify</code>: avoid encoding arrayformat comma when <code>encodeValuesOnly = true</code> (<a href="https://redirect.github.com/ljharb/qs/issues/424">#424</a>)</li>
<li>[readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li>[Tests] clean up stringify tests slightly</li>
<li>[Docs] add note and links for coercing primitive values (<a href="https://redirect.github.com/ljharb/qs/issues/408">#408</a>)</li>
<li>[meta] fix README.md (<a href="https://redirect.github.com/ljharb/qs/issues/399">#399</a>)</li>
<li>[actions] backport actions from main</li>
<li>[Dev Deps] backport updates from main</li>
<li>[Refactor] <code>stringify</code>: reduce branching</li>
<li>[meta] do not publish workflow files</li>
</ul>
<h2><strong>6.8.2</strong></h2>
<ul>
<li>[Fix] proper comma parsing of URL-encoded commas (<a href="https://redirect.github.com/ljharb/qs/issues/361">#361</a>)</li>
<li>[Fix] parses comma delimited array while having percent-encoded comma treated as normal text (<a href="https://redirect.github.com/ljharb/qs/issues/336">#336</a>)</li>
</ul>
<h2><strong>6.8.1</strong></h2>
<ul>
<li>[Fix] <code>parse</code>: Fix parsing array from object with <code>comma</code> true (<a href="https://redirect.github.com/ljharb/qs/issues/359">#359</a>)</li>
<li>[Fix] <code>parse</code>: throw a TypeError instead of an Error for bad charset (<a href="https://redirect.github.com/ljharb/qs/issues/349">#349</a>)</li>
<li>[Fix] <code>parse</code>: with comma true, handle field that holds an array of arrays (<a href="https://redirect.github.com/ljharb/qs/issues/335">#335</a>)</li>
<li>[fix] <code>parse</code>: with comma true, do not split non-string values (<a href="https://redirect.github.com/ljharb/qs/issues/334">#334</a>)</li>
<li>[meta] add tidelift marketing copy</li>
<li>[meta] add <code>funding</code> field</li>
<li>[Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>tape</code>, <code>safe-publish-latest</code>, <code>evalmd</code>, <code>has-symbols</code>, <code>iconv-lite</code>, <code>mkdirp</code>, <code>object-inspect</code></li>
<li>[Tests] <code>parse</code>: add passing <code>arrayFormat</code> tests</li>
<li>[Tests] use shared travis-ci configs</li>
<li>[Tests] <code>Buffer.from</code> in node v5.0-v5.9 and v4.0-v4.4 requires a TypedArray</li>
<li>[actions] add automatic rebasing / merge commit blocking</li>
</ul>
<h2><strong>6.8.0</strong></h2>
<ul>
<li>[New] add <code>depth=false</code> to preserve the original key; [Fix] <code>depth=0</code> should preserve the original key (<a href="https://redirect.github.com/ljharb/qs/issues/326">#326</a>)</li>
<li>[New] [Fix] stringify symbols and bigints</li>
<li>[Fix] ensure node 0.12 can stringify Symbols</li>
<li>[Fix] fix for an impossible situation: when the formatter is called with a non-string value</li>
<li>[Refactor] <code>formats</code>: tiny bit of cleanup.</li>
<li>[Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>browserify</code>, <code>safe-publish-latest</code>, <code>iconv-lite</code>, <code>tape</code></li>
<li>[Tests] add tests for <code>depth=0</code> and <code>depth=false</code> behavior, both current and intuitive/intended (<a href="https://redirect.github.com/ljharb/qs/issues/326">#326</a>)</li>
<li>[Tests] use <code>eclint</code> instead of <code>editorconfig-tools</code></li>
<li>[docs] readme: add security note</li>
<li>[meta] add github sponsorship</li>
<li>[meta] add FUNDING.yml</li>
<li>[meta] Clean up license text so it’s properly detected as BSD-3-Clause</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ljharb/qs/commit/0db55386013a5d92503944ad42022fd8c112c983"><code>0db5538</code></a> v6.8.3</li>
<li><a href="https://github.com/ljharb/qs/commit/639a381a66845925dba32531dcb9d21c446e9f1f"><code>639a381</code></a> [meta] do not publish workflow files</li>
<li><a href="https://github.com/ljharb/qs/commit/fc3682776670524a42e19709ec4a8138d0d7afda"><code>fc36827</code></a> [Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://redirect.github.com/ljharb/qs/issues/428">#428</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/4e312c487def80b879d5359e0d1991ce17685191"><code>4e312c4</code></a> [Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://redirect.github.com/ljharb/qs/issues/427">#427</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/57918dae411c17b232377759baaa52a642762950"><code>57918da</code></a> [Fix] <code>stringify</code>: avoid encoding arrayformat comma when `encodeValuesOnly = ...</li>
<li><a href="https://github.com/ljharb/qs/commit/48673cae0226de23f6f33cc0e17af893b42f5e37"><code>48673ca</code></a> [readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li><a href="https://github.com/ljharb/qs/commit/554ba810f1a49a25dd27c09a466490cedbee5c65"><code>554ba81</code></a> [Tests] clean up stringify tests slightly</li>
<li><a href="https://github.com/ljharb/qs/commit/dbb54a8f14573e3c7512ea01d99f75f6ce0571f8"><code>dbb54a8</code></a> [Docs] add note and links for coercing primitive values (<a href="https://redirect.github.com/ljharb/qs/issues/408">#408</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/6868128ca2bd247ba935fbb63d359d0417f6b283"><code>6868128</code></a> [meta] fix README.md (<a href="https://redirect.github.com/ljharb/qs/issues/399">#399</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/49bed6934b27c3f0ef50e1fcee8d76298d108d52"><code>49bed69</code></a> [actions] backport actions from main</li>
<li>Additional commits viewable in <a href="https://github.com/ljharb/qs/compare/v6.7.3...v6.8.3">compare view</a></li>
</ul>
</details>
<br />

Updates `vite` from 5.0.13 to 5.1.7
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vitejs/vite/releases">vite's releases</a>.</em></p>
<blockquote>
<h2>create-vite@5.1.0</h2>
<p>Please refer to <a href="https://github.com/vitejs/vite/blob/create-vite@5.1.0/packages/create-vite/CHANGELOG.md">CHANGELOG.md</a> for details.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vitejs/vite/blob/v5.1.7/packages/vite/CHANGELOG.md">vite's changelog</a>.</em></p>
<blockquote>
<h2><!-- raw HTML omitted -->5.1.7 (2024-03-24)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: <code>fs.deny</code> with globs with directories (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16250">#16250</a>) (<a href="https://github.com/vitejs/vite/commit/5a056dd">5a056dd</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16250">#16250</a></li>
</ul>
<h2><!-- raw HTML omitted -->5.1.6 (2024-03-11)<!-- raw HTML omitted --></h2>
<ul>
<li>chore(deps): update all non-major dependencies (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16131">#16131</a>) (<a href="https://github.com/vitejs/vite/commit/a862ecb">a862ecb</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16131">#16131</a></li>
<li>fix: check for publicDir before checking if it is a parent directory (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16046">#16046</a>) (<a href="https://github.com/vitejs/vite/commit/b6fb323">b6fb323</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16046">#16046</a></li>
<li>fix: escape single quote when relative base is used (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16060">#16060</a>) (<a href="https://github.com/vitejs/vite/commit/8f74ce4">8f74ce4</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16060">#16060</a></li>
<li>fix: handle function property extension in namespace import (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16113">#16113</a>) (<a href="https://github.com/vitejs/vite/commit/f699194">f699194</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16113">#16113</a></li>
<li>fix: server middleware mode resolve (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16122">#16122</a>) (<a href="https://github.com/vitejs/vite/commit/8403546">8403546</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16122">#16122</a></li>
<li>fix(esbuild): update tsconfck to fix bug that could cause a deadlock  (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16124">#16124</a>) (<a href="https://github.com/vitejs/vite/commit/fd9de04">fd9de04</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16124">#16124</a></li>
<li>fix(worker): hide &quot;The emitted file overwrites&quot; warning if the content is same (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16094">#16094</a>) (<a href="https://github.com/vitejs/vite/commit/60dfa9e">60dfa9e</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16094">#16094</a></li>
<li>fix(worker): throw error when circular worker import is detected and support self referencing worker (<a href="https://github.com/vitejs/vite/commit/eef9da1">eef9da1</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16103">#16103</a></li>
<li>style(utils): remove null check (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16112">#16112</a>) (<a href="https://github.com/vitejs/vite/commit/0d2df52">0d2df52</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16112">#16112</a></li>
<li>refactor(runtime): share more code between runtime and main bundle (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16063">#16063</a>) (<a href="https://github.com/vitejs/vite/commit/93be84e">93be84e</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16063">#16063</a></li>
</ul>
<h2><!-- raw HTML omitted -->5.1.5 (2024-03-04)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: <code>__vite__mapDeps</code> code injection (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15732">#15732</a>) (<a href="https://github.com/vitejs/vite/commit/aff54e1">aff54e1</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15732">#15732</a></li>
<li>fix: analysing build chunk without dependencies (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15469">#15469</a>) (<a href="https://github.com/vitejs/vite/commit/bd52283">bd52283</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15469">#15469</a></li>
<li>fix: import with query with imports field (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16085">#16085</a>) (<a href="https://github.com/vitejs/vite/commit/ab823ab">ab823ab</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16085">#16085</a></li>
<li>fix: normalize literal-only entry pattern (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16010">#16010</a>) (<a href="https://github.com/vitejs/vite/commit/1dccc37">1dccc37</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16010">#16010</a></li>
<li>fix: optimizeDeps.entries with literal-only pattern(s) (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15853">#15853</a>) (<a href="https://github.com/vitejs/vite/commit/49300b3">49300b3</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15853">#15853</a></li>
<li>fix: output correct error for empty import specifier (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16055">#16055</a>) (<a href="https://github.com/vitejs/vite/commit/a9112eb">a9112eb</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16055">#16055</a></li>
<li>fix: upgrade esbuild to 0.20.x (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16062">#16062</a>) (<a href="https://github.com/vitejs/vite/commit/899d9b1">899d9b1</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16062">#16062</a></li>
<li>fix(runtime): runtime HMR affects only imported files (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15898">#15898</a>) (<a href="https://github.com/vitejs/vite/commit/57463fc">57463fc</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15898">#15898</a></li>
<li>fix(scanner): respect  <code>experimentalDecorators: true</code> (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15206">#15206</a>) (<a href="https://github.com/vitejs/vite/commit/4144781">4144781</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15206">#15206</a></li>
<li>revert: &quot;fix: upgrade esbuild to 0.20.x&quot; (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16072">#16072</a>) (<a href="https://github.com/vitejs/vite/commit/11cceea">11cceea</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16072">#16072</a></li>
<li>refactor: share code with vite runtime (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15907">#15907</a>) (<a href="https://github.com/vitejs/vite/commit/b20d542">b20d542</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15907">#15907</a></li>
<li>refactor(runtime): use functions from <code>pathe</code> (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16061">#16061</a>) (<a href="https://github.com/vitejs/vite/commit/aac2ef7">aac2ef7</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16061">#16061</a></li>
<li>chore(deps): update all non-major dependencies (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16028">#16028</a>) (<a href="https://github.com/vitejs/vite/commit/7cfe80d">7cfe80d</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16028">#16028</a></li>
</ul>
<h2><!-- raw HTML omitted -->5.1.4 (2024-02-21)<!-- raw HTML omitted --></h2>
<ul>
<li>perf: remove unnecessary regex s modifier (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15766">#15766</a>) (<a href="https://github.com/vitejs/vite/commit/8dc1b73">8dc1b73</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15766">#15766</a></li>
<li>fix: fs cached checks disabled by default for yarn pnp (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15920">#15920</a>) (<a href="https://github.com/vitejs/vite/commit/8b11fea">8b11fea</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15920">#15920</a></li>
<li>fix: resolve directory correctly when <code>fs.cachedChecks: true</code> (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15983">#15983</a>) (<a href="https://github.com/vitejs/vite/commit/4fe971f">4fe971f</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15983">#15983</a></li>
<li>fix: srcSet with optional descriptor (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15905">#15905</a>) (<a href="https://github.com/vitejs/vite/commit/81b3bd0">81b3bd0</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15905">#15905</a></li>
<li>fix(deps): update all non-major dependencies (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15959">#15959</a>) (<a href="https://github.com/vitejs/vite/commit/571a3fd">571a3fd</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15959">#15959</a></li>
<li>fix(watch): build watch fails when outDir is empty string (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15979">#15979</a>) (<a href="https://github.com/vitejs/vite/commit/1d263d3">1d263d3</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15979">#15979</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vitejs/vite/commit/e710c2fc6d45405b5f3431bbe812abbb27946aa0"><code>e710c2f</code></a> release: v5.1.7</li>
<li><a href="https://github.com/vitejs/vite/commit/5a056dd2fc80dbafed033062fe6aaf4717309f48"><code>5a056dd</code></a> fix: <code>fs.deny</code> with globs with directories (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16250">#16250</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/6f7466e6211027686f40ad7e4ce6ec8477414546"><code>6f7466e</code></a> release: v5.1.6</li>
<li><a href="https://github.com/vitejs/vite/commit/a862ecb941a432b6e3bab62331012e4b53ddd4e8"><code>a862ecb</code></a> chore(deps): update all non-major dependencies (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16131">#16131</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/840354601a2dbdb6419429999e1f9feff31a641f"><code>8403546</code></a> fix: server middleware mode resolve (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16122">#16122</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/b6fb3235c33b1490eb0d7a33b2b62d6fa7a5496f"><code>b6fb323</code></a> fix: check for publicDir before checking if it is a parent directory (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16046">#16046</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/fd9de0473e075c8d69bb3a8867ab15300506e67b"><code>fd9de04</code></a> fix(esbuild): update tsconfck to fix bug that could cause a deadlock  (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16124">#16124</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/f6991948f59e36bc5d108e2befa5883be99f934f"><code>f699194</code></a> fix: handle function property extension in namespace import (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16113">#16113</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/0d2df527168dec95b2967a3013bbf8c1ec8b0286"><code>0d2df52</code></a> style(utils): remove null check (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16112">#16112</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/eef9da13d0028161eacc0ea699988814f29a56e4"><code>eef9da1</code></a> fix(worker): throw error when circular worker import is detected and support ...</li>
<li>Additional commits viewable in <a href="https://github.com/vitejs/vite/commits/v5.1.7/packages/vite">compare view</a></li>
</ul>
</details>
<br />

Updates `pkg` from 4.5.1 to 5.8.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vercel/pkg/releases">pkg's releases</a>.</em></p>
<blockquote>
<h2>5.8.1</h2>
<h3>Patches</h3>
<ul>
<li>Producer: properly call &quot;prebuild-install&quot; if N-API is used: dd9de59c9fca2751bf5d22b57bd9b03d43e85e80</li>
<li>Chore: clean up obsolete eslint disable comments: <a href="https://redirect.github.com/vercel/pkg/issues/1760">#1760</a></li>
<li>Chore: add prettier check in linting step: <a href="https://redirect.github.com/vercel/pkg/issues/1764">#1764</a></li>
<li>Chore: separate individual test scripts: <a href="https://redirect.github.com/vercel/pkg/issues/1759">#1759</a></li>
<li>Chore: use <code>@types/babel__generator</code> package: <a href="https://redirect.github.com/vercel/pkg/issues/1755">#1755</a></li>
<li>Chore: remove unused entry: <a href="https://redirect.github.com/vercel/pkg/issues/1766">#1766</a></li>
<li>Chore: upgrade actions runners: <a href="https://redirect.github.com/vercel/pkg/issues/1767">#1767</a></li>
<li>Style: fix typo in test-99-<a href="https://redirect.github.com/vercel/pkg/issues/1192">#1192</a>/main.js: <a href="https://redirect.github.com/vercel/pkg/issues/1790">#1790</a></li>
<li>Chore: bump prebuild-install@7.1.1: <a href="https://redirect.github.com/vercel/pkg/issues/1788">#1788</a></li>
<li>Fix: add force flag to codesign to avoid already signed error: <a href="https://redirect.github.com/vercel/pkg/issues/1756">#1756</a></li>
</ul>
<h3>Credits</h3>
<p>Huge thanks to <a href="https://github.com/ignatiusmb"><code>@​ignatiusmb</code></a>, <a href="https://github.com/eltociear"><code>@​eltociear</code></a>, <a href="https://github.com/PraveenAnaparthi"><code>@​PraveenAnaparthi</code></a>, and <a href="https://github.com/brianunlam"><code>@​brianunlam</code></a> for helping!</p>
<h2>5.8.0</h2>
<h2>Highlights</h2>
<ul>
<li>Support more language features, including but not limited to <code>classPrivateMethods</code> (<a href="https://redirect.github.com/vercel/pkg/issues/1248">#1248</a>, <a href="https://redirect.github.com/vercel/pkg/issues/1249">#1249</a>)
<ul>
<li>Note: pkg uses Babel to trace dependencies. It does NOT transform your sources. You should make sure that your code can run on the target Node.js version.</li>
</ul>
</li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>Bump to vercel/pkg-fetch@v3.4.2 by <a href="https://github.com/jesec"><code>@​jesec</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1693">vercel/pkg#1693</a>
<ul>
<li>Add Node 14.20.0, 16.16.0 and 18.5.0 binaries</li>
<li><a href="https://nodejs.org/en/blog/vulnerability/july-2022-security-releases">https://nodejs.org/en/blog/vulnerability/july-2022-security-releases</a></li>
</ul>
</li>
<li>detector: use Babel AST and default plugins by <a href="https://github.com/jesec"><code>@​jesec</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1648">vercel/pkg#1648</a></li>
<li>test: rearrange and fix order by <a href="https://github.com/jesec"><code>@​jesec</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1650">vercel/pkg#1650</a></li>
<li>fix: typo in fabricator.ts by <a href="https://github.com/eltociear"><code>@​eltociear</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1661">vercel/pkg#1661</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/eltociear"><code>@​eltociear</code></a> made their first contribution in <a href="https://redirect.github.com/vercel/pkg/pull/1661">vercel/pkg#1661</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/vercel/pkg/compare/5.7.0...5.8.0">https://github.com/vercel/pkg/compare/5.7.0...5.8.0</a></p>
<h2>5.7.0</h2>
<h2>Highlights</h2>
<ul>
<li>Node 18 is now supported!</li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>Bump to vercel/pkg-fetch@v3.4.1 by <a href="https://github.com/jesec"><code>@​jesec</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1616">vercel/pkg#1616</a>
<ul>
<li>No longer take NODE_OPTIONS from the environment of the end-user. Only the users (developers who use pkg to package their project) should have control over the flags via the &quot;bake in&quot; (--options) mechanism (Fixes: <a href="https://redirect.github.com/vercel/pkg/issues/954">vercel/pkg#954</a>, <a href="https://redirect.github.com/vercel/pkg/issues/989">vercel/pkg#989</a>, <a href="https://redirect.github.com/vercel/pkg/issues/1194">vercel/pkg#1194</a>, <a href="https://redirect.github.com/vercel/pkg/issues/1517">vercel/pkg#1517</a>)</li>
<li>Patched Node: bump to 16.15.0, add 18.1.0 and drop 17</li>
</ul>
</li>
<li>fix broken tests on node 12; latest pnpm requires node &gt;= 14.19 by <a href="https://github.com/kldzj"><code>@​kldzj</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1613">vercel/pkg#1613</a></li>
<li>dependencies: bump (minor) by <a href="https://github.com/jesec"><code>@​jesec</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1615">vercel/pkg#1615</a></li>
<li>fix(bootstrap): prevent to override existing node addon file by <a href="https://github.com/renkei"><code>@​renkei</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1611">vercel/pkg#1611</a></li>
</ul>
<h2>New Contributors</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vercel/pkg/commit/5dc987b90ffd191263eb0202833dc382cea0d47d"><code>5dc987b</code></a> 5.8.1</li>
<li><a href="https://github.com/vercel/pkg/commit/f19285db72f4592110f49335923d9199da49a137"><code>f19285d</code></a> fix: add force flag to codesign to avoid already signed error (<a href="https://redirect.github.com/vercel/pkg/issues/1756">#1756</a>)</li>
<li><a href="https://github.com/vercel/pkg/commit/e3ac4902e9cb023f0ac2a596e21ff9166d2e268c"><code>e3ac490</code></a> chore: bump prebuild-install@7.1.1 (<a href="https://redirect.github.com/vercel/pkg/issues/1788">#1788</a>)</li>
<li><a href="https://github.com/vercel/pkg/commit/be1123c474b3653abf3bfb89c068378f66b3849b"><code>be1123c</code></a> style: fix typo in test-99-<a href="https://redirect.github.com/vercel/pkg/issues/1192">#1192</a>/main.js (<a href="https://redirect.github.com/vercel/pkg/issues/1790">#1790</a>)</li>
<li><a href="https://github.com/vercel/pkg/commit/614c02a06830e0a4a898e6cf4eb35dbbf6110af3"><code>614c02a</code></a> chore: upgrade actions runners (<a href="https://redirect.github.com/vercel/pkg/issues/1767">#1767</a>)</li>
<li><a href="https://github.com/vercel/pkg/commit/39e99859fe2fd33fb59c4a75318389b477c1a443"><code>39e9985</code></a> chore: remove unused entry (<a href="https://redirect.github.com/vercel/pkg/issues/1766">#1766</a>)</li>
<li><a href="https://github.com/vercel/pkg/commit/b8deba40c0c9dced29e5c15aaefe575285e716d6"><code>b8deba4</code></a> chore: use <code>@types/babel__generator</code> package (<a href="https://redirect.github.com/vercel/pkg/issues/1755">#1755</a>)</li>
<li><a href="https://github.com/vercel/pkg/commit/332c7d971a6a8f918f6d24470557f2dcb1de5abf"><code>332c7d9</code></a> chore: separate individual test scripts (<a href="https://redirect.github.com/vercel/pkg/issues/1759">#1759</a>)</li>
<li><a href="https://github.com/vercel/pkg/commit/6efa7cfbbac323a019680609c2c78bbf7b9fff0f"><code>6efa7cf</code></a> chore: add prettier check in linting step (<a href="https://redirect.github.com/vercel/pkg/issues/1764">#1764</a>)</li>
<li><a href="https://github.com/vercel/pkg/commit/56135b583b901d552e3780e749e79e70e71fd3ea"><code>56135b5</code></a> chore: clean up obsolete eslint disable comments (<a href="https://redirect.github.com/vercel/pkg/issues/1760">#1760</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/vercel/pkg/compare/4.5.1...5.8.1">compare view</a></li>
</ul>
</details>
<br />

Updates `@adobe/css-tools` from 4.2.0 to 4.3.3
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/adobe/css-tools/blob/main/History.md"><code>@​adobe/css-tools</code>'s changelog</a>.</em></p>
<blockquote>
<h1>4.3.3 / 2024-01-24</h1>
<ul>
<li>Update export property <a href="https://redirect.github.com/adobe/css-tools/issues/271">#271</a></li>
</ul>
<h1>4.3.2 / 2023-11-28</h1>
<ul>
<li>Fix redos vulnerability with specific crafted css string - CVE-2023-48631</li>
<li>Fix Problem parsing with :is() and nested :nth-child() <a href="https://redirect.github.com/adobe/css-tools/issues/211">#211</a></li>
</ul>
<h1>4.3.1 / 2023-03-14</h1>
<ul>
<li>Fix redos vulnerability with specific crafted css string - CVE-2023-26364</li>
</ul>
<h1>4.3.0 / 2023-03-07</h1>
<ul>
<li>Update build tools</li>
<li>Update exports path and files</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/adobe/css-tools/commits">compare view</a></li>
</ul>
</details>
<br />

Updates `apollo-server-core` from 3.12.0 to 3.13.0
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/apollographql/apollo-server/commit/f93284e853efd6da46d91ae40da47a2dd15b61fe"><code>f93284e</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/4745ebed69775959212bbca7b02cff65c1f0dc64"><code>4745ebe</code></a> Rename option from disableValidation to dangerouslyDisableValidation</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/11f5981067f570c60a0003b51f3d634ebd8fa792"><code>11f5981</code></a> Add disableValidation option to apollo-server-core</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/ea2e2c3e071afc9144af00cae7b51720b9cc8b32"><code>ea2e2c3</code></a> Release</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/1dd45b8366a6cee75e4ca321eeb5acf107e6c73e"><code>1dd45b8</code></a> get CI passing</li>
<li><a href="https://github.com/apollographql/apollo-server/commit/d38b43bac88acdef4295759d7dcc3d4c348d9575"><code>d38b43b</code></a> Merge pull request from GHSA-j5g3-5c8r-7qfx</li>
<li>See full diff in <a href="https://github.com/apollographql/apollo-server/commits/apollo-server-core@3.13.0/packages/apollo-server-core">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~apollo-bot">apollo-bot</a>, a new releaser for apollo-server-core since your current version.</p>
</details>
<br />

Updates `browserify-sign` from 4.2.1 to 4.2.3
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/browserify/browserify-sign/blob/main/CHANGELOG.md">bro...

_Description has been truncated_
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-15 06:36:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3263" class=".btn">#3263</a>
            </td>
            <td>
                <b>
                    build: bump the go_modules group across 9 directories with 2 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps the go_modules group with 1 update in the /weaver/common/protos-go directory: google.golang.org/protobuf.
Bumps the go_modules group with 2 updates in the /weaver/samples/fabric/go-cli directory: google.golang.org/protobuf and [github.com/prometheus/client_golang](https://github.com/prometheus/client_golang).
Bumps the go_modules group with 1 update in the /weaver/samples/fabric/satpsimpleasset directory: google.golang.org/protobuf.
Bumps the go_modules group with 1 update in the /weaver/samples/fabric/simpleasset directory: google.golang.org/protobuf.
Bumps the go_modules group with 1 update in the /weaver/samples/fabric/simpleassetandinterop directory: google.golang.org/protobuf.
Bumps the go_modules group with 1 update in the /weaver/samples/fabric/simpleassettransfer directory: google.golang.org/protobuf.
Bumps the go_modules group with 1 update in the /weaver/samples/fabric/simplestate directory: google.golang.org/protobuf.
Bumps the go_modules group with 1 update in the /weaver/samples/fabric/simplestatewithacl directory: google.golang.org/protobuf.
Bumps the go_modules group with 1 update in the /weaver/sdks/fabric/go-sdk directory: google.golang.org/protobuf.

Updates `google.golang.org/protobuf` from 1.30.0 to 1.33.0

Updates `google.golang.org/protobuf` from 1.31.0 to 1.33.0

Updates `github.com/prometheus/client_golang` from 1.3.0 to 1.11.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/prometheus/client_golang/releases">github.com/prometheus/client_golang's releases</a>.</em></p>
<blockquote>
<h2>1.11.1 / 2022-02-15</h2>
<ul>
<li>[SECURITY FIX] promhttp: Check validity of method and code label values <a href="https://redirect.github.com/prometheus/client_golang/pull/987">prometheus/client_golang#987</a> (Addressed <a href="https://github.com/prometheus/client_golang/security/advisories/GHSA-cg3q-j54f-5p7p"><code>CVE-2022-21698</code></a>)</li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>promhttp: Check validity of method and code label values by <a href="https://github.com/bwplotka"><code>@​bwplotka</code></a> and <a href="https://github.com/kakkoyun"><code>@​kakkoyun</code></a> in  <a href="https://redirect.github.com/prometheus/client_golang/pull/987">prometheus/client_golang#987</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/prometheus/client_golang/compare/v1.11.0...v1.11.1">https://github.com/prometheus/client_golang/compare/v1.11.0...v1.11.1</a></p>
<h2>v1.11.0 / 2021-06-07</h2>
<ul>
<li>[CHANGE] Add new collectors package. <a href="https://redirect.github.com/prometheus/client_golang/issues/862">#862</a></li>
<li>[CHANGE] <code>prometheus.NewExpvarCollector</code> is deprecated, use <code>collectors.NewExpvarCollector</code> instead. <a href="https://redirect.github.com/prometheus/client_golang/issues/862">#862</a></li>
<li>[CHANGE] <code>prometheus.NewGoCollector</code> is deprecated, use <code>collectors.NewGoCollector</code> instead. <a href="https://redirect.github.com/prometheus/client_golang/issues/862">#862</a></li>
<li>[CHANGE] <code>prometheus.NewBuildInfoCollector</code> is deprecated, use <code>collectors.NewBuildInfoCollector</code> instead. <a href="https://redirect.github.com/prometheus/client_golang/issues/862">#862</a></li>
<li>[FEATURE] Add new collector for database/sql#DBStats. <a href="https://redirect.github.com/prometheus/client_golang/issues/866">#866</a></li>
<li>[FEATURE] API client: Add exemplars API support. <a href="https://redirect.github.com/prometheus/client_golang/issues/861">#861</a></li>
<li>[ENHANCEMENT] API client: Add newer fields to Rules API. <a href="https://redirect.github.com/prometheus/client_golang/issues/855">#855</a></li>
<li>[ENHANCEMENT] API client: Add missing fields to Targets API. <a href="https://redirect.github.com/prometheus/client_golang/issues/856">#856</a></li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>Synchronize common files from prometheus/prometheus by <a href="https://github.com/prombot"><code>@​prombot</code></a> in <a href="https://redirect.github.com/prometheus/client_golang/pull/846">prometheus/client_golang#846</a></li>
<li>Synchronize common files from prometheus/prometheus by <a href="https://github.com/prombot"><code>@​prombot</code></a> in <a href="https://redirect.github.com/prometheus/client_golang/pull/849">prometheus/client_golang#849</a></li>
<li>Synchronize common files from prometheus/prometheus by <a href="https://github.com/prombot"><code>@​prombot</code></a> in <a href="https://redirect.github.com/prometheus/client_golang/pull/853">prometheus/client_golang#853</a></li>
<li>Add newer fields to Rules API by <a href="https://github.com/gouthamve"><code>@​gouthamve</code></a> in <a href="https://redirect.github.com/prometheus/client_golang/pull/855">prometheus/client_golang#855</a></li>
<li>Add missing fields to targets API by <a href="https://github.com/yeya24"><code>@​yeya24</code></a> in <a href="https://redirect.github.com/prometheus/client_golang/pull/856">prometheus/client_golang#856</a></li>
<li>Synchronize common files from prometheus/prometheus by <a href="https://github.com/prombot"><code>@​prombot</code></a> in <a href="https://redirect.github.com/prometheus/client_golang/pull/857">prometheus/client_golang#857</a></li>
<li>Add exemplars API support by <a href="https://github.com/yeya24"><code>@​yeya24</code></a> in <a href="https://redirect.github.com/prometheus/client_golang/pull/861">prometheus/client_golang#861</a></li>
<li>Improve description of MaxAge in summary docs by <a href="https://github.com/Dean-Coakley"><code>@​Dean-Coakley</code></a> in <a href="https://redirect.github.com/prometheus/client_golang/pull/864">prometheus/client_golang#864</a></li>
<li>Add new collectors package by <a href="https://github.com/johejo"><code>@​johejo</code></a> in <a href="https://redirect.github.com/prometheus/client_golang/pull/862">prometheus/client_golang#862</a></li>
<li>Add collector for database/sql#DBStats by <a href="https://github.com/johejo"><code>@​johejo</code></a> in <a href="https://redirect.github.com/prometheus/client_golang/pull/866">prometheus/client_golang#866</a></li>
<li>Make dbStatsCollector more DRY by <a href="https://github.com/beorn7"><code>@​beorn7</code></a> in <a href="https://redirect.github.com/prometheus/client_golang/pull/867">prometheus/client_golang#867</a></li>
<li>Change maintainers from <a href="https://github.com/beorn7"><code>@​beorn7</code></a> to @bwplotka/<a href="https://github.com/kakkoyun"><code>@​kakkoyun</code></a> by <a href="https://github.com/beorn7"><code>@​beorn7</code></a> in <a href="https://redirect.github.com/prometheus/client_golang/pull/873">prometheus/client_golang#873</a></li>
<li>Document implications of negative observations by <a href="https://github.com/beorn7"><code>@​beorn7</code></a> in <a href="https://redirect.github.com/prometheus/client_golang/pull/871">prometheus/client_golang#871</a></li>
<li>Update Go modules by <a href="https://github.com/SuperQ"><code>@​SuperQ</code></a> in <a href="https://redirect.github.com/prometheus/client_golang/pull/875">prometheus/client_golang#875</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/gouthamve"><code>@​gouthamve</code></a> made their first contribution in <a href="https://redirect.github.com/prometheus/client_golang/pull/855">prometheus/client_golang#855</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/prometheus/client_golang/compare/v1.10.0...v1.11.0">https://github.com/prometheus/client_golang/compare/v1.10.0...v1.11.0</a></p>
<h2>1.10.0 / 2021-03-18</h2>
<ul>
<li>[CHANGE] Minimum required Go version is now 1.13.</li>
<li>[CHANGE] API client: Add matchers to <code>LabelNames</code> and <code>LabesValues</code>. <a href="https://redirect.github.com/prometheus/client_golang/issues/828">#828</a></li>
<li>[FEATURE] API client: Add buildinfo call. <a href="https://redirect.github.com/prometheus/client_golang/issues/841">#841</a></li>
<li>[BUGFIX] Fix build on riscv64. <a href="https://redirect.github.com/prometheus/client_golang/issues/833">#833</a></li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>Add SECURITY.md by <a href="https://github.com/roidelapluie"><code>@​roidelapluie</code></a> in <a href="https://redirect.github.com/prometheus/client_golang/pull/831">prometheus/client_golang#831</a></li>
<li>Bump prometheus/procfs to 0.3.0 to fix building on riscv64 by <a href="https://github.com/zhsj"><code>@​zhsj</code></a> in <a href="https://redirect.github.com/prometheus/client_golang/pull/833">prometheus/client_golang#833</a></li>
<li>Fix typo in comments in <a href="https://redirect.github.com/prometheus/client_golang/pull/835">prometheus/client_golang#835</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/prometheus/client_golang/blob/main/CHANGELOG.md">github.com/prometheus/client_golang's changelog</a>.</em></p>
<blockquote>
<h2>Unreleased</h2>
<h2>1.19.0 / 2023-02-27</h2>
<p>The module <code>prometheus/common v0.48.0</code> introduced an incompatibility when used together with client_golang (See <a href="https://redirect.github.com/prometheus/client_golang/pull/1448">prometheus/client_golang#1448</a> for more details). If your project uses client_golang and you want to use <code>prometheus/common v0.48.0</code> or higher, please update client_golang to v1.19.0.</p>
<ul>
<li>[CHANGE] Minimum required go version is now 1.20 (we also test client_golang against new 1.22 version). <a href="https://redirect.github.com/prometheus/client_golang/issues/1445">#1445</a> <a href="https://redirect.github.com/prometheus/client_golang/issues/1449">#1449</a></li>
<li>[FEATURE] collectors: Add version collector. <a href="https://redirect.github.com/prometheus/client_golang/issues/1422">#1422</a> <a href="https://redirect.github.com/prometheus/client_golang/issues/1427">#1427</a></li>
</ul>
<h2>1.18.0 / 2023-12-22</h2>
<ul>
<li>[FEATURE] promlint: Allow creation of custom metric validations. <a href="https://redirect.github.com/prometheus/client_golang/issues/1311">#1311</a></li>
<li>[FEATURE] Go programs using client_golang can be built in wasip1 OS. <a href="https://redirect.github.com/prometheus/client_golang/issues/1350">#1350</a></li>
<li>[BUGFIX] histograms: Add timer to reset ASAP after bucket limiting has happened. <a href="https://redirect.github.com/prometheus/client_golang/issues/1367">#1367</a></li>
<li>[BUGFIX] testutil: Fix comparison of metrics with empty Help strings. <a href="https://redirect.github.com/prometheus/client_golang/issues/1378">#1378</a></li>
<li>[ENHANCEMENT] Improved performance of <code>MetricVec.WithLabelValues(...)</code>. <a href="https://redirect.github.com/prometheus/client_golang/issues/1360">#1360</a></li>
</ul>
<h2>1.17.0 / 2023-09-27</h2>
<ul>
<li>[CHANGE] Minimum required go version is now 1.19 (we also test client_golang against new 1.21 version). <a href="https://redirect.github.com/prometheus/client_golang/issues/1325">#1325</a></li>
<li>[FEATURE] Add support for Created Timestamps in Counters, Summaries and Historams. <a href="https://redirect.github.com/prometheus/client_golang/issues/1313">#1313</a></li>
<li>[ENHANCEMENT] Enable detection of a native histogram without observations. <a href="https://redirect.github.com/prometheus/client_golang/issues/1314">#1314</a></li>
</ul>
<h2>1.16.0 / 2023-06-15</h2>
<ul>
<li>[BUGFIX] api: Switch to POST for LabelNames, Series, and QueryExemplars. <a href="https://redirect.github.com/prometheus/client_golang/issues/1252">#1252</a></li>
<li>[BUGFIX] api: Fix undefined execution order in return statements. <a href="https://redirect.github.com/prometheus/client_golang/issues/1260">#1260</a></li>
<li>[BUGFIX] native histograms: Fix bug in bucket key calculation. <a href="https://redirect.github.com/prometheus/client_golang/issues/1279">#1279</a></li>
<li>[ENHANCEMENT] Reduce constrainLabels allocations for all metrics. <a href="https://redirect.github.com/prometheus/client_golang/issues/1272">#1272</a></li>
<li>[ENHANCEMENT] promhttp: Add process start time header for scrape efficiency. <a href="https://redirect.github.com/prometheus/client_golang/issues/1278">#1278</a></li>
<li>[ENHANCEMENT] promlint: Improve metricUnits runtime. <a href="https://redirect.github.com/prometheus/client_golang/issues/1286">#1286</a></li>
</ul>
<h2>1.15.1 / 2023-05-3</h2>
<ul>
<li>[BUGFIX] Fixed promhttp.Instrument* handlers wrongly trying to attach exemplar to unsupported metrics (e.g. summary), <br />
causing panics. <a href="https://redirect.github.com/prometheus/client_golang/issues/1253">#1253</a></li>
</ul>
<h2>1.15.0 / 2023-04-13</h2>
<ul>
<li>[BUGFIX] Fix issue with atomic variables on ppc64le. <a href="https://redirect.github.com/prometheus/client_golang/issues/1171">#1171</a></li>
<li>[BUGFIX] Support for multiple samples within same metric. <a href="https://redirect.github.com/prometheus/client_golang/issues/1181">#1181</a></li>
<li>[BUGFIX] Bump golang.org/x/text to v0.3.8 to mitigate CVE-2022-32149. <a href="https://redirect.github.com/prometheus/client_golang/issues/1187">#1187</a></li>
<li>[ENHANCEMENT] Add exemplars and middleware examples. <a href="https://redirect.github.com/prometheus/client_golang/issues/1173">#1173</a></li>
<li>[ENHANCEMENT] Add more context to &quot;duplicate label names&quot; error to enable debugging. <a href="https://redirect.github.com/prometheus/client_golang/issues/1177">#1177</a></li>
<li>[ENHANCEMENT] Add constrained labels and constrained variant for all MetricVecs. <a href="https://redirect.github.com/prometheus/client_golang/issues/1151">#1151</a></li>
<li>[ENHANCEMENT] Moved away from deprecated github.com/golang/protobuf package. <a href="https://redirect.github.com/prometheus/client_golang/issues/1183">#1183</a></li>
<li>[ENHANCEMENT] Add possibility to dynamically get label values for http instrumentation. <a href="https://redirect.github.com/prometheus/client_golang/issues/1066">#1066</a></li>
<li>[ENHANCEMENT] Add ability to Pusher to add custom headers. <a href="https://redirect.github.com/prometheus/client_golang/issues/1218">#1218</a></li>
<li>[ENHANCEMENT] api: Extend and improve efficiency of json-iterator usage. <a href="https://redirect.github.com/prometheus/client_golang/issues/1225">#1225</a></li>
<li>[ENHANCEMENT] Added (official) support for go 1.20. <a href="https://redirect.github.com/prometheus/client_golang/issues/1234">#1234</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/prometheus/client_golang/commit/989baa30fe956631907493ccee1f8e7708660d96"><code>989baa3</code></a> promhttp: Check validity of method and code label values (<a href="https://redirect.github.com/prometheus/client_golang/issues/962">#962</a>) (<a href="https://redirect.github.com/prometheus/client_golang/issues/987">#987</a>)</li>
<li><a href="https://github.com/prometheus/client_golang/commit/8184d76b3b0bd3b01ed903690431ccb6826bf3e0"><code>8184d76</code></a> Cut v1.11.0 (<a href="https://redirect.github.com/prometheus/client_golang/issues/877">#877</a>)</li>
<li><a href="https://github.com/prometheus/client_golang/commit/253906201bda760621fa671fa1541a4ac3df29bd"><code>2539062</code></a> Merge pull request <a href="https://redirect.github.com/prometheus/client_golang/issues/875">#875</a> from prometheus/superq/update_mods</li>
<li><a href="https://github.com/prometheus/client_golang/commit/68cd1e9262e2fe03a79c9a8bab6737f04995e8a5"><code>68cd1e9</code></a> Update Go modules</li>
<li><a href="https://github.com/prometheus/client_golang/commit/f22935db759faadc48285fee37718436d5b9cb67"><code>f22935d</code></a> Merge pull request <a href="https://redirect.github.com/prometheus/client_golang/issues/871">#871</a> from prometheus/beorn7/doc</li>
<li><a href="https://github.com/prometheus/client_golang/commit/11aba26a91c3ea0581eef96f8ec9fc5cdce204f9"><code>11aba26</code></a> Change maintainers from <a href="https://github.com/beorn7"><code>@​beorn7</code></a> to @bwplotka/<a href="https://github.com/kakkoyun"><code>@​kakkoyun</code></a> (<a href="https://redirect.github.com/prometheus/client_golang/issues/873">#873</a>)</li>
<li><a href="https://github.com/prometheus/client_golang/commit/f34145a85eaff9d42ff629a2975e8118ab41773c"><code>f34145a</code></a> Document implications of negative observations</li>
<li><a href="https://github.com/prometheus/client_golang/commit/a7515ca7c9c6388a5ab84ea336faef795bbf866f"><code>a7515ca</code></a> Merge pull request <a href="https://redirect.github.com/prometheus/client_golang/issues/867">#867</a> from prometheus/beorn7/collectors</li>
<li><a href="https://github.com/prometheus/client_golang/commit/81a9556c8b4ffac3dd75f7aedf720b3ae73e1276"><code>81a9556</code></a> Make dbStatsCollector more DRY</li>
<li><a href="https://github.com/prometheus/client_golang/commit/a66da1df4a7e12cb9f84cf5ae3c7adec4539ed27"><code>a66da1d</code></a> Add collector for database/sql#DBStats (<a href="https://redirect.github.com/prometheus/client_golang/issues/866">#866</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/prometheus/client_golang/compare/v1.3.0...v1.11.1">compare view</a></li>
</ul>
</details>
<br />

Updates `google.golang.org/protobuf` from 1.30.0 to 1.33.0

Updates `google.golang.org/protobuf` from 1.30.0 to 1.33.0

Updates `google.golang.org/protobuf` from 1.30.0 to 1.33.0

Updates `google.golang.org/protobuf` from 1.30.0 to 1.33.0

Updates `google.golang.org/protobuf` from 1.30.0 to 1.33.0

Updates `google.golang.org/protobuf` from 1.30.0 to 1.33.0

Updates `google.golang.org/protobuf` from 1.31.0 to 1.33.0


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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-15 06:06:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3262" class=".btn">#3262</a>
            </td>
            <td>
                <b>
                    build: bump rustls from 0.21.9 to 0.21.12 in /packages/cactus-core-api in the cargo group across 1 directory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps the cargo group with 1 update in the /packages/cactus-core-api directory: [rustls](https://github.com/rustls/rustls).

Updates `rustls` from 0.21.9 to 0.21.12
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rustls/rustls/commit/3633152cc557cceadb0f71fa7226e6051fb6a9ee"><code>3633152</code></a> Cargo: v0.21.11 -&gt; v0.21.12</li>
<li><a href="https://github.com/rustls/rustls/commit/0baaeba7a8b7961108810fe0ae108d3dc45cf35e"><code>0baaeba</code></a> proj: MSRV 1.61 -&gt; 1.63</li>
<li><a href="https://github.com/rustls/rustls/commit/6fd691a1018297e7299b91eb2a840da579c286df"><code>6fd691a</code></a> tls13: fix clippy::unnecessary_lazy_evaluations finding</li>
<li><a href="https://github.com/rustls/rustls/commit/6da53375a2910e7dda1752b3d2072a77f1a00e39"><code>6da5337</code></a> Test for illegal IP address in server name extension</li>
<li><a href="https://github.com/rustls/rustls/commit/75f8857db71f128fb521e77135744c97453a6e4b"><code>75f8857</code></a> Ignore server_name extension containing IP address</li>
<li><a href="https://github.com/rustls/rustls/commit/7b8d1dbc1e666dc4d83640c64e96d257d39cfda4"><code>7b8d1db</code></a> Prepare 0.21.11</li>
<li><a href="https://github.com/rustls/rustls/commit/ebcb4782f23b4edf9b10a7065d9e8d4362439d9c"><code>ebcb478</code></a> complete_io: bail out if progress is impossible</li>
<li><a href="https://github.com/rustls/rustls/commit/20f35dfb6d3c353294c562723d4cb6639a8bd01b"><code>20f35df</code></a> Regression test for <code>complete_io</code> infinite loop bug</li>
<li><a href="https://github.com/rustls/rustls/commit/2f2aae15a4293639669291ab2b257835a2d4bdca"><code>2f2aae1</code></a> Don't specially handle unauthenticated close_notify alerts</li>
<li><a href="https://github.com/rustls/rustls/commit/e163587b985c894a6ce651992b91eb6897edde8b"><code>e163587</code></a> Don't deny warnings from nightly clippy</li>
<li>Additional commits viewable in <a href="https://github.com/rustls/rustls/compare/v/0.21.9...v/0.21.12">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=rustls&package-manager=cargo&previous-version=0.21.9&new-version=0.21.12)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-15 06:05:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3257" class=".btn">#3257</a>
            </td>
            <td>
                <b>
                    bump Up open-api version to 6.6.0 of rust implementation of cactus-pl…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix #2181 
changes have been made to packages/cactus-plugin-keychain-memory-wasm
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-12 12:16:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3255" class=".btn">#3255</a>
            </td>
            <td>
                <b>
                    build(plugin-keychain-memory): fix local imports broken due to .js exts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Found the solution and a long discussion about it here:
https://github.com/kulshekhar/ts-jest/issues/1057

TLDR: The Jest resolver needs a little extra information/tweak to the
config so that it can correctly handle the .js imports.

Specifically this comment provided the solution which I made here:
https://github.com/kulshekhar/ts-jest/issues/1057#issuecomment-1482644543

Fixes #3254

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-10 18:45:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3253" class=".btn">#3253</a>
            </td>
            <td>
                <b>
                    chore(build.md): update documentation regarding deprecated scripts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit** to be reviewed
---
chore(build.md): update documentation regarding deprecated scripts
```
Primary Changes
---------------

1. Remove the Youtube video links from Cactus documentation
2. Added Go installation and updated node version
3. Checked for deprecated scripts in the md files
```
fixes: #1272

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-10 04:49:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3252" class=".btn">#3252</a>
            </td>
            <td>
                <b>
                    Satp 3100 cctx fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Pull Request Requirements**
- [ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-09 12:31:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3251" class=".btn">#3251</a>
            </td>
            <td>
                <b>
                    Bridge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-09 11:57:47 +0000 UTC
    </div>
</div>

