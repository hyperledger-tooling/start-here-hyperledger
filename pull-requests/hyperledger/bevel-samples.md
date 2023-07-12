---
layout: default
title: bevel-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/bevel-samples
---

# bevel-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/bevel-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/36" class=".btn">#36</a>
            </td>
            <td>
                <b>
                    Bump semver from 5.6.0 to 5.7.2 in /examples/supplychain-app/fabric/chaincode_rest_server/rest-server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [semver](https://github.com/npm/node-semver) from 5.6.0 to 5.7.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/npm/node-semver/releases">semver's releases</a>.</em></p>
<blockquote>
<h2>v5.7.2</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v5.7.1...v5.7.2">5.7.2</a> (2023-07-10)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/2f8fd41487acf380194579ecb6f8b1bbfe116be0"><code>2f8fd41</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/585">#585</a> better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/585">#585</a>) (<a href="https://github.com/joaomoreno"><code>@​joaomoreno</code></a>, <a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/npm/node-semver/blob/v5.7.2/CHANGELOG.md">semver's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/npm/node-semver/compare/v5.7.1...v5.7.2">5.7.2</a> (2023-07-10)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/2f8fd41487acf380194579ecb6f8b1bbfe116be0"><code>2f8fd41</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/585">#585</a> better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/585">#585</a>) (<a href="https://github.com/joaomoreno"><code>@​joaomoreno</code></a>, <a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2>5.7</h2>
<ul>
<li>Add <code>minVersion</code> method</li>
</ul>
<h2>5.6</h2>
<ul>
<li>Move boolean <code>loose</code> param to an options object, with
backwards-compatibility protection.</li>
<li>Add ability to opt out of special prerelease version handling with
the <code>includePrerelease</code> option flag.</li>
</ul>
<h2>5.5</h2>
<ul>
<li>Add version coercion capabilities</li>
</ul>
<h2>5.4</h2>
<ul>
<li>Add intersection checking</li>
</ul>
<h2>5.3</h2>
<ul>
<li>Add <code>minSatisfying</code> method</li>
</ul>
<h2>5.2</h2>
<ul>
<li>Add <code>prerelease(v)</code> that returns prerelease components</li>
</ul>
<h2>5.1</h2>
<ul>
<li>Add Backus-Naur for ranges</li>
<li>Remove excessively cute inspection methods</li>
</ul>
<h2>5.0</h2>
<ul>
<li>Remove AMD/Browserified build artifacts</li>
<li>Fix ltr and gtr when using the <code>*</code> range</li>
<li>Fix for range <code>*</code> with a prerelease identifier</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/f8cc313550691a50d9662d8c94f0c033717efd7d"><code>f8cc313</code></a> chore: release 5.7.2</li>
<li><a href="https://github.com/npm/node-semver/commit/2f8fd41487acf380194579ecb6f8b1bbfe116be0"><code>2f8fd41</code></a> fix: better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/585">#585</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/deb5ad51bf58868fa243c1683775305fe9e0e365"><code>deb5ad5</code></a> chore: <code>@​npmcli/template-oss</code><a href="https://github.com/4"><code>@​4</code></a>.16.0</li>
<li><a href="https://github.com/npm/node-semver/commit/c83c18cf84f9ccaea3431c929bb285fd168c01e4"><code>c83c18c</code></a> 5.7.1</li>
<li><a href="https://github.com/npm/node-semver/commit/956e228a4eb1b0136d1fe42c6171d3eda827baef"><code>956e228</code></a> Correct typo in README</li>
<li><a href="https://github.com/npm/node-semver/commit/8055dda0aee91372e3bfc47754a62f40e8a63b98"><code>8055dda</code></a> 5.7.0</li>
<li><a href="https://github.com/npm/node-semver/commit/604e73dea1f19a05314d6c66e0a52b47b1b7b340"><code>604e73d</code></a> auto-publishing scripts</li>
<li><a href="https://github.com/npm/node-semver/commit/bed01e2316b85271f6ffff89bf19e22f41475c97"><code>bed01e2</code></a> remove the nomin comments, since we don't minify any more anyway</li>
<li><a href="https://github.com/npm/node-semver/commit/9cb68f1db72d297183233f4d8d287e935f2b6ddd"><code>9cb68f1</code></a> document parse method</li>
<li><a href="https://github.com/npm/node-semver/commit/38d42ca87a9d891fba9b2a044f914f1919fd769c"><code>38d42ca</code></a> 5.7 changelog</li>
<li>Additional commits viewable in <a href="https://github.com/npm/node-semver/compare/v5.6.0...v5.7.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~lukekarrys">lukekarrys</a>, a new releaser for semver since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=semver&package-manager=npm_and_yarn&previous-version=5.6.0&new-version=5.7.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-11 22:40:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/35" class=".btn">#35</a>
            </td>
            <td>
                <b>
                    Bump tough-cookie and web3 in /examples/supplychain-app/quorum/smartContracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Removes [tough-cookie](https://github.com/salesforce/tough-cookie). It's no longer used after updating ancestor dependency [web3](https://github.com/ChainSafe/web3.js). These dependencies need to be updated together.

Removes `tough-cookie`

Updates `web3` from 1.8.0 to 4.0.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ChainSafe/web3.js/releases">web3's releases</a>.</em></p>
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
<p><em>Sourced from <a href="https://github.com/web3/web3.js/blob/4.x/CHANGELOG.md">web3's changelog</a>.</em></p>
<blockquote>
<h2>[4.0.2]</h2>
<h3>Fixed</h3>
<h4>web3</h4>
<ul>
<li>Fixed bug <a href="https://redirect.github.com/ChainSafe/web3.js/issues/6185">#6185</a>, now web3.js compiles on typescript v5 (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6195">#6195</a>)</li>
<li>Fixed <a href="https://redirect.github.com/ChainSafe/web3.js/issues/6162">#6162</a> <code>@​types/ws</code> issue (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6205">#6205</a>)</li>
</ul>
<h4>web3-core</h4>
<ul>
<li>Fixed Batch requests erroring out on one request (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6164">#6164</a>)</li>
<li>Fixed the issue: Subscribing to multiple blockchain events causes every listener to be fired for every registered event (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6210">#6210</a>)</li>
<li>Fixed the issue: Unsubscribe at a Web3Subscription class will still have the id of the subscription at the Web3SubscriptionManager (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6210">#6210</a>)</li>
<li>Fixed the issue: A call to the provider is made for every subscription object (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6210">#6210</a>)</li>
</ul>
<h4>web3-eth-abi</h4>
<ul>
<li>Support for &quot;decoding&quot; indexed string event arguments (returns the keccak256 hash of the string value instead of the actual string value) (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6167">#6167</a>)</li>
</ul>
<h4>web3-eth-accounts</h4>
<ul>
<li>Fixed &quot;The <code>r</code> and <code>s</code> returned by <code>signTransaction</code> to does not always consist of 64 characters <a href="https://redirect.github.com/ChainSafe/web3.js/issues/6207">#6207</a>&quot; (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6216">#6216</a>)</li>
</ul>
<h4>web3-eth-contract</h4>
<ul>
<li>Event filtering using non-indexed and indexed string event arguments (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6167">#6167</a>)</li>
</ul>
<h4>web3-eth-ens</h4>
<ul>
<li>Fixed bug <a href="https://redirect.github.com/ChainSafe/web3.js/issues/6185">#6185</a>, now web3.js compiles on typescript v5 (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6195">#6195</a>)</li>
</ul>
<h4>web3-providers-ws</h4>
<ul>
<li>Fixed <a href="https://redirect.github.com/ChainSafe/web3.js/issues/6162">#6162</a> <code>@​types/ws</code> issue (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6205">#6205</a>)</li>
</ul>
<h4>web3-types</h4>
<ul>
<li>Fixed bug <a href="https://redirect.github.com/ChainSafe/web3.js/issues/6185">#6185</a>, now web3.js compiles on typescript v5 (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6195">#6195</a>)</li>
</ul>
<h3>Added</h3>
<h4>web3</h4>
<ul>
<li>Exported <code>Web3Context</code>, <code>Web3PluginBase</code>, <code>Web3EthPluginBase</code> from <code>'web3-core'</code>, and <code>Web3Validator</code> from <code>'web3-validator'</code> (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6165">#6165</a>)</li>
</ul>
<h4>web3-core</h4>
<ul>
<li>Web3Subscription constructor accept a Subscription Manager (as an alternative to accepting Request Manager that is now marked marked as deprecated) (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6210">#6210</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/web3/web3.js/commit/47583e7c1500ab087f922370293aa25dbce0d5af"><code>47583e7</code></a> version bumps</li>
<li><a href="https://github.com/web3/web3.js/commit/48bb05f7e98115359d164c652b40bbc9c787b264"><code>48bb05f</code></a> changelog updates</li>
<li><a href="https://github.com/web3/web3.js/commit/3f49e18d24af3dffe2ed47bf65dcf97c0204fc87"><code>3f49e18</code></a> Ensure <code>r</code> and <code>s</code> returned by <code>signTransaction</code> to have 64 character (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6216">#6216</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/e8d579ce6b82a3ae4184d925d1b9cfd87629717d"><code>e8d579c</code></a> Refactor subscription's logic (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6210">#6210</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/51a59f952f1d535be864b0c85966ecc571b451b3"><code>51a59f9</code></a> Few touches on the Plugin Guid (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6182">#6182</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/a2a232fe306636da05868039a934ee491e957d8a"><code>a2a232f</code></a> Add <code>.on('error')</code> test for reverted contract methods (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6194">#6194</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/023f02d890a623ba800c3033074d553fe5346971"><code>023f02d</code></a> fix: add 'receive' to FragmentTypes (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6204">#6204</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/ab0f4cb5fe08512282ae3434906fc9e9327d1786"><code>ab0f4cb</code></a> added ws types in dep (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6205">#6205</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/2130d229b13f9ff138304a9cea9ea3051fab2a76"><code>2130d22</code></a> TS v5 support (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6195">#6195</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/f8a2533c2b09ce0a62f8414f2f6eed83ab78ca1f"><code>f8a2533</code></a> 6164 batch request fix (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6166">#6166</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/ChainSafe/web3.js/compare/v1.8.0...v4.0.2">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-09 04:34:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/34" class=".btn">#34</a>
            </td>
            <td>
                <b>
                    Bump tough-cookie and web3 in /examples/supplychain-app/besu/express_nodeJS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Removes [tough-cookie](https://github.com/salesforce/tough-cookie). It's no longer used after updating ancestor dependency [web3](https://github.com/ChainSafe/web3.js). These dependencies need to be updated together.

Removes `tough-cookie`

Updates `web3` from 1.8.0 to 4.0.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ChainSafe/web3.js/releases">web3's releases</a>.</em></p>
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
<p><em>Sourced from <a href="https://github.com/web3/web3.js/blob/4.x/CHANGELOG.md">web3's changelog</a>.</em></p>
<blockquote>
<h2>[4.0.2]</h2>
<h3>Fixed</h3>
<h4>web3</h4>
<ul>
<li>Fixed bug <a href="https://redirect.github.com/ChainSafe/web3.js/issues/6185">#6185</a>, now web3.js compiles on typescript v5 (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6195">#6195</a>)</li>
<li>Fixed <a href="https://redirect.github.com/ChainSafe/web3.js/issues/6162">#6162</a> <code>@​types/ws</code> issue (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6205">#6205</a>)</li>
</ul>
<h4>web3-core</h4>
<ul>
<li>Fixed Batch requests erroring out on one request (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6164">#6164</a>)</li>
<li>Fixed the issue: Subscribing to multiple blockchain events causes every listener to be fired for every registered event (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6210">#6210</a>)</li>
<li>Fixed the issue: Unsubscribe at a Web3Subscription class will still have the id of the subscription at the Web3SubscriptionManager (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6210">#6210</a>)</li>
<li>Fixed the issue: A call to the provider is made for every subscription object (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6210">#6210</a>)</li>
</ul>
<h4>web3-eth-abi</h4>
<ul>
<li>Support for &quot;decoding&quot; indexed string event arguments (returns the keccak256 hash of the string value instead of the actual string value) (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6167">#6167</a>)</li>
</ul>
<h4>web3-eth-accounts</h4>
<ul>
<li>Fixed &quot;The <code>r</code> and <code>s</code> returned by <code>signTransaction</code> to does not always consist of 64 characters <a href="https://redirect.github.com/ChainSafe/web3.js/issues/6207">#6207</a>&quot; (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6216">#6216</a>)</li>
</ul>
<h4>web3-eth-contract</h4>
<ul>
<li>Event filtering using non-indexed and indexed string event arguments (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6167">#6167</a>)</li>
</ul>
<h4>web3-eth-ens</h4>
<ul>
<li>Fixed bug <a href="https://redirect.github.com/ChainSafe/web3.js/issues/6185">#6185</a>, now web3.js compiles on typescript v5 (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6195">#6195</a>)</li>
</ul>
<h4>web3-providers-ws</h4>
<ul>
<li>Fixed <a href="https://redirect.github.com/ChainSafe/web3.js/issues/6162">#6162</a> <code>@​types/ws</code> issue (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6205">#6205</a>)</li>
</ul>
<h4>web3-types</h4>
<ul>
<li>Fixed bug <a href="https://redirect.github.com/ChainSafe/web3.js/issues/6185">#6185</a>, now web3.js compiles on typescript v5 (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6195">#6195</a>)</li>
</ul>
<h3>Added</h3>
<h4>web3</h4>
<ul>
<li>Exported <code>Web3Context</code>, <code>Web3PluginBase</code>, <code>Web3EthPluginBase</code> from <code>'web3-core'</code>, and <code>Web3Validator</code> from <code>'web3-validator'</code> (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6165">#6165</a>)</li>
</ul>
<h4>web3-core</h4>
<ul>
<li>Web3Subscription constructor accept a Subscription Manager (as an alternative to accepting Request Manager that is now marked marked as deprecated) (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6210">#6210</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/web3/web3.js/commit/47583e7c1500ab087f922370293aa25dbce0d5af"><code>47583e7</code></a> version bumps</li>
<li><a href="https://github.com/web3/web3.js/commit/48bb05f7e98115359d164c652b40bbc9c787b264"><code>48bb05f</code></a> changelog updates</li>
<li><a href="https://github.com/web3/web3.js/commit/3f49e18d24af3dffe2ed47bf65dcf97c0204fc87"><code>3f49e18</code></a> Ensure <code>r</code> and <code>s</code> returned by <code>signTransaction</code> to have 64 character (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6216">#6216</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/e8d579ce6b82a3ae4184d925d1b9cfd87629717d"><code>e8d579c</code></a> Refactor subscription's logic (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6210">#6210</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/51a59f952f1d535be864b0c85966ecc571b451b3"><code>51a59f9</code></a> Few touches on the Plugin Guid (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6182">#6182</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/a2a232fe306636da05868039a934ee491e957d8a"><code>a2a232f</code></a> Add <code>.on('error')</code> test for reverted contract methods (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6194">#6194</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/023f02d890a623ba800c3033074d553fe5346971"><code>023f02d</code></a> fix: add 'receive' to FragmentTypes (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6204">#6204</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/ab0f4cb5fe08512282ae3434906fc9e9327d1786"><code>ab0f4cb</code></a> added ws types in dep (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6205">#6205</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/2130d229b13f9ff138304a9cea9ea3051fab2a76"><code>2130d22</code></a> TS v5 support (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6195">#6195</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/f8a2533c2b09ce0a62f8414f2f6eed83ab78ca1f"><code>f8a2533</code></a> 6164 batch request fix (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6166">#6166</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/ChainSafe/web3.js/compare/v1.8.0...v4.0.2">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-09 04:34:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/33" class=".btn">#33</a>
            </td>
            <td>
                <b>
                    Bump tough-cookie and web3 in /examples/supplychain-app/quorum/express_nodeJS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Removes [tough-cookie](https://github.com/salesforce/tough-cookie). It's no longer used after updating ancestor dependency [web3](https://github.com/ChainSafe/web3.js). These dependencies need to be updated together.

Removes `tough-cookie`

Updates `web3` from 1.8.0 to 4.0.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ChainSafe/web3.js/releases">web3's releases</a>.</em></p>
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
<p><em>Sourced from <a href="https://github.com/web3/web3.js/blob/4.x/CHANGELOG.md">web3's changelog</a>.</em></p>
<blockquote>
<h2>[4.0.2]</h2>
<h3>Fixed</h3>
<h4>web3</h4>
<ul>
<li>Fixed bug <a href="https://redirect.github.com/ChainSafe/web3.js/issues/6185">#6185</a>, now web3.js compiles on typescript v5 (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6195">#6195</a>)</li>
<li>Fixed <a href="https://redirect.github.com/ChainSafe/web3.js/issues/6162">#6162</a> <code>@​types/ws</code> issue (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6205">#6205</a>)</li>
</ul>
<h4>web3-core</h4>
<ul>
<li>Fixed Batch requests erroring out on one request (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6164">#6164</a>)</li>
<li>Fixed the issue: Subscribing to multiple blockchain events causes every listener to be fired for every registered event (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6210">#6210</a>)</li>
<li>Fixed the issue: Unsubscribe at a Web3Subscription class will still have the id of the subscription at the Web3SubscriptionManager (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6210">#6210</a>)</li>
<li>Fixed the issue: A call to the provider is made for every subscription object (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6210">#6210</a>)</li>
</ul>
<h4>web3-eth-abi</h4>
<ul>
<li>Support for &quot;decoding&quot; indexed string event arguments (returns the keccak256 hash of the string value instead of the actual string value) (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6167">#6167</a>)</li>
</ul>
<h4>web3-eth-accounts</h4>
<ul>
<li>Fixed &quot;The <code>r</code> and <code>s</code> returned by <code>signTransaction</code> to does not always consist of 64 characters <a href="https://redirect.github.com/ChainSafe/web3.js/issues/6207">#6207</a>&quot; (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6216">#6216</a>)</li>
</ul>
<h4>web3-eth-contract</h4>
<ul>
<li>Event filtering using non-indexed and indexed string event arguments (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6167">#6167</a>)</li>
</ul>
<h4>web3-eth-ens</h4>
<ul>
<li>Fixed bug <a href="https://redirect.github.com/ChainSafe/web3.js/issues/6185">#6185</a>, now web3.js compiles on typescript v5 (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6195">#6195</a>)</li>
</ul>
<h4>web3-providers-ws</h4>
<ul>
<li>Fixed <a href="https://redirect.github.com/ChainSafe/web3.js/issues/6162">#6162</a> <code>@​types/ws</code> issue (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6205">#6205</a>)</li>
</ul>
<h4>web3-types</h4>
<ul>
<li>Fixed bug <a href="https://redirect.github.com/ChainSafe/web3.js/issues/6185">#6185</a>, now web3.js compiles on typescript v5 (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6195">#6195</a>)</li>
</ul>
<h3>Added</h3>
<h4>web3</h4>
<ul>
<li>Exported <code>Web3Context</code>, <code>Web3PluginBase</code>, <code>Web3EthPluginBase</code> from <code>'web3-core'</code>, and <code>Web3Validator</code> from <code>'web3-validator'</code> (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6165">#6165</a>)</li>
</ul>
<h4>web3-core</h4>
<ul>
<li>Web3Subscription constructor accept a Subscription Manager (as an alternative to accepting Request Manager that is now marked marked as deprecated) (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6210">#6210</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/web3/web3.js/commit/47583e7c1500ab087f922370293aa25dbce0d5af"><code>47583e7</code></a> version bumps</li>
<li><a href="https://github.com/web3/web3.js/commit/48bb05f7e98115359d164c652b40bbc9c787b264"><code>48bb05f</code></a> changelog updates</li>
<li><a href="https://github.com/web3/web3.js/commit/3f49e18d24af3dffe2ed47bf65dcf97c0204fc87"><code>3f49e18</code></a> Ensure <code>r</code> and <code>s</code> returned by <code>signTransaction</code> to have 64 character (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6216">#6216</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/e8d579ce6b82a3ae4184d925d1b9cfd87629717d"><code>e8d579c</code></a> Refactor subscription's logic (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6210">#6210</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/51a59f952f1d535be864b0c85966ecc571b451b3"><code>51a59f9</code></a> Few touches on the Plugin Guid (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6182">#6182</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/a2a232fe306636da05868039a934ee491e957d8a"><code>a2a232f</code></a> Add <code>.on('error')</code> test for reverted contract methods (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6194">#6194</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/023f02d890a623ba800c3033074d553fe5346971"><code>023f02d</code></a> fix: add 'receive' to FragmentTypes (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6204">#6204</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/ab0f4cb5fe08512282ae3434906fc9e9327d1786"><code>ab0f4cb</code></a> added ws types in dep (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6205">#6205</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/2130d229b13f9ff138304a9cea9ea3051fab2a76"><code>2130d22</code></a> TS v5 support (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6195">#6195</a>)</li>
<li><a href="https://github.com/web3/web3.js/commit/f8a2533c2b09ce0a62f8414f2f6eed83ab78ca1f"><code>f8a2533</code></a> 6164 batch request fix (<a href="https://redirect.github.com/ChainSafe/web3.js/issues/6166">#6166</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/ChainSafe/web3.js/compare/v1.8.0...v4.0.2">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-09 04:34:24 +0000 UTC
    </div>
</div>

