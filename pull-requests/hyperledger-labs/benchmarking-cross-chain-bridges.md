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
                PR <a href="https://github.com/hyperledger-labs/benchmarking-cross-chain-bridges/pull/8" class=".btn">#8</a>
            </td>
            <td>
                <b>
                    refactor: yarn update and variable name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1) Upgraded packages 
2) Refactored chainlink contracts to be compatible with refactor
3) Protocol Route, Quote, etc types start with ProtocolName as prefix ex: Quote is now COWQuote or LIFIQuote
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-29 17:39:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/benchmarking-cross-chain-bridges/pull/7" class=".btn">#7</a>
            </td>
            <td>
                <b>
                    feat: uniswap swap execution
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1) added uniswap swaps
2) increased test async wait to 100,000ms from 30,000ms (uniswap multihop sometimes takes a while) 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-29 17:04:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/benchmarking-cross-chain-bridges/pull/6" class=".btn">#6</a>
            </td>
            <td>
                <b>
                    chore(deps): bump get-func-name from 2.0.0 to 2.0.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [get-func-name](https://github.com/chaijs/get-func-name) from 2.0.0 to 2.0.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/chaijs/get-func-name/releases">get-func-name's releases</a>.</em></p>
<blockquote>
<h2>v2.0.2</h2>
<h2>What's Changed</h2>
<p>Revert previous changes that shipped this as an ES module.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/chaijs/get-func-name/commits/v2.0.2">https://github.com/chaijs/get-func-name/commits/v2.0.2</a></p>
<h2>v2.0.1</h2>
<h2>What's Changed</h2>
<p>Fix <a href="https://github.com/chaijs/get-func-name/security/advisories/GHSA-4q6p-r6v2-jvc5">https://github.com/chaijs/get-func-name/security/advisories/GHSA-4q6p-r6v2-jvc5</a></p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/chaijs/get-func-name/commits/v2.0.1">https://github.com/chaijs/get-func-name/commits/v2.0.1</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/chaijs/get-func-name/commits/v2.0.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~keithamus">keithamus</a>, a new releaser for get-func-name since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=get-func-name&package-manager=npm_and_yarn&previous-version=2.0.0&new-version=2.0.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-09-27 23:52:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/benchmarking-cross-chain-bridges/pull/5" class=".btn">#5</a>
            </td>
            <td>
                <b>
                    LiFi swaps work
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1) swapping on lifi works 
2) added checks for same chain swaps where user can't swap the a token for the same token on the same chain but can across different chains
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-27 15:14:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/benchmarking-cross-chain-bridges/pull/4" class=".btn">#4</a>
            </td>
            <td>
                <b>
                    token swapping on cowswap protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added:
1) ERC20 allowance using openzeppelin 
2) Returns a cowswap route id when the execute_route.test.ts test is unskipped
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-25 14:13:18 +0000 UTC
    </div>
</div>

