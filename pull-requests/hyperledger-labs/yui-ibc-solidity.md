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
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/198" class=".btn">#198</a>
            </td>
            <td>
                <b>
                    build(deps): bump github.com/cosmos/cosmos-sdk from 0.45.7 to 0.47.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/cosmos/cosmos-sdk](https://github.com/cosmos/cosmos-sdk) from 0.45.7 to 0.47.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/cosmos/cosmos-sdk/releases">github.com/cosmos/cosmos-sdk's releases</a>.</em></p>
<blockquote>
<h2>v0.47.3</h2>
<h1>Cosmos SDK v0.47.3 Release Notes</h1>
<p>💬 <a href="https://github.com/orgs/cosmos/discussions/categories/announcements"><strong>Release Discussion</strong></a></p>
<h2>🚀 Highlights</h2>
<p>Missed the v0.47.0 announcement? Read it <a href="https://github.com/cosmos/cosmos-sdk/releases/tag/v0.47.0">here</a>.
For this third patch release of the <code>v0.47.x</code> line, some of the notable changes include:</p>
<ul>
<li>The <a href="https://forum.cosmos.network/t/cosmos-sdk-security-advisory-barberry/10825">barberry</a> security vulnerability is resolved. All chains using Cosmos SDK <code>v0.47.0-v0.47.2</code> are advised to upgrade to <code>v0.47.3</code> <strong>immediately</strong>. A chain is not affected by the vulnerability as soon as <strong>33%+1</strong> of the voting power has upgraded. A chain is safe from halting as soon as <strong>66%+1</strong> of the voting power has upgraded. Coordinate with your validators to upgrade as soon as possible. The upgrade can be applied as a rolling upgrade across the validators or as a coordinated upgrade. Networks should decide which option gets them upgraded quicker.</li>
<li>A command to be able to bootstrap comet from a local snapshot with <a href="https://docs.cosmos.network/v0.47/run-node/run-node#local-state-sync"><code>&lt;app&gt; comet bootstrap-state</code></a>.</li>
<li>Commands to manage snapshots: Add <code>snapshot.Cmd(appCreator)</code> to your chain root command for using them.</li>
<li>The default logger is now <code>cosmossdk.io/log</code>, which supports coloring 🟥🟩🟪🟦 and filtering again.</li>
<li>A bug fix in <code>x/group</code> migration. Chains migrating from v0.46.x to v0.47.x must use at least v0.47.<strong>3</strong>.</li>
</ul>
<p>Check out the <a href="https://github.com/cosmos/cosmos-sdk/blob/v0.47.3/CHANGELOG.md">changelog</a> for an exhaustive list of changes or <a href="https://github.com/cosmos/cosmos-sdk/compare/v0.47.2...v0.47.3">compare changes</a> from last release.</p>
<p>Refer to the <a href="https://github.com/cosmos/cosmos-sdk/blob/release/v0.47.x/UPGRADING.md">upgrading guide</a> when migrating from <code>v0.46.x</code> to <code>v0.47.0</code>.</p>
<h2>v0.47.2</h2>
<h1>Cosmos SDK v0.47.2 Release Notes</h1>
<p>💬 <a href="https://github.com/orgs/cosmos/discussions/6"><strong>Release Discussion</strong></a></p>
<h2>📝 Changelog</h2>
<p>Check out the <a href="https://github.com/cosmos/cosmos-sdk/blob/v0.47.2/CHANGELOG.md">changelog</a> for an exhaustive list of changes or <a href="https://github.com/cosmos/cosmos-sdk/compare/v0.47.1...v0.47.2">compare changes</a> from last release.</p>
<p>Refer to the <a href="https://github.com/cosmos/cosmos-sdk/blob/release/v0.47.x/UPGRADING.md">upgrading guide</a> when migrating from <code>v0.46.x</code> to <code>v0.47.0</code>.</p>
<h2>🚀 Highlights</h2>
<p>For this second patch release of the <code>v0.47.x</code> line, we focused on fixing bugs and improving the developer experience.
Missed the v0.47.0 announcement? Read it <a href="https://github.com/cosmos/cosmos-sdk/releases/tag/v0.47.0">here</a>.</p>
<p>Notably, <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/15683">a fix</a> for loading archival states (thank you <a href="https://github.com/catShaark"><code>@​catShaark</code></a>).
Additionally, the release fixes an issue where querying previous block heights would return an incorrect timestamp.</p>
<h2>v0.47.1</h2>
<h1>Cosmos SDK v0.47.1 Release Notes</h1>
<p>💬 <a href="https://github.com/cosmos/community"><strong>Release Discussion</strong></a></p>
<h2>📝 Changelog</h2>
<p>Check out the <a href="https://github.com/cosmos/cosmos-sdk/blob/v0.47.1/CHANGELOG.md">changelog</a> for an exhaustive list of changes, or <a href="https://github.com/cosmos/cosmos-sdk/compare/v0.47.0...v0.47.1">compare changes</a> from last release.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/cosmos/cosmos-sdk/blob/main/CHANGELOG.md">github.com/cosmos/cosmos-sdk's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/cosmos/cosmos-sdk/releases/tag/v0.47.3">v0.47.3</a> - 2023-06-08</h2>
<h3>Features</h3>
<ul>
<li>(baseapp) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/16290">#16290</a> Add circuit breaker setter in baseapp.</li>
<li>(x/group) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/16191">#16191</a> Add EventProposalPruned event to group module whenever a proposal is pruned.</li>
<li>(tx) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/15992">#15992</a> Add <code>WithExtensionOptions</code> in tx Factory to allow <code>SetExtensionOptions</code> with given extension options.</li>
</ul>
<h3>Improvements</h3>
<ul>
<li>(baseapp) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/16407">#16407</a> Make <code>DefaultProposalHandler.ProcessProposalHandler</code> return a ProcessProposal NoOp when using none or a NoOp mempool.</li>
<li>(deps) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/16083">#16083</a> Bumps <code>proto-builder</code> image to 0.13.0.</li>
<li>(client) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/16075">#16075</a> Partly revert <a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/15953">#15953</a> and <code>factory.Prepare</code> now does nothing in offline mode.</li>
<li>(server) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/15984">#15984</a> Use <code>cosmossdk.io/log</code> package for logging instead of CometBFT logger. NOTE: v0.45 and v0.46 were not using CometBFT logger either. This keeps the same underlying logger (zerolog) as in v0.45.x+ and v0.46.x+ but now properly supporting filtered logging.</li>
<li>(gov) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/15979">#15979</a> Improve gov error message when failing to convert v1 proposal to v1beta1.</li>
<li>(store) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/16067">#16067</a> Add local snapshots management commands.</li>
<li>(server) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/16061">#16061</a> Add Comet bootstrap command.</li>
<li>(snapshots) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/16060">#16060</a> Support saving and restoring snapshot locally.</li>
<li>(x/staking) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/16068">#16068</a> Update simulation to allow non-EOA accounts to stake.</li>
<li>(server) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/16142">#16142</a> Remove JSON Indentation from the GRPC to REST gateway's responses. (Saving bandwidth)</li>
<li>(types) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/16145">#16145</a> Rename interface <code>ExtensionOptionI</code> back to <code>TxExtensionOptionI</code> to avoid breaking change.</li>
<li>(baseapp) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/16193">#16193</a> Add <code>Close</code> method to <code>BaseApp</code> for custom app to cleanup resource in graceful shutdown.</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>Fix <a href="https://forum.cosmos.network/t/cosmos-sdk-security-advisory-barberry/10825">barberry</a> security vulnerability.</li>
<li>(server) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/16395">#16395</a> Do not override some Comet config is purposely set differently in <code>InterceptConfigsPreRunHandler</code>.</li>
<li>(store) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/16449">#16449</a> Fix StateSync Restore by excluding memory store.</li>
<li>(cli) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/16312">#16312</a> Allow any addresses in <code>client.ValidatePromptAddress</code>.</li>
<li>(x/group) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/16017">#16017</a> Correctly apply account number in group v2 migration.</li>
</ul>
<h3>API Breaking Changes</h3>
<ul>
<li>(testutil) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/14991">#14991</a> The <code>testutil/testdata_pulsar</code> package has moved to <code>testutil/testdata/testpb</code>.  Chains will not notice this breaking change as this package contains testing utilities only used by the SDK internally.</li>
</ul>
<h2><a href="https://github.com/cosmos/cosmos-sdk/releases/tag/v0.47.2">v0.47.2</a> - 2023-04-27</h2>
<h3>Improvements</h3>
<ul>
<li>(x/evidence) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/15908">#15908</a> Update the equivocation handler to work with ICS by removing a pubkey check that was performing a no-op for consumer chains.</li>
<li>(x/slashing) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/15908">#15908</a> Remove the validators' pubkey check in the signature handler in order to work with ICS.</li>
<li>(deps) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/15957">#15957</a> Bump CometBFT to <a href="https://github.com/cometbft/cometbft/blob/v0.37.1/CHANGELOG.md#v0371">v0.37.1</a>.</li>
<li>(store) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/15683">#15683</a> <code>rootmulti.Store.CacheMultiStoreWithVersion</code> now can handle loading archival states that don't persist any of the module stores the current state has.</li>
<li><a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/15448">#15448</a> Automatically populate the block timestamp for historical queries. In contexts where the block timestamp is needed for previous states, the timestamp will now be set. Note, when querying against a node it must be re-synced in order to be able to automatically populate the block timestamp. Otherwise, the block timestamp will be populated for heights going forward once upgraded.</li>
<li><a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/14019">#14019</a> Remove the interface casting to allow other implementations of a <code>CommitMultiStore</code>.</li>
<li>(simtestutil) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/15903">#15903</a> Add <code>AppStateFnWithExtendedCbs</code> with moduleStateCb callback function to allow access moduleState.</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>(baseapp) <a href="https://redirect.github.com/cosmos/cosmos-sdk/pull/15789">#15789</a> Ensure <code>PrepareProposal</code> and <code>ProcessProposal</code> respect <code>InitialHeight</code> set by CometBFT when set to a value greater than 1.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/cosmos/cosmos-sdk/commit/666c345ad23ddda9523cc5cd1b71187d91c26f34"><code>666c345</code></a> fix: patch barberry (<a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/16465">#16465</a>)</li>
<li><a href="https://github.com/cosmos/cosmos-sdk/commit/cfc757dc5043fb2758c47c146d2912fd010c1a45"><code>cfc757d</code></a> chore: prepare v0.47.3 (2/2) (<a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/16444">#16444</a>)</li>
<li><a href="https://github.com/cosmos/cosmos-sdk/commit/3bbc0aaed7d3270d5aaecd86d950aca33a5cecfb"><code>3bbc0aa</code></a> fix: StateSync Restore by excluding memory store (backport <a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/16449">#16449</a>) (<a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/16452">#16452</a>)</li>
<li><a href="https://github.com/cosmos/cosmos-sdk/commit/48becdf19a342e7478aa5839e6c10c985cbfc63b"><code>48becdf</code></a> docs: improve upgrading.md and changelog (backport <a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/16429">#16429</a>) (<a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/16431">#16431</a>)</li>
<li><a href="https://github.com/cosmos/cosmos-sdk/commit/dda81a2275d7a9553a74068e5edd22d942ad9124"><code>dda81a2</code></a> refactor: avoid breaking change due to <a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/16415">#16415</a> included in v0.50 (<a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/16430">#16430</a>)</li>
<li><a href="https://github.com/cosmos/cosmos-sdk/commit/ba2f1be04c4386b4b224415f0075d0ff99357d98"><code>ba2f1be</code></a> chore: change prepare and process proposal to be NoOps by default (backport #...</li>
<li><a href="https://github.com/cosmos/cosmos-sdk/commit/616841b9704dac92285834382a8aa7be89845d7b"><code>616841b</code></a> chore: small snapshot commands &amp; docs improvement (backport <a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/16404">#16404</a>) (<a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/16408">#16408</a>)</li>
<li><a href="https://github.com/cosmos/cosmos-sdk/commit/2cd72b74ba8e0e5cdd31d7a3aeb2bd2e0da68875"><code>2cd72b7</code></a> chore: prepare v0.47.3 (<a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/16248">#16248</a>)</li>
<li><a href="https://github.com/cosmos/cosmos-sdk/commit/2e70efc10af3793acddbd285d4c300e1e63b34e2"><code>2e70efc</code></a> fix: do not overwrite comet config when set in `InterceptConfigsPreRunHandler...</li>
<li><a href="https://github.com/cosmos/cosmos-sdk/commit/6d959001169ce78360887faf882680bf52b09ae8"><code>6d95900</code></a> feat: support extension options for build tx (backport: <a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/15992">#15992</a>) (<a href="https://redirect.github.com/cosmos/cosmos-sdk/issues/16317">#16317</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/cosmos/cosmos-sdk/compare/v0.45.7...v0.47.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/cosmos/cosmos-sdk&package-manager=go_modules&previous-version=0.45.7&new-version=0.47.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-ibc-solidity/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-22 20:09:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/197" class=".btn">#197</a>
            </td>
            <td>
                <b>
                    build(deps): bump @openzeppelin/contracts from 4.8.3 to 4.9.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) from 4.8.3 to 4.9.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/releases"><code>@​openzeppelin/contracts</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.9.2</h2>
<blockquote>
<p><strong>Note</strong>
This release contains a fix for <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-wprv-93r4-jj2p">https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-wprv-93r4-jj2p</a>.</p>
</blockquote>
<ul>
<li><code>MerkleProof</code>: Fix a bug in <code>processMultiProof</code> and <code>processMultiProofCalldata</code> that allows proving arbitrary leaves if the tree contains a node with value 0 at depth 1.</li>
</ul>
<h2>v4.9.1</h2>
<blockquote>
<p><strong>Note</strong>
This release contains a fix for <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-5h3x-9wvq-w4m2">https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-5h3x-9wvq-w4m2</a>.</p>
</blockquote>
<ul>
<li><code>Governor</code>: Add a mechanism to restrict the address of the proposer using a suffix in the description.</li>
</ul>
<h2>v4.9.0</h2>
<ul>
<li><code>ReentrancyGuard</code>: Add a <code>_reentrancyGuardEntered</code> function to expose the guard status. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3714">#3714</a>)</li>
<li><code>ERC721Wrapper</code>: add a new extension of the <code>ERC721</code> token which wraps an underlying token. Deposit and withdraw guarantee that the ownership of each token is backed by a corresponding underlying token with the same identifier. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3863">#3863</a>)</li>
<li><code>EnumerableMap</code>: add a <code>keys()</code> function that returns an array containing all the keys. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3920">#3920</a>)</li>
<li><code>Governor</code>: add a public <code>cancel(uint256)</code> function. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3983">#3983</a>)</li>
<li><code>Governor</code>: Enable timestamp operation for blockchains without a stable block time. This is achieved by connecting a Governor's internal clock to match a voting token's EIP-6372 interface. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3934">#3934</a>)</li>
<li><code>Strings</code>: add <code>equal</code> method. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3774">#3774</a>)</li>
<li><code>IERC5313</code>: Add an interface for EIP-5313 that is now final. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4013">#4013</a>)</li>
<li><code>IERC4906</code>: Add an interface for ERC-4906 that is now Final. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4012">#4012</a>)</li>
<li><code>StorageSlot</code>: Add support for <code>string</code> and <code>bytes</code>. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4008">#4008</a>)</li>
<li><code>Votes</code>, <code>ERC20Votes</code>, <code>ERC721Votes</code>: support timestamp checkpointing using EIP-6372. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3934">#3934</a>)</li>
<li><code>ERC4626</code>: Add mitigation to the inflation attack through virtual shares and assets. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3979">#3979</a>)</li>
<li><code>Strings</code>: add <code>toString</code> method for signed integers. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3773">#3773</a>)</li>
<li><code>ERC20Wrapper</code>: Make the <code>underlying</code> variable private and add a public accessor. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4029">#4029</a>)</li>
<li><code>EIP712</code>: add EIP-5267 support for better domain discovery. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3969">#3969</a>)</li>
<li><code>AccessControlDefaultAdminRules</code>: Add an extension of <code>AccessControl</code> with additional security rules for the <code>DEFAULT_ADMIN_ROLE</code>. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4009">#4009</a>)</li>
<li><code>SignatureChecker</code>: Add <code>isValidERC1271SignatureNow</code> for checking a signature directly against a smart contract using ERC-1271. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3932">#3932</a>)</li>
<li><code>SafeERC20</code>: Add a <code>forceApprove</code> function to improve compatibility with tokens behaving like USDT. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4067">#4067</a>)</li>
<li><code>ERC1967Upgrade</code>: removed contract-wide <code>oz-upgrades-unsafe-allow delegatecall</code> annotation, replaced by granular annotation in <code>UUPSUpgradeable</code>. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3971">#3971</a>)</li>
<li><code>ERC20Wrapper</code>: self wrapping and deposit by the wrapper itself are now explicitly forbidden. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4100">#4100</a>)</li>
<li><code>ECDSA</code>: optimize bytes32 computation by using assembly instead of <code>abi.encodePacked</code>. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3853">#3853</a>)</li>
<li><code>ERC721URIStorage</code>: Emit ERC-4906 <code>MetadataUpdate</code> in <code>_setTokenURI</code>. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4012">#4012</a>)</li>
<li><code>ShortStrings</code>: Added a library for handling short strings in a gas efficient way, with fallback to storage for longer strings. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4023">#4023</a>)</li>
<li><code>SignatureChecker</code>: Allow return data length greater than 32 from EIP-1271 signers. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4038">#4038</a>)</li>
<li><code>UUPSUpgradeable</code>: added granular <code>oz-upgrades-unsafe-allow-reachable</code> annotation to improve upgrade safety checks on latest version of the Upgrades Plugins (starting with <code>@openzeppelin/upgrades-core@1.21.0</code>). (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3971">#3971</a>)</li>
<li><code>Initializable</code>: optimize <code>_disableInitializers</code> by using <code>!=</code> instead of <code>&lt;</code>. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3787">#3787</a>)</li>
<li><code>Ownable2Step</code>: make <code>acceptOwnership</code> public virtual to enable usecases that require overriding it. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3960">#3960</a>)</li>
<li><code>UUPSUpgradeable.sol</code>: Change visibility to the functions <code>upgradeTo </code> and <code>upgradeToAndCall </code> from <code>external</code> to <code>public</code>. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3959">#3959</a>)</li>
<li><code>TimelockController</code>: Add the <code>CallSalt</code> event to emit on operation schedule. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4001">#4001</a>)</li>
<li>Reformatted codebase with latest version of Prettier Solidity. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3898">#3898</a>)</li>
<li><code>Math</code>: optimize <code>log256</code> rounding check. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3745">#3745</a>)</li>
<li><code>ERC20Votes</code>: optimize by using unchecked arithmetic. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3748">#3748</a>)</li>
<li><code>Multicall</code>: annotate <code>multicall</code> function as upgrade safe to not raise a flag for its delegatecall. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3961">#3961</a>)</li>
<li><code>ERC20Pausable</code>, <code>ERC721Pausable</code>, <code>ERC1155Pausable</code>: Add note regarding missing public pausing functionality (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4007">#4007</a>)</li>
<li><code>ECDSA</code>: Add a function <code>toDataWithIntendedValidatorHash</code> that encodes data with version 0x00 following EIP-191. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4063">#4063</a>)</li>
<li><code>MerkleProof</code>: optimize by using unchecked arithmetic. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3745">#3745</a>)</li>
</ul>
<h3>Breaking changes</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/blob/v4.9.2/CHANGELOG.md"><code>@​openzeppelin/contracts</code>'s changelog</a>.</em></p>
<blockquote>
<h2>4.9.2 (2023-06-16)</h2>
<ul>
<li><code>MerkleProof</code>: Fix a bug in <code>processMultiProof</code> and <code>processMultiProofCalldata</code> that allows proving arbitrary leaves if the tree contains a node with value 0 at depth 1.</li>
</ul>
<h2>4.9.1 (2023-06-07)</h2>
<ul>
<li><code>Governor</code>: Add a mechanism to restrict the address of the proposer using a suffix in the description.</li>
</ul>
<h2>4.9.0 (2023-05-23)</h2>
<ul>
<li><code>ReentrancyGuard</code>: Add a <code>_reentrancyGuardEntered</code> function to expose the guard status. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3714">#3714</a>)</li>
<li><code>ERC721Wrapper</code>: add a new extension of the <code>ERC721</code> token which wraps an underlying token. Deposit and withdraw guarantee that the ownership of each token is backed by a corresponding underlying token with the same identifier. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3863">#3863</a>)</li>
<li><code>EnumerableMap</code>: add a <code>keys()</code> function that returns an array containing all the keys. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3920">#3920</a>)</li>
<li><code>Governor</code>: add a public <code>cancel(uint256)</code> function. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3983">#3983</a>)</li>
<li><code>Governor</code>: Enable timestamp operation for blockchains without a stable block time. This is achieved by connecting a Governor's internal clock to match a voting token's EIP-6372 interface. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3934">#3934</a>)</li>
<li><code>Strings</code>: add <code>equal</code> method. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3774">#3774</a>)</li>
<li><code>IERC5313</code>: Add an interface for EIP-5313 that is now final. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4013">#4013</a>)</li>
<li><code>IERC4906</code>: Add an interface for ERC-4906 that is now Final. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4012">#4012</a>)</li>
<li><code>StorageSlot</code>: Add support for <code>string</code> and <code>bytes</code>. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4008">#4008</a>)</li>
<li><code>Votes</code>, <code>ERC20Votes</code>, <code>ERC721Votes</code>: support timestamp checkpointing using EIP-6372. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3934">#3934</a>)</li>
<li><code>ERC4626</code>: Add mitigation to the inflation attack through virtual shares and assets. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3979">#3979</a>)</li>
<li><code>Strings</code>: add <code>toString</code> method for signed integers. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3773">#3773</a>)</li>
<li><code>ERC20Wrapper</code>: Make the <code>underlying</code> variable private and add a public accessor. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4029">#4029</a>)</li>
<li><code>EIP712</code>: add EIP-5267 support for better domain discovery. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3969">#3969</a>)</li>
<li><code>AccessControlDefaultAdminRules</code>: Add an extension of <code>AccessControl</code> with additional security rules for the <code>DEFAULT_ADMIN_ROLE</code>. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4009">#4009</a>)</li>
<li><code>SignatureChecker</code>: Add <code>isValidERC1271SignatureNow</code> for checking a signature directly against a smart contract using ERC-1271. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3932">#3932</a>)</li>
<li><code>SafeERC20</code>: Add a <code>forceApprove</code> function to improve compatibility with tokens behaving like USDT. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4067">#4067</a>)</li>
<li><code>ERC1967Upgrade</code>: removed contract-wide <code>oz-upgrades-unsafe-allow delegatecall</code> annotation, replaced by granular annotation in <code>UUPSUpgradeable</code>. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3971">#3971</a>)</li>
<li><code>ERC20Wrapper</code>: self wrapping and deposit by the wrapper itself are now explicitly forbidden. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4100">#4100</a>)</li>
<li><code>ECDSA</code>: optimize bytes32 computation by using assembly instead of <code>abi.encodePacked</code>. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3853">#3853</a>)</li>
<li><code>ERC721URIStorage</code>: Emit ERC-4906 <code>MetadataUpdate</code> in <code>_setTokenURI</code>. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4012">#4012</a>)</li>
<li><code>ShortStrings</code>: Added a library for handling short strings in a gas efficient way, with fallback to storage for longer strings. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4023">#4023</a>)</li>
<li><code>SignatureChecker</code>: Allow return data length greater than 32 from EIP-1271 signers. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4038">#4038</a>)</li>
<li><code>UUPSUpgradeable</code>: added granular <code>oz-upgrades-unsafe-allow-reachable</code> annotation to improve upgrade safety checks on latest version of the Upgrades Plugins (starting with <code>@openzeppelin/upgrades-core@1.21.0</code>). (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3971">#3971</a>)</li>
<li><code>Initializable</code>: optimize <code>_disableInitializers</code> by using <code>!=</code> instead of <code>&lt;</code>. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3787">#3787</a>)</li>
<li><code>Ownable2Step</code>: make <code>acceptOwnership</code> public virtual to enable usecases that require overriding it. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3960">#3960</a>)</li>
<li><code>UUPSUpgradeable.sol</code>: Change visibility to the functions <code>upgradeTo </code> and <code>upgradeToAndCall </code> from <code>external</code> to <code>public</code>. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3959">#3959</a>)</li>
<li><code>TimelockController</code>: Add the <code>CallSalt</code> event to emit on operation schedule. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4001">#4001</a>)</li>
<li>Reformatted codebase with latest version of Prettier Solidity. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3898">#3898</a>)</li>
<li><code>Math</code>: optimize <code>log256</code> rounding check. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3745">#3745</a>)</li>
<li><code>ERC20Votes</code>: optimize by using unchecked arithmetic. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3748">#3748</a>)</li>
<li><code>Multicall</code>: annotate <code>multicall</code> function as upgrade safe to not raise a flag for its delegatecall. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3961">#3961</a>)</li>
<li><code>ERC20Pausable</code>, <code>ERC721Pausable</code>, <code>ERC1155Pausable</code>: Add note regarding missing public pausing functionality (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4007">#4007</a>)</li>
<li><code>ECDSA</code>: Add a function <code>toDataWithIntendedValidatorHash</code> that encodes data with version 0x00 following EIP-191. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4063">#4063</a>)</li>
<li><code>MerkleProof</code>: optimize by using unchecked arithmetic. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3745">#3745</a>)</li>
</ul>
<h3>Breaking changes</h3>
<ul>
<li><code>EIP712</code>: Addition of ERC5267 support requires support for user defined value types, which was released in Solidity version 0.8.8. This requires a pragma change from <code>^0.8.0</code> to <code>^0.8.8</code>.</li>
<li><code>EIP712</code>: Optimization of the cache for the upgradeable version affects the way <code>name</code> and <code>version</code> are set. This is no longer done through an initializer, and is instead part of the implementation's constructor. As a consequence, all proxies using the same implementation will necessarily share the same <code>name</code> and <code>version</code>. Additionally, an implementation upgrade risks changing the EIP712 domain unless the same <code>name</code> and <code>version</code> are used when deploying the new implementation contract.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/e50c24f5839db17f46991478384bfda14acfb830"><code>e50c24f</code></a> Release v4.9.2 (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4364">#4364</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/4d2383e17186be3e8ccf5a442e9686ecc7de1c55"><code>4d2383e</code></a> Merge pull request from GHSA-wprv-93r4-jj2p</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/f03420b5c77ae3cfa73fce4ffc7f4778cfa2b503"><code>f03420b</code></a> Remove automatic conflict resolution for merge from release branch (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4362">#4362</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/ded8c9eedb9a03b0703b65d430e6d0076cb0e444"><code>ded8c9e</code></a> Update index.adoc (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4336">#4336</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/281550b71c3df9a83e6b80ceefc700852c287570"><code>281550b</code></a> Release v4.9.1 (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4321">#4321</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/33ff9b086dab790e87948f6007aa4b00bf5252cc"><code>33ff9b0</code></a> Merge pull request from GHSA-5h3x-9wvq-w4m2</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/fa3a30a580e87dbc4f3a7693296901c0b83f06aa"><code>fa3a30a</code></a> Fix typo in crosschain.adoc</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/4e6deb3c56c8b054396836f52bff9c67fde766e7"><code>4e6deb3</code></a> Fix import substitution for docs examples</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/819820517d70820f80a12dd835099c32d7cebb9b"><code>8198205</code></a> Fix doc MyGovernor example doesn't compile (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4282">#4282</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/a6e267169036f90d4244683d9709e3190622c9f6"><code>a6e2671</code></a> Fix release merge script (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4273">#4273</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/compare/v4.8.3...v4.9.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts&package-manager=npm_and_yarn&previous-version=4.8.3&new-version=4.9.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-ibc-solidity/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-19 20:15:18 +0000 UTC
    </div>
</div>

