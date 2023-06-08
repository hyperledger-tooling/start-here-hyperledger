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
                PR <a href="https://github.com/hyperledger/cacti/pull/2444" class=".btn">#2444</a>
            </td>
            <td>
                <b>
                    build(deps): bump @openzeppelin/contracts-upgradeable from 4.8.3 to 4.9.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts-upgradeable](https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable) from 4.8.3 to 4.9.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/releases"><code>@​openzeppelin/contracts-upgradeable</code>'s releases</a>.</em></p>
<blockquote>
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
<ul>
<li><code>EIP712</code>: Addition of ERC5267 support requires support for user defined value types, which was released in Solidity version 0.8.8. This requires a pragma change from <code>^0.8.0</code> to <code>^0.8.8</code>.</li>
<li><code>EIP712</code>: Optimization of the cache for the upgradeable version affects the way <code>name</code> and <code>version</code> are set. This is no longer done through an initializer, and is instead part of the implementation's constructor. As a consequence, all proxies using the same implementation will necessarily share the same <code>name</code> and <code>version</code>. Additionally, an implementation upgrade risks changing the EIP712 domain unless the same <code>name</code> and <code>version</code> are used when deploying the new implementation contract.</li>
</ul>
<h3>Deprecations</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/blob/v4.9.1/CHANGELOG.md"><code>@​openzeppelin/contracts-upgradeable</code>'s changelog</a>.</em></p>
<blockquote>
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
<h3>Deprecations</h3>
<ul>
<li><code>ERC20Permit</code>: Added the file <code>IERC20Permit.sol</code> and <code>ERC20Permit.sol</code> and deprecated <code>draft-IERC20Permit.sol</code> and <code>draft-ERC20Permit.sol</code> since <a href="https://eips.ethereum.org/EIPS/eip-2612">EIP-2612</a> is no longer a Draft. Developers are encouraged to update their imports. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/3793">#3793</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/43b82754979c35abcd3ccad7b795754146c62ade"><code>43b8275</code></a> Transpile 281550b7</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/66f390fa516b550838e2c2f65132b5bc2afe1ced"><code>66f390f</code></a> Transpile 33ff9b08</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/b9fcc0867e45d2c1e75d8006fb08f20770d0285a"><code>b9fcc08</code></a> Transpile fa3a30a5</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/217c313f0cd908cbc31705168db58bf0a79c4e57"><code>217c313</code></a> Transpile 4e6deb3c</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/8b8c14a3436ac2096883d67376c14f5624083019"><code>8b8c14a</code></a> Transpile 81982051</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/bd21439257be2545e48aee9b9e329bc0bf909d99"><code>bd21439</code></a> Transpile a6e26716</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/f6febd79e2a3a17e26969dd0d450c6ebd64bf459"><code>f6febd7</code></a> Transpile 54b3f143</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/d3140631f50060d9627930484e4e299543494d15"><code>d314063</code></a> Transpile 4f7047ce</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/9a630c3f05ec1058cd7f5d6a6d6131dffeded423"><code>9a630c3</code></a> Transpile a43069e8</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/53f4295fb044136fad1ba863104e35b3131b644f"><code>53f4295</code></a> Transpile e0fe9367</li>
<li>Additional commits viewable in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/compare/v4.8.3...v4.9.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts-upgradeable&package-manager=npm_and_yarn&previous-version=4.8.3&new-version=4.9.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-08 18:12:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2443" class=".btn">#2443</a>
            </td>
            <td>
                <b>
                    chore(besu): remove web3-eea typings file 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes hyperledger#1218

Signed-off-by: micoferdinand98 <ferdinand.m.b.mico@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 07:36:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2442" class=".btn">#2442</a>
            </td>
            <td>
                <b>
                    test: fix path of and name of RIFUtil.test.ts #1515
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changed name of `RIFUtil.test.ts` to `rifUtil.test.ts` and moved the file to unit test directory.

