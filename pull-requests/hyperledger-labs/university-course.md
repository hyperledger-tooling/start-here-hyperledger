---
layout: default
title: university-course
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/university-course
---

# university-course <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/university-course){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/university-course/pull/77" class=".btn">#77</a>
            </td>
            <td>
                <b>
                    chore(deps): bump eventsource from 1.0.7 to 1.1.1 in /support/Lab06/b4s/organization/university/user-interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [eventsource](https://github.com/EventSource/eventsource) from 1.0.7 to 1.1.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/EventSource/eventsource/blob/master/HISTORY.md">eventsource's changelog</a>.</em></p>
<blockquote>
<h1><a href="https://github.com/EventSource/eventsource/compare/v1.1.0...v1.1.1">1.1.1</a></h1>
<ul>
<li>Do not include authorization and cookie headers on redirect to different origin (<a href="https://github-redirect.dependabot.com/EventSource/eventsource/pull/273">#273</a> Espen Hovlandsdal)</li>
</ul>
<h1><a href="https://github.com/EventSource/eventsource/compare/v1.0.7...v1.1.0">1.1.0</a></h1>
<ul>
<li>Improve performance for large messages across many chunks (<a href="https://github-redirect.dependabot.com/EventSource/eventsource/pull/130">#130</a> Trent Willis)</li>
<li>Add <code>createConnection</code> option for http or https requests (<a href="https://github-redirect.dependabot.com/EventSource/eventsource/pull/120">#120</a> Vasily Lavrov)</li>
<li>Support HTTP 302 redirects (<a href="https://github-redirect.dependabot.com/EventSource/eventsource/pull/116">#116</a> Ryan Bonte)</li>
<li>Prevent sequential errors from attempting multiple reconnections (<a href="https://github-redirect.dependabot.com/EventSource/eventsource/pull/125">#125</a> David Patty)</li>
<li>Add <code>new</code> to correct test (<a href="https://github-redirect.dependabot.com/EventSource/eventsource/pull/101">#111</a> Stéphane Alnet)</li>
<li>Fix reconnections attempts now happen more than once (<a href="https://github-redirect.dependabot.com/EventSource/eventsource/pull/136">#136</a> Icy Fish)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/EventSource/eventsource/commit/aa7a40843a978f42c0babdec125bf9e0a83bf515"><code>aa7a408</code></a> 1.1.1</li>
<li><a href="https://github.com/EventSource/eventsource/commit/56d489ef853a891deca121bbd463c732fee94dce"><code>56d489e</code></a> chore: rebuild polyfill</li>
<li><a href="https://github.com/EventSource/eventsource/commit/4a951e58b04118c9c4d3da3d27d454972a1b4b8d"><code>4a951e5</code></a> docs: update history for 1.1.1</li>
<li><a href="https://github.com/EventSource/eventsource/commit/f9f6416567bff62c1af2f4314be51d9870e94bc2"><code>f9f6416</code></a> fix: strip sensitive headers on redirect to different origin</li>
<li><a href="https://github.com/EventSource/eventsource/commit/9dd06876ab43af37c3313c679fbdc7f722293a0d"><code>9dd0687</code></a> 1.1.0</li>
<li><a href="https://github.com/EventSource/eventsource/commit/49497ba7107a7a94d7dbc73b6e5cc0117f8606e8"><code>49497ba</code></a> Update history for 1.1.0 (<a href="https://github-redirect.dependabot.com/EventSource/eventsource/issues/146">#146</a>)</li>
<li><a href="https://github.com/EventSource/eventsource/commit/3a3853793f63eb5dab9d863504817a9d37b992e6"><code>3a38537</code></a> Update history for <a href="https://github-redirect.dependabot.com/EventSource/eventsource/issues/136">#136</a></li>
<li><a href="https://github.com/EventSource/eventsource/commit/46fe04e03e54f4129a28bf75b3a1e5f4ab68b52a"><code>46fe04e</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/EventSource/eventsource/issues/136">#136</a> from icy-fish/master</li>
<li><a href="https://github.com/EventSource/eventsource/commit/9a4190f65e761ee672d786a6d01c60392950064b"><code>9a4190f</code></a> Fix issue: reconnection only happends for 1 time after connection drops</li>
<li><a href="https://github.com/EventSource/eventsource/commit/61e1b19c8616aa151835a4ae599b299afb574ebf"><code>61e1b19</code></a> test: destroy both proxied request and response on close</li>
<li>Additional commits viewable in <a href="https://github.com/EventSource/eventsource/compare/v1.0.7...v1.1.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=eventsource&package-manager=npm_and_yarn&previous-version=1.0.7&new-version=1.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/university-course/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-01 20:11:45 +0000 UTC
    </div>
</div>

