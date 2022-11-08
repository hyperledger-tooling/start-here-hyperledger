---
layout: default
title: blockchain-explorer
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-explorer
---

# blockchain-explorer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-explorer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/308" class=".btn">#308</a>
            </td>
            <td>
                <b>
                    Bump terser from 4.8.0 to 4.8.1 in /client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [terser](https://github.com/terser/terser) from 4.8.0 to 4.8.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/terser/terser/blob/master/CHANGELOG.md">terser's changelog</a>.</em></p>
<blockquote>
<h2>v4.8.1 (backport)</h2>
<ul>
<li>Security fix for RegExps that should not be evaluated (regexp DDOS)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/terser/terser/commit/40674a433e2b2fd9dfe7aaa93a0da224fb5e76b9"><code>40674a4</code></a> update changelog, version</li>
<li><a href="https://github.com/terser/terser/commit/d8cc5691be980d663c29cc4d5ce67e852d597012"><code>d8cc569</code></a> backport fix to potential regexp DDOS</li>
<li>See full diff in <a href="https://github.com/terser/terser/compare/v4.8.0...v4.8.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=terser&package-manager=npm_and_yarn&previous-version=4.8.0&new-version=4.8.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-11-07 14:52:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/307" class=".btn">#307</a>
            </td>
            <td>
                <b>
                    Bump moment-timezone from 0.5.34 to 0.5.35 in /client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [moment-timezone](https://github.com/moment/moment-timezone) from 0.5.34 to 0.5.35.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/moment/moment-timezone/releases">moment-timezone's releases</a>.</em></p>
<blockquote>
<h2>Release 0.5.35</h2>
<ul>
<li>Fix command injection in data pipeline <a href="https://github.com/moment/moment-timezone/security/advisories/GHSA-56x4-j7p9-fcf9">https://github.com/moment/moment-timezone/security/advisories/GHSA-56x4-j7p9-fcf9</a></li>
<li>Fix cleartext transmission of sensitive information <a href="https://github.com/moment/moment-timezone/security/advisories/GHSA-v78c-4p63-2j6c">https://github.com/moment/moment-timezone/security/advisories/GHSA-v78c-4p63-2j6c</a></li>
</ul>
<p>Thanks to the OpenSSF Alpha-Omega project for reporting these!</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/moment/moment-timezone/blob/develop/changelog.md">moment-timezone's changelog</a>.</em></p>
<blockquote>
<h3><code>0.5.35</code> <em>2022-08-23</em></h3>
<ul>
<li>Fix command injection in data pipeline <a href="https://github.com/moment/moment-timezone/security/advisories/GHSA-56x4-j7p9-fcf9">https://github.com/moment/moment-timezone/security/advisories/GHSA-56x4-j7p9-fcf9</a></li>
<li>Fix cleartext transmission of sensitive information <a href="https://github.com/moment/moment-timezone/security/advisories/GHSA-v78c-4p63-2j6c">https://github.com/moment/moment-timezone/security/advisories/GHSA-v78c-4p63-2j6c</a></li>
</ul>
<p>Thanks to the OpenSSF Alpha-Omega project for reporting these!</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/moment/moment-timezone/commit/b8fb1bad6d304f9f085c2fb64b7ea1b6dda47680"><code>b8fb1ba</code></a> Build moment-timezone 0.5.35</li>
<li><a href="https://github.com/moment/moment-timezone/commit/f1b5e5aec11ac5d948f19c7cd0a7c4c6d172c0f7"><code>f1b5e5a</code></a> Add changelog for 0.5.35</li>
<li><a href="https://github.com/moment/moment-timezone/commit/8b0eb0ca6d6ba65f161bd667f98e87221fda0d42"><code>8b0eb0c</code></a> Bump version to 0.5.35</li>
<li><a href="https://github.com/moment/moment-timezone/commit/7915ac567ab19700e44ad6b5d8ef0b85e48a9e75"><code>7915ac5</code></a> Bugfix: Prevent cleartext transmission of tz data during build</li>
<li><a href="https://github.com/moment/moment-timezone/commit/ce955a301ff372e8e9fb3a5b516620c60e7a082a"><code>ce955a3</code></a> Bugfix: Fix command injection vulnerability in grunt tzdata pipeline</li>
<li><a href="https://github.com/moment/moment-timezone/commit/9430b4c2895819e06942096108862374f438a358"><code>9430b4c</code></a> Merge remote-tracking branch 'origin/master' into develop</li>
<li><a href="https://github.com/moment/moment-timezone/commit/feaf90069c469822b2cee35d9d0cd37560d351ef"><code>feaf900</code></a> Updated contributing.md + added 2021e files</li>
<li><a href="https://github.com/moment/moment-timezone/commit/704cfacd51fb175f10b08b36588b6328aeb6447d"><code>704cfac</code></a> updated contributing.md</li>
<li><a href="https://github.com/moment/moment-timezone/commit/877c86344f3f230e1bf5881253c29f89e39fe3d2"><code>877c863</code></a> Updated contributing.md + added 2021e files</li>
<li><a href="https://github.com/moment/moment-timezone/commit/5a3015ce5482b1e9d23c3761dddf4e8fc63e84e6"><code>5a3015c</code></a> updated contributing.md</li>
<li>Additional commits viewable in <a href="https://github.com/moment/moment-timezone/compare/0.5.34...0.5.35">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=moment-timezone&package-manager=npm_and_yarn&previous-version=0.5.34&new-version=0.5.35)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-11-07 14:51:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/306" class=".btn">#306</a>
            </td>
            <td>
                <b>
                    Bump jpeg-js from 0.4.2 to 0.4.4 in /client/e2e-test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [jpeg-js](https://github.com/eugeneware/jpeg-js) from 0.4.2 to 0.4.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/eugeneware/jpeg-js/releases">jpeg-js's releases</a>.</em></p>
<blockquote>
<h2>v0.4.4</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h2><!-- raw HTML omitted -->v0.4.4 (2022-06-07)<!-- raw HTML omitted --></h2>
<ul>
<li>feat: add comment tag encoding (<a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/87">#87</a>) (<a href="https://github.com/eugeneware/jpeg-js/commits/13e1ffa">13e1ffa</a>), closes <a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/87">#87</a></li>
<li>fix: validate sampling factors (<a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/106">#106</a>) (<a href="https://github.com/eugeneware/jpeg-js/commits/9ccd35f">9ccd35f</a>), closes <a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/106">#106</a></li>
<li>fix(decoder): rethrow a more helpful error if Buffer is undefined (<a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/93">#93</a>) (<a href="https://github.com/eugeneware/jpeg-js/commits/b58cc11">b58cc11</a>), closes <a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/93">#93</a></li>
<li>chore(ci): migrate to github actions (<a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/86">#86</a>) (<a href="https://github.com/eugeneware/jpeg-js/commits/417e8e2">417e8e2</a>), closes <a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/86">#86</a></li>
<li>chore(deps): bump y18n from 4.0.0 to 4.0.3 (<a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/98">#98</a>) (<a href="https://github.com/eugeneware/jpeg-js/commits/2c90858">2c90858</a>), closes <a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/98">#98</a></li>
<li>chore(deps): bump ws from 7.2.3 to 7.4.6 (<a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/91">#91</a>) (<a href="https://github.com/eugeneware/jpeg-js/commits/fd73289">fd73289</a>), closes <a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/91">#91</a></li>
<li>chore(deps): bump hosted-git-info from 2.8.8 to 2.8.9 (<a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/90">#90</a>) (<a href="https://github.com/eugeneware/jpeg-js/commits/9449a8b">9449a8b</a>), closes <a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/90">#90</a></li>
<li>chore(deps): bump lodash from 4.17.15 to 4.17.21 (<a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/89">#89</a>) (<a href="https://github.com/eugeneware/jpeg-js/commits/ffdc4a4">ffdc4a4</a>), closes <a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/89">#89</a></li>
</ul>
<h2>v0.4.3</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h2><!-- raw HTML omitted -->v0.4.3 (2021-01-11)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: handle 0x00E1 / 0x00E0 segments from Pixel phones (<a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/84">#84</a>) (<a href="https://github.com/eugeneware/jpeg-js/commits/a2d7ed9">a2d7ed9</a>), closes <a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/84">#84</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jpeg-js/jpeg-js/commit/9ccd35fb5f55a6c4f1902ac5b0f270f675750c27"><code>9ccd35f</code></a> fix: validate sampling factors (<a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/106">#106</a>)</li>
<li><a href="https://github.com/jpeg-js/jpeg-js/commit/b58cc11b29a66f853b4195d31e9e2de6080fcd7a"><code>b58cc11</code></a> fix(decoder): rethrow a more helpful error if Buffer is undefined (<a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/93">#93</a>)</li>
<li><a href="https://github.com/jpeg-js/jpeg-js/commit/2c90858c95832e9fdf49170bcd09f3079567e417"><code>2c90858</code></a> chore(deps): bump y18n from 4.0.0 to 4.0.3 (<a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/98">#98</a>)</li>
<li><a href="https://github.com/jpeg-js/jpeg-js/commit/fd73289664cbdd3d18b5841c49874dfef7ea55fd"><code>fd73289</code></a> chore(deps): bump ws from 7.2.3 to 7.4.6 (<a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/91">#91</a>)</li>
<li><a href="https://github.com/jpeg-js/jpeg-js/commit/9449a8bcda9340b9fd8ca475e2b699fefc2c2828"><code>9449a8b</code></a> chore(deps): bump hosted-git-info from 2.8.8 to 2.8.9 (<a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/90">#90</a>)</li>
<li><a href="https://github.com/jpeg-js/jpeg-js/commit/ffdc4a4d595e1e249a72b08d095363bff739aad7"><code>ffdc4a4</code></a> chore(deps): bump lodash from 4.17.15 to 4.17.21 (<a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/89">#89</a>)</li>
<li><a href="https://github.com/jpeg-js/jpeg-js/commit/13e1ffa04670d7c7a363d54eab92e31f01243cd7"><code>13e1ffa</code></a> feat: add comment tag encoding (<a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/87">#87</a>)</li>
<li><a href="https://github.com/jpeg-js/jpeg-js/commit/417e8e2baff2d1e546fdf68c492fba88205d3fb5"><code>417e8e2</code></a> chore(ci): migrate to github actions (<a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/86">#86</a>)</li>
<li><a href="https://github.com/jpeg-js/jpeg-js/commit/a2d7ed93e5322a98ec1ce953896b2e10b46a5ee1"><code>a2d7ed9</code></a> fix: handle 0x00E1 / 0x00E0 segments from Pixel phones (<a href="https://github-redirect.dependabot.com/eugeneware/jpeg-js/issues/84">#84</a>)</li>
<li>See full diff in <a href="https://github.com/eugeneware/jpeg-js/compare/v0.4.2...v0.4.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jpeg-js&package-manager=npm_and_yarn&previous-version=0.4.2&new-version=0.4.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-11-07 14:51:32 +0000 UTC
    </div>
</div>

