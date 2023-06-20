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
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/682" class=".btn">#682</a>
            </td>
            <td>
                <b>
                    Bump @openzeppelin/contracts from 4.7.3 to 4.9.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) from 4.7.3 to 4.9.2.
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
<li>Additional commits viewable in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/compare/v4.7.3...v4.9.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts&package-manager=npm_and_yarn&previous-version=4.7.3&new-version=4.9.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-06-19 19:51:22 +0000 UTC
    </div>
</div>