fixes: #1515
Signed-off-by: Arnab Nandi <arnabnandi2002@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-03 08:01:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2441" class=".btn">#2441</a>
            </td>
            <td>
                <b>
                    build(deps): bump cryptography from 39.0.1 to 41.0.0 in /packages-python/cactus_validator_socketio_indy/validator-python
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [cryptography](https://github.com/pyca/cryptography) from 39.0.1 to 41.0.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pyca/cryptography/blob/main/CHANGELOG.rst">cryptography's changelog</a>.</em></p>
<blockquote>
<p>41.0.0 - 2023-05-30</p>
<pre><code>
* **BACKWARDS INCOMPATIBLE:** Support for OpenSSL less than 1.1.1d has been
  removed.  Users on older version of OpenSSL will need to upgrade.
* **BACKWARDS INCOMPATIBLE:** Support for Python 3.6 has been removed.
* **BACKWARDS INCOMPATIBLE:** Dropped support for LibreSSL &lt; 3.6.
* Updated the minimum supported Rust version (MSRV) to 1.56.0, from 1.48.0.
* Updated Windows, macOS, and Linux wheels to be compiled with OpenSSL 3.1.1.
* Added support for the :class:`~cryptography.x509.OCSPAcceptableResponses`
  OCSP extension.
* Added support for the :class:`~cryptography.x509.MSCertificateTemplate`
  proprietary Microsoft certificate extension.
* Implemented support for equality checks on all asymmetric public key types.
* Added support for ``aes256-gcm@openssh.com`` encrypted keys in
  :func:`~cryptography.hazmat.primitives.serialization.load_ssh_private_key`.
* Added support for obtaining X.509 certificate signature algorithm parameters
  (including PSS) via
  :meth:`~cryptography.x509.Certificate.signature_algorithm_parameters`.
* Support signing :class:`~cryptography.hazmat.primitives.asymmetric.padding.PSS`
  X.509 certificates via the new keyword-only argument ``rsa_padding`` on
  :meth:`~cryptography.x509.CertificateBuilder.sign`.
* Added support for
  :class:`~cryptography.hazmat.primitives.ciphers.aead.ChaCha20Poly1305`
  on BoringSSL.
<p>.. _v40-0-2:</p>
<p>40.0.2 - 2023-04-14
</code></pre></p>
<ul>
<li>Fixed compilation when using LibreSSL 3.7.2.</li>
<li>Added some functions to support an upcoming <code>pyOpenSSL</code> release.</li>
</ul>
<p>.. _v40-0-1:</p>
<p>40.0.1 - 2023-03-24</p>
<pre><code>
* Fixed a bug where certain operations would fail if an object happened to be
  in the top-half of the memory-space. This only impacted 32-bit systems.
<p>.. _v40-0-0:</p>
<p>40.0.0 - 2023-03-24
</code></pre></p>
<ul>
<li><strong>BACKWARDS INCOMPATIBLE:</strong> As announced in the 39.0.0 changelog, the way
<code>cryptography</code> links OpenSSL has changed. This only impacts users who</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pyca/cryptography/commit/c4d494fd3ee907316bd846e90cbf4a8df75a25ac"><code>c4d494f</code></a> 41.0.0 version bump (<a href="https://redirect.github.com/pyca/cryptography/issues/8991">#8991</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/8708245ccdeaff21d65eea68a4f8d2a7c5949a22"><code>8708245</code></a> new openssl day (<a href="https://redirect.github.com/pyca/cryptography/issues/8990">#8990</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/31436a486661cd863d4c77e40facf93fbb2d9f54"><code>31436a4</code></a> admit to the existence of nuance in HKDF (<a href="https://redirect.github.com/pyca/cryptography/issues/8987">#8987</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/91e41898e6d1d2a9a6e980c39e2f8baa2fa8a1f8"><code>91e4189</code></a> Port DSA to Rust (<a href="https://redirect.github.com/pyca/cryptography/issues/8978">#8978</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/f302d28b81607aab28d22b653da78d564824f267"><code>f302d28</code></a> Update CI for new LibreSSL releases (<a href="https://redirect.github.com/pyca/cryptography/issues/8975">#8975</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/851d8ccb340bfc93c827b9e80af939a216b34925"><code>851d8cc</code></a> Bump openssl from 0.10.52 to 0.10.53 in /src/rust (<a href="https://redirect.github.com/pyca/cryptography/issues/8986">#8986</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/0918c7236c94c29272e0790ba0227cfa9401943b"><code>0918c72</code></a> Bump coverage from 7.2.6 to 7.2.7 (<a href="https://redirect.github.com/pyca/cryptography/issues/8985">#8985</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/730a5ce11a91f40c1bb0f881ab22bc52d6cecef6"><code>730a5ce</code></a> Bump openssl-sys from 0.9.87 to 0.9.88 in /src/rust (<a href="https://redirect.github.com/pyca/cryptography/issues/8984">#8984</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/88e8c288975709228005e70301644034463d9823"><code>88e8c28</code></a> Bump BoringSSL and/or OpenSSL in CI (<a href="https://redirect.github.com/pyca/cryptography/issues/8983">#8983</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/3e24e44527a69884ca0c3247e1b5e9c8bbf590c9"><code>3e24e44</code></a> Bump once_cell from 1.17.1 to 1.17.2 in /src/rust (<a href="https://redirect.github.com/pyca/cryptography/issues/8982">#8982</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pyca/cryptography/compare/39.0.1...41.0.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cryptography&package-manager=pip&previous-version=39.0.1&new-version=41.0.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-02 20:18:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2440" class=".btn">#2440</a>
            </td>
            <td>
                <b>
                    build(deps): bump cryptography from 39.0.1 to 41.0.0 in /packages-python/cactus_validator_socketio_indy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [cryptography](https://github.com/pyca/cryptography) from 39.0.1 to 41.0.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pyca/cryptography/blob/main/CHANGELOG.rst">cryptography's changelog</a>.</em></p>
<blockquote>
<p>41.0.0 - 2023-05-30</p>
<pre><code>
* **BACKWARDS INCOMPATIBLE:** Support for OpenSSL less than 1.1.1d has been
  removed.  Users on older version of OpenSSL will need to upgrade.
* **BACKWARDS INCOMPATIBLE:** Support for Python 3.6 has been removed.
* **BACKWARDS INCOMPATIBLE:** Dropped support for LibreSSL &lt; 3.6.
* Updated the minimum supported Rust version (MSRV) to 1.56.0, from 1.48.0.
* Updated Windows, macOS, and Linux wheels to be compiled with OpenSSL 3.1.1.
* Added support for the :class:`~cryptography.x509.OCSPAcceptableResponses`
  OCSP extension.
* Added support for the :class:`~cryptography.x509.MSCertificateTemplate`
  proprietary Microsoft certificate extension.
* Implemented support for equality checks on all asymmetric public key types.
* Added support for ``aes256-gcm@openssh.com`` encrypted keys in
  :func:`~cryptography.hazmat.primitives.serialization.load_ssh_private_key`.
* Added support for obtaining X.509 certificate signature algorithm parameters
  (including PSS) via
  :meth:`~cryptography.x509.Certificate.signature_algorithm_parameters`.
* Support signing :class:`~cryptography.hazmat.primitives.asymmetric.padding.PSS`
  X.509 certificates via the new keyword-only argument ``rsa_padding`` on
  :meth:`~cryptography.x509.CertificateBuilder.sign`.
* Added support for
  :class:`~cryptography.hazmat.primitives.ciphers.aead.ChaCha20Poly1305`
  on BoringSSL.
<p>.. _v40-0-2:</p>
<p>40.0.2 - 2023-04-14
</code></pre></p>
<ul>
<li>Fixed compilation when using LibreSSL 3.7.2.</li>
<li>Added some functions to support an upcoming <code>pyOpenSSL</code> release.</li>
</ul>
<p>.. _v40-0-1:</p>
<p>40.0.1 - 2023-03-24</p>
<pre><code>
* Fixed a bug where certain operations would fail if an object happened to be
  in the top-half of the memory-space. This only impacted 32-bit systems.
<p>.. _v40-0-0:</p>
<p>40.0.0 - 2023-03-24
</code></pre></p>
<ul>
<li><strong>BACKWARDS INCOMPATIBLE:</strong> As announced in the 39.0.0 changelog, the way
<code>cryptography</code> links OpenSSL has changed. This only impacts users who</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pyca/cryptography/commit/c4d494fd3ee907316bd846e90cbf4a8df75a25ac"><code>c4d494f</code></a> 41.0.0 version bump (<a href="https://redirect.github.com/pyca/cryptography/issues/8991">#8991</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/8708245ccdeaff21d65eea68a4f8d2a7c5949a22"><code>8708245</code></a> new openssl day (<a href="https://redirect.github.com/pyca/cryptography/issues/8990">#8990</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/31436a486661cd863d4c77e40facf93fbb2d9f54"><code>31436a4</code></a> admit to the existence of nuance in HKDF (<a href="https://redirect.github.com/pyca/cryptography/issues/8987">#8987</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/91e41898e6d1d2a9a6e980c39e2f8baa2fa8a1f8"><code>91e4189</code></a> Port DSA to Rust (<a href="https://redirect.github.com/pyca/cryptography/issues/8978">#8978</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/f302d28b81607aab28d22b653da78d564824f267"><code>f302d28</code></a> Update CI for new LibreSSL releases (<a href="https://redirect.github.com/pyca/cryptography/issues/8975">#8975</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/851d8ccb340bfc93c827b9e80af939a216b34925"><code>851d8cc</code></a> Bump openssl from 0.10.52 to 0.10.53 in /src/rust (<a href="https://redirect.github.com/pyca/cryptography/issues/8986">#8986</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/0918c7236c94c29272e0790ba0227cfa9401943b"><code>0918c72</code></a> Bump coverage from 7.2.6 to 7.2.7 (<a href="https://redirect.github.com/pyca/cryptography/issues/8985">#8985</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/730a5ce11a91f40c1bb0f881ab22bc52d6cecef6"><code>730a5ce</code></a> Bump openssl-sys from 0.9.87 to 0.9.88 in /src/rust (<a href="https://redirect.github.com/pyca/cryptography/issues/8984">#8984</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/88e8c288975709228005e70301644034463d9823"><code>88e8c28</code></a> Bump BoringSSL and/or OpenSSL in CI (<a href="https://redirect.github.com/pyca/cryptography/issues/8983">#8983</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/3e24e44527a69884ca0c3247e1b5e9c8bbf590c9"><code>3e24e44</code></a> Bump once_cell from 1.17.1 to 1.17.2 in /src/rust (<a href="https://redirect.github.com/pyca/cryptography/issues/8982">#8982</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pyca/cryptography/compare/39.0.1...41.0.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cryptography&package-manager=pip&previous-version=39.0.1&new-version=41.0.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-02 20:18:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2439" class=".btn">#2439</a>
            </td>
            <td>
                <b>
                    style: changes made for fixing #1357
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                submitting fixes for issue #1357 minus the linter warning ID 79 and 80 as they have been already solved in batch 9 #1478.
I have added types of variables and objects wherever necessary in place of 'any' and for packages/cactus-common/src/test/typescript/unit/logging/logger.test.ts I have declared a interface for prototyping the stdOutDataHandler function.

fixes #1357
Signed-off-by: Arnab Nandi arnabnandi2002@gmail.com
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-02 15:22:24 +0000 UTC
    </div>
</div>

