---
layout: default
title: weaver-dlt-interoperability
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/weaver-dlt-interoperability
---

# weaver-dlt-interoperability <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/weaver-dlt-interoperability){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/345" class=".btn">#345</a>
            </td>
            <td>
                <b>
                    Bump @openzeppelin/contracts from 4.6.0 to 4.7.3 in /samples/besu/simplestate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) from 4.6.0 to 4.7.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/releases"><code>@​openzeppelin/contracts</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.7.3</h2>
<p>:warning: This is a patch for a high severity issue. For more information <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-4h98-2769-gh6h">visit the security advisory</a>.</p>
<h3>Breaking changes</h3>
<ul>
<li><code>ECDSA</code>: <code>recover(bytes32,bytes)</code> and <code>tryRecover(bytes32,bytes)</code> no longer accept compact signatures to prevent malleability. Compact signature support remains available using <code>recover(bytes32,bytes32,bytes32)</code> and <code>tryRecover(bytes32,bytes32,bytes32)</code>.</li>
</ul>
<h2>v4.7.2</h2>
<p>:warning: This is a patch for three issues, including a high severity issue in <code>GovernorVotesQuorumFraction</code>. For more information visit the security advisories (<a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-xrc4-737v-9q75">1</a>, <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-7grf-83vw-6f5x">2</a>, <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-9j3m-g383-29qr">3</a>).</p>
<ol>
<li><code>GovernorVotesQuorumFraction</code>: Fixed quorum updates so they do not affect past proposals that failed due to lack of quorum. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3561">#3561</a>)</li>
<li><code>ERC165Checker</code>: Added protection against large returndata. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3587">#3587</a>)</li>
<li><code>LibArbitrumL2</code>, <code>CrossChainEnabledArbitrumL2</code>: Fixed detection of cross-chain calls for EOAs. Previously, calls from EOAs would be classified as cross-chain calls. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3578">#3578</a>)</li>
</ol>
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
<h2>4.7.3</h2>
<h3>Breaking changes</h3>
<ul>
<li><code>ECDSA</code>: <code>recover(bytes32,bytes)</code> and <code>tryRecover(bytes32,bytes)</code> no longer accept compact signatures to prevent malleability. Compact signature support remains available using <code>recover(bytes32,bytes32,bytes32)</code> and <code>tryRecover(bytes32,bytes32,bytes32)</code>.</li>
</ul>
<h2>4.7.2</h2>
<ul>
<li><code>LibArbitrumL2</code>, <code>CrossChainEnabledArbitrumL2</code>: Fixed detection of cross-chain calls for EOAs. Previously, calls from EOAs would be classified as cross-chain calls. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3578">#3578</a>)</li>
<li><code>GovernorVotesQuorumFraction</code>: Fixed quorum updates so they do not affect past proposals that failed due to lack of quorum. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3561">#3561</a>)</li>
<li><code>ERC165Checker</code>: Added protection against large returndata. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3587">#3587</a>)</li>
</ul>
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
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/ecd2ca2cd7cac116f7a37d0e474bbb3d7d5e1c4d"><code>ecd2ca2</code></a> 4.7.3</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/e1878ace8c2908b85d39f9925c68c6f738cf3325"><code>e1878ac</code></a> Fix ECDSA signature malleability (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3610">#3610</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/64e48203cecad94f02de9891ecdeed4d629c6dae"><code>64e4820</code></a> 4.7.2</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/b66fe1606a173f2b78694567b543d480cb39cfe4"><code>b66fe16</code></a> Update changelog</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/8fb5f5774e3e8cfc10699f58749d8a34ec9d3e86"><code>8fb5f57</code></a> Avoid returnbomb in ERC165Checker (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3587">#3587</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/67b2572c6a050563990637f5017af8eeda111b21"><code>67b2572</code></a> Keep track of historical quorum values (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3561">#3561</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/4337192dc02b64785885787e80126f93ee3f2659"><code>4337192</code></a> Fix arbitrum L1 to L2 crosschain call detection (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3578">#3578</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/41c7b25a65f636feaef7f0dc932ec4c44baa12f3"><code>41c7b25</code></a> Fix error in documentation and typo (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3567">#3567</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/e15862f2893f024e0872f0f1abcf275c4b436834"><code>e15862f</code></a> Remove test for feature not in 4.7</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/3b8b4ba82c880c31cd3b96dd5e15741d7e26658e"><code>3b8b4ba</code></a> 4.7.1</li>
<li>Additional commits viewable in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/compare/v4.6.0...v4.7.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts&package-manager=npm_and_yarn&previous-version=4.6.0&new-version=4.7.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-12 11:44:51 +0000 UTC
    </div>
</div>

