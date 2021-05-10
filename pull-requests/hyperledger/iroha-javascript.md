---
layout: default
title: iroha-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-javascript
---

# iroha-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-javascript/pull/56" class=".btn">#56</a>
            </td>
            <td>
                <b>
                    Bump hosted-git-info from 2.8.8 to 2.8.9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [hosted-git-info](https://github.com/npm/hosted-git-info) from 2.8.8 to 2.8.9.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/npm/hosted-git-info/blob/v2.8.9/CHANGELOG.md">hosted-git-info's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/npm/hosted-git-info/compare/v2.8.8...v2.8.9">2.8.9</a> (2021-04-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>backport regex fix from <a href="https://github-redirect.dependabot.com/npm/hosted-git-info/issues/76">#76</a> (<a href="https://github.com/npm/hosted-git-info/commit/29adfe5">29adfe5</a>), closes <a href="https://github-redirect.dependabot.com/npm/hosted-git-info/issues/84">#84</a></li>
</ul>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/hosted-git-info/commit/8d4b3697d79bcd89cdb36d1db165e3696c783a01"><code>8d4b369</code></a> chore(release): 2.8.9</li>
<li><a href="https://github.com/npm/hosted-git-info/commit/29adfe5ef789784c861b2cdeb15051ec2ba651a7"><code>29adfe5</code></a> fix: backport regex fix from <a href="https://github-redirect.dependabot.com/npm/hosted-git-info/issues/76">#76</a></li>
<li>See full diff in <a href="https://github.com/npm/hosted-git-info/compare/v2.8.8...v2.8.9">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~nlf">nlf</a>, a new releaser for hosted-git-info since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=hosted-git-info&package-manager=npm_and_yarn&previous-version=2.8.8&new-version=2.8.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/iroha-javascript/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-10 03:49:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-javascript/pull/55" class=".btn">#55</a>
            </td>
            <td>
                <b>
                    Bump lodash from 4.17.20 to 4.17.21
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [lodash](https://github.com/lodash/lodash) from 4.17.20 to 4.17.21.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/lodash/lodash/commit/f299b52f39486275a9e6483b60a410e06520c538"><code>f299b52</code></a> Bump to v4.17.21</li>
<li><a href="https://github.com/lodash/lodash/commit/c4847ebe7d14540bb28a8b932a9ce1b9ecbfee1a"><code>c4847eb</code></a> Improve performance of <code>toNumber</code>, <code>trim</code> and <code>trimEnd</code> on large input strings</li>
<li><a href="https://github.com/lodash/lodash/commit/3469357cff396a26c363f8c1b5a91dde28ba4b1c"><code>3469357</code></a> Prevent command injection through <code>_.template</code>'s <code>variable</code> option</li>
<li>See full diff in <a href="https://github.com/lodash/lodash/compare/4.17.20...4.17.21">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=lodash&package-manager=npm_and_yarn&previous-version=4.17.20&new-version=4.17.21)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/iroha-javascript/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-08 10:57:57 +0000 UTC
    </div>
</div>

