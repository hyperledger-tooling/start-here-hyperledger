---
layout: default
title: cello
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cello
---

# cello <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cello){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/613" class=".btn">#613</a>
            </td>
            <td>
                <b>
                    Fixed the chaincode information display issue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The chaincode's ```package_id``` and ```description``` are correctly displayed now.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-22 03:43:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/612" class=".btn">#612</a>
            </td>
            <td>
                <b>
                    Manually calculate the package id
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Calculated the sha256 value of the chaincode file and combined it with the label to get the ```package_id```.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-17 01:37:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/611" class=".btn">#611</a>
            </td>
            <td>
                <b>
                    Bump sqlparse from 0.4.4 to 0.5.0 in /src/api-engine
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [sqlparse](https://github.com/andialbrecht/sqlparse) from 0.4.4 to 0.5.0.
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
</blockquote>
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
<li>Additional commits viewable in <a href="https://github.com/andialbrecht/sqlparse/compare/0.4.4...0.5.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=sqlparse&package-manager=pip&previous-version=0.4.4&new-version=0.5.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cello/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-15 22:55:59 +0000 UTC
    </div>
</div>

