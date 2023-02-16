---
layout: default
title: firefly-tokens-erc20-erc721
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-tokens-erc20-erc721
---

# firefly-tokens-erc20-erc721 <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-tokens-erc20-erc721){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/121" class=".btn">#121</a>
            </td>
            <td>
                <b>
                    Bump cacheable-request, @nomiclabs/hardhat-waffle, ethereum-waffle and solidity-coverage in /samples/solidity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Removes [cacheable-request](https://github.com/jaredwray/cacheable-request). It's no longer used after updating ancestor dependencies [cacheable-request](https://github.com/jaredwray/cacheable-request), [@nomiclabs/hardhat-waffle](https://github.com/NomicFoundation/hardhat-waffle), [ethereum-waffle](https://github.com/EthWorks/Waffle) and [solidity-coverage](https://github.com/sc-forks/solidity-coverage). These dependencies need to be updated together.

Removes `cacheable-request`

Updates `@nomiclabs/hardhat-waffle` from 2.0.3 to 2.0.5
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/NomicFoundation/hardhat-waffle/releases"><code>@​nomiclabs/hardhat-waffle</code>'s releases</a>.</em></p>
<blockquote>
<h2><code>@​nomiclabs/hardaht-waffle</code> v2.0.5 released</h2>
<p>This is the first version of the plugin published in collaboration with the <a href="https://truefi.io/">TrueFi</a> team, the maintainers of Waffle 🚀</p>
<p>We moved this plugin to its own repository, cleaned it up in the process, and implemented some small improvements.</p>
<h2>Changes</h2>
<ul>
<li>c5b5c29: Introduce skipEstimateGas and injectCallHistory fields to hardhat config</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/NomicFoundation/hardhat-waffle/blob/main/CHANGELOG.md"><code>@​nomiclabs/hardhat-waffle</code>'s changelog</a>.</em></p>
<blockquote>
<h2>2.0.5</h2>
<h3>Patch Changes</h3>
<ul>
<li>36441d8: Add hardhat chai matchers incompatibility check</li>
<li>c5b5c29: Introduce skipEstimateGas and injectCallHistory fields to hardhat config</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/NomicFoundation/hardhat-waffle/commits/v2.0.5">compare view</a></li>
</ul>
</details>
<br />

Updates `ethereum-waffle` from 3.4.4 to 4.0.9
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/EthWorks/Waffle/releases">ethereum-waffle's releases</a>.</em></p>
<blockquote>
<h2><code>@​ethereum-waffle/chai</code><a href="https://github.com/4"><code>@​4</code></a>.0.9</h2>
<h3>Patch Changes</h3>
<ul>
<li>216f1d8: Switch hardhat error priority</li>
</ul>
<h2>ethereum-waffle@4.0.9</h2>
<h3>Patch Changes</h3>
<ul>
<li>Updated dependencies [216f1d8]
<ul>
<li><code>@​ethereum-waffle/chai</code><a href="https://github.com/4"><code>@​4</code></a>.0.9</li>
<li><code>@​ethereum-waffle/compiler</code><a href="https://github.com/4"><code>@​4</code></a>.0.3</li>
<li><code>@​ethereum-waffle/mock-contract</code><a href="https://github.com/4"><code>@​4</code></a>.0.3</li>
</ul>
</li>
</ul>
<h2><code>@​ethereum-waffle/chai</code><a href="https://github.com/4"><code>@​4</code></a>.0.8</h2>
<h3>Patch Changes</h3>
<ul>
<li>f93abe9: Move call history injection logic to hardhat plugin</li>
<li>9602243: 👔 revertedWith().withArgs no longer fails for uint values exceeding JavaScript's max int limit</li>
<li>b54c6b9: Add delta to balance changing matchers</li>
<li>64707ae: Allow special characters in revertedWith regex</li>
<li>702c6ab: 🗾 Extend matching of Hardhat revert reasons</li>
<li>a0f721a: Move ethers to peer deps</li>
<li>f6d240e: 🛶 Updates for hardhat v2.11</li>
<li>Updated dependencies [ee1d1b8]</li>
<li>Updated dependencies [a0f721a]
<ul>
<li><code>@​ethereum-waffle/provider</code><a href="https://github.com/4"><code>@​4</code></a>.0.5</li>
</ul>
</li>
</ul>
<h2>ethereum-waffle@4.0.8</h2>
<h3>Patch Changes</h3>
<ul>
<li>f93abe9: Move call history injection logic to hardhat plugin</li>
<li>a0f721a: Move ethers to peer deps</li>
<li>Updated dependencies [da92375]</li>
<li>Updated dependencies [f93abe9]</li>
<li>Updated dependencies [46b954e]</li>
<li>Updated dependencies [9602243]</li>
<li>Updated dependencies [fb6863d]</li>
<li>Updated dependencies [b54c6b9]</li>
<li>Updated dependencies [64707ae]</li>
<li>Updated dependencies [1fa1312]</li>
<li>Updated dependencies [ee1d1b8]</li>
<li>Updated dependencies [702c6ab]</li>
<li>Updated dependencies [a0f721a]</li>
<li>Updated dependencies [f6d240e]
<ul>
<li><code>@​ethereum-waffle/mock-contract</code><a href="https://github.com/4"><code>@​4</code></a>.0.3</li>
<li><code>@​ethereum-waffle/chai</code><a href="https://github.com/4"><code>@​4</code></a>.0.8</li>
<li><code>@​ethereum-waffle/provider</code><a href="https://github.com/4"><code>@​4</code></a>.0.5</li>
<li><code>@​ethereum-waffle/compiler</code><a href="https://github.com/4"><code>@​4</code></a>.0.3</li>
</ul>
</li>
</ul>
<h2><code>@​ethereum-waffle/chai</code><a href="https://github.com/4"><code>@​4</code></a>.0.7</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/TrueFiEng/Waffle/commit/a1d89d0063c7cc3d9d2e9b23cb17d9590fa1b7fd"><code>a1d89d0</code></a> 🎉 Release new version (<a href="https://github-redirect.dependabot.com/EthWorks/Waffle/issues/821">#821</a>)</li>
<li><a href="https://github.com/TrueFiEng/Waffle/commit/216f1d8cdfd98d02c6a335d7789831559aecf955"><code>216f1d8</code></a> 🌏 Switch hardhat errors priority (<a href="https://github-redirect.dependabot.com/EthWorks/Waffle/issues/820">#820</a>)</li>
<li><a href="https://github.com/TrueFiEng/Waffle/commit/13d1af063fe5d78a84aafeb549b2e3073f2e57c1"><code>13d1af0</code></a> 🎉 Release new version (<a href="https://github-redirect.dependabot.com/EthWorks/Waffle/issues/796">#796</a>)</li>
<li><a href="https://github.com/TrueFiEng/Waffle/commit/5637cc55a81ede4976ab5863c3a04840fff395eb"><code>5637cc5</code></a> 🦉 Optimism tests use latest commit (<a href="https://github-redirect.dependabot.com/EthWorks/Waffle/issues/819">#819</a>)</li>
<li><a href="https://github.com/TrueFiEng/Waffle/commit/1fa13127d199e43226178ffc45a661fddd657045"><code>1fa1312</code></a> 🥑 Add mock contract typing (<a href="https://github-redirect.dependabot.com/EthWorks/Waffle/issues/818">#818</a>)</li>
<li><a href="https://github.com/TrueFiEng/Waffle/commit/702c6ab299d78c1dbbb42ea72aa8bfbfce0c8390"><code>702c6ab</code></a> 🗾 Extend matching of Hardhat revert reasons (<a href="https://github-redirect.dependabot.com/EthWorks/Waffle/issues/802">#802</a>)</li>
<li><a href="https://github.com/TrueFiEng/Waffle/commit/46b954e1f9cbf9036ece5837c574ce800e6cdacc"><code>46b954e</code></a> 🖼 Mock contract chaining behaviour (<a href="https://github-redirect.dependabot.com/EthWorks/Waffle/issues/816">#816</a>)</li>
<li><a href="https://github.com/TrueFiEng/Waffle/commit/fb6863d0a795db091b925385e1c1c670aa53eedd"><code>fb6863d</code></a> 🍶 Implement mocking receive function to revert (<a href="https://github-redirect.dependabot.com/EthWorks/Waffle/issues/807">#807</a>)</li>
<li><a href="https://github.com/TrueFiEng/Waffle/commit/da9237577597618afa306161edfbdcad7a426542"><code>da92375</code></a> 🗽 Add address parameter to the mock contract (<a href="https://github-redirect.dependabot.com/EthWorks/Waffle/issues/815">#815</a>)</li>
<li><a href="https://github.com/TrueFiEng/Waffle/commit/b54c6b93dee70dd54f831b2b6af60b11e4f8c827"><code>b54c6b9</code></a> 🗿 Add error to balance changing matchers (<a href="https://github-redirect.dependabot.com/EthWorks/Waffle/issues/814">#814</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/EthWorks/Waffle/compare/ethereum-waffle@3.4.4...ethereum-waffle@4.0.9">compare view</a></li>
</ul>
</details>
<br />

Updates `solidity-coverage` from 0.7.21 to 0.8.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sc-forks/solidity-coverage/releases">solidity-coverage's releases</a>.</em></p>
<blockquote>
<h2>0.8.2</h2>
<h2>What's Changed</h2>
<ul>
<li>Set web3-utils dep to ^1.3.6 by <a href="https://github.com/MarkuSchick"><code>@​MarkuSchick</code></a> in <a href="https://github-redirect.dependabot.com/sc-forks/solidity-coverage/pull/744">sc-forks/solidity-coverage#744</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/MarkuSchick"><code>@​MarkuSchick</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/sc-forks/solidity-coverage/pull/744">sc-forks/solidity-coverage#744</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sc-forks/solidity-coverage/compare/v0.8.1...v0.8.2">https://github.com/sc-forks/solidity-coverage/compare/v0.8.1...v0.8.2</a></p>
<h2>0.8.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Bug fix: restore missing web3-utils dependency by <a href="https://github.com/cgewecke"><code>@​cgewecke</code></a> in <a href="https://github-redirect.dependabot.com/sc-forks/solidity-coverage/pull/743">sc-forks/solidity-coverage#743</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sc-forks/solidity-coverage/compare/v0.8.0...v0.8.1">https://github.com/sc-forks/solidity-coverage/compare/v0.8.0...v0.8.1</a></p>
<h2>0.8.0</h2>
<p>Hi!</p>
<h4>⚠️ This version requires Hardhat &gt;= 2.11.0 (Ethereum Merge)</h4>
<h2>New Features</h2>
<p>A central focus of the 0.8.0 release is improving the coverage tool's branch detection.</p>
<p>Beginning with this version the following syntax is measured as a branch:</p>
<h3>OR conditions</h3>
<p>When a logical expression is composed with the <code>||</code> operator, both sides can be considered branches. To test the entire expression</p>
<pre lang="solidity"><code>if (a == 1 || a == 2)
</code></pre>
<p>... <code>a</code> must equal 1, 2 <em>and</em> neither of those values. (Thanks to Gnosis engineer <a href="https://github.com/rmeissner"><code>@​rmeissner</code></a> for proposing this in <a href="https://github-redirect.dependabot.com/sc-forks/solidity-coverage/issues/175">#175</a>)</p>
<p><img src="https://user-images.githubusercontent.com/7332026/104411309-fd2e9380-551e-11eb-8502-85cc72033b26.png" alt="Screen Shot 2021-01-12 at 9 41 09 PM" /></p>
<h3>Ternary Conditionals</h3>
<p>Long ago, when Solidity was 0.4, solidity-coverage treated ternary conditionals like regular if/else statements. Some language improvements v0.5 subsequently made this impossible. Now it's back...</p>
<p><img src="https://user-images.githubusercontent.com/7332026/104411766-db81dc00-551f-11eb-88a2-fd3e3867909e.png" alt="Screen Shot 2021-01-12 at 9 47 43 PM" /></p>
<h3>Modifier Invocations</h3>
<p>Solidity-coverage already covers the code within modifier definitions. However, each modifier invocation at the function level should really be considered its own branch. Some of the most critical logic in Solidity contracts is handled this way (ex: <code>onlyOwner</code>). Testing the pass/fail cases for each occurrence of these gates protects you from accidentally removing them during a refactor.</p>
<p>Because it's possible to write a modifier which performs a preparatory task and never reverts, there's a new option (<code>modifierWhitelist</code>) which allows you to exclude specific modifiers from branch measurement.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/sc-forks/solidity-coverage/blob/master/CHANGELOG.md">solidity-coverage's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<h1>0.8.1 / 2022-09-06</h1>
<ul>
<li>Restore web3-utils (<a href="https://github-redirect.dependabot.com/sc-forks/solidity-coverage/issues/743">sc-forks/solidity-coverage#743</a>)</li>
</ul>
<h1>0.8.0 / 2022-09-05</h1>
<ul>
<li>See release notes at: <a href="https://github.com/sc-forks/solidity-coverage/releases/tag/v0.8.0">https://github.com/sc-forks/solidity-coverage/releases/tag/v0.8.0</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/sc-forks/solidity-coverage/commits/v0.8.2">compare view</a></li>
</ul>
</details>
<br />


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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/firefly-tokens-erc20-erc721/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-12 03:42:31 +0000 UTC
    </div>
</div>

