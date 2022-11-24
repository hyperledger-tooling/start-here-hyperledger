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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/848" class=".btn">#848</a>
            </td>
            <td>
                <b>
                    Bump postgresql from 42.5.0 to 42.5.1 in /backend/business-partner-agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">java</span>
            </td>
            <td>
                Bumps [postgresql](https://github.com/pgjdbc/pgjdbc) from 42.5.0 to 42.5.1.
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
<p>[42.5.1] (2022-11-21 15:21:59 -0500)</p>
<h3>Security</h3>
<ul>
<li>security: StreamWrapper spills to disk if setText, or setBytea sends very large Strings or arrays to the server. createTempFile creates a file which can be read by other users on unix like systems (Not macos).
This has been fixed in this version fixes CVE-2022-41946 see the <a href="https://github.com/pgjdbc/pgjdbc/security/advisories/GHSA-562r-vg33-8x8h">security advisory</a> for more details. Reported by <a href="https://github.com/JLLeitschuh">Jonathan Leitschuh</a> This has been fixed in versions 42.5.1, 42.4.3 42.3.8, 42.2.27.jre7. Note there is no fix for 42.2.26.jre6. See the security advisory for work arounds.</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>fix: make sure we select array_in from pg_catalog to avoid duplicate array_in functions fixes <a href="https://github-redirect.dependabot.com/pgjdbc/pgjdbc/issues/2548">#Issue 2548</a> [PR <a href="https://github-redirect.dependabot.com/pgjdbc/pgjdbc/issues/2552">#2552</a>](<a href="https://github-redirect.dependabot.com/pgjdbc/pgjdbc/issues/2552">pgjdbc/pgjdbc#2552</a>)</li>
<li>fix: binary decoding of bool values [PR <a href="https://github-redirect.dependabot.com/pgjdbc/pgjdbc/issues/2640">#2640</a>](<a href="https://github-redirect.dependabot.com/pgjdbc/pgjdbc/pull/2640">pgjdbc/pgjdbc#2640</a>)</li>
<li>perf: improve performance of PgResultSet getByte/getShort/getInt/getLong for float-typed columns [PR <a href="https://github-redirect.dependabot.com/pgjdbc/pgjdbc/issues/2634">#2634</a>](<a href="https://github-redirect.dependabot.com/pgjdbc/pgjdbc/pull/2634">pgjdbc/pgjdbc#2634</a>)</li>
<li>chore: fix various spelling errors [PR <a href="https://github-redirect.dependabot.com/pgjdbc/pgjdbc/issues/2592">#2592</a>](<a href="https://github-redirect.dependabot.com/pgjdbc/pgjdbc/pull/2592">pgjdbc/pgjdbc#2592</a>)</li>
<li>chore: Feature/urlparser improve URLParser [PR <a href="https://github-redirect.dependabot.com/pgjdbc/pgjdbc/issues/2641">#2641</a>](<a href="https://github-redirect.dependabot.com/pgjdbc/pgjdbc/pull/2592">pgjdbc/pgjdbc#2592</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pgjdbc/pgjdbc/commit/9008dc9aade6dbfe4efafcd6872ebc55f4699cf5"><code>9008dc9</code></a> Merge pull request from GHSA-562r-vg33-8x8h</li>
<li><a href="https://github.com/pgjdbc/pgjdbc/commit/135be5a4395033a4ba23a1dd70ad76e0bd443a8d"><code>135be5a</code></a> chore: bump Checkstyle to 9.3</li>
<li><a href="https://github.com/pgjdbc/pgjdbc/commit/1d7465af15b38f1ef5ab2735554f204f54ed3e59"><code>1d7465a</code></a> chore: bump Gradle to 7.5.1</li>
<li><a href="https://github.com/pgjdbc/pgjdbc/commit/4743ccf7f96439c9eb956787f6c86ddff2568a19"><code>4743ccf</code></a> minor: Update the LeftCurly according to the updation in checkstyle</li>
<li><a href="https://github.com/pgjdbc/pgjdbc/commit/d5ed52ef391670e83ae5265af2f7301c615ce4ca"><code>d5ed52e</code></a> chore: add .git-blame-ignore-revst to hide reformatting commits from GitHub b...</li>
<li><a href="https://github.com/pgjdbc/pgjdbc/commit/98c04a0c903e90f2d5d10a09baf1f753747b2556"><code>98c04a0</code></a> exclude ArrayTest versions less than 9.1 (<a href="https://github-redirect.dependabot.com/pgjdbc/pgjdbc/issues/2645">#2645</a>)</li>
<li><a href="https://github.com/pgjdbc/pgjdbc/commit/9f90de920a969a066324b42cbd19e29d296ce970"><code>9f90de9</code></a> revert change to PGProperty.get() to keep the API the same (<a href="https://github-redirect.dependabot.com/pgjdbc/pgjdbc/issues/2644">#2644</a>)</li>
<li><a href="https://github.com/pgjdbc/pgjdbc/commit/ee06e22ee1f628877ee8d7664351b58b69dd0a1f"><code>ee06e22</code></a> Feature/urlparser improve3 pr1 (<a href="https://github-redirect.dependabot.com/pgjdbc/pgjdbc/issues/2641">#2641</a>)</li>
<li><a href="https://github.com/pgjdbc/pgjdbc/commit/56a487c113c8a3f860a1047852380d5668e9feba"><code>56a487c</code></a> fix: binary decoding of bool values (<a href="https://github-redirect.dependabot.com/pgjdbc/pgjdbc/issues/2640">#2640</a>)</li>
<li><a href="https://github.com/pgjdbc/pgjdbc/commit/b73899106949e92e497e3143b24f613cf2f9f203"><code>b738991</code></a> remove javadoc links for java 17 and above (<a href="https://github-redirect.dependabot.com/pgjdbc/pgjdbc/issues/2637">#2637</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pgjdbc/pgjdbc/compare/REL42.5.0...REL42.5.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=org.postgresql:postgresql&package-manager=maven&previous-version=42.5.0&new-version=42.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/business-partner-agent/network/alerts).

</details>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/848"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-23 22:18:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/847" class=".btn">#847</a>
            </td>
            <td>
                <b>
                    Fix returned credential exchange id 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">load-test</span>
            </td>
            <td>
                The response of issuing(send) a credential to a holder is the credential exchange id, but the returned id is not the UUID which is needed to refer to the appropriate credential exchange.

Usage:
- this is needed to automate revocation in the load test scenario (jmeter)

Signed-off-by: Driton Goxhufi <driton.goxhufi@bosch.io>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/847"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-17 12:54:58 +0000 UTC
    </div>
</div>

