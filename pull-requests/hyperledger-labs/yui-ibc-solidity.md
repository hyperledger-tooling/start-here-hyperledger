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
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/161" class=".btn">#161</a>
            </td>
            <td>
                <b>
                    build(deps): bump github.com/ethereum/go-ethereum from 1.9.25 to 1.10.22
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/ethereum/go-ethereum](https://github.com/ethereum/go-ethereum) from 1.9.25 to 1.10.22.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/ethereum/go-ethereum/releases">github.com/ethereum/go-ethereum's releases</a>.</em></p>
<blockquote>
<h2>Promavess (v1.10.22)</h2>
<h3>WARNING: This release seems to contain a regression that can corrupt the local state. Please hold on with updating while we investigate the issue!</h3>
<hr />
<p>Geth v1.10.22 <strong>enables the Merge for the Ethereum mainnet at a Terminal Total Difficulty of</strong> <code>58_750_000_000_000_000_000_000</code>.</p>
<p>This TTD is expected to be reached on the 15. September 2022.</p>
<h4>Merge EIPs</h4>
<ul>
<li><a href="https://eips.ethereum.org/EIPS/eip-3675">EIP-3676</a>: Upgrade consensus to Proof-of-Stake</li>
<li><a href="https://eips.ethereum.org/EIPS/eip-4399">EIP-4339</a>: Supplant DIFFICULTY opcode with PREVRANDAO</li>
</ul>
<h4>Additional notes about the merge changes</h4>
<ul>
<li>This release configures the Terminal Total Difficulty for mainnet. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25528">#25528</a>)</li>
<li>Many engine API issues found by hive have been fixed for this release. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25552">#25552</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25423">#25423</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25414">#25414</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25416">#25416</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25428">#25428</a>)</li>
<li>The Goerli testnet is now internally configured as 'successfully merged'. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25519">#25519</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/24538">#24538</a>)</li>
</ul>
<h4>JSON-RPC API</h4>
<ul>
<li>The log filtering system now uses a LRU cache for block logs, speeding up repeated queries for the same block range. The cache size can be configured using the <code>--cache.blocklogs</code> command-line flag. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25459">#25459</a>)</li>
<li><code>eth_createAccessList</code> is now much faster when no gas limit is provided. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25467">#25467</a>)</li>
<li><code>eth_feeHistory</code> now also works with the <code>finalized</code> block specifier. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25442">#25442</a>)</li>
<li>The built-in callTracer now supports an option <code>onlyTopCall</code>. Enabling this option makes the tracer skip internal calls. We added this option to enable use of the <code>callTracer</code> to get the return data of reverted transactions. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25430">#25430</a>)</li>
</ul>
<h4>Go-library changes</h4>
<ul>
<li>Storage of trie node hash preimages is now disabled by default. You can enable it again using the <code>--cache.preimages</code> flag. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25287">#25287</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25538">#25538</a>, <a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25533">#25533</a>)</li>
<li>The ethash mining implemenation now removes temporary DAG files, which could be left of disk when geth was interrupted while generating a DAG. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25381">#25381</a>)</li>
<li>ethclient now supports the <code>eth_feeHistory</code> method. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25403">#25403</a>)</li>
<li>The eth wire protocol test suite now supports protocol version eth/67. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25306">#25306</a>)</li>
<li>RLP-decoding of trie nodes is ~33% faster due to reduced allocations in the decoder. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25357">#25357</a>)</li>
<li>The RPC server supports a new option <code>ReadHeaderTimeout</code>. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25338">#25338</a>)</li>
<li>Registering of clef ruleset UIs should now work correctly. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25455">#25455</a>)</li>
</ul>
<h4>Build</h4>
<ul>
<li>Geth binaries in docker are now statically-linked. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25492">#25492</a>)</li>
<li>This release is built using Go 1.18.5. (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/pull/25461">#25461</a>)</li>
</ul>
<p>For a full rundown of the changes please consult the Geth <a href="https://github.com/ethereum/go-ethereum/milestone/134?closed=1">1.10.22 release milestone</a></p>
<hr />
<p>As with all our previous releases, you can find the:</p>
<ul>
<li>Pre-built binaries for all platforms on our <a href="https://geth.ethereum.org/downloads/">downloads page</a>.</li>
<li>Docker images published under <a href="https://cloud.docker.com/u/ethereum/repository/docker/ethereum/client-go"><code>ethereum/client-go</code></a>.</li>
<li>Ubuntu packages in our <a href="https://launchpad.net/~ethereum/+archive/ubuntu/ethereum">Launchpad PPA repository</a>.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ethereum/go-ethereum/commit/2de49b04e56cf07f011d6d91f9d5c08847aabe8e"><code>2de49b0</code></a> params: release go-ethereum v1.10.22</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/395f3d4bf689c199e93e05af57ebff09b10f1c9a"><code>395f3d4</code></a> eth/catalyst: warn less frequently if no beacon client is available (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/25569">#25569</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/02418c2fa965e61f5bc1e66e1063482eb5293e5d"><code>02418c2</code></a> Revert &quot;eth/fetcher: don't spend too much time on transaction inclusion&quot; (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/25">#25</a>...</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/0ce494b60cd00d70f1f9f2dd0b9bfbd76204168a"><code>0ce494b</code></a> eth/fetcher: don't spend too much time on transaction inclusion (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/25524">#25524</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/ac7ad811b4d2ba0b93f9272e2487253026620b48"><code>ac7ad81</code></a> internal/ethapi: fix build regression (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/25555">#25555</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/08658806268f4c570c682e87681881ac35123fe9"><code>0865880</code></a> accounts/abi: fix set function (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/25477">#25477</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/36874b63a1b56eed2b8e4b47ccea0337920b84b8"><code>36874b6</code></a> eth/filters: add global block logs cache (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/25459">#25459</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/77308cd6fceb99e276c1e2753d92ff82c6f1a962"><code>77308cd</code></a> consensus/beacon: check ttd reached on pos blocks (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/25552">#25552</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/9762ddf8b0e9d471600c99f158479912f4870c52"><code>9762ddf</code></a> cmd/geth: parse uint64 value with ParseUint instead of Atoi (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/25545">#25545</a>)</li>
<li><a href="https://github.com/ethereum/go-ethereum/commit/656dc8cc0034d3dd57b5e1baecb788d9c4e9929d"><code>656dc8c</code></a> eth, les: unlock downloader peerSet if there's an error (<a href="https://github-redirect.dependabot.com/ethereum/go-ethereum/issues/25546">#25546</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/ethereum/go-ethereum/compare/v1.9.25...v1.10.22">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/ethereum/go-ethereum&package-manager=go_modules&previous-version=1.9.25&new-version=1.10.22)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-ibc-solidity/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 02:19:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/160" class=".btn">#160</a>
            </td>
            <td>
                <b>
                    build(deps): bump @openzeppelin/contracts from 4.8.0 to 4.8.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) from 4.8.0 to 4.8.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/releases"><code>@​openzeppelin/contracts</code>'s releases</a>.</em></p>
<blockquote>
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
<li><code>ERC4626</code>: Use staticcall instead of call when fetching underlying ERC-20 decimals. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3943">#3943</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/CHANGELOG.md"><code>@​openzeppelin/contracts</code>'s changelog</a>.</em></p>
<blockquote>
<h2>4.8.2 (2023-03-02)</h2>
<ul>
<li><code>ERC721Consecutive</code>: Fixed a bug when <code>_mintConsecutive</code> is used for batches of size 1 that could lead to balance overflow. Refer to the breaking changes section in the changelog for a note on the behavior of <code>ERC721._beforeTokenTransfer</code>.</li>
</ul>
<h3>Breaking changes</h3>
<ul>
<li><code>ERC721</code>: The internal function <code>_beforeTokenTransfer</code> no longer updates balances, which it previously did when <code>batchSize</code> was greater than 1. This change has no consequence unless a custom ERC721 extension is explicitly invoking <code>_beforeTokenTransfer</code>. Balance updates in extensions must now be done explicitly using <code>__unsafe_increaseBalance</code>, with a name that indicates that there is an invariant that has to be manually verified.</li>
</ul>
<h2>4.8.1 (2023-01-12)</h2>
<ul>
<li><code>ERC4626</code>: Use staticcall instead of call when fetching underlying ERC-20 decimals. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3943">#3943</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/d00acef4059807535af0bd0dd0ddf619747a044b"><code>d00acef</code></a> 4.8.2</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/ab9cc4c4dbdd3be4a2e0935a76c160b31fb9deba"><code>ab9cc4c</code></a> Ignore reentrancy in<code>executeBatch</code> and update Slither config (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3955">#3955</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/43aa7ff1f5d3e463421a87a8b9036108fb6011fb"><code>43aa7ff</code></a> Update <code>forge-std</code> submodule to <code>v1.2.0</code> (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3885">#3885</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/167bf67ed3907f4a674043496019fa346cee7705"><code>167bf67</code></a> Fix ERC721Consecutive balance update on batch size 1</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/82d47ca7b3752293d73324e18cb3375add03c78c"><code>82d47ca</code></a> Add Subgraphs to docs sidebar</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/357022c1e8b89bddc4d7a6d45afb9c18d71a7dbd"><code>357022c</code></a> Update Tally screenshots (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/4030">#4030</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/9b610d3db4cf640d82cf185ca4585a9aa19cc08b"><code>9b610d3</code></a> Add warning for <code>supportsERC165InterfaceUnchecked</code> edge case (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/4017">#4017</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/c018c9cf36dbac7f890bb4361d98f795df1fc298"><code>c018c9c</code></a> Remove outdated note about virtual view functions (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/4014">#4014</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/d13316e8b1061ae6c9277e0e0b2ae4667f720692"><code>d13316e</code></a> Add <code>ERC*Pausable</code> warning for public pausing mechanism (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/4007">#4007</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/3ab2e115a29628f15785f6a3a483a1a21ad32d31"><code>3ab2e11</code></a> Show if event parameter is indexed in docs (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3958">#3958</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/compare/v4.8.0...v4.8.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts&package-manager=npm_and_yarn&previous-version=4.8.0&new-version=4.8.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-ibc-solidity/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 20:09:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/159" class=".btn">#159</a>
            </td>
            <td>
                <b>
                    relay: follow-up #130: remove unused field from proto
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
        Created At 2023-03-03 10:17:45 +0000 UTC
    </div>
</div>

