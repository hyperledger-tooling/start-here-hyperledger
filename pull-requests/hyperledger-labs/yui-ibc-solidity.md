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
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/201" class=".btn">#201</a>
            </td>
            <td>
                <b>
                    build(deps): bump @openzeppelin/contracts from 4.8.3 to 4.9.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) from 4.8.3 to 4.9.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/releases"><code>@​openzeppelin/contracts</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.9.3</h2>
<blockquote>
<p><strong>Note</strong>
This release contains a fix for <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-g4vp-m682-qqmp">GHSA-g4vp-m682-qqmp</a>.</p>
</blockquote>
<ul>
<li><code>ERC2771Context</code>: Return the forwarder address whenever the <code>msg.data</code> of a call originating from a trusted forwarder is not long enough to contain the request signer address (i.e. <code>msg.data.length</code> is less than 20 bytes), as specified by ERC-2771. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4481">#4481</a>)</li>
<li><code>ERC2771Context</code>: Prevent revert in <code>_msgData()</code> when a call originating from a trusted forwarder is not long enough to contain the request signer address (i.e. <code>msg.data.length</code> is less than 20 bytes). Return the full calldata in that case. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4484">#4484</a>)</li>
</ul>
<h2>v4.9.2</h2>
<blockquote>
<p><strong>Note</strong>
This release contains a fix for <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-wprv-93r4-jj2p">GHSA-wprv-93r4-jj2p</a>.</p>
</blockquote>
<ul>
<li><code>MerkleProof</code>: Fix a bug in <code>processMultiProof</code> and <code>processMultiProofCalldata</code> that allows proving arbitrary leaves if the tree contains a node with value 0 at depth 1.</li>
</ul>
<h2>v4.9.1</h2>
<blockquote>
<p><strong>Note</strong>
This release contains a fix for <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-5h3x-9wvq-w4m2">GHSA-5h3x-9wvq-w4m2</a>.</p>
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
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/blob/v4.9.3/CHANGELOG.md"><code>@​openzeppelin/contracts</code>'s changelog</a>.</em></p>
<blockquote>
<h2>4.9.3 (2023-07-28)</h2>
<ul>
<li><code>ERC2771Context</code>: Return the forwarder address whenever the <code>msg.data</code> of a call originating from a trusted forwarder is not long enough to contain the request signer address (i.e. <code>msg.data.length</code> is less than 20 bytes), as specified by ERC-2771. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4481">#4481</a>)</li>
<li><code>ERC2771Context</code>: Prevent revert in <code>_msgData()</code> when a call originating from a trusted forwarder is not long enough to contain the request signer address (i.e. <code>msg.data.length</code> is less than 20 bytes). Return the full calldata in that case. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4484">#4484</a>)</li>
</ul>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/fd81a96f01cc42ef1c9a5399364968d0e07e9e90"><code>fd81a96</code></a> Release v4.9.3 (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4482">#4482</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/70dea74ac7d969321d56cebdb96cf31cd9f1fb8a"><code>70dea74</code></a> Add changeset PR numbers</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/e4435eed757d4309436b1e06608e97b6d6e2fdb5"><code>e4435ee</code></a> Adjust ERC2771Context._msgData for msg.data.length &lt; 20 (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4484">#4484</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/7ec712baa50525353360a43700f953912bebef9c"><code>7ec712b</code></a> Make ERC2771Context return original sender address if <code>msg.data.length &lt;= 20</code>...</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/d26025b4103b8d053684a75129a16852d1ae95c0"><code>d26025b</code></a> Fix error when running hardhat test with parameters (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4265">#4265</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/a54f6398e5463081909e1d24248942c953b272a3"><code>a54f639</code></a> Update docs for <code>SafeERC20.forceApprove</code> (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4231">#4231</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/e50c24f5839db17f46991478384bfda14acfb830"><code>e50c24f</code></a> Release v4.9.2 (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4364">#4364</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/4d2383e17186be3e8ccf5a442e9686ecc7de1c55"><code>4d2383e</code></a> Merge pull request from GHSA-wprv-93r4-jj2p</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/f03420b5c77ae3cfa73fce4ffc7f4778cfa2b503"><code>f03420b</code></a> Remove automatic conflict resolution for merge from release branch (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4362">#4362</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/ded8c9eedb9a03b0703b65d430e6d0076cb0e444"><code>ded8c9e</code></a> Update index.adoc (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4336">#4336</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/compare/v4.8.3...v4.9.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts&package-manager=npm_and_yarn&previous-version=4.8.3&new-version=4.9.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-08-11 19:30:57 +0000 UTC
    </div>
</div>

