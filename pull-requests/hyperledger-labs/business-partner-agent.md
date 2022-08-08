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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/796" class=".btn">#796</a>
            </td>
            <td>
                <b>
                    Support for oob exchanges with attachments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backend:

- [x] indy v1 credential offer
- [x] indy v2 credential offer
- [ ] dif credential offer
- [x] indy v1 presentation request
- [x] indy v2 presentation request
- [x] dif presentation request

Frontend:

- [x] indy v1 credential offer
- [x] indy v2 credential offer
- [ ] dif credential offer
- [ ] indy v1 presentation request
- [ ] indy v2 presentation request
- [ ] dif presentation request
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-08 14:14:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/794" class=".btn">#794</a>
            </td>
            <td>
                <b>
                    Bump postgresql from 42.4.0 to 42.4.1 in /backend/business-partner-agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">java</span>
            </td>
            <td>
                Bumps [postgresql](https://github.com/pgjdbc/pgjdbc) from 42.4.0 to 42.4.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pgjdbc/pgjdbc/blob/master/CHANGELOG.md">postgresql's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<p>Notable changes since version 42.0.0, read the complete <a href="https://jdbc.postgresql.org/documentation/changelog.html">History of Changes</a>.</p>
<p>The format is based on <a href="http://keepachangelog.com/en/1.0.0/">Keep a Changelog</a>.</p>
<h2>[Unreleased]</h2>
<h3>Changed</h3>
<h3>Added</h3>
<h3>Fixed</h3>
<p>[42.4.1] (2022-08-01 16:24:20 -0400)</p>
<h3>Security</h3>
<ul>
<li>fix: CVE-2022-31197 Fixes SQL generated in PgResultSet.refresh() to escape column identifiers so as to prevent SQL injection.
<ul>
<li>Previously, the column names for both key and data columns in the table were copied as-is into the generated
SQL. This allowed a malicious table with column names that include statement terminator to be parsed and
executed as multiple separate commands.</li>
<li>Also adds a new test class ResultSetRefreshTest to verify this change.</li>
<li>Reported by <a href="https://github.com/kato-sho">Sho Kato</a></li>
</ul>
</li>
</ul>
<h3>Changed</h3>
<ul>
<li>chore: skip publishing pgjdbc-osgi-test to Central</li>
<li>chore: bump Gradle to 7.5</li>
<li>test: update JUnit to 5.8.2</li>
</ul>
<h3>Added</h3>
<ul>
<li>chore: added Gradle Wrapper Validation for verifying gradle-wrapper.jar</li>
<li>chore: added &quot;permissions: contents: read&quot; for GitHub Actions to avoid unintentional modifications by the CI</li>
<li>chore: support building pgjdbc with Java 17</li>
</ul>
<h3>Fixed</h3>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pgjdbc/pgjdbc/commit/bd91c4cc76cdfc1ffd0322be80c85ddfe08a38c2"><code>bd91c4c</code></a> Prepare for release (<a href="https://github-redirect.dependabot.com/pgjdbc/pgjdbc/issues/2580">#2580</a>)</li>
<li><a href="https://github.com/pgjdbc/pgjdbc/commit/739e599d52ad80f8dcd6efedc6157859b1a9d637"><code>739e599</code></a> Merge pull request from GHSA-r38f-c4h4-hqq2</li>
<li><a href="https://github.com/pgjdbc/pgjdbc/commit/736f9598c5b32a19c645ad33f118d2c9c266e90e"><code>736f959</code></a> fix: replace syncronization in Connection.close with compareAndSet</li>
<li><a href="https://github.com/pgjdbc/pgjdbc/commit/4673fd271c63a24b2a363149945187bad911888a"><code>4673fd2</code></a> feat: synchronize statement executions (e.g. avoid deadlock when Connection.i...</li>
<li><a href="https://github.com/pgjdbc/pgjdbc/commit/fd31a06f9c64a2ad69ce274de99ec31d0e1c3b6d"><code>fd31a06</code></a> update the website content (<a href="https://github-redirect.dependabot.com/pgjdbc/pgjdbc/issues/2578">#2578</a>)</li>
<li><a href="https://github.com/pgjdbc/pgjdbc/commit/a6044d05b80e1bda2fbe2f4e6bd0a714b8e74030"><code>a6044d0</code></a> set a timeout to get the return from requesting SSL upgrade. (<a href="https://github-redirect.dependabot.com/pgjdbc/pgjdbc/issues/2572">#2572</a>)</li>
<li><a href="https://github.com/pgjdbc/pgjdbc/commit/58d6fa085fef483d5f972146c9e7e8f805d144d9"><code>58d6fa0</code></a> test: bump system-stubs-jupiter to 2.0.1 to support Java 16+</li>
<li><a href="https://github.com/pgjdbc/pgjdbc/commit/b452d8c6d16ffdcd79495e5857ce9ba37bd8a87b"><code>b452d8c</code></a> test: avoid concurrent executions of tests that update environment and system...</li>
<li><a href="https://github.com/pgjdbc/pgjdbc/commit/aa5758a18893ced9c1b20655be6042444d746440"><code>aa5758a</code></a> test: update JUnit to 5.8.2</li>
<li><a href="https://github.com/pgjdbc/pgjdbc/commit/36cd24c300118c36a8b408665118a1f83b82751d"><code>36cd24c</code></a> fix: log connection URL when it can't be parsed</li>
<li>Additional commits viewable in <a href="https://github.com/pgjdbc/pgjdbc/compare/REL42.4.0...REL42.4.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=org.postgresql:postgresql&package-manager=maven&previous-version=42.4.0&new-version=42.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/794"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-06 06:08:27 +0000 UTC
    </div>
</div>

