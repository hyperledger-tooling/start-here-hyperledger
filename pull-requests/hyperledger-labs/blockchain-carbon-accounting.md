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
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/588" class=".btn">#588</a>
            </td>
            <td>
                <b>
                    Bump @openzeppelin/contracts from 4.6.0 to 4.7.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) from 4.6.0 to 4.7.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/releases"><code>@​openzeppelin/contracts</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.7.1</h2>
<p>:warning: This is a patch for a medium severity issue affecting <code>SignatureChecker</code> and a high severity issue affecting <code>ERC165Checker</code>. For more information visit the security advisories (<a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-4g63-c64m-25w9">1</a>, <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-qh9x-gcfh-pcrw">2</a>).</p>
<ul>
<li><code>SignatureChecker</code>: Fix an issue that causes <code>isValidSignatureNow</code> to revert when the target contract returns ill-encoded data. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3552">#3552</a>)</li>
<li><code>ERC165Checker</code>: Fix an issue that causes <code>supportsInterface</code> to revert when the target contract returns ill-encoded data. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3552">#3552</a>)</li>
</ul>
<h2>v4.7.0</h2>
<ul>
<li><code>TimelockController</code>: Migrate <code>_call</code> to <code>_execute</code> and allow inheritance and overriding similar to <code>Governor</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3317">#3317</a>)</li>
<li><code>CrossChainEnabledPolygonChild</code>: replace the <code>require</code> statement with the custom error <code>NotCrossChainCall</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3380">#3380</a>)</li>
<li><code>ERC20FlashMint</code>: Add customizable flash fee receiver. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3327">#3327</a>)</li>
<li><code>ERC4626</code>: add an extension of <code>ERC20</code> that implements the ERC4626 Tokenized Vault Standard. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3171">#3171</a>)</li>
<li><code>SafeERC20</code>: add <code>safePermit</code> as mitigation against phantom permit functions. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3280">#3280</a>)</li>
<li><code>Math</code>: add a <code>mulDiv</code> function that can round the result either up or down. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3171">#3171</a>)</li>
<li><code>Math</code>: Add a <code>sqrt</code> function to compute square roots of integers, rounding either up or down. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3242">#3242</a>)</li>
<li><code>Strings</code>: add a new overloaded function <code>toHexString</code> that converts an <code>address</code> with fixed length of 20 bytes to its not checksummed ASCII <code>string</code> hexadecimal representation. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3403">#3403</a>)</li>
<li><code>EnumerableMap</code>: add new <code>UintToUintMap</code> map type. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3338">#3338</a>)</li>
<li><code>EnumerableMap</code>: add new <code>Bytes32ToUintMap</code> map type. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3416">#3416</a>)</li>
<li><code>SafeCast</code>: add support for many more types, using procedural code generation. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3245">#3245</a>)</li>
<li><code>MerkleProof</code>: add <code>multiProofVerify</code> to prove multiple values are part of a Merkle tree. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3276">#3276</a>)</li>
<li><code>MerkleProof</code>: add calldata versions of the functions to avoid copying input arrays to memory and save gas. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3200">#3200</a>)</li>
<li><code>ERC721</code>, <code>ERC1155</code>: simplified revert reasons. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3254">#3254</a>, (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3438">#3438</a>))</li>
<li><code>ERC721</code>: removed redundant require statement. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3434">#3434</a>)</li>
<li><code>PaymentSplitter</code>: add <code>releasable</code> getters. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3350">#3350</a>)</li>
<li><code>Initializable</code>: refactored implementation of modifiers for easier understanding. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3450">#3450</a>)</li>
<li><code>Proxies</code>: remove runtime check of ERC1967 storage slots. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3455">#3455</a>)</li>
</ul>
<h3>Breaking changes</h3>
<ul>
<li><code>Initializable</code>: functions decorated with the modifier <code>reinitializer(1)</code> may no longer invoke each other.</li>
</ul>
<h2>v4.7.0-rc.0</h2>
<p>This prerelease is now available for open review! Let us know your feedback and if you find any security issues.</p>
<p>We have a <a href="https://immunefi.com/bounty/openzeppelin/">bug bounty</a> with rewards of up to USD $25,000 and a special POAP for submitting a valid issue.</p>
<p>See the <a href="https://forum.openzeppelin.com/t/release-candidate-for-contracts-4-7-open-review-period/29443">announcement</a> for more details.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/CHANGELOG.md"><code>@​openzeppelin/contracts</code>'s changelog</a>.</em></p>
<blockquote>
<h2>4.7.1</h2>
<ul>
<li><code>SignatureChecker</code>: Fix an issue that causes <code>isValidSignatureNow</code> to revert when the target contract returns ill-encoded data. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3552">#3552</a>)</li>
<li><code>ERC165Checker</code>: Fix an issue that causes <code>supportsInterface</code> to revert when the target contract returns ill-encoded data. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3552">#3552</a>)</li>
</ul>
<h2>4.7.0 (2022-06-29)</h2>
<ul>
<li><code>TimelockController</code>: Migrate <code>_call</code> to <code>_execute</code> and allow inheritance and overriding similar to <code>Governor</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3317">#3317</a>)</li>
<li><code>CrossChainEnabledPolygonChild</code>: replace the <code>require</code> statement with the custom error <code>NotCrossChainCall</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3380">#3380</a>)</li>
<li><code>ERC20FlashMint</code>: Add customizable flash fee receiver. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3327">#3327</a>)</li>
<li><code>ERC4626</code>: add an extension of <code>ERC20</code> that implements the ERC4626 Tokenized Vault Standard. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3171">#3171</a>)</li>
<li><code>SafeERC20</code>: add <code>safePermit</code> as mitigation against phantom permit functions. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3280">#3280</a>)</li>
<li><code>Math</code>: add a <code>mulDiv</code> function that can round the result either up or down. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3171">#3171</a>)</li>
<li><code>Math</code>: Add a <code>sqrt</code> function to compute square roots of integers, rounding either up or down. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3242">#3242</a>)</li>
<li><code>Strings</code>: add a new overloaded function <code>toHexString</code> that converts an <code>address</code> with fixed length of 20 bytes to its not checksummed ASCII <code>string</code> hexadecimal representation. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3403">#3403</a>)</li>
<li><code>EnumerableMap</code>: add new <code>UintToUintMap</code> map type. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3338">#3338</a>)</li>
<li><code>EnumerableMap</code>: add new <code>Bytes32ToUintMap</code> map type. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3416">#3416</a>)</li>
<li><code>SafeCast</code>: add support for many more types, using procedural code generation. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3245">#3245</a>)</li>
<li><code>MerkleProof</code>: add <code>multiProofVerify</code> to prove multiple values are part of a Merkle tree. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3276">#3276</a>)</li>
<li><code>MerkleProof</code>: add calldata versions of the functions to avoid copying input arrays to memory and save gas. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3200">#3200</a>)</li>
<li><code>ERC721</code>, <code>ERC1155</code>: simplified revert reasons. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3254">#3254</a>, (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3438">#3438</a>))</li>
<li><code>ERC721</code>: removed redundant require statement. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3434">#3434</a>)</li>
<li><code>PaymentSplitter</code>: add <code>releasable</code> getters. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3350">#3350</a>)</li>
<li><code>Initializable</code>: refactored implementation of modifiers for easier understanding. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3450">#3450</a>)</li>
<li><code>Proxies</code>: remove runtime check of ERC1967 storage slots. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3455">#3455</a>)</li>
</ul>
<h3>Breaking changes</h3>
<ul>
<li><code>Initializable</code>: functions decorated with the modifier <code>reinitializer(1)</code> may no longer invoke each other.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/3b8b4ba82c880c31cd3b96dd5e15741d7e26658e"><code>3b8b4ba</code></a> 4.7.1</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/212de08e7f47b9836acca681ce0c9c6f91fe78aa"><code>212de08</code></a> Fix issues caused by abi.decode reverting (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3552">#3552</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/8c49ad74eae76ee389d038780d407cf90b4ae1de"><code>8c49ad7</code></a> 4.7.0</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/0b238a536d64b7e59d795747abb131e164de10a5"><code>0b238a5</code></a> Minor wording fixes <code>ERC4626</code> contract (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3510">#3510</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/e4748fbba125d7d1b9261c7a72b713cb364dcab6"><code>e4748fb</code></a> Support memory arrays in MerkleTree multiproof (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3493">#3493</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/b9710923a82a34e02c90b402ed51e94ee69e3b7c"><code>b971092</code></a> Make ERC4626 _deposit and _withdraw internal virtual (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3504">#3504</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/4307d7496680f9f63873a3d543ee5d445af236bf"><code>4307d74</code></a> Add a caution note to ERC4626 about EOA access (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3503">#3503</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/1e7d73538949bfec7fdbcae0bcc76fee775df914"><code>1e7d735</code></a> Clarify PaymentSplitter shares are static</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/029706d1676e541d182eebc90d9bb7a7fca7c0f0"><code>029706d</code></a> Fix check for generated code when last updated is a release candidate</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/97c46a7d002e929440b0d37949389877af8b0a14"><code>97c46a7</code></a> Output diff when test:generation fails</li>
<li>Additional commits viewable in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/compare/v4.6.0...v4.7.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts&package-manager=npm_and_yarn&previous-version=4.6.0&new-version=4.7.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-07-21 22:48:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/587" class=".btn">#587</a>
            </td>
            <td>
                <b>
                    Bump @openzeppelin/contracts-upgradeable from 4.6.0 to 4.7.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts-upgradeable](https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable) from 4.6.0 to 4.7.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/releases"><code>@​openzeppelin/contracts-upgradeable</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.7.1</h2>
