---
layout: default
title: aries-agent-controller
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/aries-agent-controller
---

# aries-agent-controller <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/aries-agent-controller){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/aries-agent-controller/pull/10" class=".btn">#10</a>
            </td>
            <td>
                <b>
                    Bump sqlparse from 0.3.0 to 0.5.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [sqlparse](https://github.com/andialbrecht/sqlparse) from 0.3.0 to 0.5.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/andialbrecht/sqlparse/blob/master/CHANGELOG">sqlparse's changelog</a>.</em></p>
<blockquote>
<h2>Release 0.5.0 (Apr 13, 2024)</h2>
<p>Notable Changes</p>
<ul>
<li>Drop support for Python 3.5, 3.6, and 3.7.</li>
<li>Python 3.12 is now supported (pr725, by hugovk).</li>
<li>IMPORTANT: Fixes a potential denial of service attack (DOS) due to recursion
error for deeply nested statements. Instead of recursion error a generic
SQLParseError is raised. See the security advisory for details:
<a href="https://github.com/andialbrecht/sqlparse/security/advisories/GHSA-2m57-hf25-phgg">https://github.com/andialbrecht/sqlparse/security/advisories/GHSA-2m57-hf25-phgg</a>
The vulnerability was discovered by <a href="https://github.com/uriyay-jfrog"><code>@​uriyay-jfrog</code></a>. Thanks for reporting!</li>
</ul>
<p>Enhancements:</p>
<ul>
<li>Splitting statements now allows to remove the semicolon at the end.
Some database backends love statements without semicolon (issue742).</li>
<li>Support TypedLiterals in get_parameters (pr649, by Khrol).</li>
<li>Improve splitting of Transact SQL when using GO keyword (issue762).</li>
<li>Support for some JSON operators (issue682).</li>
<li>Improve formatting of statements containing JSON operators (issue542).</li>
<li>Support for BigQuery and Snowflake keywords (pr699, by griffatrasgo).</li>
<li>Support parsing of OVER clause (issue701, pr768 by r33s3n6).</li>
</ul>
<p>Bug Fixes</p>
<ul>
<li>Ignore dunder attributes when creating Tokens (issue672).</li>
<li>Allow operators to precede dollar-quoted strings (issue763).</li>
<li>Fix parsing of nested order clauses (issue745, pr746 by john-bodley).</li>
<li>Thread-safe initialization of Lexer class (issue730).</li>
<li>Classify TRUNCATE as DDL and GRANT/REVOKE as DCL keywords (based on pr719
by josuc1, thanks for bringing this up!).</li>
<li>Fix parsing of PRIMARY KEY (issue740).</li>
</ul>
<p>Other</p>
<ul>
<li>Optimize performance of matching function (pr799, by admachainz).</li>
</ul>
<h2>Release 0.4.4 (Apr 18, 2023)</h2>
<p>Notable Changes</p>
<ul>
<li>IMPORTANT: This release fixes a security vulnerability in the
parser where a regular expression vulnerable to ReDOS (Regular
Expression Denial of Service) was used. See the security advisory
for details: <a href="https://github.com/andialbrecht/sqlparse/security/advisories/GHSA-rrm6-wvj7-cwh2">https://github.com/andialbrecht/sqlparse/security/advisories/GHSA-rrm6-wvj7-cwh2</a>
The vulnerability was discovered by <a href="https://github.com/erik-krogh"><code>@​erik-krogh</code></a> from GitHub
Security Lab (GHSL). Thanks for reporting!</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/ddbd0ec3592545c914fe71e47118c04582d8bfb0"><code>ddbd0ec</code></a> Bump version.</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/29f2e0a6609ddc1fa248faef1bc41616043c544e"><code>29f2e0a</code></a> Raise recursion limit for tests.</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/b4a39d9850969b4e1d6940d32094ee0b42a2cf03"><code>b4a39d9</code></a> Raise SQLParseError instead of RecursionError.</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/f1bcf2f8a7ddf6854c99990c56ff5394f4981d58"><code>f1bcf2f</code></a> Update AUHTORS and Changelog.</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/e03b74e608b71dd06824c2cb42421c0d790248e3"><code>e03b74e</code></a> Fix Function.get_parameters(), add Funtion.get_window()</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/617b8f6cd3c55bacf2c80130901508518753f7e1"><code>617b8f6</code></a> Add OVER clause, and group it into Function (fixes <a href="https://redirect.github.com/andialbrecht/sqlparse/issues/701">#701</a>)</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/d8f81471cfc2c39ac43128e2a0c8cc67c313cc40"><code>d8f8147</code></a> Update AUHTORS and Changelog.</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/012c9f10c8ddfa47ccf17ead28122492155cf6fc"><code>012c9f1</code></a> Optimize sqlparse.utils.imt().</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/46971e5a804b29e7dbd437155a8ceffab8ef1cd5"><code>46971e5</code></a> Fix parsing of PRIMARY KEY (fixes <a href="https://redirect.github.com/andialbrecht/sqlparse/issues/740">#740</a>).</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/fc4b0beab89c5598d556572cb6db0165affb017b"><code>fc4b0be</code></a> Code cleanup.</li>
<li>Additional commits viewable in <a href="https://github.com/andialbrecht/sqlparse/compare/0.3.0...0.5.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=sqlparse&package-manager=pip&previous-version=0.3.0&new-version=0.5.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/aries-agent-controller/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-15 22:53:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/aries-agent-controller/pull/9" class=".btn">#9</a>
            </td>
            <td>
                <b>
                    Bump sqlparse from 0.3.0 to 0.5.0 in /docker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [sqlparse](https://github.com/andialbrecht/sqlparse) from 0.3.0 to 0.5.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/andialbrecht/sqlparse/blob/master/CHANGELOG">sqlparse's changelog</a>.</em></p>
<blockquote>
<h2>Release 0.5.0 (Apr 13, 2024)</h2>
<p>Notable Changes</p>
<ul>
<li>Drop support for Python 3.5, 3.6, and 3.7.</li>
<li>Python 3.12 is now supported (pr725, by hugovk).</li>
<li>IMPORTANT: Fixes a potential denial of service attack (DOS) due to recursion
error for deeply nested statements. Instead of recursion error a generic
SQLParseError is raised. See the security advisory for details:
<a href="https://github.com/andialbrecht/sqlparse/security/advisories/GHSA-2m57-hf25-phgg">https://github.com/andialbrecht/sqlparse/security/advisories/GHSA-2m57-hf25-phgg</a>
The vulnerability was discovered by <a href="https://github.com/uriyay-jfrog"><code>@​uriyay-jfrog</code></a>. Thanks for reporting!</li>
</ul>
<p>Enhancements:</p>
<ul>
<li>Splitting statements now allows to remove the semicolon at the end.
Some database backends love statements without semicolon (issue742).</li>
<li>Support TypedLiterals in get_parameters (pr649, by Khrol).</li>
<li>Improve splitting of Transact SQL when using GO keyword (issue762).</li>
<li>Support for some JSON operators (issue682).</li>
<li>Improve formatting of statements containing JSON operators (issue542).</li>
<li>Support for BigQuery and Snowflake keywords (pr699, by griffatrasgo).</li>
<li>Support parsing of OVER clause (issue701, pr768 by r33s3n6).</li>
</ul>
<p>Bug Fixes</p>
<ul>
<li>Ignore dunder attributes when creating Tokens (issue672).</li>
<li>Allow operators to precede dollar-quoted strings (issue763).</li>
<li>Fix parsing of nested order clauses (issue745, pr746 by john-bodley).</li>
<li>Thread-safe initialization of Lexer class (issue730).</li>
<li>Classify TRUNCATE as DDL and GRANT/REVOKE as DCL keywords (based on pr719
by josuc1, thanks for bringing this up!).</li>
<li>Fix parsing of PRIMARY KEY (issue740).</li>
</ul>
<p>Other</p>
<ul>
<li>Optimize performance of matching function (pr799, by admachainz).</li>
</ul>
<h2>Release 0.4.4 (Apr 18, 2023)</h2>
<p>Notable Changes</p>
<ul>
<li>IMPORTANT: This release fixes a security vulnerability in the
parser where a regular expression vulnerable to ReDOS (Regular
Expression Denial of Service) was used. See the security advisory
for details: <a href="https://github.com/andialbrecht/sqlparse/security/advisories/GHSA-rrm6-wvj7-cwh2">https://github.com/andialbrecht/sqlparse/security/advisories/GHSA-rrm6-wvj7-cwh2</a>
The vulnerability was discovered by <a href="https://github.com/erik-krogh"><code>@​erik-krogh</code></a> from GitHub
Security Lab (GHSL). Thanks for reporting!</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/ddbd0ec3592545c914fe71e47118c04582d8bfb0"><code>ddbd0ec</code></a> Bump version.</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/29f2e0a6609ddc1fa248faef1bc41616043c544e"><code>29f2e0a</code></a> Raise recursion limit for tests.</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/b4a39d9850969b4e1d6940d32094ee0b42a2cf03"><code>b4a39d9</code></a> Raise SQLParseError instead of RecursionError.</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/f1bcf2f8a7ddf6854c99990c56ff5394f4981d58"><code>f1bcf2f</code></a> Update AUHTORS and Changelog.</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/e03b74e608b71dd06824c2cb42421c0d790248e3"><code>e03b74e</code></a> Fix Function.get_parameters(), add Funtion.get_window()</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/617b8f6cd3c55bacf2c80130901508518753f7e1"><code>617b8f6</code></a> Add OVER clause, and group it into Function (fixes <a href="https://redirect.github.com/andialbrecht/sqlparse/issues/701">#701</a>)</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/d8f81471cfc2c39ac43128e2a0c8cc67c313cc40"><code>d8f8147</code></a> Update AUHTORS and Changelog.</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/012c9f10c8ddfa47ccf17ead28122492155cf6fc"><code>012c9f1</code></a> Optimize sqlparse.utils.imt().</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/46971e5a804b29e7dbd437155a8ceffab8ef1cd5"><code>46971e5</code></a> Fix parsing of PRIMARY KEY (fixes <a href="https://redirect.github.com/andialbrecht/sqlparse/issues/740">#740</a>).</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/fc4b0beab89c5598d556572cb6db0165affb017b"><code>fc4b0be</code></a> Code cleanup.</li>
<li>Additional commits viewable in <a href="https://github.com/andialbrecht/sqlparse/compare/0.3.0...0.5.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=sqlparse&package-manager=pip&previous-version=0.3.0&new-version=0.5.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/aries-agent-controller/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-15 20:44:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/aries-agent-controller/pull/8" class=".btn">#8</a>
            </td>
            <td>
                <b>
                    Bump idna from 2.8 to 3.7 in /docker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [idna](https://github.com/kjd/idna) from 2.8 to 3.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/kjd/idna/releases">idna's releases</a>.</em></p>
<blockquote>
<h2>v3.7</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix issue where specially crafted inputs to encode() could take exceptionally long amount of time to process. [CVE-2024-3651]</li>
</ul>
<p>Thanks to Guido Vranken for reporting the issue.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/kjd/idna/compare/v3.6...v3.7">https://github.com/kjd/idna/compare/v3.6...v3.7</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/kjd/idna/blob/master/HISTORY.rst">idna's changelog</a>.</em></p>
<blockquote>
<p>3.7 (2024-04-11)
++++++++++++++++</p>
<ul>
<li>Fix issue where specially crafted inputs to encode() could
take exceptionally long amount of time to process. [CVE-2024-3651]</li>
</ul>
<p>Thanks to Guido Vranken for reporting the issue.</p>
<p>3.6 (2023-11-25)
++++++++++++++++</p>
<ul>
<li>Fix regression to include tests in source distribution.</li>
</ul>
<p>3.5 (2023-11-24)
++++++++++++++++</p>
<ul>
<li>Update to Unicode 15.1.0</li>
<li>String codec name is now &quot;idna2008&quot; as overriding the system codec
&quot;idna&quot; was not working.</li>
<li>Fix typing error for codec encoding</li>
<li>&quot;setup.cfg&quot; has been added for this release due to some downstream
lack of adherence to PEP 517. Should be removed in a future release
so please prepare accordingly.</li>
<li>Removed reliance on a symlink for the &quot;idna-data&quot; tool to comport
with PEP 517 and the Python Packaging User Guide for sdist archives.</li>
<li>Added security reporting protocol for project</li>
</ul>
<p>Thanks Jon Ribbens, Diogo Teles Sant'Anna, Wu Tingfeng for contributions
to this release.</p>
<p>3.4 (2022-09-14)
++++++++++++++++</p>
<ul>
<li>Update to Unicode 15.0.0</li>
<li>Migrate to pyproject.toml for build information (PEP 621)</li>
<li>Correct another instance where generic exception was raised instead of
IDNAError for malformed input</li>
<li>Source distribution uses zeroized file ownership for improved
reproducibility</li>
</ul>
<p>Thanks to Seth Michael Larson for contributions to this release.</p>
<p>3.3 (2021-10-13)
++++++++++++++++</p>
<ul>
<li>Update to Unicode 14.0.0</li>
<li>Update to in-line type annotations</li>
<li>Throw IDNAError exception correctly for some malformed input</li>
<li>Advertise support for Python 3.10</li>
<li>Improve testing regime on Github</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/kjd/idna/commit/1d365e17e10d72d0b7876316fc7b9ca0eebdd38d"><code>1d365e1</code></a> Release v3.7</li>
<li><a href="https://github.com/kjd/idna/commit/c1b3154939907fab67c5754346afaebe165ce8e6"><code>c1b3154</code></a> Merge pull request <a href="https://redirect.github.com/kjd/idna/issues/172">#172</a> from kjd/optimize-contextj</li>
<li><a href="https://github.com/kjd/idna/commit/0394ec76ff022813e770ba1fd89658790ea35623"><code>0394ec7</code></a> Merge branch 'master' into optimize-contextj</li>
<li><a href="https://github.com/kjd/idna/commit/cd58a23173d2b0a40b95ee680baf3e59e8d33966"><code>cd58a23</code></a> Merge pull request <a href="https://redirect.github.com/kjd/idna/issues/152">#152</a> from elliotwutingfeng/dev</li>
<li><a href="https://github.com/kjd/idna/commit/5beb28b9dd77912c0dd656d8b0fdba3eb80222e7"><code>5beb28b</code></a> More efficient resolution of joiner contexts</li>
<li><a href="https://github.com/kjd/idna/commit/1b121483ed04d9576a1291758f537e1318cddc8b"><code>1b12148</code></a> Update ossf/scorecard-action to v2.3.1</li>
<li><a href="https://github.com/kjd/idna/commit/d516b874c3388047934938a500c7488d52c4e067"><code>d516b87</code></a> Update Github actions/checkout to v4</li>
<li><a href="https://github.com/kjd/idna/commit/c095c75943413c75ebf8ac74179757031b7f80b7"><code>c095c75</code></a> Merge branch 'master' into dev</li>
<li><a href="https://github.com/kjd/idna/commit/60a0a4cb61ec6834d74306bd8a1fa46daac94c98"><code>60a0a4c</code></a> Fix typo in GitHub Actions workflow key</li>
<li><a href="https://github.com/kjd/idna/commit/5918a0ef8034379c2e409ae93ee11d24295bb201"><code>5918a0e</code></a> Merge branch 'master' into dev</li>
<li>Additional commits viewable in <a href="https://github.com/kjd/idna/compare/v2.8...v3.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=idna&package-manager=pip&previous-version=2.8&new-version=3.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/aries-agent-controller/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-11 23:40:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/aries-agent-controller/pull/7" class=".btn">#7</a>
            </td>
            <td>
                <b>
                    Bump idna from 2.8 to 3.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [idna](https://github.com/kjd/idna) from 2.8 to 3.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/kjd/idna/releases">idna's releases</a>.</em></p>
<blockquote>
<h2>v3.7</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix issue where specially crafted inputs to encode() could take exceptionally long amount of time to process. [CVE-2024-3651]</li>
</ul>
<p>Thanks to Guido Vranken for reporting the issue.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/kjd/idna/compare/v3.6...v3.7">https://github.com/kjd/idna/compare/v3.6...v3.7</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/kjd/idna/blob/master/HISTORY.rst">idna's changelog</a>.</em></p>
<blockquote>
<p>3.7 (2024-04-11)
++++++++++++++++</p>
<ul>
<li>Fix issue where specially crafted inputs to encode() could
take exceptionally long amount of time to process. [CVE-2024-3651]</li>
</ul>
<p>Thanks to Guido Vranken for reporting the issue.</p>
<p>3.6 (2023-11-25)
++++++++++++++++</p>
<ul>
<li>Fix regression to include tests in source distribution.</li>
</ul>
<p>3.5 (2023-11-24)
++++++++++++++++</p>
<ul>
<li>Update to Unicode 15.1.0</li>
<li>String codec name is now &quot;idna2008&quot; as overriding the system codec
&quot;idna&quot; was not working.</li>
<li>Fix typing error for codec encoding</li>
<li>&quot;setup.cfg&quot; has been added for this release due to some downstream
lack of adherence to PEP 517. Should be removed in a future release
so please prepare accordingly.</li>
<li>Removed reliance on a symlink for the &quot;idna-data&quot; tool to comport
with PEP 517 and the Python Packaging User Guide for sdist archives.</li>
<li>Added security reporting protocol for project</li>
</ul>
<p>Thanks Jon Ribbens, Diogo Teles Sant'Anna, Wu Tingfeng for contributions
to this release.</p>
<p>3.4 (2022-09-14)
++++++++++++++++</p>
<ul>
<li>Update to Unicode 15.0.0</li>
<li>Migrate to pyproject.toml for build information (PEP 621)</li>
<li>Correct another instance where generic exception was raised instead of
IDNAError for malformed input</li>
<li>Source distribution uses zeroized file ownership for improved
reproducibility</li>
</ul>
<p>Thanks to Seth Michael Larson for contributions to this release.</p>
<p>3.3 (2021-10-13)
++++++++++++++++</p>
<ul>
<li>Update to Unicode 14.0.0</li>
<li>Update to in-line type annotations</li>
<li>Throw IDNAError exception correctly for some malformed input</li>
<li>Advertise support for Python 3.10</li>
<li>Improve testing regime on Github</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/kjd/idna/commit/1d365e17e10d72d0b7876316fc7b9ca0eebdd38d"><code>1d365e1</code></a> Release v3.7</li>
<li><a href="https://github.com/kjd/idna/commit/c1b3154939907fab67c5754346afaebe165ce8e6"><code>c1b3154</code></a> Merge pull request <a href="https://redirect.github.com/kjd/idna/issues/172">#172</a> from kjd/optimize-contextj</li>
<li><a href="https://github.com/kjd/idna/commit/0394ec76ff022813e770ba1fd89658790ea35623"><code>0394ec7</code></a> Merge branch 'master' into optimize-contextj</li>
<li><a href="https://github.com/kjd/idna/commit/cd58a23173d2b0a40b95ee680baf3e59e8d33966"><code>cd58a23</code></a> Merge pull request <a href="https://redirect.github.com/kjd/idna/issues/152">#152</a> from elliotwutingfeng/dev</li>
<li><a href="https://github.com/kjd/idna/commit/5beb28b9dd77912c0dd656d8b0fdba3eb80222e7"><code>5beb28b</code></a> More efficient resolution of joiner contexts</li>
<li><a href="https://github.com/kjd/idna/commit/1b121483ed04d9576a1291758f537e1318cddc8b"><code>1b12148</code></a> Update ossf/scorecard-action to v2.3.1</li>
<li><a href="https://github.com/kjd/idna/commit/d516b874c3388047934938a500c7488d52c4e067"><code>d516b87</code></a> Update Github actions/checkout to v4</li>
<li><a href="https://github.com/kjd/idna/commit/c095c75943413c75ebf8ac74179757031b7f80b7"><code>c095c75</code></a> Merge branch 'master' into dev</li>
<li><a href="https://github.com/kjd/idna/commit/60a0a4cb61ec6834d74306bd8a1fa46daac94c98"><code>60a0a4c</code></a> Fix typo in GitHub Actions workflow key</li>
<li><a href="https://github.com/kjd/idna/commit/5918a0ef8034379c2e409ae93ee11d24295bb201"><code>5918a0e</code></a> Merge branch 'master' into dev</li>
<li>Additional commits viewable in <a href="https://github.com/kjd/idna/compare/v2.8...v3.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=idna&package-manager=pip&previous-version=2.8&new-version=3.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/aries-agent-controller/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-11 22:38:01 +0000 UTC
    </div>
</div>

