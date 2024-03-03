---
layout: default
title: learning-tokens
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/learning-tokens
---

# learning-tokens <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/learning-tokens){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/learning-tokens/pull/24" class=".btn">#24</a>
            </td>
            <td>
                <b>
                    Update README.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Includes all comments and suggestions from Diana and Jackson. It moves figures and tables to their correct location. It includes the Authors section. (NOTE) We still need to verify that the TTF link provided by GBBC includes OUR Learning Tokens
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-02 18:30:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/learning-tokens/pull/23" class=".btn">#23</a>
            </td>
            <td>
                <b>
                    Update README.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                28 Footnotes numbers included in the text
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-02 12:59:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/learning-tokens/pull/22" class=".btn">#22</a>
            </td>
            <td>
                <b>
                    Update README.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                updating the numbers within the text to reference endnotes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-01 16:23:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/learning-tokens/pull/21" class=".btn">#21</a>
            </td>
            <td>
                <b>
                    Bump @openzeppelin/contracts from 4.9.3 to 4.9.6 in /src/learning-token
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) from 4.9.3 to 4.9.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/releases"><code>@​openzeppelin/contracts</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.9.6</h2>
<ul>
<li><code>Base64</code>: Fix issue where dirty memory located just after the input buffer is affecting the result. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4929">#4929</a>)</li>
</ul>
<h2>v4.9.5</h2>
<ul>
<li><code>Multicall</code>: Make aware of non-canonical context (i.e. <code>msg.sender</code> is not <code>_msgSender()</code>), allowing compatibility with <code>ERC2771Context</code>. Patch duplicated <code>Address.functionDelegateCall</code> in v4.9.4 (removed).</li>
</ul>
<h2>v4.9.4</h2>
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
<h2>4.9.6 (2024-02-29)</h2>
<ul>
<li><code>Base64</code>: Fix issue where dirty memory located just after the input buffer is affecting the result. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4929">#4929</a>)</li>
</ul>
<h2>4.9.5 (2023-12-08)</h2>
<ul>
<li><code>Multicall</code>: Make aware of non-canonical context (i.e. <code>msg.sender</code> is not <code>_msgSender()</code>), allowing compatibility with <code>ERC2771Context</code>. Patch duplicated <code>Address.functionDelegateCall</code> in v4.9.4 (removed).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/dc44c9f1a4c3b10af99492eed84f83ed244203f6"><code>dc44c9f</code></a> Release v4.9.6 (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4931">#4931</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/a6286d0fded8771b3a645e5813e51993c490399c"><code>a6286d0</code></a> Port Base64 tests to truffle (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4926">#4926</a>) (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4929">#4929</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/bd325d56b4c62c9c5c1aff048c37c6bb18ac0290"><code>bd325d5</code></a> Release v4.9.5 (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4790">#4790</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/ad6a5b6893c2c04217ba3f01c7d05331d017cf2f"><code>ad6a5b6</code></a> Add changeset</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/88ac712e06832bce73b41e8166cded2729e25205"><code>88ac712</code></a> Replace double <code>functionDelegateCall</code></li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/a83918df1491d9c6a642a16f8c9a8ff93bf042cc"><code>a83918d</code></a> Bump node CI version to 16.x</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/0d5f54e69b2a2058bc98651a2e200f558c84a953"><code>0d5f54e</code></a> Release v4.9.4 (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4784">#4784</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/ccfffe13e815f2e8eba20d3ab16d568557e97dd6"><code>ccfffe1</code></a> Make Multicall context-aware</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/9329cfacd4c7d20bcb43d772d947ff9e39b65df9"><code>9329cfa</code></a> Remove Wizard page from 4.x</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/e1b3d8c7ee2c97868f4ab107fe8b7e19f0a8db9f"><code>e1b3d8c</code></a> Remove Wizard from 4.x navigation</li>
<li>Additional commits viewable in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/compare/v4.9.3...v4.9.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts&package-manager=npm_and_yarn&previous-version=4.9.3&new-version=4.9.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/learning-tokens/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-29 20:40:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/learning-tokens/pull/20" class=".btn">#20</a>
            </td>
            <td>
                <b>
                    Bump @openzeppelin/contracts from 4.9.3 to 4.9.6 in /src/quorum-test-network/dapps/quorumToken
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [@openzeppelin/contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) from 4.9.3 to 4.9.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/releases"><code>@​openzeppelin/contracts</code>'s releases</a>.</em></p>
<blockquote>
<h2>v4.9.6</h2>
<ul>
<li><code>Base64</code>: Fix issue where dirty memory located just after the input buffer is affecting the result. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4929">#4929</a>)</li>
</ul>
<h2>v4.9.5</h2>
<ul>
<li><code>Multicall</code>: Make aware of non-canonical context (i.e. <code>msg.sender</code> is not <code>_msgSender()</code>), allowing compatibility with <code>ERC2771Context</code>. Patch duplicated <code>Address.functionDelegateCall</code> in v4.9.4 (removed).</li>
</ul>
<h2>v4.9.4</h2>
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
<h2>4.9.6 (2024-02-29)</h2>
<ul>
<li><code>Base64</code>: Fix issue where dirty memory located just after the input buffer is affecting the result. (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/pull/4929">#4929</a>)</li>
</ul>
<h2>4.9.5 (2023-12-08)</h2>
<ul>
<li><code>Multicall</code>: Make aware of non-canonical context (i.e. <code>msg.sender</code> is not <code>_msgSender()</code>), allowing compatibility with <code>ERC2771Context</code>. Patch duplicated <code>Address.functionDelegateCall</code> in v4.9.4 (removed).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/dc44c9f1a4c3b10af99492eed84f83ed244203f6"><code>dc44c9f</code></a> Release v4.9.6 (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4931">#4931</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/a6286d0fded8771b3a645e5813e51993c490399c"><code>a6286d0</code></a> Port Base64 tests to truffle (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4926">#4926</a>) (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4929">#4929</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/bd325d56b4c62c9c5c1aff048c37c6bb18ac0290"><code>bd325d5</code></a> Release v4.9.5 (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4790">#4790</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/ad6a5b6893c2c04217ba3f01c7d05331d017cf2f"><code>ad6a5b6</code></a> Add changeset</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/88ac712e06832bce73b41e8166cded2729e25205"><code>88ac712</code></a> Replace double <code>functionDelegateCall</code></li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/a83918df1491d9c6a642a16f8c9a8ff93bf042cc"><code>a83918d</code></a> Bump node CI version to 16.x</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/0d5f54e69b2a2058bc98651a2e200f558c84a953"><code>0d5f54e</code></a> Release v4.9.4 (<a href="https://redirect.github.com/OpenZeppelin/openzeppelin-contracts/issues/4784">#4784</a>)</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/ccfffe13e815f2e8eba20d3ab16d568557e97dd6"><code>ccfffe1</code></a> Make Multicall context-aware</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/9329cfacd4c7d20bcb43d772d947ff9e39b65df9"><code>9329cfa</code></a> Remove Wizard page from 4.x</li>
<li><a href="https://github.com/OpenZeppelin/openzeppelin-contracts/commit/e1b3d8c7ee2c97868f4ab107fe8b7e19f0a8db9f"><code>e1b3d8c</code></a> Remove Wizard from 4.x navigation</li>
<li>Additional commits viewable in <a href="https://github.com/OpenZeppelin/openzeppelin-contracts/compare/v4.9.3...v4.9.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@openzeppelin/contracts&package-manager=npm_and_yarn&previous-version=4.9.3&new-version=4.9.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/learning-tokens/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-29 20:39:40 +0000 UTC
    </div>
</div>

