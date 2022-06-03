---
layout: default
title: business-partner-agent
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/business-partner-agent
---

# business-partner-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/business-partner-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/758" class=".btn">#758</a>
            </td>
            <td>
                <b>
                    latest working node version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/758"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-02 15:17:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/757" class=".btn">#757</a>
            </td>
            <td>
                <b>
                    Fix Frontend Build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                build does not work any more with latest node version 16.15.1 with npm 8.11 as it breaks the whole dependency tree. The attached changes fix the build, but introduce loads of unneeded dependencies. The proper fix is properly the upgrade to vue3 as we have many very old dependencies lying around.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-02 14:52:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/756" class=".btn">#756</a>
            </td>
            <td>
                <b>
                    Bump eventsource from 1.1.0 to 1.1.1 in /frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [eventsource](https://github.com/EventSource/eventsource) from 1.1.0 to 1.1.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/EventSource/eventsource/blob/master/HISTORY.md">eventsource's changelog</a>.</em></p>
<blockquote>
<h1><a href="https://github.com/EventSource/eventsource/compare/v1.1.0...v1.1.1">1.1.1</a></h1>
<ul>
<li>Do not include authorization and cookie headers on redirect to different origin (<a href="https://github-redirect.dependabot.com/EventSource/eventsource/pull/273">#273</a> Espen Hovlandsdal)</li>
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
<li>See full diff in <a href="https://github.com/EventSource/eventsource/compare/v1.1.0...v1.1.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=eventsource&package-manager=npm_and_yarn&previous-version=1.1.0&new-version=1.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/business-partner-agent/network/alerts).

</details>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/756"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-01 22:14:41 +0000 UTC
    </div>
</div>

