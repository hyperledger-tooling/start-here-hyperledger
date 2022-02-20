---
layout: default
title: blockchain-explorer
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/blockchain-explorer
---

# blockchain-explorer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/blockchain-explorer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/blockchain-explorer/pull/279" class=".btn">#279</a>
            </td>
            <td>
                <b>
                    Deleted $ symbols from wget commands, it doesn't work if we use copy …
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …and paste on terminal

By removing $, all 3 statements can be copied and pasted easily, without requirement to delete it manually
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-20 13:46:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/blockchain-explorer/pull/278" class=".btn">#278</a>
            </td>
            <td>
                <b>
                    Bump url-parse from 1.5.3 to 1.5.7 in /client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [url-parse](https://github.com/unshiftio/url-parse) from 1.5.3 to 1.5.7.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/unshiftio/url-parse/commit/8b3f5f2c88a4cfc2880f2319c307994cb25bb10a"><code>8b3f5f2</code></a> 1.5.7</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/ef45a1355375a8244063793a19059b4f62fc8788"><code>ef45a13</code></a> [fix] Readd the empty userinfo to <code>url.href</code> (<a href="https://github-redirect.dependabot.com/unshiftio/url-parse/issues/226">#226</a>)</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/88df2346855f70cec9713b362ca32a4691dc271a"><code>88df234</code></a> [doc] Add soft deprecation notice</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/78e9f2f41285d83e7d91706be5bd439656fe3bc3"><code>78e9f2f</code></a> [security] Fix nits</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/e6fa43422c52f34c73146552ec9916125dc59525"><code>e6fa434</code></a> [security] Add credits for incorrect handling of userinfo vulnerability</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/4c9fa234c01dca52698666378360ad2fdfb05470"><code>4c9fa23</code></a> 1.5.6</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/7b0b8a6671f806458e88b1f44feb0fdd742cdf06"><code>7b0b8a6</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/unshiftio/url-parse/issues/223">#223</a> from unshiftio/fix/at-sign-handling-in-userinfo</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/e4a5807d95b971577e4d888f5b99d64a40851386"><code>e4a5807</code></a> 1.5.5</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/193b44baf3d203560735e05eedc99d8244c9e16c"><code>193b44b</code></a> [minor] Simplify whitespace regex</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/319851bf1c294796fc73e29ff31b14d9084e4a0d"><code>319851b</code></a> [fix] Remove CR, HT, and LF</li>
<li>Additional commits viewable in <a href="https://github.com/unshiftio/url-parse/compare/1.5.3...1.5.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=url-parse&package-manager=npm_and_yarn&previous-version=1.5.3&new-version=1.5.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/blockchain-explorer/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-17 15:17:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/blockchain-explorer/pull/277" class=".btn">#277</a>
            </td>
            <td>
                <b>
                    Bump follow-redirects from 1.14.7 to 1.14.8
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [follow-redirects](https://github.com/follow-redirects/follow-redirects) from 1.14.7 to 1.14.8.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/3d81dc3237b4ffe8b722bb3d1c70a7866657166e"><code>3d81dc3</code></a> Release version 1.14.8 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/62e546a99c07c3ee5e4e0718c84a6ca127c5c445"><code>62e546a</code></a> Drop confidential headers across schemes.</li>
<li>See full diff in <a href="https://github.com/follow-redirects/follow-redirects/compare/v1.14.7...v1.14.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=follow-redirects&package-manager=npm_and_yarn&previous-version=1.14.7&new-version=1.14.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/blockchain-explorer/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-14 08:21:37 +0000 UTC
    </div>
</div>

