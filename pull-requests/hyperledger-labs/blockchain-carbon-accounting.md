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
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/375" class=".btn">#375</a>
            </td>
            <td>
                <b>
                    build(deps): bump @openzeppelin/contracts from 3.3.0 to 4.4.1 in /net-emissions-token-network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) from 3.3.0 to 4.4.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/releases"><code>@​openzeppelin/contracts</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.4.1</h2>
<p>:warning: This is a patch for a low severity vulnerability. For more information <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-9c22-pwxw-p6hx">visit the security advisory</a>.</p>
<ul>
<li><code>Initializable</code>: change the existing <code>initializer</code> modifier and add a new <code>onlyInitializing</code> modifier to prevent reentrancy risk. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3006">#3006</a>)</li>
</ul>
<h3>Breaking change</h3>
<p>It is no longer possible to call an <code>initializer</code>-protected function from within another <code>initializer</code> function outside the context of a constructor. Projects using OpenZeppelin upgradeable proxies should continue to work as is, since in the common case the initializer is invoked in the constructor directly. If this is not the case for you, the suggested change is to use the new <code>onlyInitializing</code> modifier in the following way:</p>
<pre lang="diff"><code> contract A {
-    function initialize() public   initializer { ... }
+    function initialize() internal onlyInitializing { ... }
 }
 contract B is A {
     function initialize() public initializer {
         A.initialize();
     }
 }
