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

