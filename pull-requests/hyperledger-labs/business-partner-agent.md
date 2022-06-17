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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/766" class=".btn">#766</a>
            </td>
            <td>
                <b>
                    Bump undici from 5.4.0 to 5.5.1 in /frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [undici](https://github.com/nodejs/undici) from 5.4.0 to 5.5.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nodejs/undici/releases">undici's releases</a>.</em></p>
<blockquote>
<h2>v5.5.1</h2>
<h2>⚠️ v5.5.1 - Security release</h2>
<p>This releases fixes CVE CVE-2022-32210. See <a href="https://github.com/nodejs/undici/security/advisories/GHSA-pgw7-wx7w-2w33">https://github.com/nodejs/undici/security/advisories/GHSA-pgw7-wx7w-2w33</a> for more details:</p>
<blockquote>
<p>Undici.ProxyAgent never verifies the remote server's certificate, and always exposes all request &amp; response data to the proxy. This unexpectedly means that proxies can MitM all HTTPS traffic, and if the proxy's URL is HTTP then it also means that nominally HTTPS requests are actually sent via plain-text HTTP between Undici and the proxy server.</p>
</blockquote>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.5.0...v5.5.1">https://github.com/nodejs/undici/compare/v5.5.0...v5.5.1</a></p>
<h2>v5.5.0</h2>
<h2>What's Changed</h2>
<ul>
<li>ci: skip automerge job if user is not dependabot by <a href="https://github.com/Fdawgs"><code>@​Fdawgs</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1478">nodejs/undici#1478</a></li>
<li>test: skip IPv6 tests if not supported by <a href="https://github.com/LiviaMedeiros"><code>@​LiviaMedeiros</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1476">nodejs/undici#1476</a></li>
<li>ci: remove git credentials after checkout by <a href="https://github.com/Fdawgs"><code>@​Fdawgs</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1477">nodejs/undici#1477</a></li>
<li>fix(fetch): typo by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1474">nodejs/undici#1474</a></li>
<li>fix: support <code>TypedArray</code> and <code>DataView</code> as Request body by <a href="https://github.com/LiviaMedeiros"><code>@​LiviaMedeiros</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1472">nodejs/undici#1472</a></li>
<li>fix: connector types by <a href="https://github.com/S222em"><code>@​S222em</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1362">nodejs/undici#1362</a></li>
<li>fix(tests): broken <code>node-fetch</code> tests by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1486">nodejs/undici#1486</a></li>
<li>fix: readme example codestyle by <a href="https://github.com/mainarthur"><code>@​mainarthur</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1488">nodejs/undici#1488</a></li>
<li>feat: implement <code>FormData Iterator</code> by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1473">nodejs/undici#1473</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/LiviaMedeiros"><code>@​LiviaMedeiros</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1476">nodejs/undici#1476</a></li>
<li><a href="https://github.com/S222em"><code>@​S222em</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1362">nodejs/undici#1362</a></li>
<li><a href="https://github.com/mainarthur"><code>@​mainarthur</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1488">nodejs/undici#1488</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.4.0...v5.5.0">https://github.com/nodejs/undici/compare/v5.4.0...v5.5.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nodejs/undici/commit/19563f76ad38a8b4b2b1bfc78957c384775686e3"><code>19563f7</code></a> Bumped v5.5.1</li>
<li><a href="https://github.com/nodejs/undici/commit/6b42910e14b9862525d1416a5441c4888efc0258"><code>6b42910</code></a> Fix support for Node v12</li>
<li><a href="https://github.com/nodejs/undici/commit/6fc7ffbb5203e8d52d98dc20f1eaaceab2668530"><code>6fc7ffb</code></a> test: add rejectUnauthorized for agent1 cert</li>
<li><a href="https://github.com/nodejs/undici/commit/df4f7e0e95f5112322a96fd7a666cb28c1d48327"><code>df4f7e0</code></a> Merge pull request from GHSA-pgw7-wx7w-2w33</li>
<li><a href="https://github.com/nodejs/undici/commit/2717d70b308e2216a3f8cf04bbbf8566f5254a6e"><code>2717d70</code></a> Bumped v5.5.0</li>
<li><a href="https://github.com/nodejs/undici/commit/3fa762e2746eeb98875094ed6db60848b996a91c"><code>3fa762e</code></a> fix: update error messages</li>
<li><a href="https://github.com/nodejs/undici/commit/a6cc7e481ab3f4ba32418cf925bc0a8943f9ed55"><code>a6cc7e4</code></a> feat: add <code>FormData.prototype.forEach</code></li>
<li><a href="https://github.com/nodejs/undici/commit/282a52bc758782dba91fe883140144186f6d71a6"><code>282a52b</code></a> feat: implement <code>FormData Iterator</code></li>
<li><a href="https://github.com/nodejs/undici/commit/30a464b07bbd322e280e04bc203f2eb2988648be"><code>30a464b</code></a> fix: moved async code in examples to top-level-await</li>
<li><a href="https://github.com/nodejs/undici/commit/e00bd1d7043b8954e75a0ff83573f96ae5a08c34"><code>e00bd1d</code></a> fix: readme example codestyle</li>
<li>Additional commits viewable in <a href="https://github.com/nodejs/undici/compare/v5.4.0...v5.5.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=undici&package-manager=npm_and_yarn&previous-version=5.4.0&new-version=5.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/766"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 02:00:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/765" class=".btn">#765</a>
            </td>
            <td>
                <b>
                    fix duplicated api calls on credential request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/765"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 08:59:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/761" class=".btn">#761</a>
            </td>
            <td>
                <b>
                    Fix not all exchanges being removed on partner delete
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-13 13:28:54 +0000 UTC
    </div>
</div>