</code></pre>
<h2>v4.4.0</h2>
<p>Check out the first <a href="https://www.youtube.com/watch?v=ed96DWbfliQ"><strong>OpenZeppelin Community Call</strong></a> where the team discussed everything that is included in this release.</p>
<p>And if you missed it, we recently announced an official <strong>bug bounty program</strong> for OpenZeppelin Contracts. <a href="https://forum.openzeppelin.com/t/openzeppelin-contracts-bug-bounty-program-on-immunefi/19279">Check it out!</a></p>
<ul>
<li><code>Ownable</code>: add an internal <code>_transferOwnership(address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2568">#2568</a>)</li>
<li><code>AccessControl</code>: add internal <code>_grantRole(bytes32,address)</code> and <code>_revokeRole(bytes32,address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2568">#2568</a>)</li>
<li><code>AccessControl</code>: mark <code>_setupRole(bytes32,address)</code> as deprecated in favor of <code>_grantRole(bytes32,address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2568">#2568</a>)</li>
<li><code>AccessControlEnumerable</code>: hook into <code>_grantRole(bytes32,address)</code> and <code>_revokeRole(bytes32,address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2946">#2946</a>)</li>
<li><code>EIP712</code>: cache <code>address(this)</code> to immutable storage to avoid potential issues if a vanilla contract is used in a delegatecall context. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2852">#2852</a>)</li>
<li>Add internal <code>_setApprovalForAll</code> to <code>ERC721</code> and <code>ERC1155</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2834">#2834</a>)</li>
<li><code>Governor</code>: shift vote start and end by one block to better match Compound's GovernorBravo and prevent voting at the Governor level if the voting snapshot is not ready. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2892">#2892</a>)</li>
<li><code>GovernorCompatibilityBravo</code>: consider quorum an inclusive rather than exclusive minimum to match Compound's GovernorBravo. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2974">#2974</a>)</li>
<li><code>GovernorSettings</code>: a new governor module that manages voting settings updatable through governance actions. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2904">#2904</a>)</li>
<li><code>PaymentSplitter</code>: now supports ERC20 assets in addition to Ether. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2858">#2858</a>)</li>
<li><code>ECDSA</code>: add a variant of <code>toEthSignedMessageHash</code> for arbitrary length message hashing. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2865">#2865</a>)</li>
<li><code>MerkleProof</code>: add a <code>processProof</code> function that returns the rebuilt root hash given a leaf and a proof. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2841">#2841</a>)</li>
<li><code>VestingWallet</code>: new contract that handles the vesting of Ether and ERC20 tokens following a customizable vesting schedule. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2748">#2748</a>)</li>
<li><code>Governor</code>: enable receiving Ether when a Timelock contract is not used. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2849">#2748</a>)</li>
<li><code>GovernorTimelockCompound</code>: fix ability to use Ether stored in the Timelock contract. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2849">#2748</a>)</li>
</ul>
<h2>v4.3.3</h2>
<p>:warning: This is a security patch. For more information visit the <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-wmpv-c2jp-j2xg">security advisory</a>.</p>
<ul>
<li><code>ERC1155Supply</code>: Handle <code>totalSupply</code> changes by hooking into <code>_beforeTokenTransfer</code> to ensure consistency of balances and supply during <code>IERC1155Receiver.onERC1155Received</code> calls.</li>
</ul>
<h2>v4.3.2</h2>
<p>:warning: This is a security patch. For more information visit the <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-5vp3-v4hc-gx76">security advisory</a>.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/CHANGELOG.md"><code>@​openzeppelin/contracts</code>'s changelog</a>.</em></p>
<blockquote>
<h2>4.4.1 (2021-12-14)</h2>
<ul>
<li><code>Initializable</code>: change the existing <code>initializer</code> modifier and add a new <code>onlyInitializing</code> modifier to prevent reentrancy risk. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3006">#3006</a>)</li>
</ul>
<h3>Breaking change</h3>
<p>It is no longer possible to call an <code>initializer</code>-protected function from within another <code>initializer</code> function outside the context of a constructor. Projects using OpenZeppelin upgradeable proxies should continue to work as is, since in the common case the initializer is invoked in the constructor directly. If this is not the case for you, the suggested change is to use the new <code>onlyInitializing</code> modifier in the following way:</p>
<pre lang="diff"><code> contract A {
-    function initialize() public   initializer { ... }
+    function initialize() internal onlyInitializing { ... }
 }
 contract B is A {
     function initialize() public initializer {
         A.initialize();
     }
 }
</code></pre>
<h2>4.4.0 (2021-11-25)</h2>
<ul>
<li><code>Ownable</code>: add an internal <code>_transferOwnership(address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2568">#2568</a>)</li>
<li><code>AccessControl</code>: add internal <code>_grantRole(bytes32,address)</code> and <code>_revokeRole(bytes32,address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2568">#2568</a>)</li>
<li><code>AccessControl</code>: mark <code>_setupRole(bytes32,address)</code> as deprecated in favor of <code>_grantRole(bytes32,address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2568">#2568</a>)</li>
<li><code>AccessControlEnumerable</code>: hook into <code>_grantRole(bytes32,address)</code> and <code>_revokeRole(bytes32,address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2946">#2946</a>)</li>
<li><code>EIP712</code>: cache <code>address(this)</code> to immutable storage to avoid potential issues if a vanilla contract is used in a delegatecall context. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2852">#2852</a>)</li>
<li>Add internal <code>_setApprovalForAll</code> to <code>ERC721</code> and <code>ERC1155</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2834">#2834</a>)</li>
<li><code>Governor</code>: shift vote start and end by one block to better match Compound's GovernorBravo and prevent voting at the Governor level if the voting snapshot is not ready. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2892">#2892</a>)</li>
<li><code>GovernorCompatibilityBravo</code>: consider quorum an inclusive rather than exclusive minimum to match Compound's GovernorBravo. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2974">#2974</a>)</li>
<li><code>GovernorSettings</code>: a new governor module that manages voting settings updatable through governance actions. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2904">#2904</a>)</li>
<li><code>PaymentSplitter</code>: now supports ERC20 assets in addition to Ether. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2858">#2858</a>)</li>
<li><code>ECDSA</code>: add a variant of <code>toEthSignedMessageHash</code> for arbitrary length message hashing. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2865">#2865</a>)</li>
<li><code>MerkleProof</code>: add a <code>processProof</code> function that returns the rebuilt root hash given a leaf and a proof. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2841">#2841</a>)</li>
<li><code>VestingWallet</code>: new contract that handles the vesting of Ether and ERC20 tokens following a customizable vesting schedule. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2748">#2748</a>)</li>
<li><code>Governor</code>: enable receiving Ether when a Timelock contract is not used. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2849">#2748</a>)</li>
<li><code>GovernorTimelockCompound</code>: fix ability to use Ether stored in the Timelock contract. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2849">#2748</a>)</li>
</ul>
<h2>4.3.3</h2>
<ul>
<li><code>ERC1155Supply</code>: Handle <code>totalSupply</code> changes by hooking into <code>_beforeTokenTransfer</code> to ensure consistency of balances and supply during <code>IERC1155Receiver.onERC1155Received</code> calls.</li>
</ul>
<h2>4.3.2 (2021-09-14)</h2>
<ul>
<li><code>UUPSUpgradeable</code>: Add modifiers to prevent <code>upgradeTo</code> and <code>upgradeToAndCall</code> being executed on any contract that is not the active ERC1967 proxy. This prevents these functions being called on implementation contracts or minimal ERC1167 clones, in particular.</li>
</ul>
<h2>4.3.1 (2021-08-26)</h2>
<ul>
<li><code>TimelockController</code>: Add additional isOperationReady check.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/6bd6b76d1156e20e45d1016f355d154141c7e5b9"><code>6bd6b76</code></a> 4.4.1</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/13a6ec753a3e9c56a3d9dec845a9b5cbd616b658"><code>13a6ec7</code></a> Remove bad date from changelog</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/553c8fdec708ea10dd5f4a2977364af7a562566f"><code>553c8fd</code></a> Update initializer modifier to prevent reentrancy during initialization (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3006">#3006</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/4961a51cc736c7d4aa9bd2e11e4cbbaff73efee9"><code>4961a51</code></a> 4.4.0</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/94a0b8f573e0033d5338689030d2b721e4a5177a"><code>94a0b8f</code></a> Make VestingWallet token event argument indexed (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/2988">#2988</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/0413d58860e0253f30cd6d18c6caaf20ebb4de33"><code>0413d58</code></a> add bug bounty info</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/a4cee9ed37d5d406c1ae742d1cd4c3122f930ba5"><code>a4cee9e</code></a> make setters in GovernorSettings virtual</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/65ef662a2ba263b62de0f45b062c8942362ba8c8"><code>65ef662</code></a> 4.4.0-rc.1</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/8b8ee57a1a09656d7f10826c1dac7c8720d5b51c"><code>8b8ee57</code></a> Make quorum behavior match GovernorBravo (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/2974">#2974</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/cf6e32fc541b4436de7cec3e87aee684dff18bb5"><code>cf6e32f</code></a> Fix Timelock Controller description typo (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/2960">#2960</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/compare/v3.3.0...v4.4.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts&package-manager=npm_and_yarn&previous-version=3.3.0&new-version=4.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-14 22:02:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/374" class=".btn">#374</a>
            </td>
            <td>
                <b>
                    build(deps): bump @openzeppelin/contracts-upgradeable from 3.4.1 to 4.4.1 in /net-emissions-token-network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts-upgradeable](https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable) from 3.4.1 to 4.4.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/releases"><code>@​openzeppelin/contracts-upgradeable</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.4.1</h2>
<p>:warning: This is a patch for a low severity vulnerability. For more information <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-9c22-pwxw-p6hx">visit the security advisory</a>.</p>
<ul>
<li><code>Initializable</code>: change the existing <code>initializer</code> modifier and add a new <code>onlyInitializing</code> modifier to prevent reentrancy risk. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3006">#3006</a>)</li>
</ul>
<h3>Breaking change</h3>
<p>It is no longer possible to call an <code>initializer</code>-protected function from within another <code>initializer</code> function outside the context of a constructor. Projects using OpenZeppelin upgradeable proxies should continue to work as is, since in the common case the initializer is invoked in the constructor directly. If this is not the case for you, the suggested change is to use the new <code>onlyInitializing</code> modifier in the following way:</p>
<pre lang="diff"><code> contract A {
-    function initialize() public   initializer { ... }
+    function initialize() internal onlyInitializing { ... }
 }
 contract B is A {
     function initialize() public initializer {
         A.initialize();
     }
 }
</code></pre>
<h2>v4.4.0</h2>
<p>Check out the first <a href="https://www.youtube.com/watch?v=ed96DWbfliQ"><strong>OpenZeppelin Community Call</strong></a> where the team discussed everything that is included in this release.</p>
<p>And if you missed it, we recently announced an official <strong>bug bounty program</strong> for OpenZeppelin Contracts. <a href="https://forum.openzeppelin.com/t/openzeppelin-contracts-bug-bounty-program-on-immunefi/19279">Check it out!</a></p>
<ul>
<li><code>Ownable</code>: add an internal <code>_transferOwnership(address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2568">#2568</a>)</li>
<li><code>AccessControl</code>: add internal <code>_grantRole(bytes32,address)</code> and <code>_revokeRole(bytes32,address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2568">#2568</a>)</li>
<li><code>AccessControl</code>: mark <code>_setupRole(bytes32,address)</code> as deprecated in favor of <code>_grantRole(bytes32,address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2568">#2568</a>)</li>
<li><code>AccessControlEnumerable</code>: hook into <code>_grantRole(bytes32,address)</code> and <code>_revokeRole(bytes32,address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2946">#2946</a>)</li>
<li><code>EIP712</code>: cache <code>address(this)</code> to immutable storage to avoid potential issues if a vanilla contract is used in a delegatecall context. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2852">#2852</a>)</li>
<li>Add internal <code>_setApprovalForAll</code> to <code>ERC721</code> and <code>ERC1155</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2834">#2834</a>)</li>
<li><code>Governor</code>: shift vote start and end by one block to better match Compound's GovernorBravo and prevent voting at the Governor level if the voting snapshot is not ready. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2892">#2892</a>)</li>
<li><code>GovernorCompatibilityBravo</code>: consider quorum an inclusive rather than exclusive minimum to match Compound's GovernorBravo. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2974">#2974</a>)</li>
<li><code>GovernorSettings</code>: a new governor module that manages voting settings updatable through governance actions. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2904">#2904</a>)</li>
<li><code>PaymentSplitter</code>: now supports ERC20 assets in addition to Ether. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2858">#2858</a>)</li>
<li><code>ECDSA</code>: add a variant of <code>toEthSignedMessageHash</code> for arbitrary length message hashing. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2865">#2865</a>)</li>
<li><code>MerkleProof</code>: add a <code>processProof</code> function that returns the rebuilt root hash given a leaf and a proof. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2841">#2841</a>)</li>
<li><code>VestingWallet</code>: new contract that handles the vesting of Ether and ERC20 tokens following a customizable vesting schedule. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2748">#2748</a>)</li>
<li><code>Governor</code>: enable receiving Ether when a Timelock contract is not used. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2849">#2748</a>)</li>
<li><code>GovernorTimelockCompound</code>: fix ability to use Ether stored in the Timelock contract. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2849">#2748</a>)</li>
</ul>
<h2>v4.3.3</h2>
<p>:warning: This is a security patch. For more information visit the <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-wmpv-c2jp-j2xg">security advisory</a>.</p>
<ul>
<li><code>ERC1155Supply</code>: Handle <code>totalSupply</code> changes by hooking into <code>_beforeTokenTransfer</code> to ensure consistency of balances and supply during <code>IERC1155Receiver.onERC1155Received</code> calls.</li>
</ul>
<h2>v4.3.2</h2>
<p>:warning: This is a security patch. For more information visit the <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/security/advisories/GHSA-q4h9-46xg-m3x9">security advisory</a>.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/blob/master/CHANGELOG.md"><code>@​openzeppelin/contracts-upgradeable</code>'s changelog</a>.</em></p>
<blockquote>
<h2>4.4.1 (2021-12-10)</h2>
<ul>
<li><code>Initializable</code>: change the existing <code>initializer</code> modifier and add a new <code>onlyInitializing</code> modifier to prevent reentrancy risk. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3006">#3006</a>)</li>
</ul>
<h3>Breaking change</h3>
<p>It is no longer possible to call an <code>initializer</code>-protected function from within another <code>initializer</code> function outside the context of a constructor. Projects using OpenZeppelin upgradeable proxies should continue to work as is, since in the common case the initializer is invoked in the constructor directly. If this is not the case for you, the suggested change is to use the new <code>onlyInitializing</code> modifier in the following way:</p>
<pre lang="diff"><code> contract A {
-    function initialize() public   initializer { ... }
+    function initialize() internal onlyInitializing { ... }
 }
 contract B is A {
     function initialize() public initializer {
         A.initialize();
     }
 }
</code></pre>
<h2>4.4.0 (2021-11-25)</h2>
<ul>
<li><code>Ownable</code>: add an internal <code>_transferOwnership(address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2568">#2568</a>)</li>
<li><code>AccessControl</code>: add internal <code>_grantRole(bytes32,address)</code> and <code>_revokeRole(bytes32,address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2568">#2568</a>)</li>
<li><code>AccessControl</code>: mark <code>_setupRole(bytes32,address)</code> as deprecated in favor of <code>_grantRole(bytes32,address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2568">#2568</a>)</li>
<li><code>AccessControlEnumerable</code>: hook into <code>_grantRole(bytes32,address)</code> and <code>_revokeRole(bytes32,address)</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2946">#2946</a>)</li>
<li><code>EIP712</code>: cache <code>address(this)</code> to immutable storage to avoid potential issues if a vanilla contract is used in a delegatecall context. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2852">#2852</a>)</li>
<li>Add internal <code>_setApprovalForAll</code> to <code>ERC721</code> and <code>ERC1155</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2834">#2834</a>)</li>
<li><code>Governor</code>: shift vote start and end by one block to better match Compound's GovernorBravo and prevent voting at the Governor level if the voting snapshot is not ready. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2892">#2892</a>)</li>
<li><code>GovernorCompatibilityBravo</code>: consider quorum an inclusive rather than exclusive minimum to match Compound's GovernorBravo. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2974">#2974</a>)</li>
<li><code>GovernorSettings</code>: a new governor module that manages voting settings updatable through governance actions. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2904">#2904</a>)</li>
<li><code>PaymentSplitter</code>: now supports ERC20 assets in addition to Ether. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2858">#2858</a>)</li>
<li><code>ECDSA</code>: add a variant of <code>toEthSignedMessageHash</code> for arbitrary length message hashing. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2865">#2865</a>)</li>
<li><code>MerkleProof</code>: add a <code>processProof</code> function that returns the rebuilt root hash given a leaf and a proof. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2841">#2841</a>)</li>
<li><code>VestingWallet</code>: new contract that handles the vesting of Ether and ERC20 tokens following a customizable vesting schedule. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2748">#2748</a>)</li>
<li><code>Governor</code>: enable receiving Ether when a Timelock contract is not used. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2849">#2748</a>)</li>
<li><code>GovernorTimelockCompound</code>: fix ability to use Ether stored in the Timelock contract. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/2849">#2748</a>)</li>
</ul>
<h2>4.3.3</h2>
<ul>
<li><code>ERC1155Supply</code>: Handle <code>totalSupply</code> changes by hooking into <code>_beforeTokenTransfer</code> to ensure consistency of balances and supply during <code>IERC1155Receiver.onERC1155Received</code> calls.</li>
</ul>
<h2>4.3.2 (2021-09-14)</h2>
<ul>
<li><code>UUPSUpgradeable</code>: Add modifiers to prevent <code>upgradeTo</code> and <code>upgradeToAndCall</code> being executed on any contract that is not the active ERC1967 proxy. This prevents these functions being called on implementation contracts or minimal ERC1167 clones, in particular.</li>
</ul>
<h2>4.3.1 (2021-08-26)</h2>
<ul>
<li><code>TimelockController</code>: Add additional isOperationReady check.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commits/v4.4.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts-upgradeable&package-manager=npm_and_yarn&previous-version=3.4.1&new-version=4.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-14 22:01:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/373" class=".btn">#373</a>
            </td>
            <td>
                <b>
                    feat (test): Test if emission factors for the correct region are used
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR modifies the test setup script to insert emission factors for Germany, along with a utility identifier in the same region. Then, 2 emissions are recorded, one in the region of Germany, and the other in the US. Then we assert the following conditions:

- The emissions amounts of both years must not be equal
- The emissions amounts of each region should match the value calculated as per the emissions factors of that year
- In case of the emission recorded in Germany, the amounts of renewable and non-renewable energy must also match the values calculated as per the percent of renewables used in the region
- The emissions data is fetched from the CouchDB database using the HTTP /db/_find API. Then, the emissions factors are calculated and checked against the values stored on the ledger.

Closes #317.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 19:00:18 +0000 UTC
    </div>
</div>

