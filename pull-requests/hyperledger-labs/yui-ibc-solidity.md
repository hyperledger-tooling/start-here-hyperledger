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
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/276" class=".btn">#276</a>
            </td>
            <td>
                <b>
                    Bump node to v20
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
        Created At 2024-05-16 10:33:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/275" class=".btn">#275</a>
            </td>
            <td>
                <b>
                    Bump github.com/cosmos/ibc-go/v7 from 7.3.0 to 7.4.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/cosmos/ibc-go/v7](https://github.com/cosmos/ibc-go) from 7.3.0 to 7.4.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/cosmos/ibc-go/releases">github.com/cosmos/ibc-go/v7's releases</a>.</em></p>
<blockquote>
<h2>v7.4.0</h2>
<p>This release includes a fix for the <a href="https://github.com/cosmos/ibc-go/security/advisories/GHSA-j496-crgh-34mx">ASA-2024-007 security advisory</a>. Credits to Maxwell Dulin (<a href="https://github.com/mdulin2"><code>@​mdulin2</code></a>) at <a href="https://www.asymmetric.re/">Asymmetric Research</a> for the discovery and disclosure via our <a href="https://hackerone.com/cosmos">bug bounty program</a>.</p>
<p>Please note that this release, as indicated in our <a href="https://github.com/cosmos/ibc-go/blob/main/RELEASES.md">release versioning policy</a>, is state machine breaking and requires a coordinated upgrade.</p>
<p>Please see the <a href="https://github.com/cosmos/ibc-go/blob/v7.4.0/CHANGELOG.md">v7.4.0 changelog</a> for the full set of changes included in this release.</p>
<hr />
<p>To learn more about ibc-go versioning, please read our <a href="https://github.com/cosmos/ibc-go/blob/main/RELEASES.md">RELEASES.md</a>.</p>
<p>IMPORTANT: Please read the migration guides for any versions of ibc-go that you might be going through when upgrading to this version. For example: if you upgrade from the IBC module contained in the Cosmos SDK 0.42.0 to SDK v0.47.8 and ibc-go v7.4.0, please follow:</p>
<ol>
<li>The <a href="https://github.com/cosmos/ibc-go/blob/v7.4.0/docs/migrations/sdk-to-v1.md">migration from SDK 0.41.x or 0.42.x to the IBC module in the ibc-go repository based on the SDK v0.44.x</a>.</li>
<li>The <a href="https://github.com/cosmos/ibc-go/blob/v7.4.0/docs/migrations/v1-to-v2.md">migration from ibc-go v1 to v2</a>.</li>
<li>The <a href="https://github.com/cosmos/ibc-go/blob/v7.4.0/docs/migrations/v2-to-v3.md">migration from ibc-go v2 to v3</a>.</li>
<li>The <a href="https://github.com/cosmos/ibc-go/blob/v7.4.0/docs/migrations/v3-to-v4.md">migration from ibc-go v3 to v4</a>.</li>
<li>The <a href="https://github.com/cosmos/ibc-go/blob/v7.4.0/docs/migrations/v4-to-v5.md">migration from ibc-go v4 to v5</a>.</li>
<li>The <a href="https://github.com/cosmos/ibc-go/blob/v7.4.0/docs/migrations/v5-to-v6.md">migration from ibc-go v5 to v6</a>.</li>
<li>The <a href="https://github.com/cosmos/ibc-go/blob/v7.4.0/docs/migrations/v6-to-v7.md">migration from ibc-go v6 to v7</a>.</li>
</ol>
<h2>v7.3.2</h2>
<h3>UPDATES</h3>
<ul>
<li>5th April 2024: This release is NOT recommended since it is impacted by the <a href="https://github.com/cosmos/ibc-go/security/advisories/GHSA-j496-crgh-34mx">ASA-2024-007 security advisory</a>. <strong>Please use version &gt;= 7.4.0</strong>.</li>
</ul>
<hr />
<p>We present here a summary of the most relevant changes, please see the <a href="https://github.com/cosmos/ibc-go/blob/v7.3.2/CHANGELOG.md">v7.3.2 changelog</a> for the full set of changes included in this release.</p>
<h3>dependencies</h3>
<ul>
<li>Cosmos SDK has been bumped to <a href="https://github.com/cosmos/cosmos-sdk/releases/tag/v0.47.8">v0.47.8</a>.</li>
<li>CometBFT has been bumped to <a href="https://github.com/cometbft/cometbft/releases/tag/v0.37.4">v0.37.4</a>.</li>
</ul>
<h3>core</h3>
<ul>
<li>The emission of events on erroneous IBC application callbacks was removed due to the <a href="https://github.com/cosmos/ibc-go/security/advisories/GHSA-3v7p-4x7p-4rx7">huckleberry security advisory</a>. Since then, many users have been unable to debug their IBC applications effectively causing a considerable uptick in support requests across many chains. In this release we are introducing re-enabling emission of events on erroneous IBC application callbacks by appending the prefix <code>ibccallbackerror-</code> to all event type and attribute keys.</li>
</ul>
<p>Special thanks to our external contributors in this release: <a href="https://github.com/emidev98"><code>@​emidev98</code></a></p>
<hr />
<p>To learn more about ibc-go versioning, please read our <a href="https://github.com/cosmos/ibc-go/blob/main/RELEASES.md">RELEASES.md</a>.</p>
<p>IMPORTANT: Please read the migration guides for any versions of ibc-go that you might be going through when upgrading to this version. For example: if you upgrade from the IBC module contained in the Cosmos SDK 0.42.0 to SDK v0.47.8 and ibc-go v7.3.2, please follow:</p>
<ol>
<li>The <a href="https://github.com/cosmos/ibc-go/blob/v7.3.2/docs/migrations/sdk-to-v1.md">migration from SDK 0.41.x or 0.42.x to the IBC module in the ibc-go repository based on the SDK v0.44.x</a>.</li>
<li>The <a href="https://github.com/cosmos/ibc-go/blob/v7.3.2/docs/migrations/v1-to-v2.md">migration from ibc-go v1 to v2</a>.</li>
<li>The <a href="https://github.com/cosmos/ibc-go/blob/v7.3.2/docs/migrations/v2-to-v3.md">migration from ibc-go v2 to v3</a>.</li>
</ol>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/cosmos/ibc-go/blob/main/CHANGELOG.md">github.com/cosmos/ibc-go/v7's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/cosmos/ibc-go/releases/tag/v7.4.0">v7.4.0</a> - 2024-04-05</h2>
<h2><a href="https://github.com/cosmos/ibc-go/releases/tag/v7.3.2">v7.3.2</a> - 2024-01-31</h2>
<h3>Dependencies</h3>
<ul>
<li><a href="https://redirect.github.com/cosmos/ibc-go/pull/5717">#5717</a> Update Cosmos SDK to v0.47.8 and CometBFT to v0.37.4.</li>
</ul>
<h3>Improvements</h3>
<ul>
<li>(core) <a href="https://redirect.github.com/cosmos/ibc-go/pull/5541">#5541</a> Enable emission of events on erroneous IBC application callbacks by appending a prefix to all event type and attribute keys.</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>(apps/27-interchain-accounts) <a href="https://redirect.github.com/cosmos/ibc-go/pull/4944">#4944</a> Add missing proto interface registration.</li>
</ul>
<h2><a href="https://github.com/cosmos/ibc-go/releases/tag/v7.3.1">v7.3.1</a> - 2023-10-20</h2>
<h3>Dependencies</h3>
<ul>
<li><a href="https://redirect.github.com/cosmos/ibc-go/pull/4539">#4539</a> Update Cosmos SDK to v0.47.5.</li>
</ul>
<h3>Improvements</h3>
<ul>
<li>(apps/27-interchain-accounts) <a href="https://redirect.github.com/cosmos/ibc-go/pull/4537">#4537</a> Add argument to <code>generate-packet-data</code> cli to choose the encoding format for the messages in the ICA packet data.</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>(apps/transfer) <a href="https://redirect.github.com/cosmos/ibc-go/pull/4709">#4709</a> Order query service RPCs to fix availability of denom traces endpoint when no args are provided.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/cosmos/ibc-go/commit/802ca265dba74a293747e1ccb8b7999aa985af19"><code>802ca26</code></a> Update CHANGELOG.md</li>
<li><a href="https://github.com/cosmos/ibc-go/commit/90c6f370fbdd8cfbbeedbf194906ac649c242fd3"><code>90c6f37</code></a> update changelog before v7.4.0</li>
<li><a href="https://github.com/cosmos/ibc-go/commit/e78b3a2b9c9ce80a67d6b1c2b7f9abcb225cc219"><code>e78b3a2</code></a> Merge pull request from GHSA-j496-crgh-34mx</li>
<li><a href="https://github.com/cosmos/ibc-go/commit/373fc7f54b2eb3965ca199703ef980099d73fba4"><code>373fc7f</code></a> Update CHANGELOG.md</li>
<li><a href="https://github.com/cosmos/ibc-go/commit/747eb6fe37443f93313cbfbb29aebf288ec0228a"><code>747eb6f</code></a> update changelog before v7.3.2 release</li>
<li><a href="https://github.com/cosmos/ibc-go/commit/5a45edaebc35bbed824eecfdd0b6dbabbcf4a48f"><code>5a45eda</code></a> deps(<code>release/v7.3.x</code>): update sdk v0.47.8 (<a href="https://redirect.github.com/cosmos/ibc-go/issues/5717">#5717</a>)</li>
<li><a href="https://github.com/cosmos/ibc-go/commit/825fe90f9765edbaef099282defe083c94b35fa8"><code>825fe90</code></a> imp(core): allow huckleberry events with a prefix (backport <a href="https://redirect.github.com/cosmos/ibc-go/issues/5541">#5541</a>) (<a href="https://redirect.github.com/cosmos/ibc-go/issues/5574">#5574</a>)</li>
<li><a href="https://github.com/cosmos/ibc-go/commit/bef2278049ac46ed97d06c9f94738406355ad739"><code>bef2278</code></a> fix(msg): register proto interface (backport <a href="https://redirect.github.com/cosmos/ibc-go/issues/4944">#4944</a>) (<a href="https://redirect.github.com/cosmos/ibc-go/issues/4953">#4953</a>)</li>
<li><a href="https://github.com/cosmos/ibc-go/commit/d73c6d012a710850fd6c6363cbebd1452a5dea95"><code>d73c6d0</code></a> Update CHANGELOG.md</li>
<li><a href="https://github.com/cosmos/ibc-go/commit/bc741464d48ba636ac4a6f8627e8b3e753fec083"><code>bc74146</code></a> prepare changelog for v7.3.1 release</li>
<li>Additional commits viewable in <a href="https://github.com/cosmos/ibc-go/compare/v7.3.0...v7.4.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/cosmos/ibc-go/v7&package-manager=go_modules&previous-version=7.3.0&new-version=7.4.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-ibc-solidity/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-16 10:03:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/274" class=".btn">#274</a>
            </td>
            <td>
                <b>
                    Bump github.com/dvsekhvalnov/jose2go from 1.5.0 to 1.6.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/dvsekhvalnov/jose2go](https://github.com/dvsekhvalnov/jose2go) from 1.5.0 to 1.6.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dvsekhvalnov/jose2go/commit/48ba0b76bc881767cff2723388f4dd1a47c5104a"><code>48ba0b7</code></a> Merge pull request <a href="https://redirect.github.com/dvsekhvalnov/jose2go/issues/32">#32</a> from dvsekhvalnov/issue-31-security-tuning</li>
<li><a href="https://github.com/dvsekhvalnov/jose2go/commit/05eb00788125e3996824d2005e850ed8b37d5aa4"><code>05eb007</code></a> docs</li>
<li><a href="https://github.com/dvsekhvalnov/jose2go/commit/e0264a274aa4c14e22f197c5325599224c1dd412"><code>e0264a2</code></a> added helper matchers: Alg and Eng</li>
<li><a href="https://github.com/dvsekhvalnov/jose2go/commit/0f6c7c346282f2d264aef1d7dec8be71f9190b08"><code>0f6c7c3</code></a> MatchAlg helper</li>
<li><a href="https://github.com/dvsekhvalnov/jose2go/commit/cf0a53b05fc1faf3e655a30bd7d523cb3a2c6dbd"><code>cf0a53b</code></a> docs</li>
<li><a href="https://github.com/dvsekhvalnov/jose2go/commit/299576231d2311655289f451218678044d6ddbc9"><code>2995762</code></a> docs</li>
<li><a href="https://github.com/dvsekhvalnov/jose2go/commit/9a18aff07b6c5574e02d74439ad7d7ae88510b6f"><code>9a18aff</code></a> docs</li>
<li><a href="https://github.com/dvsekhvalnov/jose2go/commit/675bb14fb3216d48f571b7e5d4274faf4aceb069"><code>675bb14</code></a> docs</li>
<li><a href="https://github.com/dvsekhvalnov/jose2go/commit/8e9e0d1c6b39ac448a6042ed1275efa70a81c7b7"><code>8e9e0d1</code></a> updated p2c limits with new OWASP numbers, docs</li>
<li><a href="https://github.com/dvsekhvalnov/jose2go/commit/ed5dd96763d198ce95dc10b9252cb96854522114"><code>ed5dd96</code></a> Unit tests for custom 'p2c' headers min/max limits</li>
<li>Additional commits viewable in <a href="https://github.com/dvsekhvalnov/jose2go/compare/v1.5...v1.6.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/dvsekhvalnov/jose2go&package-manager=go_modules&previous-version=1.5.0&new-version=1.6.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-ibc-solidity/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-16 10:02:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/273" class=".btn">#273</a>
            </td>
            <td>
                <b>
                    Bump github.com/cosmos/cosmos-sdk from 0.47.4 to 0.50.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/cosmos/cosmos-sdk](https://github.com/cosmos/cosmos-sdk) from 0.47.4 to 0.50.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/cosmos/cosmos-sdk/releases">github.com/cosmos/cosmos-sdk's releases</a>.</em></p>
<blockquote>
<h2>v0.50.5</h2>
<h1>Cosmos SDK v0.50.5 Release Notes</h1>
<p>💬 <a href="https://github.com/orgs/cosmos/discussions/58"><strong>Release Discussion</strong></a></p>
<h2>🚀 Highlights</h2>
<p>This is time for another patch release of Cosmos SDK Eden.
This release includes a few notable fixes:</p>
<ul>
<li>Fix a bypass delegator slashing: <a href="https://github.com/cosmos/cosmos-sdk/security/advisories/GHSA-86h5-xcpx-cfqc">GHSA-86h5-xcpx-cfqc</a></li>
<li>Fix an issue in <code>baseapp.ValidateVoteExtensions</code> helper: <a href="https://github.com/cosmos/cosmos-sdk/security/advisories/GHSA-95rx-m9m5-m94v">GHSA-95rx-m9m5-m94v</a></li>
<li>Allow to provide custom signers for <code>x/auth/tx</code> using depinject</li>
</ul>
<p>We recommended to upgrade to this patch release as soon as possible.<br />
When upgrading from &lt;= v0.50.4, please ensure that 2/3 of the validator power upgrade to v0.50.5.</p>
<h2>📝 Changelog</h2>
<p>Check out the <a href="https://github.com/cosmos/cosmos-sdk/blob/v0.50.5/CHANGELOG.md">changelog</a> for an exhaustive list of changes, or <a href="https://github.com/cosmos/cosmos-sdk/compare/release/v0.50.4...v0.50.5">compare changes</a> from the last release.</p>
<p>Refer to the <a href="https://github.com/cosmos/cosmos-sdk/blob/release/v0.50.x/UPGRADING.md">upgrading guide</a> when migrating from <code>v0.47.x</code> to <code>v0.50.1</code>.
Note, that the next SDK release, v0.51, will not include <code>x/params</code> migration, when migrating from &lt; v0.47, v0.50.x <strong>or</strong> v0.47.x, is a mandatory migration.</p>
<h2>v0.50.4</h2>
<h1>Cosmos SDK v0.50.4 Release Notes</h1>
<p>💬 <a href="https://github.com/orgs/cosmos/discussions/58"><strong>Release Discussion</strong></a></p>
<h2>🚀 Highlights</h2>
<p>Some months ago Cosmos SDK Eden was released. Missed the announcement? Read it <a href="https://github.com/cosmos/cosmos-sdk/releases/tag/v0.50.1">here</a>.
For this month patch release of the v0.50.x line, a few features and improvements were added to the SDK.</p>
<p>Notably, we added and fixed the following:</p>
<ul>
<li>Adds in-place testnet CLI command for creating testnets from local state (kudos to <a href="https://github.com/czarcas7ic"><code>@​czarcas7ic</code></a>)</li>
<li>Multiple fixes in baseapp, with fixes in <code>DefaultProposalHandler</code> and vote extensions</li>
<li>Add a missed check in <code>x/auth/vesting</code>: <a href="https://github.com/cosmos/cosmos-sdk/security/advisories/GHSA-4j93-fm92-rp4m">GHSA-4j93-fm92-rp4m</a></li>
</ul>
<p>We recommended to upgrade to this patch release as soon as possible.<br />
When upgrading from &lt;= v0.50.3, please ensure that 2/3 of the validator power upgrade to v0.50.4.</p>
<h2>📝 Changelog</h2>
<p>Check out the <a href="https://github.com/cosmos/cosmos-sdk/blob/v0.50.4/CHANGELOG.md">changelog</a> for an exhaustive list of changes, or <a href="https://github.com/cosmos/cosmos-sdk/compare/release/v0.50.3...v0.50.4">compare changes</a> from the last release.</p>
<p>Refer to the <a href="https://github.com/cosmos/cosmos-sdk/blob/release/v0.50.x/UPGRADING.md">upgrading guide</a> when migrating from <code>v0.47.x</code> to <code>v0.50.1</code>.
Note, that the next SDK release, v0.51.0, will not include <code>x/params</code> migration, when migrating from &lt; v0.47, v0.50.x <strong>or</strong> v0.47.x, is a mandatory migration.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/cosmos/cosmos-sdk/blob/main/CHANGELOG.md">github.com/cosmos/cosmos-sdk's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/cosmos/cosmos-sdk/releases/tag/v0.50.5">v0.50.5</a> - 2024-03-12</h2>
<h3>Features</h3>
<ul>
<li>(baseapp) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/19626">#19626</a> Add <code>DisableBlockGasMeter</code> option to <code>BaseApp</code>, which removes the block gas meter during transaction execution.</li>
</ul>
<h3>Improvements</h3>
<ul>
<li>(x/distribution) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/19707">#19707</a> Add autocli config for <code>DelegationTotalRewards</code> for CLI consistency with <code>q rewards</code> commands in previous versions.</li>
<li>(x/auth) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/19651">#19651</a> Allow empty public keys in <code>GetSignBytesAdapter</code>.</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>(x/gov) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/19725">#19725</a> Fetch a failed proposal tally from proposal.FinalTallyResult in the gprc query.</li>
<li>(types) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/19709">#19709</a> Fix skip staking genesis export when using <code>CoreAppModuleAdaptor</code> / <code>CoreAppModuleBasicAdaptor</code> for it.</li>
<li>(x/auth) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/19549">#19549</a> Accept custom get signers when injecting <code>x/auth/tx</code>.</li>
<li>(x/staking) Fix a possible bypass of delegator slashing: <a href="https://github.com/cosmos/cosmos-sdk/security/advisories/GHSA-86h5-xcpx-cfqc">GHSA-86h5-xcpx-cfqc</a></li>
<li>(baseapp) Fix a bug in <code>baseapp.ValidateVoteExtensions</code> helper (<a href="https://github.com/cosmos/cosmos-sdk/security/advisories/GHSA-95rx-m9m5-m94v">GHSA-95rx-m9m5-m94v</a>). The helper has been fixed and for avoiding API breaking changes <code>currentHeight</code> and <code>chainID</code> arguments are ignored. Those arguments are removed from the helper in v0.51+.</li>
</ul>
<h2><a href="https://github.com/cosmos/cosmos-sdk/releases/tag/v0.50.4">v0.50.4</a> - 2023-02-19</h2>
<h3>Features</h3>
<ul>
<li>(server) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/19280">#19280</a> Adds in-place testnet CLI command.</li>
</ul>
<h3>Improvements</h3>
<ul>
<li>(client) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/19393/">#19393</a> Add <code>ReadDefaultValuesFromDefaultClientConfig</code> to populate the default values from the default client config in client.Context without creating a app folder.</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>(x/auth/vesting) <a href="https://github.com/cosmos/cosmos-sdk/blob/main/#bug-fixes">GHSA-4j93-fm92-rp4m</a> Add <code>BlockedAddr</code> check in <code>CreatePeriodicVestingAccount</code>.</li>
<li>(baseapp) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/19338">#19338</a> Set HeaderInfo in context when calling <code>setState</code>.</li>
<li>(baseapp): <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/19200">#19200</a> Ensure that sdk side ve math matches cometbft.</li>
<li><a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/19106">#19106</a> Allow empty public keys when setting signatures. Public keys aren't needed for every transaction.</li>
<li>(baseapp) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/19198">#19198</a> Remove usage of pointers in logs in all optimistic execution goroutines.</li>
<li>(baseapp) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/19177">#19177</a> Fix baseapp <code>DefaultProposalHandler</code> same-sender non-sequential sequence.</li>
<li>(crypto) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/19371">#19371</a> Avoid CLI redundant log in stdout, log to stderr instead.</li>
</ul>
<h2><a href="https://github.com/cosmos/cosmos-sdk/releases/tag/v0.50.3">v0.50.3</a> - 2023-01-15</h2>
<h3>Features</h3>
<ul>
<li>(types) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/18991">#18991</a> Add SignerExtractionAdapter to PriorityNonceMempool/Config and provide Default implementation matching existing behavior.</li>
<li>(gRPC) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/19043">#19043</a> Add <code>halt_height</code> to the gRPC <code>/cosmos/base/node/v1beta1/config</code> request.</li>
</ul>
<h3>Improvements</h3>
<ul>
<li>(x/bank) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/18956">#18956</a> Introduced a new <code>DenomOwnersByQuery</code> query method for <code>DenomOwners</code>, which accepts the denom value as a query string parameter, resolving issues with denoms containing slashes.</li>
<li>(x/gov) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/18707">#18707</a> Improve genesis validation.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/cosmos/cosmos-sdk/commit/a32186608aab0bd436049377ddb34f90006fcbf7"><code>a321866</code></a> chore: prepare v0.50.5 (<a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/19715">#19715</a>)</li>
<li><a href="https://github.com/cosmos/cosmos-sdk/commit/a877c47d47e910b55264dbe3ff3b9514c850aff5"><code>a877c47</code></a> fix(x/gov): grpc query tally for failed proposal (backport <a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/19725">#19725</a>) (<a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/19727">#19727</a>)</li>
<li><a href="https://github.com/cosmos/cosmos-sdk/commit/c382225138caa85159183985cc66145a04c914d8"><code>c382225</code></a> feat(x/distribution): add rewards-by-validator autocli config (backport <a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/1970">#1970</a>...</li>
<li><a href="https://github.com/cosmos/cosmos-sdk/commit/f055cde5d10643325f88ddf910f370a47e4bf0a0"><code>f055cde</code></a> feat(baseapp): add option to disable block gas meter (<a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/19626">#19626</a>)</li>
<li><a href="https://github.com/cosmos/cosmos-sdk/commit/4467110df40797ebe916c23ebfd45c9ee7583897"><code>4467110</code></a> Merge pull request from GHSA-95rx-m9m5-m94v</li>
<li><a href="https://github.com/cosmos/cosmos-sdk/commit/6689e3689b16c02f8b3c46efec31f8c7d04aa833"><code>6689e36</code></a> build(deps): Bump deps (backport <a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/19655">#19655</a>) (<a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/19711">#19711</a>)</li>
<li><a href="https://github.com/cosmos/cosmos-sdk/commit/3382e8ea8235eea8b27cc86ebc632b82970c05b6"><code>3382e8e</code></a> fix(types): check for HasABCIGenesis in CoreAppModuleBasicAdaptor (<a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/19709">#19709</a>)</li>
<li><a href="https://github.com/cosmos/cosmos-sdk/commit/f9041cde5c863c4be7d7ec5fc6484ab544f551ba"><code>f9041cd</code></a> refactor(x/auth): allow empty public keys for GetSignBytesAdapter (backport #...</li>
<li><a href="https://github.com/cosmos/cosmos-sdk/commit/2abd2ec8a52fe9eefcf750e8a1b3c35d0c9361c8"><code>2abd2ec</code></a> feat(client/v2): marshal enum as string (<a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/19653">#19653</a>)</li>
<li><a href="https://github.com/cosmos/cosmos-sdk/commit/09a49fe260b6e6f152fa0347cb32a7098c033508"><code>09a49fe</code></a> build(deps): Bump cosmossdk.io/x/tx from 0.13.0 to 0.13.1 (<a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/19665">#19665</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/cosmos/cosmos-sdk/compare/v0.47.4...v0.50.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/cosmos/cosmos-sdk&package-manager=go_modules&previous-version=0.47.4&new-version=0.50.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-ibc-solidity/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-16 10:02:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/272" class=".btn">#272</a>
            </td>
            <td>
                <b>
                    Bump github.com/ethereum/go-ethereum from 1.11.6 to 1.13.15
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/ethereum/go-ethereum](https://github.com/ethereum/go-ethereum) from 1.11.6 to 1.13.15.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ethereum/go-ethereum/releases">github.com/ethereum/go-ethereum's releases</a>.</em></p>
<blockquote>
<h2>Ontamalca (v1.13.15)</h2>
<p>Geth v1.13.15 is a maintenance-release that contains some fixes mainly to avoid snapsync-related data-corruption.</p>
<p>We recommend all users to upgrade to v1.13.15 as soon as possible.</p>
<hr />
<p>As with all our previous releases, you can find the:</p>
<ul>
<li>Pre-built binaries for all platforms on our <a href="https://geth.ethereum.org/downloads/">downloads page</a>.</li>
<li>Docker images published under <a href="https://cloud.docker.com/u/ethereum/repository/docker/ethereum/client-go"><code>ethereum/client-go</code></a>.</li>
<li>Ubuntu packages in our <a href="https://launchpad.net/~ethereum/+archive/ubuntu/ethereum">Launchpad PPA repository</a>.</li>
<li>OSX packages in our <a href="https://github.com/ethereum/homebrew-ethereum">Homebrew Tap repository</a>.</li>
</ul>
<h2>Altaaya (v1.13.14)</h2>
<p>Geth v1.13.14 is a small maintenance release with a handful of polishes to the blob pool:</p>
<ul>
<li>Disallow blob transactions below the protocol minimum of 1 wei to enter the pool (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/29081">#29081</a>).</li>
<li>Reduce the blob pool's max capacity to 2.5GB for the rollout. (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/29090">#29090</a>).</li>
<li>Fix gas estimation for blob transactions (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/29085">#29085</a>).</li>
</ul>
<p><em><strong>This release is NOT critical for the Cancun fork, but recommended to make Geth lighter in anticipation to unknown blob load.</strong></em></p>
<p>Other fixes:</p>
<ul>
<li>Support overriding the basefee during tracing (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/29051">#29051</a>).</li>
<li>Fix call tracers missing top level logs in top-only mode (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/29068">#29068</a>).</li>
<li>Support unlimited gas for <code>eth_createAccessList</code> if <code>--gascap=0</code> (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/28846">#28846</a>).</li>
</ul>
<p>For a full rundown of the changes please consult the Geth <a href="https://github.com/ethereum/go-ethereum/milestone/162?closed=1">1.13.14 release milestone</a>.</p>
<hr />
<p>As with all our previous releases, you can find the:</p>
<ul>
<li>Pre-built binaries for all platforms on our <a href="https://geth.ethereum.org/downloads/">downloads page</a>.</li>
<li>Docker images published under <a href="https://cloud.docker.com/u/ethereum/repository/docker/ethereum/client-go"><code>ethereum/client-go</code></a>.</li>
<li>Ubuntu packages in our <a href="https://launchpad.net/~ethereum/+archive/ubuntu/ethereum">Launchpad PPA repository</a>.</li>
<li>OSX packages in our <a href="https://github.com/ethereum/homebrew-ethereum">Homebrew Tap repository</a>.</li>
</ul>
<h2>Alsages (v1.13.13)</h2>
<p>This is a minor release with fixes for several issues related to the upcoming Cancun mainnet fork. As such, it is recommended for all mainnet users.</p>
<p>Changes in this release:</p>
<ul>
<li>Block-building performance with blob transactions has been improved a lot. (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/29026">#29026</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/29008">#29008</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/29005">#29005</a>)</li>
<li>A corner case in the EVM related to out-of-order fork scheduling has been fixed. (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/29023">#29023</a>)</li>
<li><code>eth_fillTransaction</code> has seen some bug fixes related to blob transactions as well. (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/28929">#28929</a>, <a href="https://redirect.github.com/ethereum/go-ethereum/pull/29037">#29037</a>)</li>
<li>A rare panic in the ethstats client related to chain reorgs is resolved. (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/29020">#29020</a>)</li>
<li>The blobpool database will now recover from disk corruption faults instead of crashing geth on startup. (<a href="https://redirect.github.com/ethereum/go-ethereum/pull/29001">#29001</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ethereum/go-ethereum/commit/c5ba367eb6232e3eddd7d6226bfd374449c63164"><code>c5ba367</code></a> params: release Geth v 1.13.15</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/35e0525bf47a16eb1deb2a278552707a324b4c23"><code>35e0525</code></a> core, eth/protocols/snap, trie: fix cause for snap-sync corruption, implement...</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/7bcb5532a5c5da3f5ace3abef23c8f807dd9ab79"><code>7bcb553</code></a> eth/filters: enforce topic-limit early on filter criterias (<a href="https://redirect.github.com/ethereum/go-ethereum/issues/29535">#29535</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/e343ddf9eb39a68c12effd1575275c4888c1cbc9"><code>e343ddf</code></a> core/rawdb: add sanity-limit to header accessor (<a href="https://redirect.github.com/ethereum/go-ethereum/issues/29534">#29534</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/5dcf5032b5590e1a74a7bc65f47860cf9ffda5e8"><code>5dcf503</code></a> eth/protocols/snap: skip retrieval for completed storages (<a href="https://redirect.github.com/ethereum/go-ethereum/issues/29378">#29378</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/2bd6bd01d2e8561dd7fc21b631f4a34ac16627a1"><code>2bd6bd0</code></a> Merge branch 'master' into release/1.13</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/9038ba69428a6ecada1f2acace6981854482748b"><code>9038ba6</code></a> params: release Geth v1.13.14</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/51b479e56459d663a12f95fd8eaba82716c0d5ce"><code>51b479e</code></a> core/txpool: elevate the 'already reserved' error into a constant (<a href="https://redirect.github.com/ethereum/go-ethereum/issues/29095">#29095</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/5a0f468f8cb15b939bd85445d33c614a36942a8e"><code>5a0f468</code></a> eth/tracers: Fix callTracer logs on onlyTopCall == true (<a href="https://redirect.github.com/ethereum/go-ethereum/issues/29068">#29068</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/45a272c7b96cb260528bbc2e31d657488f97c4b0"><code>45a272c</code></a> core/txpool: no need to log loud rotate if no local txs (<a href="https://redirect.github.com/ethereum/go-ethereum/issues/29083">#29083</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/ethereum/go-ethereum/compare/v1.11.6...v1.13.15">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/ethereum/go-ethereum&package-manager=go_modules&previous-version=1.11.6&new-version=1.13.15)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-ibc-solidity/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-16 10:02:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/271" class=".btn">#271</a>
            </td>
            <td>
                <b>
                    Bump github.com/btcsuite/btcd from 0.22.1 to 0.24.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/btcsuite/btcd](https://github.com/btcsuite/btcd) from 0.22.1 to 0.24.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/btcsuite/btcd/releases">github.com/btcsuite/btcd's releases</a>.</em></p>
<blockquote>
<h2>btcd v0.24.0</h2>
<p>This release is a major release that includes several general bug fixes, <strong>security bug fixes</strong> (please update!), and also a series of performance improvements that dramatically reduce the time for initial block download from ~45 hours+ to around 6 hours! With this release,<code>btcd</code> now also supports BIP 155 and has gained support for pruning (<code>--prune=MiB</code>).</p>
<h1>Verifying the Release</h1>
<p>In order to verify the release, you'll need to have <code>gpg</code> or <code>gpg2</code> installed on your system. Once you've obtained a copy (and hopefully verified that as well), you'll first need to import the keys that have signed this release if you haven't done so already:</p>
<pre><code>curl https://raw.githubusercontent.com/lightningnetwork/lnd/master/scripts/keys/roasbeef.asc | gpg --import
</code></pre>
<p>Once you have the required PGP keys, you can verify the release (assuming <code>manifest-roasbeef-v0.24.0.sig</code> and <code>manifest-v0.24.0.txt</code> are in the current directory) with:</p>
<pre><code>gpg --verify manifest-roasbeef-v0.24.0.sig manifest-v0.24.0.txt
</code></pre>
<p>You should see the following if the verification was successful:</p>
<pre><code>gpg: Signature made Sat Dec 30 17:11:22 2023 PST
gpg:                using RSA key 60A1FA7DA5BFF08BDCBBE7903BBD59E99B280306
gpg: Good signature from &quot;Olaoluwa Osuntokun &lt;laolu32@gmail.com&gt;&quot; [ultimate]
</code></pre>
<p>That will verify the signature of the manifest file, which ensures integrity and authenticity of the archive you've downloaded locally containing the binaries. Next, depending on your operating system, you should then re-compute the <code>sha256</code> hash of the archive with <code>shasum -a 256 &lt;filename&gt;</code>, compare it with the corresponding one in the manifest file, and ensure they match <em>exactly</em>.</p>
<h1>What's Changed</h1>
<ul>
<li>Musig2: Update to 1.0.0.rc2 by <a href="https://github.com/sputn1ck"><code>@​sputn1ck</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1913">btcsuite/btcd#1913</a></li>
<li>btcec/schnorr/musig2: fix BenchmarkPartialVerify by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1920">btcsuite/btcd#1920</a></li>
<li>base58: fix decoding issue by <a href="https://github.com/guggero"><code>@​guggero</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1923">btcsuite/btcd#1923</a></li>
<li>Update Docker documentation towards building your own image by <a href="https://github.com/guiand888"><code>@​guiand888</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1925">btcsuite/btcd#1925</a></li>
<li>chainhash: JSON marshal hash as string by <a href="https://github.com/ffranr"><code>@​ffranr</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1932">btcsuite/btcd#1932</a></li>
<li>Update Dockerfile to Alpine 3.16 by <a href="https://github.com/guiand888"><code>@​guiand888</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1924">btcsuite/btcd#1924</a></li>
<li>Fix memory leak in connmanager by <a href="https://github.com/hxw"><code>@​hxw</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1576">btcsuite/btcd#1576</a></li>
<li>Update mining.md by <a href="https://github.com/jagottsicher"><code>@​jagottsicher</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1938">btcsuite/btcd#1938</a></li>
<li>Sighash taproot keyspend bug fix by <a href="https://github.com/Roasbeef"><code>@​Roasbeef</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1941">btcsuite/btcd#1941</a></li>
<li>btcutil/psbt: export helper functions, fix/add encoding of unknown fields by <a href="https://github.com/guggero"><code>@​guggero</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1942">btcsuite/btcd#1942</a></li>
<li>docs: Update Go version as per the Readme. by <a href="https://github.com/hristog"><code>@​hristog</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1944">btcsuite/btcd#1944</a></li>
<li>txscript: Fix typo in IsUnspendable() comment by <a href="https://github.com/kcalvinalvin"><code>@​kcalvinalvin</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1945">btcsuite/btcd#1945</a></li>
<li>txscript: allow script builder capacity to be specified by <a href="https://github.com/guggero"><code>@​guggero</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1954">btcsuite/btcd#1954</a></li>
<li>Export MakeScritpNum, AsSmallInt, and IsSmallInt by <a href="https://github.com/martonp"><code>@​martonp</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1956">btcsuite/btcd#1956</a></li>
<li>chainhash: JSON Unmarshal hash from appropriate string. by <a href="https://github.com/LindenWang01"><code>@​LindenWang01</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1952">btcsuite/btcd#1952</a></li>
<li>psbt: add verification method for utxo data by <a href="https://github.com/ziggie1984"><code>@​ziggie1984</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1964">btcsuite/btcd#1964</a></li>
<li>txscript: fix typos by <a href="https://github.com/hieblmi"><code>@​hieblmi</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1957">btcsuite/btcd#1957</a></li>
<li>chaincfg: Update checkpoints by <a href="https://github.com/kcalvinalvin"><code>@​kcalvinalvin</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1968">btcsuite/btcd#1968</a></li>
<li>btcd: Add memory profiling flag by <a href="https://github.com/kcalvinalvin"><code>@​kcalvinalvin</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1953">btcsuite/btcd#1953</a></li>
<li>blockchain: Use slices when fetching utxos by <a href="https://github.com/kcalvinalvin"><code>@​kcalvinalvin</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1972">btcsuite/btcd#1972</a></li>
<li>main: Update README.md's minimum go version by <a href="https://github.com/kcalvinalvin"><code>@​kcalvinalvin</code></a> in <a href="https://redirect.github.com/btcsuite/btcd/pull/1977">btcsuite/btcd#1977</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/btcsuite/btcd/commit/b1b94202082b8e22160df31349992f37fb360f75"><code>b1b9420</code></a> Merge pull request <a href="https://redirect.github.com/btcsuite/btcd/issues/2082">#2082</a> from btcsuite/btcd-24</li>
<li><a href="https://github.com/btcsuite/btcd/commit/4ec8f016b99d7295313c1d2b094033daf447ab11"><code>4ec8f01</code></a> rpcclient: fix race condition in <code>doDisconnect</code></li>
<li><a href="https://github.com/btcsuite/btcd/commit/8d2ab63e36fd6a58967fa53aa4a1df8b9abe09fd"><code>8d2ab63</code></a> build: bump version to btcd v0.24</li>
<li><a href="https://github.com/btcsuite/btcd/commit/3c2478514f224b14721499386c8efc35c412dba3"><code>3c24785</code></a> chaincfg: update mainnet block hashes</li>
<li><a href="https://github.com/btcsuite/btcd/commit/bf23715f9090e4d1386a54409262021f6624cb90"><code>bf23715</code></a> btcd: add SECURITY.md</li>
<li><a href="https://github.com/btcsuite/btcd/commit/d64de4a905b5b5b62559e9359dddfba801b26ff4"><code>d64de4a</code></a> build: update to btcutil v1.1.5</li>
<li><a href="https://github.com/btcsuite/btcd/commit/16684f6cbc9bdd91bef32e056df8b1f5ea1793a3"><code>16684f6</code></a> Merge pull request <a href="https://redirect.github.com/btcsuite/btcd/issues/2073">#2073</a> from Roasbeef/wire-opts</li>
<li><a href="https://github.com/btcsuite/btcd/commit/790c570dda5d37e4e4f8c521548594db31f39619"><code>790c570</code></a> Merge pull request <a href="https://redirect.github.com/btcsuite/btcd/issues/2081">#2081</a> from Roasbeef/dont-serialize-tx-for-txhash</li>
<li><a href="https://github.com/btcsuite/btcd/commit/b0e9636689d9283e034f548a55e60342b5742b3f"><code>b0e9636</code></a> wire: consistently use defer for returning scratch buffers</li>
<li><a href="https://github.com/btcsuite/btcd/commit/e102a81268be375eb74092fb7416108269f50fc4"><code>e102a81</code></a> btcutil: add benchmarks for Hash + WitnessHash</li>
<li>Additional commits viewable in <a href="https://github.com/btcsuite/btcd/compare/v0.22.1...v0.24.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/btcsuite/btcd&package-manager=go_modules&previous-version=0.22.1&new-version=0.24.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-ibc-solidity/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-16 10:02:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/270" class=".btn">#270</a>
            </td>
            <td>
                <b>
                    Bump github.com/cometbft/cometbft from 0.37.2 to 0.38.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/cometbft/cometbft](https://github.com/cometbft/cometbft) from 0.37.2 to 0.38.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/cometbft/cometbft/releases">github.com/cometbft/cometbft's releases</a>.</em></p>
<blockquote>
<h2>v0.38.6</h2>
<p>See the <a href="https://github.com/cometbft/cometbft/blob/v0.38.6/CHANGELOG.md#v0386">CHANGELOG</a> for this release.</p>
<h2>v0.38.5</h2>
<p>See the <a href="https://github.com/cometbft/cometbft/blob/v0.38.5/CHANGELOG.md#v0385">CHANGELOG</a> for this release.</p>
<h2>v0.38.4</h2>
<p>See the <a href="https://github.com/cometbft/cometbft/blob/v0.38.4/CHANGELOG.md#v0384">CHANGELOG</a> for this release.</p>
<h2>v0.38.3</h2>
<p>See the <a href="https://github.com/cometbft/cometbft/blob/v0.38.3/CHANGELOG.md#v0383">CHANGELOG</a> for this release.</p>
<h2>v0.38.2</h2>
<p>See the <a href="https://github.com/cometbft/cometbft/blob/v0.38.2/CHANGELOG.md#v0382">CHANGELOG</a> for this release.</p>
<h2>v0.38.1</h2>
<p>See the <a href="https://github.com/cometbft/cometbft/blob/v0.38.1/CHANGELOG.md#v0381">CHANGELOG</a> for this release.</p>
<h2>v0.38.0</h2>
<p>See the <a href="https://github.com/cometbft/cometbft/blob/v0.38.0/CHANGELOG.md#v0380">CHANGELOG</a> for this release.</p>
<h2>v0.38.0-rc3</h2>
<p>See the <a href="https://github.com/cometbft/cometbft/blob/v0.38.0-rc3/CHANGELOG.md">CHANGELOG</a> for changes available in this pre-release, but not yet officially released.</p>
<h2>v0.38.0-rc2</h2>
<p>See the <a href="https://github.com/cometbft/cometbft/blob/v0.38.0-rc2/CHANGELOG.md">CHANGELOG</a> for changes available in this pre-release, but not yet officially released.</p>
<h2>v0.38.0-rc1</h2>
<p>See the <a href="https://github.com/cometbft/cometbft/blob/v0.38.0-rc1/CHANGELOG.md">CHANGELOG</a> for changes available in this pre-release, but not yet officially released.</p>
<h2>v0.38.0-alpha.2</h2>
<p>See the <a href="https://github.com/cometbft/cometbft/blob/v0.38.0-alpha.2/CHANGELOG.md">CHANGELOG</a> for changes available in this pre-release, but not yet officially released.</p>
<h2>v0.38.0-alpha.1</h2>
<p>See the <a href="https://github.com/cometbft/cometbft/blob/v0.38.0-alpha.1/CHANGELOG.md">CHANGELOG</a> for changes available in this pre-release, but not yet officially released.</p>
<h2>v0.37.6</h2>
<p>See the <a href="https://github.com/cometbft/cometbft/blob/v0.37.6/CHANGELOG.md#v0376">CHANGELOG</a> for this release.</p>
<h2>v0.37.5</h2>
<p>See the <a href="https://github.com/cometbft/cometbft/blob/v0.37.5/CHANGELOG.md#v0375">CHANGELOG</a> for this release.</p>
<h2>v0.37.4</h2>
<p>See the <a href="https://github.com/cometbft/cometbft/blob/v0.37.4/CHANGELOG.md#v0374">CHANGELOG</a> for this release.</p>
<h2>v0.37.3</h2>
<p>See the <a href="https://github.com/cometbft/cometbft/blob/v0.37.3/CHANGELOG.md#v0373">CHANGELOG</a> for this release.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/cometbft/cometbft/blob/v0.38.6/CHANGELOG.md">github.com/cometbft/cometbft's changelog</a>.</em></p>
<blockquote>
<h2>v0.38.6</h2>
<p><em>March 12, 2024</em></p>
<p>This release fixes a security bug in the light client. It also introduces many
improvements to the block sync in collaboration with the
<a href="https://osmosis.zone/">Osmosis</a> team.</p>
<h3>BUG FIXES</h3>
<ul>
<li><code>[privval]</code> Retry accepting a connection (<a href="https://redirect.github.com/cometbft/cometbft/pull/2047">#2047</a>)</li>
<li><code>[state]</code> Fix rollback to a specific height
(<a href="https://redirect.github.com/cometbft/cometbft/pull/2136">#2136</a>)</li>
</ul>
<h3>FEATURES</h3>
<ul>
<li><code>[e2e]</code> Add <code>block_max_bytes</code> option to the manifest file.
(<a href="https://redirect.github.com/cometbft/cometbft/pull/2362">#2362</a>)</li>
</ul>
<h3>IMPROVEMENTS</h3>
<ul>
<li><code>[blocksync]</code> Avoid double-calling <code>types.BlockFromProto</code> for performance
reasons (<a href="https://redirect.github.com/cometbft/cometbft/pull/2016">#2016</a>)</li>
<li><code>[e2e]</code> Add manifest option <code>load_max_txs</code> to limit the number of transactions generated by the
<code>load</code> command. (<a href="https://redirect.github.com/cometbft/cometbft/pull/2094">#2094</a>)</li>
<li><code>[jsonrpc]</code> enable HTTP basic auth in websocket client (<a href="https://redirect.github.com/cometbft/cometbft/pull/2434">#2434</a>)</li>
<li><code>[blocksync]</code> make the max number of downloaded blocks dynamic.
Previously it was a const 600. Now it's <code>peersCount * maxPendingRequestsPerPeer (20)</code>
<a href="https://redirect.github.com/cometbft/cometbft/pull/2467">#2467</a></li>
<li><code>[blocksync]</code> Request a block from peer B if we are approaching pool's height
(less than 50 blocks) and the current peer A is slow in sending us the
block <a href="https://redirect.github.com/cometbft/cometbft/pull/2475">#2475</a></li>
<li><code>[blocksync]</code> Request the block N from peer B immediately after getting
<code>NoBlockResponse</code> from peer A
<a href="https://redirect.github.com/cometbft/cometbft/pull/2475">#2475</a></li>
<li><code>[blocksync]</code> Sort peers by download rate (the fastest peer is picked first)
<a href="https://redirect.github.com/cometbft/cometbft/pull/2475">#2475</a></li>
</ul>
<h2>v0.38.5</h2>
<p><em>January 24, 2024</em></p>
<p>This release fixes a problem introduced in <code>v0.38.3</code>: if an application
updates the value of ConsensusParam <code>VoteExtensionsEnableHeight</code> to the same value
(actually a &quot;noop&quot; update) this is accepted in <code>v0.38.2</code> but rejected under some
conditions in <code>v0.38.3</code> and <code>v0.38.4</code>. Even if rejecting a useless update would make sense
in general, in a point release we should not reject a set of inputs to
a function that was previuosly accepted (unless there is a good reason
for it). The goal of this release is to accept again all &quot;noop&quot; updates, like <code>v0.38.2</code> did.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/cometbft/cometbft/commit/151956229550209d8a1946a4b02a8ed5c4069d78"><code>1519562</code></a> Release v0.38.6 (<a href="https://redirect.github.com/cometbft/cometbft/issues/2592">#2592</a>)</li>
<li><a href="https://github.com/cometbft/cometbft/commit/9db2930cfe2703ecb926b9a1b24cdb66fc395f71"><code>9db2930</code></a> fix(blocksync): use timer instead of time.After (backport <a href="https://redirect.github.com/cometbft/cometbft/issues/2584">#2584</a>) (<a href="https://redirect.github.com/cometbft/cometbft/issues/2587">#2587</a>)</li>
<li><a href="https://github.com/cometbft/cometbft/commit/6cf6978f0235e9616435da8a6d5da1b2f80e6b2f"><code>6cf6978</code></a> feat(blocksync): sort peers by download rate &amp; multiple requests for closer b...</li>
<li><a href="https://github.com/cometbft/cometbft/commit/6d606ce6676f2c4f65e656e26bdd1e1bd0d50fc1"><code>6d606ce</code></a> feat(blocksync): set the max number of (concurrently) downloaded blocks (back...</li>
<li><a href="https://github.com/cometbft/cometbft/commit/d27a96e5c1bba179e8db1e4e2d801f071c5ad069"><code>d27a96e</code></a> build(deps): Bump docker/build-push-action from 5.1.0 to 5.2.0 (<a href="https://redirect.github.com/cometbft/cometbft/issues/2567">#2567</a>)</li>
<li><a href="https://github.com/cometbft/cometbft/commit/2a105034b6065f767b78357f8be4878a7b1f98ee"><code>2a10503</code></a> build(deps): Bump bufbuild/buf-setup-action from 1.29.0 to 1.30.0 (<a href="https://redirect.github.com/cometbft/cometbft/issues/2566">#2566</a>)</li>
<li><a href="https://github.com/cometbft/cometbft/commit/f356b790cd127579debffe6e216f6d68c1fede58"><code>f356b79</code></a> spec(abci): fixes the spec to inform about the presence of invalid extensions...</li>
<li><a href="https://github.com/cometbft/cometbft/commit/6ddf85bb09033e2dda7822e7bda8a4b6bcff617e"><code>6ddf85b</code></a> build(deps): Bump docker/setup-buildx-action from 3.0.0 to 3.1.0 (<a href="https://redirect.github.com/cometbft/cometbft/issues/2509">#2509</a>)</li>
<li><a href="https://github.com/cometbft/cometbft/commit/99c18160d185e474f06c5480b2708aaf8863a4f6"><code>99c1816</code></a> ci: check metrics generation in CI checks (backport <a href="https://redirect.github.com/cometbft/cometbft/issues/2483">#2483</a>) (<a href="https://redirect.github.com/cometbft/cometbft/issues/2485">#2485</a>)</li>
<li><a href="https://github.com/cometbft/cometbft/commit/91413e67c7e3627f48431605938697115a937939"><code>91413e6</code></a> docs(changelog): add missing entry for <a href="https://redirect.github.com/cometbft/cometbft/issues/2136">#2136</a> (backport <a href="https://redirect.github.com/cometbft/cometbft/issues/2459">#2459</a>) (<a href="https://redirect.github.com/cometbft/cometbft/issues/2464">#2464</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/cometbft/cometbft/compare/v0.37.2...v0.38.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/cometbft/cometbft&package-manager=go_modules&previous-version=0.37.2&new-version=0.38.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-ibc-solidity/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-16 10:02:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/269" class=".btn">#269</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/protobuf from 1.31.0 to 1.33.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps google.golang.org/protobuf from 1.31.0 to 1.33.0.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/protobuf&package-manager=go_modules&previous-version=1.31.0&new-version=1.33.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-ibc-solidity/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-16 10:01:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/268" class=".btn">#268</a>
            </td>
            <td>
                <b>
                    Bump golang.org/x/net from 0.12.0 to 0.23.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/net](https://github.com/golang/net) from 0.12.0 to 0.23.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/golang/net/commit/c48da131589f122489348be5dfbcb6457640046f"><code>c48da13</code></a> http2: fix TestServerContinuationFlood flakes</li>
<li><a href="https://github.com/golang/net/commit/762b58d1cf6e0779780decad89c6c1523386638d"><code>762b58d</code></a> http2: fix tipos in comment</li>
<li><a href="https://github.com/golang/net/commit/ba872109ef2dc8f1da778651bd1fd3792d0e4587"><code>ba87210</code></a> http2: close connections when receiving too many headers</li>
<li><a href="https://github.com/golang/net/commit/ebc8168ac8ac742194df729305175940790c55a2"><code>ebc8168</code></a> all: fix some typos</li>
<li><a href="https://github.com/golang/net/commit/3678185f8a652e52864c44049a9ea96b7bcc066a"><code>3678185</code></a> http2: make TestCanonicalHeaderCacheGrowth faster</li>
<li><a href="https://github.com/golang/net/commit/448c44f9287b6745f958d74aa2a17ec7761c2f13"><code>448c44f</code></a> http2: remove clientTester</li>
<li><a href="https://github.com/golang/net/commit/c7877ac4213b2f859831366f5a35b353e0dc9f66"><code>c7877ac</code></a> http2: convert the remaining clientTester tests to testClientConn</li>
<li><a href="https://github.com/golang/net/commit/d8870b0bf2f2426fc8d19a9332f652da5c25418f"><code>d8870b0</code></a> http2: use synthetic time in TestIdleConnTimeout</li>
<li><a href="https://github.com/golang/net/commit/d73acffdc9493532acb85777105bb4a351eea702"><code>d73acff</code></a> http2: only set up deadline when Server.IdleTimeout is positive</li>
<li><a href="https://github.com/golang/net/commit/89f602b7bbf237abe0467031a18b42fc742ced08"><code>89f602b</code></a> http2: validate client/outgoing trailers</li>
<li>Additional commits viewable in <a href="https://github.com/golang/net/compare/v0.12.0...v0.23.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/net&package-manager=go_modules&previous-version=0.12.0&new-version=0.23.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-ibc-solidity/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-16 10:01:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/267" class=".btn">#267</a>
            </td>
            <td>
                <b>
                    QBFT support
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
        Created At 2024-05-15 09:16:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/266" class=".btn">#266</a>
            </td>
            <td>
                <b>
                    Remove some npm dependencies
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
        Created At 2024-05-15 07:18:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/265" class=".btn">#265</a>
            </td>
            <td>
                <b>
                    Mkdir clients/{09-localhost,ibft2,mock} and move implementations into the directories respectively
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
        Created At 2024-05-15 06:07:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/264" class=".btn">#264</a>
            </td>
            <td>
                <b>
                    ibft2: add trusting period validation
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
        Created At 2024-05-14 14:47:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/263" class=".btn">#263</a>
            </td>
            <td>
                <b>
                    Fix typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix typos
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 06:22:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/262" class=".btn">#262</a>
            </td>
            <td>
                <b>
                    ics20: Remove unused `Address` library
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
        Created At 2024-05-13 03:11:03 +0000 UTC
    </div>
</div>

