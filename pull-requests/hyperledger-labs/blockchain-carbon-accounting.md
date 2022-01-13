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
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/389" class=".btn">#389</a>
            </td>
            <td>
                <b>
                    build(deps): bump @openzeppelin/contracts from 4.4.1 to 4.4.2 in /net-emissions-token-network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) from 4.4.1 to 4.4.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/releases"><code>@​openzeppelin/contracts</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.4.2</h2>
<p>:warning: This is a patch for a medium severity issue. For more information <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-m6w8-fq7v-ph4m">visit the security advisory</a>.</p>
<ul>
<li><code>GovernorCompatibilityBravo</code>: Fix error in the encoding of calldata for proposals submitted through the compatibility interface with explicit signatures. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/%5B#3100%5D(https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3100)">#3100</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/CHANGELOG.md"><code>@​openzeppelin/contracts</code>'s changelog</a>.</em></p>
<blockquote>
<h2>4.4.2 (2022-01-11)</h2>
<h3>Bugfixes</h3>
<ul>
<li><code>GovernorCompatibilityBravo</code>: Fix error in the encoding of calldata for proposals submitted through the compatibility interface with explicit signatures. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/%5B#3100%5D(https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3100)">#3100</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/b53c43242fc9c0e435b66178c3847c4a1b417cc1"><code>b53c432</code></a> 4.4.2</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/9cae52c59135874a75d219b7130d3893103a7c58"><code>9cae52c</code></a> Use abi.encodePacked instead of bytes.concat</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/93d2d1508a69232b87004ebeb6a9e861ea8c2b0b"><code>93d2d15</code></a> Make script executable</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/eff4ad7c1d4e56b27a570b5a15a6c821228387e2"><code>eff4ad7</code></a> Fix encoding of signature+calldata in GovernorCompatibilityBravo (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3100">#3100</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/66436cbb4e757cd79054ab1b1cc38f7f5a948005"><code>66436cb</code></a> Change release script to only update version comment for changed files (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/issues/3033">#3033</a>)</li>
<li>See full diff in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/compare/v4.4.1...v4.4.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts&package-manager=npm_and_yarn&previous-version=4.4.1&new-version=4.4.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-01-13 16:12:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/388" class=".btn">#388</a>
            </td>
            <td>
                <b>
                    build(deps): bump @openzeppelin/contracts-upgradeable from 4.4.1 to 4.4.2 in /net-emissions-token-network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts-upgradeable](https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable) from 4.4.1 to 4.4.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/releases"><code>@​openzeppelin/contracts-upgradeable</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.4.2</h2>
<p>:warning: This is a patch for a medium severity issue. For more information <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/security/advisories/GHSA-m6w8-fq7v-ph4m">visit the security advisory</a>.</p>
<ul>
<li><code>GovernorCompatibilityBravo</code>: Fix error in the encoding of calldata for proposals submitted through the compatibility interface with explicit signatures. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/%5B#3100%5D(https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts-upgradeable/issues/3100)">#3100</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/blob/master/CHANGELOG.md"><code>@​openzeppelin/contracts-upgradeable</code>'s changelog</a>.</em></p>
<blockquote>
<h2>4.4.2 (2022-01-11)</h2>
<h3>Bugfixes</h3>
<ul>
<li><code>GovernorCompatibilityBravo</code>: Fix error in the encoding of calldata for proposals submitted through the compatibility interface with explicit signatures. (<a href="https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts/pull/%5B#3100%5D(https://github-redirect.dependabot.com/OpenZeppelin/openzeppelin-contracts-upgradeable/issues/3100)">#3100</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/commit/06ab69e525435f2f4487e72676522fda670244cb"><code>06ab69e</code></a> Transpile 79cb606f</li>
<li>See full diff in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/compare/v4.4.1...v4.4.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts-upgradeable&package-manager=npm_and_yarn&previous-version=4.4.1&new-version=4.4.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-01-13 16:10:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/387" class=".btn">#387</a>
            </td>
            <td>
                <b>
                    Updates to CarbonTraker NFT contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit introduces major changes to the CarbonTracker contract
It also updates carbon-tracker.md describing how the CarbonTracker contract works in more detail
This includes mathmatical forumlae for how carbon intensities and emissions are calculated across tracker NFTs
and a diagram with a basic fuel supply chain example

Signed-off-by: brioux <Bertrand.rioux@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-13 10:43:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/384" class=".btn">#384</a>
            </td>
            <td>
                <b>
                    Initial UI for carbon tracker 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Assigning roles is not working yet but you can issue tokens and see them.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-11 00:56:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/382" class=".btn">#382</a>
            </td>
            <td>
                <b>
                    feat(scripts): Add script for packaging and installing chaincode locally
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added a script that executes the Fabric chaincode lifecycle locally instead of using the chaincode from an external container, so that changes in the chaincode may be tested out quickly. Now the chaincode is installed directly on the peer itself, and the created dev-peer containers may be used for easily debugging chaincode.

Closes #376. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-10 09:08:24 +0000 UTC
    </div>
</div>

