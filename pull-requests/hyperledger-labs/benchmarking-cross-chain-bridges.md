---
layout: default
title: benchmarking-cross-chain-bridges
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/benchmarking-cross-chain-bridges
---

# benchmarking-cross-chain-bridges <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/benchmarking-cross-chain-bridges){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/benchmarking-cross-chain-bridges/pull/24" class=".btn">#24</a>
            </td>
            <td>
                <b>
                    chore(deps): bump @openzeppelin/contracts from 5.0.0 to 5.0.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) from 5.0.0 to 5.0.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/releases"><code>@​openzeppelin/contracts</code>'s releases</a>.</em></p>
<blockquote>
<h2>v5.0.2</h2>
<ul>
<li><code>Base64</code>: Fix issue where dirty memory located just after the input buffer is affecting the result. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4926">#4926</a>)</li>
</ul>
<h2>v5.0.1</h2>
<ul>
<li><code>ERC2771Context</code> and <code>Context</code>: Introduce a <code>_contextPrefixLength()</code> getter, used to trim extra information appended to <code>msg.data</code>.</li>
<li><code>Multicall</code>: Make aware of non-canonical context (i.e. <code>msg.sender</code> is not <code>_msgSender()</code>), allowing compatibility with <code>ERC2771Context</code>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/CHANGELOG.md"><code>@​openzeppelin/contracts</code>'s changelog</a>.</em></p>
<blockquote>
<h2>5.0.2 (2024-02-29)</h2>
<ul>
<li><code>Base64</code>: Fix issue where dirty memory located just after the input buffer is affecting the result. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4926">#4926</a>)</li>
</ul>
<h2>5.0.1 (2023-12-07)</h2>
<ul>
<li><code>ERC2771Context</code> and <code>Context</code>: Introduce a <code>_contextPrefixLength()</code> getter, used to trim extra information appended to <code>msg.data</code>.</li>
<li><code>Multicall</code>: Make aware of non-canonical context (i.e. <code>msg.sender</code> is not <code>_msgSender()</code>), allowing compatibility with <code>ERC2771Context</code>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/dbb6104ce834628e473d2173bbc9d47f81a9eec3"><code>dbb6104</code></a> Release v5.0.2 (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4928">#4928</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/26b4b6099936fc785309f3da118ec8607b6716ed"><code>26b4b60</code></a> Port Base64 tests to truffle (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4926">#4926</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/d4ec2782b724be9e56bf33aa91ff599df185c0b0"><code>d4ec278</code></a> List every contract in each API doc section (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4848">#4848</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/f7bb9881a8d5119b7a1aaf8dc8a589b48bca64dd"><code>f7bb988</code></a> Replace Defender Admin with Transaction Proposals (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4804">#4804</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/e53f81b7044657e4e14e85a587e92a995e2c266b"><code>e53f81b</code></a> Remove Governor's guide ERC6372 disclaimer for Tally (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4801">#4801</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/01ef448981be9d20ca85f2faf6ebdf591ce409f3"><code>01ef448</code></a> Release v5.0.1 (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4785">#4785</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/9ce0340466bb125d6bb9f22bfcb5e37e062e26e2"><code>9ce0340</code></a> Make Multicall context-aware</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/4eb67a408c13e8c67f7b99a9d618aa442ad53a84"><code>4eb67a4</code></a> Close <code>access-control.adoc</code> code block (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4726">#4726</a>) (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4727">#4727</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/83330a6e4c8efeded3ea2b8d6aae5ac2ffc18555"><code>83330a6</code></a> Add <code>AccessManager</code> guide (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4691">#4691</a>) (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4724">#4724</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/ab967b863964b5de4a8be5c30796180a78fb3b6e"><code>ab967b8</code></a> Update the &quot;utilities&quot; documentation page (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4678">#4678</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/compare/v5.0.0...v5.0.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts&package-manager=npm_and_yarn&previous-version=5.0.0&new-version=5.0.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/benchmarking-cross-chain-bridges/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-29 20:11:14 +0000 UTC
    </div>
</div>

