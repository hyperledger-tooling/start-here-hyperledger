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
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/33" class=".btn">#33</a>
            </td>
            <td>
                <b>
                    Add support for approvals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Both ERC20 and ERC721 support an "infinite" approval.

ERC20 also supports an approval with a fixed allowance, and
ERC721 supports appointing a single approved operator per NFT.
These can be set with extra "config" parameters.

Resolves #29

Did not add any new tests yet (only patched the existing ones).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 03:02:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/32" class=".btn">#32</a>
            </td>
            <td>
                <b>
                    Bump simple-get from 2.8.1 to 2.8.2 in /solidity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [simple-get](https://github.com/feross/simple-get) from 2.8.1 to 2.8.2.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/feross/simple-get/commit/4e156b6bb19e11ccfad05fad310ea799d63f890d"><code>4e156b6</code></a> 2.8.2</li>
<li><a href="https://github.com/feross/simple-get/commit/43c272db3e4b1383cb03d80338dba3e08c451641"><code>43c272d</code></a> Bug fix: Thirdparty cookie leak</li>
<li>See full diff in <a href="https://github.com/feross/simple-get/compare/v2.8.1...v2.8.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~linusu">linusu</a>, a new releaser for simple-get since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=simple-get&package-manager=npm_and_yarn&previous-version=2.8.1&new-version=2.8.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-03-18 02:48:48 +0000 UTC
    </div>
</div>

