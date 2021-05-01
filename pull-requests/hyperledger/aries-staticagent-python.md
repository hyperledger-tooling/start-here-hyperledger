---
layout: default
title: aries-staticagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-staticagent-python
---

# aries-staticagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-staticagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-staticagent-python/pull/57" class=".btn">#57</a>
            </td>
            <td>
                <b>
                    Bump rexml from 3.2.4 to 3.2.5 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [rexml](https://github.com/ruby/rexml) from 3.2.4 to 3.2.5.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ruby/rexml/blob/master/NEWS.md">rexml's changelog</a>.</em></p>
<blockquote>
<h2>3.2.5 - 2021-04-05 {#version-3-2-5}</h2>
<h3>Improvements</h3>
<ul>
<li>
<p>Add more validations to XPath parser.</p>
</li>
<li>
<p><code>require &quot;rexml/document&quot;</code> by default.
[GitHub#36][Patch by Koichi ITO]</p>
</li>
<li>
<p>Don't add <code>#dcloe</code> method to core classes globally.
[GitHub#37][Patch by Akira Matsuda]</p>
</li>
<li>
<p>Add more documentations.
[Patch by Burdette Lamar]</p>
</li>
<li>
<p>Added <code>REXML::Elements#parent</code>.
[GitHub#52][Patch by Burdette Lamar]</p>
</li>
</ul>
<h3>Fixes</h3>
<ul>
<li>
<p>Fixed a bug that <code>REXML::DocType#clone</code> doesn't copy external ID
information.</p>
</li>
<li>
<p>Fixed round-trip vulnerability bugs.
See also: <a href="https://www.ruby-lang.org/en/news/2021/04/05/xml-round-trip-vulnerability-in-rexml-cve-2021-28965/">https://www.ruby-lang.org/en/news/2021/04/05/xml-round-trip-vulnerability-in-rexml-cve-2021-28965/</a>
[HackerOne#1104077][CVE-2021-28965][Reported by Juho Nurminen]</p>
</li>
</ul>
<h3>Thanks</h3>
<ul>
<li>
<p>Koichi ITO</p>
</li>
<li>
<p>Akira Matsuda</p>
</li>
<li>
<p>Burdette Lamar</p>
</li>
<li>
<p>Juho Nurminen</p>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ruby/rexml/commit/a622645e980ea5b91ad7b4d6fec32d113f15df88"><code>a622645</code></a> Add 3.2.5 entry</li>
<li><a href="https://github.com/ruby/rexml/commit/3c137eb119550874b2b3e27d12b733ca67033377"><code>3c137eb</code></a> Fix a parser bug that some data may be ignored before DOCTYPE</li>
<li><a href="https://github.com/ruby/rexml/commit/9b311e59ae05749e082eb6bbefa1cb620d1a786e"><code>9b311e5</code></a> Fix a bug that invalid document declaration may be accepted</li>
<li><a href="https://github.com/ruby/rexml/commit/f9d88e4948b4a43294c25dc0edb16815bd9d8618"><code>f9d88e4</code></a> Fix a bug that invalid document declaration may be generated</li>
<li><a href="https://github.com/ruby/rexml/commit/f7bab8937513b1403cea5aff874cbf32fd5e8551"><code>f7bab89</code></a> Fix a bug that invalid element end may be accepted</li>
<li><a href="https://github.com/ruby/rexml/commit/6a250d2cd1194c2be72becbdd9c3e770aa16e752"><code>6a250d2</code></a> Fix a bug that invalid element start may be accepted</li>
<li><a href="https://github.com/ruby/rexml/commit/2fe62e29094d95921d7e19abbd2e26b23d78dc5b"><code>2fe62e2</code></a> Fix a bug that invalid notation declaration may be accepted</li>
<li><a href="https://github.com/ruby/rexml/commit/a659c63e37414506dfb0d4655e031bb7a2e73fc8"><code>a659c63</code></a> Fix a bug that invalid notation declaration may be generated</li>
<li><a href="https://github.com/ruby/rexml/commit/790dd113ce693ce831cbbc53f2f990a317643f75"><code>790dd11</code></a> Use ruby/setup-ruby (<a href="https://github-redirect.dependabot.com/ruby/rexml/issues/66">#66</a>)</li>
<li><a href="https://github.com/ruby/rexml/commit/eda1b2007dd8751f381bf741f16c9e33c5d3e52a"><code>eda1b20</code></a> Clean up and enhance high-level RDoc (<a href="https://github-redirect.dependabot.com/ruby/rexml/issues/65">#65</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/ruby/rexml/compare/v3.2.4...v3.2.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=rexml&package-manager=bundler&previous-version=3.2.4&new-version=3.2.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-staticagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-30 21:07:15 +0000 UTC
    </div>
</div>

