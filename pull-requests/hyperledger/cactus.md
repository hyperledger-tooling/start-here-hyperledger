---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2147" class=".btn">#2147</a>
            </td>
            <td>
                <b>
                    build(deps): bump @openzeppelin/contracts from 4.7.1 to 4.7.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) from 4.7.1 to 4.7.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/releases"><code>@​openzeppelin/contracts</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.7.2</h2>
<p>:warning: This is a patch for three issues, including a high severity issue in <code>GovernorVotesQuorumFraction</code>. For more information visit the security advisories (<a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-xrc4-737v-9q75">1</a>, <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-7grf-83vw-6f5x">2</a>, <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-9j3m-g383-29qr">3</a>).</p>
<ol>
<li><code>GovernorVotesQuorumFraction</code>: Fixed quorum updates so they do not affect past proposals that failed due to lack of quorum. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3561">#3561</a>)</li>
<li><code>ERC165Checker</code>: Added protection against large returndata. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3587">#3587</a>)</li>
<li><code>LibArbitrumL2</code>, <code>CrossChainEnabledArbitrumL2</code>: Fixed detection of cross-chain calls for EOAs. Previously, calls from EOAs would be classified as cross-chain calls. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3578">#3578</a>)</li>
</ol>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/CHANGELOG.md"><code>@​openzeppelin/contracts</code>'s changelog</a>.</em></p>
<blockquote>
<h2>4.7.2</h2>
<ul>
<li><code>LibArbitrumL2</code>, <code>CrossChainEnabledArbitrumL2</code>: Fixed detection of cross-chain calls for EOAs. Previously, calls from EOAs would be classified as cross-chain calls. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3578">#3578</a>)</li>
<li><code>GovernorVotesQuorumFraction</code>: Fixed quorum updates so they do not affect past proposals that failed due to lack of quorum. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3561">#3561</a>)</li>
<li><code>ERC165Checker</code>: Added protection against large returndata. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3587">#3587</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/64e48203cecad94f02de9891ecdeed4d629c6dae"><code>64e4820</code></a> 4.7.2</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/b66fe1606a173f2b78694567b543d480cb39cfe4"><code>b66fe16</code></a> Update changelog</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/8fb5f5774e3e8cfc10699f58749d8a34ec9d3e86"><code>8fb5f57</code></a> Avoid returnbomb in ERC165Checker (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3587">#3587</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/67b2572c6a050563990637f5017af8eeda111b21"><code>67b2572</code></a> Keep track of historical quorum values (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3561">#3561</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/4337192dc02b64785885787e80126f93ee3f2659"><code>4337192</code></a> Fix arbitrum L1 to L2 crosschain call detection (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3578">#3578</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/41c7b25a65f636feaef7f0dc932ec4c44baa12f3"><code>41c7b25</code></a> Fix error in documentation and typo (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3567">#3567</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/e15862f2893f024e0872f0f1abcf275c4b436834"><code>e15862f</code></a> Remove test for feature not in 4.7</li>
<li>See full diff in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/compare/v4.7.1...v4.7.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts&package-manager=npm_and_yarn&previous-version=4.7.1&new-version=4.7.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cactus/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-14 00:38:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2146" class=".btn">#2146</a>
            </td>
            <td>
                <b>
                    build(deps): bump @openzeppelin/contracts-upgradeable from 4.7.1 to 4.7.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts-upgradeable](https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable) from 4.7.1 to 4.7.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/releases"><code>@​openzeppelin/contracts-upgradeable</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.7.2</h2>
<p>:warning: This is a patch for three issues, including a high severity issue in <code>GovernorVotesQuorumFraction</code>. For more information visit the security advisories (<a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-xrc4-737v-9q75">1</a>, <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-7grf-83vw-6f5x">2</a>, <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-9j3m-g383-29qr">3</a>).</p>
<ol>
<li><code>GovernorVotesQuorumFraction</code>: Fixed quorum updates so they do not affect past proposals that failed due to lack of quorum. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3561">#3561</a>)</li>
<li><code>ERC165Checker</code>: Added protection against large returndata. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3587">#3587</a>)</li>
<li><code>LibArbitrumL2</code>, <code>CrossChainEnabledArbitrumL2</code>: Fixed detection of cross-chain calls for EOAs. Previously, calls from EOAs would be classified as cross-chain calls. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3578">#3578</a>)</li>
</ol>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/blob/master/CHANGELOG.md"><code>@​openzeppelin/contracts-upgradeable</code>'s changelog</a>.</em></p>
<blockquote>
<h2>4.7.2</h2>
<ul>
<li><code>LibArbitrumL2</code>, <code>CrossChainEnabledArbitrumL2</code>: Fixed detection of cross-chain calls for EOAs. Previously, calls from EOAs would be classified as cross-chain calls. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3578">#3578</a>)</li>
<li><code>GovernorVotesQuorumFraction</code>: Fixed quorum updates so they do not affect past proposals that failed due to lack of quorum. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3561">#3561</a>)</li>
<li><code>ERC165Checker</code>: Added protection against large returndata. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/3587">#3587</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/12ad9ea7c8e8e78f6eba9ad71ad156645d3c5b4c"><code>12ad9ea</code></a> Transpile dc57a7ea</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/5843c07216c63c46b0b8a598b889667537070440"><code>5843c07</code></a> Transpile 6b9fbb14</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/e2bcd078fe446b4eb3f7b35ac48d31bc7c862ebe"><code>e2bcd07</code></a> Transpile e64bfd92</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/da834e3976e5421747bdb76ed40c51463a132c74"><code>da834e3</code></a> Transpile b19184c5</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/e12164187031c97601490172bcb4e9a6b7ca3c78"><code>e121641</code></a> Transpile 4e23f642</li>
<li>See full diff in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/compare/v4.7.1...v4.7.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts-upgradeable&package-manager=npm_and_yarn&previous-version=4.7.1&new-version=4.7.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cactus/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-14 00:38:09 +0000 UTC
    </div>
</div>

