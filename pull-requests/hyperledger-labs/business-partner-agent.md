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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/786" class=".btn">#786</a>
            </td>
            <td>
                <b>
                    Bump undici from 5.5.1 to 5.8.0 in /frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [undici](https://github.com/nodejs/undici) from 5.5.1 to 5.8.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nodejs/undici/releases">undici's releases</a>.</em></p>
<blockquote>
<h2>v5.8.0</h2>
<h2>⚠️ Security Fixes ⚠️</h2>
<ul>
<li>CRLF injection in request path, method, and headers <a href="https://github.com/nodejs/undici/security/advisories/GHSA-3cvr-822r-rqcc">https://github.com/nodejs/undici/security/advisories/GHSA-3cvr-822r-rqcc</a>, CVE CVE-2022-31150, reported by <a href="https://github.com/Haxatron"><code>@​Haxatron</code></a></li>
<li>Cookies uncleared on cross-host / cross-origin redirect <a href="https://github.com/nodejs/undici/security/advisories/GHSA-q768-x9m6-m9qp">https://github.com/nodejs/undici/security/advisories/GHSA-q768-x9m6-m9qp</a>, CVE CVE-2022-31150, reported by <a href="https://github.com/Haxatron"><code>@​Haxatron</code></a></li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>Drop PR title validation by <a href="https://github.com/mcollina"><code>@​mcollina</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1543">nodejs/undici#1543</a></li>
<li>chore: exclude windows node 16 by <a href="https://github.com/mcollina"><code>@​mcollina</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1542">nodejs/undici#1542</a></li>
<li>feat: use weighted round robin in balancedPool by <a href="https://github.com/jodevsa"><code>@​jodevsa</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1069">nodejs/undici#1069</a></li>
<li>Fix up <code>exclude</code> in CI by <a href="https://github.com/dominykas"><code>@​dominykas</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1544">nodejs/undici#1544</a></li>
<li>fix(mock utils): set Readable.abort by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1549">nodejs/undici#1549</a></li>
<li>fix(body mixin): only allow Uint8Array chunks by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1550">nodejs/undici#1550</a></li>
<li>docs: updated proxy docs - renamed already used const proxy to proxyServer by <a href="https://github.com/dancastillo"><code>@​dancastillo</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1552">nodejs/undici#1552</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/jodevsa"><code>@​jodevsa</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1069">nodejs/undici#1069</a></li>
<li><a href="https://github.com/dancastillo"><code>@​dancastillo</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1552">nodejs/undici#1552</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.7.0...v5.7.1">https://github.com/nodejs/undici/compare/v5.7.0...v5.7.1</a></p>
<h2>v5.7.0</h2>
<h2>What's Changed</h2>
<ul>
<li>fix(fetch): re-add support for node v16.8.0+ by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1534">nodejs/undici#1534</a></li>
<li>fix(Headers): lowercase name in <code>Headers.prototype.set</code> by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1535">nodejs/undici#1535</a></li>
<li>fix: allow optional body for mock reply by <a href="https://github.com/JustinBeckwith"><code>@​JustinBeckwith</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1536">nodejs/undici#1536</a></li>
<li>fix: faster direct read approach by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1537">nodejs/undici#1537</a></li>
<li>feat: update to llhttp v6.0.7 by <a href="https://github.com/mcollina"><code>@​mcollina</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1539">nodejs/undici#1539</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1537">nodejs/undici#1537</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.6.1...v5.7.0">https://github.com/nodejs/undici/compare/v5.6.1...v5.7.0</a></p>
<h2>v5.6.1</h2>
<h2>What's Changed</h2>
<ul>
<li>docs: add example with <code>HEAD</code> method to garbage collection section by <a href="https://github.com/mrkldshv"><code>@​mrkldshv</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1522">nodejs/undici#1522</a></li>
<li>fix: improper handling of relative location header by <a href="https://github.com/PrincessRavy"><code>@​PrincessRavy</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1523">nodejs/undici#1523</a></li>
<li>build(deps-dev): bump tsd from 0.21.0 to 0.22.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1530">nodejs/undici#1530</a></li>
<li>fix(fetch): do not assign default value to <code>RequestInit.method</code> by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1529">nodejs/undici#1529</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/mrkldshv"><code>@​mrkldshv</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1522">nodejs/undici#1522</a></li>
<li><a href="https://github.com/PrincessRavy"><code>@​PrincessRavy</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1523">nodejs/undici#1523</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.6.0...v5.6.1">https://github.com/nodejs/undici/compare/v5.6.0...v5.6.1</a></p>
<h2>v5.6.0</h2>
<h2>What's Changed</h2>
<ul>
<li>build(deps-dev): bump tsd from 0.20.0 to 0.21.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1493">nodejs/undici#1493</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nodejs/undici/commit/26f60b7b6e612bb831133d7f85914963d1955011"><code>26f60b7</code></a> Bumped v5.8.0</li>
<li><a href="https://github.com/nodejs/undici/commit/0a5bee9465e627be36bac88edf7d9bbc9626126d"><code>0a5bee9</code></a> Merge pull request from GHSA-q768-x9m6-m9qp</li>
<li><a href="https://github.com/nodejs/undici/commit/a29a151d0140d095742d21a004023d024fe93259"><code>a29a151</code></a> Merge pull request from GHSA-3cvr-822r-rqcc</li>
<li><a href="https://github.com/nodejs/undici/commit/722976cf862b532d2a4a7ce45d9469946c0f5558"><code>722976c</code></a> docs: updated proxy docs - renamed already used const proxy to proxyServer (#...</li>
<li><a href="https://github.com/nodejs/undici/commit/b6af4e6eb5177444bc91f740b68de4eb8a43c561"><code>b6af4e6</code></a> fix(body mixin): only allow Uint8Array chunks (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1550">#1550</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/6c9e6344018982ff0a241f6f8a71682546410ebe"><code>6c9e634</code></a> fix(mock utils): set Readable.abort (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1549">#1549</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/22e2f39aad33f1537f3a1768842eef73da226745"><code>22e2f39</code></a> ci: fix up <code>exclude</code> (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1544">#1544</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/99205ec1e6dbaecb5e4b4494341d64c0a7b479eb"><code>99205ec</code></a> feat: use weighted round robin in balancedPool (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1069">#1069</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/5b57e8c6ad923c95bd9fc1dd7072083bc7542c82"><code>5b57e8c</code></a> chore: exclude windows node 16 (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1542">#1542</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/93e31a21c02defaf2625f9ec7e7a8936f495d3bc"><code>93e31a2</code></a> Drop PR title validation (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1543">#1543</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/nodejs/undici/compare/v5.5.1...v5.8.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=undici&package-manager=npm_and_yarn&previous-version=5.5.1&new-version=5.8.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/786"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-21 21:02:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/785" class=".btn">#785</a>
            </td>
            <td>
                <b>
                    Bump terser from 4.8.0 to 4.8.1 in /frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
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
<li>See full diff in <a href="https://github.com/terser/terser/commits">compare view</a></li>
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/business-partner-agent/network/alerts).

</details>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/785"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-21 18:50:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/783" class=".btn">#783</a>
            </td>
            <td>
                <b>
                    Feature/vue3 upgrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Preparations for upgrading vue2 to vue3

- upgrade vue, vue-cli-service and vue/cli-service plugins
- use migration build 
- fix compiler warnings (filters, v-bind, key on template tag, template without directives)

- fix some errors by commenting problematic lines
 



<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/783"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 09:18:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/782" class=".btn">#782</a>
            </td>
            <td>
                <b>
                    fixed genesis-url 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                genesis url is now defined in the genesis-transaction-list.yml


Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/782"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 08:39:36 +0000 UTC
    </div>
</div>

