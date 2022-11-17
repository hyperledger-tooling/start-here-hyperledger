---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3432" class=".btn">#3432</a>
            </td>
            <td>
                <b>
                    Update package for checking CredentialMsgType
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Minh Huy, Tran <94397738+NhoxxKienn@users.noreply.github.com>

Use the following template for your PR (make sure you follow our
[guidelines](CONTRIBUTING.md#pull-request):

**Title:**
Update outdated doc.go

**Description:**
The package for checking CredentialMsgType is currently not presentproof but didcomm/protocol/issuecredential

**Summary:**
Change presentproof to an appropriate package issuecredential and Match the type of the MsgType with the example_test.go (V2)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-17 09:24:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3430" class=".btn">#3430</a>
            </td>
            <td>
                <b>
                    chore(deps): bump loader-utils from 1.2.3 to 1.4.2 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [loader-utils](https://github.com/webpack/loader-utils) from 1.2.3 to 1.4.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/loader-utils/releases">loader-utils's releases</a>.</em></p>
<blockquote>
<h2>v1.4.2</h2>
<h3><a href="https://github.com/webpack/loader-utils/compare/v1.4.1...v1.4.2">1.4.2</a> (2022-11-11)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>ReDoS problem (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/226">#226</a>) (<a href="https://github.com/webpack/loader-utils/commit/17cbf8fa8989c1cb45bdd2997aa524729475f1fa">17cbf8f</a>)</li>
</ul>
<h2>v1.4.1</h2>
<h3><a href="https://github.com/webpack/loader-utils/compare/v1.4.0...v1.4.1">1.4.1</a> (2022-11-07)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>security problem (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/220">#220</a>) (<a href="https://github.com/webpack/loader-utils/commit/4504e34c4796a5836ef70458327351675aed48a5">4504e34</a>)</li>
</ul>
<h2>v1.4.0</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1><a href="https://github.com/webpack/loader-utils/compare/v1.3.0...v1.4.0">1.4.0</a> (2020-02-19)</h1>
<h3>Features</h3>
<ul>
<li>the <code>resourceQuery</code> is passed to the <code>interpolateName</code> method (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/163">#163</a>) (<a href="https://github.com/webpack/loader-utils/commit/cd0e428">cd0e428</a>)</li>
</ul>
<h2>v1.3.0</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1><a href="https://github.com/webpack/loader-utils/compare/v1.2.3...v1.3.0">1.3.0</a> (2020-02-19)</h1>
<h3>Features</h3>
<ul>
<li>support the <code>[query]</code> template for the <code>interpolatedName</code> method (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/162">#162</a>) (<a href="https://github.com/webpack/loader-utils/commit/469eeba">469eeba</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/webpack/loader-utils/blob/v1.4.2/CHANGELOG.md">loader-utils's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/webpack/loader-utils/compare/v1.4.1...v1.4.2">1.4.2</a> (2022-11-11)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>ReDoS problem (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/226">#226</a>) (<a href="https://github.com/webpack/loader-utils/commit/17cbf8fa8989c1cb45bdd2997aa524729475f1fa">17cbf8f</a>)</li>
</ul>
<h3><a href="https://github.com/webpack/loader-utils/compare/v1.4.0...v1.4.1">1.4.1</a> (2022-11-07)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>security problem (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/220">#220</a>) (<a href="https://github.com/webpack/loader-utils/commit/4504e34c4796a5836ef70458327351675aed48a5">4504e34</a>)</li>
</ul>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1><a href="https://github.com/webpack/loader-utils/compare/v1.3.0...v1.4.0">1.4.0</a> (2020-02-19)</h1>
<h3>Features</h3>
<ul>
<li>the <code>resourceQuery</code> is passed to the <code>interpolateName</code> method (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/163">#163</a>) (<a href="https://github.com/webpack/loader-utils/commit/cd0e428">cd0e428</a>)</li>
</ul>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1><a href="https://github.com/webpack/loader-utils/compare/v1.2.3...v1.3.0">1.3.0</a> (2020-02-19)</h1>
<h3>Features</h3>
<ul>
<li>support the <code>[query]</code> template for the <code>interpolatedName</code> method (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/162">#162</a>) (<a href="https://github.com/webpack/loader-utils/commit/469eeba">469eeba</a>)</li>
</ul>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/loader-utils/commit/331ad5067d9a1a7b8d646692e6959639969210d1"><code>331ad50</code></a> chore(release): 1.4.2</li>
<li><a href="https://github.com/webpack/loader-utils/commit/17cbf8fa8989c1cb45bdd2997aa524729475f1fa"><code>17cbf8f</code></a> fix: ReDoS problem (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/226">#226</a>)</li>
<li><a href="https://github.com/webpack/loader-utils/commit/8f082b39f6903929f30fe29dab34f4d9c7ef070a"><code>8f082b3</code></a> chore(release): 1.4.1</li>
<li><a href="https://github.com/webpack/loader-utils/commit/4504e34c4796a5836ef70458327351675aed48a5"><code>4504e34</code></a> fix: security problem (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/220">#220</a>)</li>
<li><a href="https://github.com/webpack/loader-utils/commit/d95b8b53f0ad547133b47ac8226f735c479f76de"><code>d95b8b5</code></a> chore(release): 1.4.0</li>
<li><a href="https://github.com/webpack/loader-utils/commit/cd0e4284a0aa090f8776c4eb1045d4b1080e7161"><code>cd0e428</code></a> feat: the <code>resourceQuery</code> is passed to the <code>interpolateName</code> method (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/163">#163</a>)</li>
<li><a href="https://github.com/webpack/loader-utils/commit/06d36cf3a619cab20b08608204cb7ea9bddaceab"><code>06d36cf</code></a> chore(release): 1.3.0</li>
<li><a href="https://github.com/webpack/loader-utils/commit/469eeba9095b879a3a988cde23d2035e454da9c2"><code>469eeba</code></a> feat: support the <code>[query]</code> template for the <code>interpolatedName</code> method (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/162">#162</a>)</li>
<li><a href="https://github.com/webpack/loader-utils/commit/909c99d3f85da40478b9f02338d4113332819cfd"><code>909c99d</code></a> chore: funding.yml config and CI fix (<a href="https://github-redirect.dependabot.com/webpack/loader-utils/issues/159">#159</a>)</li>
<li><a href="https://github.com/webpack/loader-utils/commit/b5b74f010cace25ca70a652ebef078f6b1cfaddb"><code>b5b74f0</code></a> Set up CI with Azure Pipelines</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/loader-utils/compare/v1.2.3...v1.4.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=loader-utils&package-manager=npm_and_yarn&previous-version=1.2.3&new-version=1.4.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-go/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-13 01:04:33 +0000 UTC
    </div>
</div>

