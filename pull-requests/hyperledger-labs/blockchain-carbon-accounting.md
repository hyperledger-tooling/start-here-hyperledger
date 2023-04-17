---
layout: default
title: blockchain-carbon-accounting
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-carbon-accounting
---

# blockchain-carbon-accounting <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-carbon-accounting){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/680" class=".btn">#680</a>
            </td>
            <td>
                <b>
                    Bump @openzeppelin/contracts from 4.7.3 to 4.8.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) from 4.7.3 to 4.8.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/releases"><code>@​openzeppelin/contracts</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.8.3</h2>
<blockquote>
<p><strong>Note</strong>
This release contains fixes for <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-mx2q-35m2-x2rh">https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-mx2q-35m2-x2rh</a> and <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-93hq-5wgc-jc82">https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-93hq-5wgc-jc82</a>.</p>
</blockquote>
<ul>
<li><code>GovernorCompatibilityBravo</code>: Fix encoding of proposal data when signatures are missing.</li>
<li><code>TransparentUpgradeableProxy</code>: Fix transparency in case of selector clash with non-decodable calldata or payable mutability. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4154">#4154</a>)</li>
</ul>
<h2>v4.8.2</h2>
<blockquote>
<p><strong>Note</strong>
This release contains a fix for <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-878m-3g6q-594q">https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-878m-3g6q-594q</a>.</p>
</blockquote>
<ul>
<li><code>ERC721Consecutive</code>: Fixed a bug when <code>_mintConsecutive</code> is used for batches of size 1 that could lead to balance overflow. Refer to the breaking changes section in the changelog for a note on the behavior of <code>ERC721._beforeTokenTransfer</code>.</li>
</ul>
<h3>Breaking changes</h3>
<ul>
<li><code>ERC721</code>: The internal function <code>_beforeTokenTransfer</code> no longer updates balances, which it previously did when <code>batchSize</code> was greater than 1. This change has no consequence unless a custom ERC721 extension is explicitly invoking <code>_beforeTokenTransfer</code>. Balance updates in extensions must now be done explicitly using <code>__unsafe_increaseBalance</code>, with a name that indicates that there is an invariant that has to be manually verified.</li>
</ul>
<h2>v4.8.1</h2>
<ul>
<li><code>ERC4626</code>: Use staticcall instead of call when fetching underlying ERC-20 decimals. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3943">#3943</a>)</li>
</ul>
<h2>v4.8.0</h2>
<blockquote>
<p><strong>Note</strong>
Don't miss the section on <strong>Breaking changes</strong> at the end.</p>
</blockquote>
<ul>
<li><code>TimelockController</code>: Added a new <code>admin</code> constructor parameter that is assigned the admin role instead of the deployer account. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3722">#3722</a>)</li>
<li><code>Initializable</code>: add internal functions <code>_getInitializedVersion</code> and <code>_isInitializing</code> (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3598">#3598</a>)</li>
<li><code>ERC165Checker</code>: add <code>supportsERC165InterfaceUnchecked</code> for consulting individual interfaces without the full ERC165 protocol. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3339">#3339</a>)</li>
<li><code>Address</code>: optimize <code>functionCall</code> by calling <code>functionCallWithValue</code> directly. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3468">#3468</a>)</li>
<li><code>Address</code>: optimize <code>functionCall</code> functions by checking contract size only if there is no returned data. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3469">#3469</a>)</li>
<li><code>Governor</code>: make the <code>relay</code> function payable, and add support for EOA payments. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3730">#3730</a>)</li>
<li><code>GovernorCompatibilityBravo</code>: remove unused <code>using</code> statements. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3506">#3506</a>)</li>
<li><code>ERC20</code>: optimize <code>_transfer</code>, <code>_mint</code> and <code>_burn</code> by using <code>unchecked</code> arithmetic when possible. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3513">#3513</a>)</li>
<li><code>ERC20Votes</code>, <code>ERC721Votes</code>: optimize <code>getPastVotes</code> for looking up recent checkpoints. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3673">#3673</a>)</li>
<li><code>ERC20FlashMint</code>: add an internal <code>_flashFee</code> function for overriding. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3551">#3551</a>)</li>
<li><code>ERC4626</code>: use the same <code>decimals()</code> as the underlying asset by default (if available). (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3639">#3639</a>)</li>
<li><code>ERC4626</code>: add internal <code>_initialConvertToShares</code> and <code>_initialConvertToAssets</code> functions to customize empty vaults behavior. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3639">#3639</a>)</li>
<li><code>ERC721</code>: optimize transfers by making approval clearing implicit instead of emitting an event. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3481">#3481</a>)</li>
<li><code>ERC721</code>: optimize burn by making approval clearing implicit instead of emitting an event. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3538">#3538</a>)</li>
<li><code>ERC721</code>: Fix balance accounting when a custom <code>_beforeTokenTransfer</code> hook results in a transfer of the token under consideration. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3611">#3611</a>)</li>
<li><code>ERC721</code>: use unchecked arithmetic for balance updates. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3524">#3524</a>)</li>
<li><code>ERC721Consecutive</code>: Implementation of EIP-2309 that allows batch minting of ERC721 tokens during construction. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3311">#3311</a>)</li>
<li><code>ReentrancyGuard</code>: Reduce code size impact of the modifier by using internal functions. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3515">#3515</a>)</li>
<li><code>SafeCast</code>: optimize downcasting of signed integers. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3565">#3565</a>)</li>
<li><code>ECDSA</code>: Remove redundant check on the <code>v</code> value. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3591">#3591</a>)</li>
<li><code>VestingWallet</code>: add <code>releasable</code> getters. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3580">#3580</a>)</li>
<li><code>VestingWallet</code>: remove unused library <code>Math.sol</code>. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3605">#3605</a>)</li>
<li><code>VestingWallet</code>: make constructor payable. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3665">#3665</a>)</li>
<li><code>Create2</code>: optimize address computation by using assembly instead of <code>abi.encodePacked</code>. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3600">#3600</a>)</li>
<li><code>Clones</code>: optimized the assembly to use only the scratch space during deployments, and optimized <code>predictDeterministicAddress</code> to use fewer operations. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3640">#3640</a>)</li>
<li><code>Checkpoints</code>: Use procedural generation to support multiple key/value lengths. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3589">#3589</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/blob/v4.8.3/CHANGELOG.md"><code>@​openzeppelin/contracts</code>'s changelog</a>.</em></p>
<blockquote>
<h2>4.8.3 (2023-04-13)</h2>
<ul>
<li><code>GovernorCompatibilityBravo</code>: Fix encoding of proposal data when signatures are missing.</li>
<li><code>TransparentUpgradeableProxy</code>: Fix transparency in case of selector clash with non-decodable calldata or payable mutability. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4154">#4154</a>)</li>
</ul>
<h2>4.8.2 (2023-03-02)</h2>
<ul>
<li><code>ERC721Consecutive</code>: Fixed a bug when <code>_mintConsecutive</code> is used for batches of size 1 that could lead to balance overflow. Refer to the breaking changes section in the changelog for a note on the behavior of <code>ERC721._beforeTokenTransfer</code>.</li>
</ul>
<h3>Breaking changes</h3>
<ul>
<li><code>ERC721</code>: The internal function <code>_beforeTokenTransfer</code> no longer updates balances, which it previously did when <code>batchSize</code> was greater than 1. This change has no consequence unless a custom ERC721 extension is explicitly invoking <code>_beforeTokenTransfer</code>. Balance updates in extensions must now be done explicitly using <code>__unsafe_increaseBalance</code>, with a name that indicates that there is an invariant that has to be manually verified.</li>
</ul>
<h2>4.8.1 (2023-01-13)</h2>
<ul>
<li><code>ERC4626</code>: Use staticcall instead of call when fetching underlying ERC-20 decimals. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3943">#3943</a>)</li>
</ul>
<h2>4.8.0 (2022-11-08)</h2>
<ul>
<li><code>TimelockController</code>: Added a new <code>admin</code> constructor parameter that is assigned the admin role instead of the deployer account. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3722">#3722</a>)</li>
<li><code>Initializable</code>: add internal functions <code>_getInitializedVersion</code> and <code>_isInitializing</code> (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3598">#3598</a>)</li>
<li><code>ERC165Checker</code>: add <code>supportsERC165InterfaceUnchecked</code> for consulting individual interfaces without the full ERC165 protocol. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3339">#3339</a>)</li>
<li><code>Address</code>: optimize <code>functionCall</code> by calling <code>functionCallWithValue</code> directly. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3468">#3468</a>)</li>
<li><code>Address</code>: optimize <code>functionCall</code> functions by checking contract size only if there is no returned data. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3469">#3469</a>)</li>
<li><code>Governor</code>: make the <code>relay</code> function payable, and add support for EOA payments. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3730">#3730</a>)</li>
<li><code>GovernorCompatibilityBravo</code>: remove unused <code>using</code> statements. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3506">#3506</a>)</li>
<li><code>ERC20</code>: optimize <code>_transfer</code>, <code>_mint</code> and <code>_burn</code> by using <code>unchecked</code> arithmetic when possible. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3513">#3513</a>)</li>
<li><code>ERC20Votes</code>, <code>ERC721Votes</code>: optimize <code>getPastVotes</code> for looking up recent checkpoints. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3673">#3673</a>)</li>
<li><code>ERC20FlashMint</code>: add an internal <code>_flashFee</code> function for overriding. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3551">#3551</a>)</li>
<li><code>ERC4626</code>: use the same <code>decimals()</code> as the underlying asset by default (if available). (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3639">#3639</a>)</li>
<li><code>ERC4626</code>: add internal <code>_initialConvertToShares</code> and <code>_initialConvertToAssets</code> functions to customize empty vaults behavior. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3639">#3639</a>)</li>
<li><code>ERC721</code>: optimize transfers by making approval clearing implicit instead of emitting an event. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3481">#3481</a>)</li>
<li><code>ERC721</code>: optimize burn by making approval clearing implicit instead of emitting an event. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3538">#3538</a>)</li>
<li><code>ERC721</code>: Fix balance accounting when a custom <code>_beforeTokenTransfer</code> hook results in a transfer of the token under consideration. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3611">#3611</a>)</li>
<li><code>ERC721</code>: use unchecked arithmetic for balance updates. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3524">#3524</a>)</li>
<li><code>ERC721Consecutive</code>: Implementation of EIP-2309 that allows batch minting of ERC721 tokens during construction. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3311">#3311</a>)</li>
<li><code>ReentrancyGuard</code>: Reduce code size impact of the modifier by using internal functions. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3515">#3515</a>)</li>
<li><code>SafeCast</code>: optimize downcasting of signed integers. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3565">#3565</a>)</li>
<li><code>ECDSA</code>: Remove redundant check on the <code>v</code> value. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3591">#3591</a>)</li>
<li><code>VestingWallet</code>: add <code>releasable</code> getters. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3580">#3580</a>)</li>
<li><code>VestingWallet</code>: remove unused library <code>Math.sol</code>. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3605">#3605</a>)</li>
<li><code>VestingWallet</code>: make constructor payable. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3665">#3665</a>)</li>
<li><code>Create2</code>: optimize address computation by using assembly instead of <code>abi.encodePacked</code>. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3600">#3600</a>)</li>
<li><code>Clones</code>: optimized the assembly to use only the scratch space during deployments, and optimized <code>predictDeterministicAddress</code> to use fewer operations. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3640">#3640</a>)</li>
<li><code>Checkpoints</code>: Use procedural generation to support multiple key/value lengths. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3589">#3589</a>)</li>
<li><code>Checkpoints</code>: Add new lookup mechanisms. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3589">#3589</a>)</li>
<li><code>Arrays</code>: Add <code>unsafeAccess</code> functions that allow reading and writing to an element in a storage array bypassing Solidity's &quot;out-of-bounds&quot; check. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3589">#3589</a>)</li>
<li><code>Strings</code>: optimize <code>toString</code>. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3573">#3573</a>)</li>
<li><code>Ownable2Step</code>: extension of <code>Ownable</code> that makes the ownership transfers a two step process. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3620">#3620</a>)</li>
<li><code>Math</code> and <code>SignedMath</code>: optimize function <code>max</code> by using <code>&gt;</code> instead of <code>&gt;=</code>. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3679">#3679</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/0a25c1940ca220686588c4af3ec526f725fe2582"><code>0a25c19</code></a> 4.8.3</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/7bdd255a0594b5fd907a364c177cc2fea401332c"><code>7bdd255</code></a> Update changelog</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/ea595f59605534945a3d349a2f86a26fc7d3b9d1"><code>ea595f5</code></a> Merge pull request from GHSA-93hq-5wgc-jc82</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/61b45a28500e6996fc980c1101b9e0d321f80243"><code>61b45a2</code></a> Improve docs for transparent proxy (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4181">#4181</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/db9ee953a17166a51fff42b3c4a29203ef92a492"><code>db9ee95</code></a> Merge changesets for transparency improvements (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4165">#4165</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/c01ea99123a9be7494557b6b2ca5942c6be487f9"><code>c01ea99</code></a> Fix TransparentUpgradeableProxy's transparency (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4154">#4154</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/8dfeb5d79e6a31dce4ddcd6983db0e0456a02cf2"><code>8dfeb5d</code></a> Improve TransparentUpgradeableProxy's transparency (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/3977">#3977</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/9eee01c5a2757fa9bf8421a2810776b885995d2f"><code>9eee01c</code></a> Bump and pin Forge Std submodule (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4102">#4102</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/d00acef4059807535af0bd0dd0ddf619747a044b"><code>d00acef</code></a> 4.8.2</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/ab9cc4c4dbdd3be4a2e0935a76c160b31fb9deba"><code>ab9cc4c</code></a> Ignore reentrancy in<code>executeBatch</code> and update Slither config (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/3955">#3955</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/compare/v4.7.3...v4.8.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts&package-manager=npm_and_yarn&previous-version=4.7.3&new-version=4.8.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-17 17:16:39 +0000 UTC
    </div>
</div>

