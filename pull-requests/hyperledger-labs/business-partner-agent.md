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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/805" class=".btn">#805</a>
            </td>
            <td>
                <b>
                    Bump undici from 5.8.0 to 5.9.1 in /frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [undici](https://github.com/nodejs/undici) from 5.8.0 to 5.9.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nodejs/undici/releases">undici's releases</a>.</em></p>
<blockquote>
<h2>v5.9.1</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: don't timeout while waiting for client to send request (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1604">#1604</a>)</li>
<li>Fix array headers by <a href="https://github.com/mateonunez"><code>@​mateonunez</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1598">nodejs/undici#1598</a></li>
<li>fix(fetch): implement fully read body algorithm by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1597">nodejs/undici#1597</a></li>
<li>fix: add support for <code>integrity</code> option to Fetch by <a href="https://github.com/jelmervdl"><code>@​jelmervdl</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1596">nodejs/undici#1596</a></li>
<li>fix(File): respect typed array <code>byteOffset</code> and <code>byteLength</code> by <a href="https://github.com/mrbbot"><code>@​mrbbot</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1601">nodejs/undici#1601</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/mateonunez"><code>@​mateonunez</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1598">nodejs/undici#1598</a></li>
<li><a href="https://github.com/jelmervdl"><code>@​jelmervdl</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1596">nodejs/undici#1596</a></li>
<li><a href="https://github.com/mrbbot"><code>@​mrbbot</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1601">nodejs/undici#1601</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.8.2...v5.9.1">https://github.com/nodejs/undici/compare/v5.8.2...v5.9.1</a></p>
<h2>v5.8.2</h2>
<h2>⚠️ Security Release ⚠️</h2>
<ul>
<li>CRLF Injection in Nodejs ‘undici’ via Content-Type <a href="https://github.com/nodejs/undici/security/advisories/GHSA-f772-66g8-q5h3">GHSA-f772-66g8-q5h3</a> CVE-2022-35948</li>
<li><code>undici.request</code> vulnerable to SSRF using absolute URL on <code>pathname</code> <a href="https://github.com/nodejs/undici/security/advisories/GHSA-8qr4-xgw6-wmr3">GHSA-8qr4-xgw6-wmr3</a> CVE-2022-35949</li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>docs: mock different endpoints in a single file by <a href="https://github.com/ritvik130"><code>@​ritvik130</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1589">nodejs/undici#1589</a></li>
<li>feat(webidl): better error message for ByteString converter by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1591">nodejs/undici#1591</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/ritvik130"><code>@​ritvik130</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1589">nodejs/undici#1589</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.8.1...v5.8.2">https://github.com/nodejs/undici/compare/v5.8.1...v5.8.2</a></p>
<h2>v5.8.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Do not decode the body while we are following a redirect by <a href="https://github.com/mcollina"><code>@​mcollina</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1554">nodejs/undici#1554</a></li>
<li>docs: Fix spelling/grammar in &quot;Mocking Request&quot; by <a href="https://github.com/meyfa"><code>@​meyfa</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1555">nodejs/undici#1555</a></li>
<li>fix(MockInterceptor): callback options.headers w/ fetch by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1559">nodejs/undici#1559</a></li>
<li>fix(fetch): ByteString checks &amp; conversion in Headers by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1560">nodejs/undici#1560</a></li>
<li>test: update client certificates with ones that expires in 100 years by <a href="https://github.com/jodevsa"><code>@​jodevsa</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1566">nodejs/undici#1566</a></li>
<li>fix: x-www-form-urlencoded parser keep the BOM by <a href="https://github.com/cola119"><code>@​cola119</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1563">nodejs/undici#1563</a></li>
<li>fix: prioritise error events over timeouts by <a href="https://github.com/jodevsa"><code>@​jodevsa</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1551">nodejs/undici#1551</a></li>
<li>fix: add <code>isErrorLike</code> by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1570">nodejs/undici#1570</a></li>
<li>fix(types): add missing pool stats by <a href="https://github.com/SkeLLLa"><code>@​SkeLLLa</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1573">nodejs/undici#1573</a></li>
<li>fix: fetch a long base64 url will crash and nothing happens (close: <a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1574">#1574</a>) by <a href="https://github.com/ahaoboy"><code>@​ahaoboy</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1575">nodejs/undici#1575</a></li>
<li>fix: follow signal.reason in Request by <a href="https://github.com/LiviaMedeiros"><code>@​LiviaMedeiros</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1580">nodejs/undici#1580</a></li>
<li>docs: Fix DiagnosticsChannel sidebar link by <a href="https://github.com/trentm"><code>@​trentm</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1582">nodejs/undici#1582</a></li>
<li>fix: make mock headers case-insensitive by <a href="https://github.com/cola119"><code>@​cola119</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1585">nodejs/undici#1585</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/meyfa"><code>@​meyfa</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1555">nodejs/undici#1555</a></li>
<li><a href="https://github.com/cola119"><code>@​cola119</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1563">nodejs/undici#1563</a></li>
<li><a href="https://github.com/SkeLLLa"><code>@​SkeLLLa</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1573">nodejs/undici#1573</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nodejs/undici/commit/5890e16ddd2703151ce0be0a468e13d685b89f60"><code>5890e16</code></a> 5.9.1</li>
<li><a href="https://github.com/nodejs/undici/commit/ecae314c90534d665b6a2b1da085cff80c138c1b"><code>ecae314</code></a> fix: don't timeout while waiting for client to send request (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1604">#1604</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/fa9fd9066569b6357acacffb806aa804b688c9d8"><code>fa9fd90</code></a> fix(File): respect typed array <code>byteOffset</code> and <code>byteLength</code> (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1601">#1601</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/ae6f554e6af3aecee633b6e3ce359396b387eb4b"><code>ae6f554</code></a> fix: add support for <code>integrity</code> option to Fetch (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1596">#1596</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/deed6284ad97df01df92cee7576384bff7da1ad9"><code>deed628</code></a> fix(fetch): implement fully read body algorithm (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1597">#1597</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/0d1419ce8980e8c0f289e876448bf1e6eb755a8d"><code>0d1419c</code></a> Fix array headers (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1598">#1598</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/52d1ce56f7641d0c0d8359fc76537ebe15473e7e"><code>52d1ce5</code></a> Bumped v5.8.2</li>
<li><a href="https://github.com/nodejs/undici/commit/66165d604fd0aee70a93ed5c44ad4cc2df395f80"><code>66165d6</code></a> Merge pull request from GHSA-f772-66g8-q5h3</li>
<li><a href="https://github.com/nodejs/undici/commit/124f7ebf705366b2e1844dff721928d270f87895"><code>124f7eb</code></a> Merge pull request from GHSA-8qr4-xgw6-wmr3</li>
<li><a href="https://github.com/nodejs/undici/commit/aef314c7fd81a925b1c87217145a65ab6e6e895d"><code>aef314c</code></a> feat(webidl): better error message for ByteString converter (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1591">#1591</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/nodejs/undici/compare/v5.8.0...v5.9.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=undici&package-manager=npm_and_yarn&previous-version=5.8.0&new-version=5.9.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/805"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-18 20:03:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/804" class=".btn">#804</a>
            </td>
            <td>
                <b>
                    fix basic auth being active when keycloak is configured
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/804"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-18 15:39:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/803" class=".btn">#803</a>
            </td>
            <td>
                <b>
                    build pipeline updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - got rid of external snapshot repository by directly building the plugin in the pipeline
- moved license attribution and container creation into own build job
- added jacoco plugin and instrumentation
- added dependabot check job

Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/803"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-12 14:33:19 +0000 UTC
    </div>
</div>

