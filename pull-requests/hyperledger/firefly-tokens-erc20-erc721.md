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
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/105" class=".btn">#105</a>
            </td>
            <td>
                <b>
                    Bump json5 and tsconfig-paths
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [json5](https://github.com/json5/json5) to 2.2.3 and updates ancestor dependency [tsconfig-paths](https://github.com/dividab/tsconfig-paths). These dependencies need to be updated together.

Updates `json5` from 2.2.1 to 2.2.3
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/releases">json5's releases</a>.</em></p>
<blockquote>
<h2>v2.2.3</h2>
<ul>
<li>Fix: json5@2.2.3 is now the 'latest' release according to npm instead of v1.0.2. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/299">#299</a>)</li>
</ul>
<h2>v2.2.2</h2>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays.
(<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by
Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/blob/main/CHANGELOG.md">json5's changelog</a>.</em></p>
<blockquote>
<h3>v2.2.3 [<a href="https://github.com/json5/json5/tree/v2.2.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.2...v2.2.3">diff</a>]</h3>
<ul>
<li>Fix: json5@2.2.3 is now the 'latest' release according to npm instead of
v1.0.2. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/299">#299</a>)</li>
</ul>
<h3>v2.2.2 [<a href="https://github.com/json5/json5/tree/v2.2.2">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.1...v2.2.2">diff</a>]</h3>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays.
(<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by
Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/json5/json5/commit/c3a75242772a5026a49c4017a16d9b3543b62776"><code>c3a7524</code></a> 2.2.3</li>
<li><a href="https://github.com/json5/json5/commit/94fd06d82eeed225fa172f6fb2ca27375cbd2e39"><code>94fd06d</code></a> docs: update CHANGELOG for v2.2.3</li>
<li><a href="https://github.com/json5/json5/commit/3b8cebf0c474a8b20c78bd75c89cca0c4dce84ce"><code>3b8cebf</code></a> docs(security): use GitHub security advisories</li>
<li><a href="https://github.com/json5/json5/commit/f0fd9e194dde282caff114a110f4fac635f3a62c"><code>f0fd9e1</code></a> docs: publish a security policy</li>
<li><a href="https://github.com/json5/json5/commit/6a91a05fffeda16ff6b3b5008b6b340d42d31ec0"><code>6a91a05</code></a> docs(template): bug -&gt; bug report</li>
<li><a href="https://github.com/json5/json5/commit/14f8cb186e8abdfaccf6527171da7b1224374650"><code>14f8cb1</code></a> 2.2.2</li>
<li><a href="https://github.com/json5/json5/commit/10cc7ca9169b59c5e0f5afc03dbd870cd06bcc46"><code>10cc7ca</code></a> docs: update CHANGELOG for v2.2.2</li>
<li><a href="https://github.com/json5/json5/commit/7774c1097993bc3ce9f0ac4b722a32bf7d6871c8"><code>7774c10</code></a> fix: add <strong>proto</strong> to objects and arrays</li>
<li><a href="https://github.com/json5/json5/commit/edde30abd8b22facf2c06c72586b9f6edf12700d"><code>edde30a</code></a> Readme: slight tweak to intro</li>
<li><a href="https://github.com/json5/json5/commit/97286f8bd542c89dcee096bc05dd28ed2dfc1e16"><code>97286f8</code></a> Improve example in readme</li>
<li>Additional commits viewable in <a href="https://github.com/json5/json5/compare/v2.2.1...v2.2.3">compare view</a></li>
</ul>
</details>
<br />

Updates `tsconfig-paths` from 3.12.0 to 4.1.2
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/dividab/tsconfig-paths/blob/master/CHANGELOG.md">tsconfig-paths's changelog</a>.</em></p>
<blockquote>
<h2>[4.1.2] - 2023-01-02</h2>
<h3>Fixed</h3>
<ul>
<li>Bump JSON5 dependency to 2.2.2 to fix CVE-2022-46175. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/232">#232</a>. Thanks to <a href="https://github.com/oparisblue"><code>@​oparisblue</code></a> for this PR!</li>
</ul>
<h2>[4.1.1] - 2022-11-30</h2>
<h3>Fixed</h3>
<ul>
<li>Skip stat call / throwing an exception when source files don't exist. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/225">#225</a>. Thanks to <a href="https://github.com/robstolarz"><code>@​robstolarz</code></a> for this PR!</li>
</ul>
<h2>[4.1.0] - 2022-08-06</h2>
<ul>
<li>Add support for nested main field selectors #. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/218">#218</a>. Thanks to <a href="https://github.com/aaronadamsCA"><code>@​aaronadamsCA</code></a> for this PR!</li>
</ul>
<h2>[4.0.0] - 2022-05-02</h2>
<h3>Changed</h3>
<ul>
<li>Ignore <code>--project</code>/<code>-P</code> CLI flag when explicit options are passed to <code>register</code>. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/206">#206</a>.</li>
<li>Tolerate an undefined <code>baseUrl</code> compiler option. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/208">#208</a>.</li>
</ul>
<h3>Added</h3>
<ul>
<li>Add <code>cwd</code> option to <code>register</code> function that overrides where the <code>tsconfig.json</code> search begins. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/205">#205</a>.</li>
<li>Add support for <code>jsconfig.json</code>. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/199">#199</a>. Thanks to <a href="https://github.com/F3n67u"><code>@​F3n67u</code></a> for this PR!</li>
<li>Let <code>paths</code> mappings be absolute paths. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/184">#184</a>.</li>
<li>Allow <code>baseUrl</code> in <code>tsconfig.json</code> to be an absolute path. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/174">#174</a>. Thanks to <a href="https://github.com/nwalters512"><code>@​nwalters512</code></a> for this PR!</li>
</ul>
<h2>[3.14.1] - 2022-03-22</h2>
<h3>Fixed</h3>
<ul>
<li>Use minimist 1.2.6 for all depencencies becuase of pollution vulnerability. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/197">#197</a>. Thanks to <a href="https://github.com/gopijaganthan"><code>@​gopijaganthan</code></a> for this fix!</li>
</ul>
<h2>[3.14.0] - 2022-03-13</h2>
<h3>Added</h3>
<ul>
<li>Support for path mapping starting with <code>/</code>. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/180">#180</a>, issue <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/113">#113</a>, and issue <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/128">#128</a>. Thanks to <a href="https://github.com/benevbright"><code>@​benevbright</code></a> for this fix!</li>
</ul>
<h2>[3.13.0] - 2022-03-03</h2>
<h3>Added</h3>
<ul>
<li>Include file extension in paths resolved from package.json &quot;main&quot; field. See PR <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/pull/135">#135</a> and issue <a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/133">#133</a>. Thanks to <a href="https://github.com/katywings"><code>@​katywings</code></a> for this fix!</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/76dab7661d3cc158c751eba64b363b1d5e032e0f"><code>76dab76</code></a> v4.1.2</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/4a5bfeed6a3bc4a0f34ae4a16ad376529e03a6a0"><code>4a5bfee</code></a> Update changelog for 4.1.2</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/9721a98718c9f6a35bb4029292204aaa90474bab"><code>9721a98</code></a> Bump JSON5 dependency to 2.2.2 to fix CVE-2022-46175 (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/232">#232</a>)</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/1b71683fa7d48a2e7b9cbae4825410594a1c7c81"><code>1b71683</code></a> v4.1.1</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/73fdd5991d6542df4da0a6d22dbb18f5656b091d"><code>73fdd59</code></a> Update changelog for 4.1.1</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/b732fcf0b894a65af5e997b284c40fc3e155837d"><code>b732fcf</code></a> Skip stat call / throwing when files don't exist (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/225">#225</a>)</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/206e49a4dd016e9f7086c8a938266f74f9301568"><code>206e49a</code></a> v4.1.0</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/e71c964000808500a34d7ac4ced6c8b7e98b99b3"><code>e71c964</code></a> Update changelog for 4.1.0</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/9124aa60f18efb52562431d0ec8dd03b4b36ba6a"><code>9124aa6</code></a> Add support for nested main field selectors (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/218">#218</a>)</li>
<li><a href="https://github.com/dividab/tsconfig-paths/commit/f42003925f4d56458d41daed80013c8ad23c88ea"><code>f420039</code></a> Explicitly specify minimum Node.js version (<a href="https://github-redirect.dependabot.com/dividab/tsconfig-paths/issues/212">#212</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/dividab/tsconfig-paths/compare/v3.12.0...v4.1.2">compare view</a></li>
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
        Created At 2023-01-02 05:25:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/104" class=".btn">#104</a>
            </td>
            <td>
                <b>
                    Support passing an ABI directly in any mint/burn/transfer/approval call
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In a chain with #103.
Part of [FIR-16](https://github.com/hyperledger/firefly-fir/pull/16).

**Background**
Currently this connector supports a small set of ABIs, which are checked in to `src/abi`. There are 2 flavors of ERC20 (ERC20NoData and ERC20WithData) and 2 of ERC721 (ERC721NoData and ERC721WithData). When a new pool is created, the connector probes the contract (via ERC165 "supportsInterface") to determine if it is the "WithData" variant. If not, it assumes it is the "NoData" variant. From that point forward, whenever a mint/burn/transfer/approval call is needed, the connector refers to the ABI that it inferred for the contract, in order to determine what method to call.

This works for many cases, but does not cover all common variants of these contracts. However, expanding beyond 2 flavors of each within the current system (ie continuing to rely on probing the contract and making educated guesses about its methods) could quickly become complex and fragile.

**New Enhancements**
With this PR, the mint/burn/transfer/approval APIs all accept a new `interface: { abi: [ ... ] }` parameter. If this is populated with a list of ABI methods, the connector will look at this list _instead_ of any ABI it has previously inferred, to see if the list contains a method it knows how to use.

In addition, the connector now understands some additional flavors of mint/burn methods that are generated by OpenZeppelin (and which differ slightly from any variant in the 4 ABIs checked in to this connector). This means that a contract using these other flavors of mint/burn can now be utilized by the connector, as long as the ABI (or relevant portion of it) is passed in on the mint/burn HTTP request. This is demonstrated and verified in a few new Jest E2E tests.

**Breaking Changes**
The `info.uri` field will no longer be populated when creating a non-fungible pool against a pre-deployed ERC721 that has a base token URI configured. Justification for this:
* It relied on a `baseTokenUri()` method that is not part of the ERC721 standard (unlike other queryable methods like `name` and `symbol`, which are defined in the standard)
* It was inconsistent in that `info.uri` would be populated for pre-deployed ERC721 contracts, but _not_ for ERC721 contracts deployed asynchronously by a factory
* The field is not used by FireFly, and as far as I'm aware, is not widely used in application development (if at all)
* The `baseTokenUri()` method is left in place on the sample ERC721 contract, so it still can be queried directly if needed, even though the connector will no longer query it

**Future Plans**
Currently the changes in this PR won't be exercised in actual FireFly deployments, because FireFly does not pass an ABI to mint/burn/transfer/approval calls. A follow-on step will be to add the ability in FireFly to tie a contract interface to a token pool at creation time, and then cause it to pass the ABI (or a subset) to mint/burn/transfer/approval calls within that pool.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-28 17:50:53 +0000 UTC
    </div>
</div>