<p>:warning: This is a patch for a medium severity issue affecting <code>SignatureChecker</code> and a high severity issue affecting <code>ERC165Checker</code>. For more information visit the security advisories (<a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-4g63-c64m-25w9">1</a>, <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-qh9x-gcfh-pcrw">2</a>).</p>
<ul>
<li><code>SignatureChecker</code>: Fix an issue that causes <code>isValidSignatureNow</code> to revert when the target contract returns ill-encoded data. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3552">#3552</a>)</li>
<li><code>ERC165Checker</code>: Fix an issue that causes <code>supportsInterface</code> to revert when the target contract returns ill-encoded data. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3552">#3552</a>)</li>
</ul>
<h2>v4.7.0</h2>
<ul>
<li><code>TimelockController</code>: Migrate <code>_call</code> to <code>_execute</code> and allow inheritance and overriding similar to <code>Governor</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3317">#3317</a>)</li>
<li><code>CrossChainEnabledPolygonChild</code>: replace the <code>require</code> statement with the custom error <code>NotCrossChainCall</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3380">#3380</a>)</li>
<li><code>ERC20FlashMint</code>: Add customizable flash fee receiver. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3327">#3327</a>)</li>
<li><code>ERC4626</code>: add an extension of <code>ERC20</code> that implements the ERC4626 Tokenized Vault Standard. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3171">#3171</a>)</li>
<li><code>SafeERC20</code>: add <code>safePermit</code> as mitigation against phantom permit functions. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3280">#3280</a>)</li>
<li><code>Math</code>: add a <code>mulDiv</code> function that can round the result either up or down. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3171">#3171</a>)</li>
<li><code>Math</code>: Add a <code>sqrt</code> function to compute square roots of integers, rounding either up or down. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3242">#3242</a>)</li>
<li><code>Strings</code>: add a new overloaded function <code>toHexString</code> that converts an <code>address</code> with fixed length of 20 bytes to its not checksummed ASCII <code>string</code> hexadecimal representation. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3403">#3403</a>)</li>
<li><code>EnumerableMap</code>: add new <code>UintToUintMap</code> map type. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3338">#3338</a>)</li>
<li><code>EnumerableMap</code>: add new <code>Bytes32ToUintMap</code> map type. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3416">#3416</a>)</li>
<li><code>SafeCast</code>: add support for many more types, using procedural code generation. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3245">#3245</a>)</li>
<li><code>MerkleProof</code>: add <code>multiProofVerify</code> to prove multiple values are part of a Merkle tree. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3276">#3276</a>)</li>
<li><code>MerkleProof</code>: add calldata versions of the functions to avoid copying input arrays to memory and save gas. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3200">#3200</a>)</li>
<li><code>ERC721</code>, <code>ERC1155</code>: simplified revert reasons. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3254">#3254</a>, (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3438">#3438</a>))</li>
<li><code>ERC721</code>: removed redundant require statement. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3434">#3434</a>)</li>
<li><code>PaymentSplitter</code>: add <code>releasable</code> getters. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3350">#3350</a>)</li>
<li><code>Initializable</code>: refactored implementation of modifiers for easier understanding. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3450">#3450</a>)</li>
<li><code>Proxies</code>: remove runtime check of ERC1967 storage slots. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3455">#3455</a>)</li>
</ul>
<h3>Breaking changes</h3>
<ul>
<li><code>Initializable</code>: functions decorated with the modifier <code>reinitializer(1)</code> may no longer invoke each other.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/blob/master/CHANGELOG.md"><code>@​openzeppelin/contracts-upgradeable</code>'s changelog</a>.</em></p>
<blockquote>
<h2>4.7.1</h2>
<ul>
<li><code>SignatureChecker</code>: Fix an issue that causes <code>isValidSignatureNow</code> to revert when the target contract returns ill-encoded data. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3552">#3552</a>)</li>
<li><code>ERC165Checker</code>: Fix an issue that causes <code>supportsInterface</code> to revert when the target contract returns ill-encoded data. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3552">#3552</a>)</li>
</ul>
<h2>4.7.0 (2022-06-29)</h2>
<ul>
<li><code>TimelockController</code>: Migrate <code>_call</code> to <code>_execute</code> and allow inheritance and overriding similar to <code>Governor</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3317">#3317</a>)</li>
<li><code>CrossChainEnabledPolygonChild</code>: replace the <code>require</code> statement with the custom error <code>NotCrossChainCall</code>. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3380">#3380</a>)</li>
<li><code>ERC20FlashMint</code>: Add customizable flash fee receiver. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3327">#3327</a>)</li>
<li><code>ERC4626</code>: add an extension of <code>ERC20</code> that implements the ERC4626 Tokenized Vault Standard. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3171">#3171</a>)</li>
<li><code>SafeERC20</code>: add <code>safePermit</code> as mitigation against phantom permit functions. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3280">#3280</a>)</li>
<li><code>Math</code>: add a <code>mulDiv</code> function that can round the result either up or down. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3171">#3171</a>)</li>
<li><code>Math</code>: Add a <code>sqrt</code> function to compute square roots of integers, rounding either up or down. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3242">#3242</a>)</li>
<li><code>Strings</code>: add a new overloaded function <code>toHexString</code> that converts an <code>address</code> with fixed length of 20 bytes to its not checksummed ASCII <code>string</code> hexadecimal representation. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3403">#3403</a>)</li>
<li><code>EnumerableMap</code>: add new <code>UintToUintMap</code> map type. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3338">#3338</a>)</li>
<li><code>EnumerableMap</code>: add new <code>Bytes32ToUintMap</code> map type. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3416">#3416</a>)</li>
<li><code>SafeCast</code>: add support for many more types, using procedural code generation. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3245">#3245</a>)</li>
<li><code>MerkleProof</code>: add <code>multiProofVerify</code> to prove multiple values are part of a Merkle tree. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3276">#3276</a>)</li>
<li><code>MerkleProof</code>: add calldata versions of the functions to avoid copying input arrays to memory and save gas. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3200">#3200</a>)</li>
<li><code>ERC721</code>, <code>ERC1155</code>: simplified revert reasons. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3254">#3254</a>, (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3438">#3438</a>))</li>
<li><code>ERC721</code>: removed redundant require statement. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3434">#3434</a>)</li>
<li><code>PaymentSplitter</code>: add <code>releasable</code> getters. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3350">#3350</a>)</li>
<li><code>Initializable</code>: refactored implementation of modifiers for easier understanding. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3450">#3450</a>)</li>
<li><code>Proxies</code>: remove runtime check of ERC1967 storage slots. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3455">#3455</a>)</li>
</ul>
<h3>Breaking changes</h3>
<ul>
<li><code>Initializable</code>: functions decorated with the modifier <code>reinitializer(1)</code> may no longer invoke each other.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/5e9bccb282ee8f3c9c4abaccc74b40b9d34ccffa"><code>5e9bccb</code></a> Transpile 138d0948</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/6b9807b0639e1dd75e07fa062e9432eb3f35dd8c"><code>6b9807b</code></a> Transpile ec1fcdde</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/366f3daf7517fbc9f64368de389aa5db8aa729a7"><code>366f3da</code></a> Transpile 6d4c354e</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/d2ec96a77f25bd095bcf0d0e1e0b56be3f6be711"><code>d2ec96a</code></a> Transpile c319c806</li>
<li>See full diff in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/compare/v4.6.0...v4.7.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts-upgradeable&package-manager=npm_and_yarn&previous-version=4.6.0&new-version=4.7.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-07-21 22:40:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/586" class=".btn">#586</a>
            </td>
            <td>
                <b>
                    Bump undici from 5.5.1 to 5.8.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [undici](https://github.com/nodejs/undici) from 5.5.1 to 5.8.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nodejs/undici/releases">undici's releases</a>.</em></p>
<blockquote>
<h2>v5.8.0</h2>
<h2>⚠️ Security Fixes ⚠️</h2>
<ul>
<li>CRLF injection in request path, method, and headers <a href="https://github.com/nodejs/undici/security/advisories/GHSA-3cvr-822r-rqcc">https://github.com/nodejs/undici/security/advisories/GHSA-3cvr-822r-rqcc</a>, CVE CVE-2022-31150, reported by <a href="https://github.com/Haxatron"><code>@​Haxatron</code></a></li>
<li>Cookies uncleared on cross-host / cross-origin redirect <a href="https://github.com/nodejs/undici/security/advisories/GHSA-q768-x9m6-m9qp">https://github.com/nodejs/undici/security/advisories/GHSA-q768-x9m6-m9qp</a>, CVE CVE-2022-31150, reported by <a href="https://github.com/Haxatron"><code>@​Haxatron</code></a></li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>Drop PR title validation by <a href="https://github.com/mcollina"><code>@​mcollina</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1543">nodejs/undici#1543</a></li>
<li>chore: exclude windows node 16 by <a href="https://github.com/mcollina"><code>@​mcollina</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1542">nodejs/undici#1542</a></li>
<li>feat: use weighted round robin in balancedPool by <a href="https://github.com/jodevsa"><code>@​jodevsa</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1069">nodejs/undici#1069</a></li>
<li>Fix up <code>exclude</code> in CI by <a href="https://github.com/dominykas"><code>@​dominykas</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1544">nodejs/undici#1544</a></li>
<li>fix(mock utils): set Readable.abort by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1549">nodejs/undici#1549</a></li>
<li>fix(body mixin): only allow Uint8Array chunks by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1550">nodejs/undici#1550</a></li>
<li>docs: updated proxy docs - renamed already used const proxy to proxyServer by <a href="https://github.com/dancastillo"><code>@​dancastillo</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1552">nodejs/undici#1552</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/jodevsa"><code>@​jodevsa</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1069">nodejs/undici#1069</a></li>
<li><a href="https://github.com/dancastillo"><code>@​dancastillo</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1552">nodejs/undici#1552</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.7.0...v5.7.1">https://github.com/nodejs/undici/compare/v5.7.0...v5.7.1</a></p>
<h2>v5.7.0</h2>
<h2>What's Changed</h2>
<ul>
<li>fix(fetch): re-add support for node v16.8.0+ by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1534">nodejs/undici#1534</a></li>
<li>fix(Headers): lowercase name in <code>Headers.prototype.set</code> by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1535">nodejs/undici#1535</a></li>
<li>fix: allow optional body for mock reply by <a href="https://github.com/JustinBeckwith"><code>@​JustinBeckwith</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1536">nodejs/undici#1536</a></li>
<li>fix: faster direct read approach by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1537">nodejs/undici#1537</a></li>
<li>feat: update to llhttp v6.0.7 by <a href="https://github.com/mcollina"><code>@​mcollina</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1539">nodejs/undici#1539</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1537">nodejs/undici#1537</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.6.1...v5.7.0">https://github.com/nodejs/undici/compare/v5.6.1...v5.7.0</a></p>
<h2>v5.6.1</h2>
<h2>What's Changed</h2>
<ul>
<li>docs: add example with <code>HEAD</code> method to garbage collection section by <a href="https://github.com/mrkldshv"><code>@​mrkldshv</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1522">nodejs/undici#1522</a></li>
<li>fix: improper handling of relative location header by <a href="https://github.com/PrincessRavy"><code>@​PrincessRavy</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1523">nodejs/undici#1523</a></li>
<li>build(deps-dev): bump tsd from 0.21.0 to 0.22.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1530">nodejs/undici#1530</a></li>
<li>fix(fetch): do not assign default value to <code>RequestInit.method</code> by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1529">nodejs/undici#1529</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/mrkldshv"><code>@​mrkldshv</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1522">nodejs/undici#1522</a></li>
<li><a href="https://github.com/PrincessRavy"><code>@​PrincessRavy</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1523">nodejs/undici#1523</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.6.0...v5.6.1">https://github.com/nodejs/undici/compare/v5.6.0...v5.6.1</a></p>
<h2>v5.6.0</h2>
<h2>What's Changed</h2>
<ul>
<li>build(deps-dev): bump tsd from 0.20.0 to 0.21.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1493">nodejs/undici#1493</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nodejs/undici/commit/26f60b7b6e612bb831133d7f85914963d1955011"><code>26f60b7</code></a> Bumped v5.8.0</li>
<li><a href="https://github.com/nodejs/undici/commit/0a5bee9465e627be36bac88edf7d9bbc9626126d"><code>0a5bee9</code></a> Merge pull request from GHSA-q768-x9m6-m9qp</li>
<li><a href="https://github.com/nodejs/undici/commit/a29a151d0140d095742d21a004023d024fe93259"><code>a29a151</code></a> Merge pull request from GHSA-3cvr-822r-rqcc</li>
<li><a href="https://github.com/nodejs/undici/commit/722976cf862b532d2a4a7ce45d9469946c0f5558"><code>722976c</code></a> docs: updated proxy docs - renamed already used const proxy to proxyServer (#...</li>
<li><a href="https://github.com/nodejs/undici/commit/b6af4e6eb5177444bc91f740b68de4eb8a43c561"><code>b6af4e6</code></a> fix(body mixin): only allow Uint8Array chunks (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1550">#1550</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/6c9e6344018982ff0a241f6f8a71682546410ebe"><code>6c9e634</code></a> fix(mock utils): set Readable.abort (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1549">#1549</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/22e2f39aad33f1537f3a1768842eef73da226745"><code>22e2f39</code></a> ci: fix up <code>exclude</code> (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1544">#1544</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/99205ec1e6dbaecb5e4b4494341d64c0a7b479eb"><code>99205ec</code></a> feat: use weighted round robin in balancedPool (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1069">#1069</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/5b57e8c6ad923c95bd9fc1dd7072083bc7542c82"><code>5b57e8c</code></a> chore: exclude windows node 16 (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1542">#1542</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/93e31a21c02defaf2625f9ec7e7a8936f495d3bc"><code>93e31a2</code></a> Drop PR title validation (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1543">#1543</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/nodejs/undici/compare/v5.5.1...v5.8.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=undici&package-manager=npm_and_yarn&previous-version=5.5.1&new-version=5.8.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-07-21 21:09:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/585" class=".btn">#585</a>
            </td>
            <td>
                <b>
                    Bump terser from 5.14.1 to 5.14.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [terser](https://github.com/terser/terser) from 5.14.1 to 5.14.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/terser/terser/blob/master/CHANGELOG.md">terser's changelog</a>.</em></p>
<blockquote>
<h2>v5.14.2</h2>
<ul>
<li>Security fix for RegExps that should not be evaluated (regexp DDOS)</li>
<li>Source maps improvements (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1211">#1211</a>)</li>
<li>Performance improvements in long property access evaluation (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1213">#1213</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/terser/terser/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=terser&package-manager=npm_and_yarn&previous-version=5.14.1&new-version=5.14.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-07-21 06:21:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/583" class=".btn">#583</a>
            </td>
            <td>
                <b>
                    Api-oracle-branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Achintya Kumar <ackintya@gmail.com>
Added api-oracle and relevant documentation with tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-18 13:34:57 +0000 UTC
    </div>
</div>

