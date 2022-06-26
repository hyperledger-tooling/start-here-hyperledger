---
layout: default
title: aries-framework-javascript-ext
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript-ext
---

# aries-framework-javascript-ext <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript-ext){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/129" class=".btn">#129</a>
            </td>
            <td>
                <b>
                    feat(rest): upgrade to AFJ 0.2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                TODO: Add PR description
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-23 21:34:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/128" class=".btn">#128</a>
            </td>
            <td>
                <b>
                    feat(react-hooks): revocation notification events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Extends PR #114 

* Updates to latest AFJ version
* Fixes validation warnings
* Update credential provider hooks to listen for generic record events over specific state changed/revocation notification events
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-23 21:19:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/127" class=".btn">#127</a>
            </td>
            <td>
                <b>
                    build(deps): bump got from 11.8.3 to 11.8.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [got](https://github.com/sindresorhus/got) from 11.8.3 to 11.8.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sindresorhus/got/releases">got's releases</a>.</em></p>
<blockquote>
<h2>v11.8.5</h2>
<ul>
<li>Backport security fix <a href="https://github.com/sindresorhus/got/commit/861ccd9ac2237df762a9e2beed7edd88c60782dc">https://github.com/sindresorhus/got/commit/861ccd9ac2237df762a9e2beed7edd88c60782dc</a>
<ul>
<li><a href="https://nvd.nist.gov/vuln/detail/CVE-2022-33987">CVE-2022-33987</a></li>
</ul>
</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v11.8.4...v11.8.5">https://github.com/sindresorhus/got/compare/v11.8.4...v11.8.5</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sindresorhus/got/commit/5e17bb748c260b02e4cf716c2f4079a1c6a7481e"><code>5e17bb7</code></a> 11.8.5</li>
<li><a href="https://github.com/sindresorhus/got/commit/bce8ce7d528a675bd5a8d996e110b73674e290d2"><code>bce8ce7</code></a> Backport 861ccd9ac2237df762a9e2beed7edd88c60782dc</li>
<li><a href="https://github.com/sindresorhus/got/commit/8ced19215603f3eda25a9f5dce390f1b152fe9a3"><code>8ced192</code></a> Fix build</li>
<li><a href="https://github.com/sindresorhus/got/commit/670eb04b5b01622f489277d6fb1dd04a41d3cb51"><code>670eb04</code></a> 11.8.4</li>
<li><a href="https://github.com/sindresorhus/got/commit/20f29fe3726a4ddd104f557456dbd5275685e879"><code>20f29fe</code></a> Backport <a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/1543">#1543</a>: Initialize globalResponse in case of ignored HTTPError (<a href="https://github-redirect.dependabot.com/sindresorhus/got/issues/2017">#2017</a>)</li>
<li>See full diff in <a href="https://github.com/sindresorhus/got/compare/v11.8.3...v11.8.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=got&package-manager=npm_and_yarn&previous-version=11.8.3&new-version=11.8.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-javascript-ext/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-23 06:53:58 +0000 UTC
    </div>
</div>

