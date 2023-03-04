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

