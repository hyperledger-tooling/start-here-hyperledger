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
                PR <a href="https://github.com/hyperledger/cacti/pull/2403" class=".btn">#2403</a>
            </td>
            <td>
                <b>
                    feat(openssl): version upgrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …tements in cactus-plugin-keychain-vault package
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-24 03:20:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2402" class=".btn">#2402</a>
            </td>
            <td>
                <b>
                    chore(ci): revert to free runners
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
        Created At 2023-04-22 14:45:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2401" class=".btn">#2401</a>
            </td>
            <td>
                <b>
                    feat(driver): added Monitor to fabric driver for missed events and fabric testnet upgrade to 2.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. chore(testnet): upgrade fabric testnet to v2.5 in weaver and fix for mac
2. feat(driver): added Monitor to fabric driver for missed events
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-20 19:12:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2400" class=".btn">#2400</a>
            </td>
            <td>
                <b>
                    build(deps): bump h2 from 0.3.12 to 0.3.18 in /packages/cactus-plugin-keychain-vault/src/cactus-keychain-vault-server/rust/gen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [h2](https://github.com/hyperium/h2) from 0.3.12 to 0.3.18.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/h2/releases">h2's releases</a>.</em></p>
<blockquote>
<h2>v0.3.18</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: pending-accept remotely-reset streams pattern was checking is_local by <a href="https://github.com/seanmonstar"><code>@​seanmonstar</code></a> in <a href="https://redirect.github.com/hyperium/h2/pull/676">hyperium/h2#676</a></li>
</ul>
<h2>v0.3.17</h2>
<h2>What's Changed</h2>
<ul>
<li>Add <code>Error::is_library()</code> method to check if the originated inside <code>h2</code>.</li>
<li>Add <code>max_pending_accept_reset_streams(usize)</code> option to client and server
builders.</li>
<li>Fix theoretical memory growth when receiving too many HEADERS and then
RST_STREAM frames faster than an application can accept them off the queue.
(CVE-2023-26964)</li>
</ul>
<h2>v0.3.16</h2>
<h2>What's Changed</h2>
<ul>
<li>Set <code>Protocol</code> extension on requests when received Extended CONNECT requests.</li>
<li>Remove <code>B: Unpin + 'static</code> bound requiremented of bufs</li>
<li>Fix releasing of frames when stream is finished, reducing memory usage.</li>
<li>Fix panic when trying to send data and connection window is available, but stream window is not.</li>
<li>Fix spurious wakeups when stream capacity is not available.</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/vi"><code>@​vi</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/646">hyperium/h2#646</a></li>
<li><a href="https://github.com/silence-coding"><code>@​silence-coding</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/651">hyperium/h2#651</a></li>
<li><a href="https://github.com/gtsiam"><code>@​gtsiam</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/649">hyperium/h2#649</a></li>
<li><a href="https://github.com/howardjohn"><code>@​howardjohn</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/658">hyperium/h2#658</a></li>
<li><a href="https://github.com/cloneable"><code>@​cloneable</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/655">hyperium/h2#655</a></li>
<li><a href="https://github.com/aftersnow"><code>@​aftersnow</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/657">hyperium/h2#657</a></li>
<li><a href="https://github.com/vadim-eg"><code>@​vadim-eg</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/661">hyperium/h2#661</a></li>
</ul>
<h2>v0.3.15</h2>
<h2>What's Changed</h2>
<ul>
<li>Remove <code>B: Buf</code> bound on <code>SendStream</code>'s parameter by <a href="https://github.com/djkoloski"><code>@​djkoloski</code></a> in <a href="https://redirect.github.com/hyperium/h2/pull/614">hyperium/h2#614</a></li>
<li>add accessor for StreamId u32 by <a href="https://github.com/ehaydenr"><code>@​ehaydenr</code></a> in <a href="https://redirect.github.com/hyperium/h2/pull/639">hyperium/h2#639</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/ehaydenr"><code>@​ehaydenr</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/639">hyperium/h2#639</a></li>
</ul>
<h2>v0.3.14</h2>
<ul>
<li>Add <code>Error::is_reset</code> function.</li>
<li>Bump MSRV to Rust 1.56.</li>
<li>Return <code>RST_STREAM(NO_ERROR)</code> when the server early responds.</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/djkoloski"><code>@​djkoloski</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/616">hyperium/h2#616</a></li>
<li><a href="https://github.com/bruceg"><code>@​bruceg</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/618">hyperium/h2#618</a></li>
<li><a href="https://github.com/ryanrussell"><code>@​ryanrussell</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/620">hyperium/h2#620</a></li>
<li><a href="https://github.com/kckeiks"><code>@​kckeiks</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/625">hyperium/h2#625</a></li>
<li><a href="https://github.com/erebe"><code>@​erebe</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/634">hyperium/h2#634</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/h2/blob/master/CHANGELOG.md">h2's changelog</a>.</em></p>
<blockquote>
<h1>0.3.18 (April 17, 2023)</h1>
<ul>
<li>Fix panic because of opposite check in <code>is_remote_local()</code>.</li>
</ul>
<h1>0.3.17 (April 13, 2023)</h1>
<ul>
<li>Add <code>Error::is_library()</code> method to check if the originated inside <code>h2</code>.</li>
<li>Add <code>max_pending_accept_reset_streams(usize)</code> option to client and server
builders.</li>
<li>Fix theoretical memory growth when receiving too many HEADERS and then
RST_STREAM frames faster than an application can accept them off the queue.
(CVE-2023-26964)</li>
</ul>
<h1>0.3.16 (February 27, 2023)</h1>
<ul>
<li>Set <code>Protocol</code> extension on requests when received Extended CONNECT requests.</li>
<li>Remove <code>B: Unpin + 'static</code> bound requiremented of bufs</li>
<li>Fix releasing of frames when stream is finished, reducing memory usage.</li>
<li>Fix panic when trying to send data and connection window is available, but stream window is not.</li>
<li>Fix spurious wakeups when stream capacity is not available.</li>
</ul>
<h1>0.3.15 (October 21, 2022)</h1>
<ul>
<li>Remove <code>B: Buf</code> bound on <code>SendStream</code>'s parameter</li>
<li>add accessor for <code>StreamId</code> u32</li>
</ul>
<h1>0.3.14 (August 16, 2022)</h1>
<ul>
<li>Add <code>Error::is_reset</code> function.</li>
<li>Bump MSRV to Rust 1.56.</li>
<li>Return <code>RST_STREAM(NO_ERROR)</code> when the server early responds.</li>
</ul>
<h1>0.3.13 (March 31, 2022)</h1>
<ul>
<li>Update private internal <code>tokio-util</code> dependency.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperium/h2/commit/1b9f0704ff24d5f7939d16162082c5a764a0bfaa"><code>1b9f070</code></a> v0.3.18</li>
<li><a href="https://github.com/hyperium/h2/commit/1c6fa285afe436ca2a1f8abd38a6389353f360b6"><code>1c6fa28</code></a> fix: pending-accept remotely-reset streams pattern was checking is_local</li>
<li><a href="https://github.com/hyperium/h2/commit/af4bcacf6d3770e9e3dc10fdc631fc8c0bdd472b"><code>af4bcac</code></a> v0.3.17</li>
<li><a href="https://github.com/hyperium/h2/commit/d3f37e9fbad6608ba74419c355eb1892bd55d977"><code>d3f37e9</code></a> feat: add <code>max_pending_accept_reset_streams(n)</code> options</li>
<li><a href="https://github.com/hyperium/h2/commit/5bc8e72e5fcbd8ae2d3d9bc78a1c0ef0040bcc39"><code>5bc8e72</code></a> fix: limit the amount of pending-accept reset streams</li>
<li><a href="https://github.com/hyperium/h2/commit/8088ca658d90a3874fb6b136b85776424265295b"><code>8088ca6</code></a> feat: add Error::is_library method</li>
<li><a href="https://github.com/hyperium/h2/commit/481c31d5283bf32b90c83388c037494548934971"><code>481c31d</code></a> chore: Use Cargo metadata for the MSRV build job</li>
<li><a href="https://github.com/hyperium/h2/commit/d3d50ef8123f0a1b6d16faa2d9edc01418da7c00"><code>d3d50ef</code></a> chore: Replace unmaintained/outdated GitHub Actions</li>
<li><a href="https://github.com/hyperium/h2/commit/45b9bccdfcb26cfe9907123a1e975a22eb84c44f"><code>45b9bcc</code></a> chore: set rust-version in Cargo.toml (<a href="https://redirect.github.com/hyperium/h2/issues/664">#664</a>)</li>
<li><a href="https://github.com/hyperium/h2/commit/b9dcd39915420ab1d9f4a8ad0f96c86af8f86558"><code>b9dcd39</code></a> v0.3.16</li>
<li>Additional commits viewable in <a href="https://github.com/hyperium/h2/compare/v0.3.12...v0.3.18">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=h2&package-manager=cargo&previous-version=0.3.12&new-version=0.3.18)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-04-20 11:15:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2399" class=".btn">#2399</a>
            </td>
            <td>
                <b>
                    chore(ci): move to dedicated Cacti runners
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This puts Cacti into a tranche of runners
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-19 00:55:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2398" class=".btn">#2398</a>
            </td>
            <td>
                <b>
                    build(deps): bump @openzeppelin/contracts from 4.7.3 to 4.8.3
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-17 17:15:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2397" class=".btn">#2397</a>
            </td>
            <td>
                <b>
                    build(deps): bump @openzeppelin/contracts-upgradeable from 4.7.3 to 4.8.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts-upgradeable](https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable) from 4.7.3 to 4.8.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/releases"><code>@​openzeppelin/contracts-upgradeable</code>'s releases</a>.</em></p>
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
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/blob/v4.8.3/CHANGELOG.md"><code>@​openzeppelin/contracts-upgradeable</code>'s changelog</a>.</em></p>
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
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/58fa0f81c4036f1a3b616fdffad2fd27e5d5ce21"><code>58fa0f8</code></a> Transpile 7415e3ca</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/f6c4c9c4ec601665ca74d2c9dddf547fc425658c"><code>f6c4c9c</code></a> Transpile c53d925e</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/9d777df668e0f3bf11f9e1e772a76033188dab45"><code>9d777df</code></a> Transpile 7e2f66ae</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/6753832ca0a76ec99fde0548834c64af3a83234d"><code>6753832</code></a> Transpile 84df2bc2</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/cb0c1443f9b0aded3b08dfb3088f5ed5c9c72bea"><code>cb0c144</code></a> Transpile e541d4ae</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/c10536c6330d1727811c48d7b0084886287f0cc7"><code>c10536c</code></a> Transpile 01015911</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/7ec6d2a3117eb3487a5f9029203e80ceb89bd984"><code>7ec6d2a</code></a> Transpile a87691d1</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/ce3f7f86516bd48074d7b7cdbc58aa804c7cfcb1"><code>ce3f7f8</code></a> Transpile 9ac253cb</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/477b4ce3ef3417e8d72e133993ef69af497459d9"><code>477b4ce</code></a> Transpile 630ea587</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/48de7022cd443b475d2aaddae6a18657bf034799"><code>48de702</code></a> Transpile cff1e672</li>
<li>Additional commits viewable in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/compare/v4.7.3...v4.8.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts-upgradeable&package-manager=npm_and_yarn&previous-version=4.7.3&new-version=4.8.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-04-17 16:51:08 +0000 UTC
    </div>
</div>

