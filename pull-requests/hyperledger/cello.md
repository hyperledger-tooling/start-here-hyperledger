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
                PR <a href="https://github.com/hyperledger/cello/pull/525" class=".btn">#525</a>
            </td>
            <td>
                <b>
                    Bump sqlparse from 0.4.2 to 0.4.4 in /src/api-engine
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [sqlparse](https://github.com/andialbrecht/sqlparse) from 0.4.2 to 0.4.4.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/andialbrecht/sqlparse/blob/master/CHANGELOG">sqlparse's changelog</a>.</em></p>
<blockquote>
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
<p>Bug Fixes</p>
<ul>
<li>Revert a change from 0.4.0 that changed IN to be a comparison (issue694).
The primary expectation is that IN is treated as a keyword and not as a
comparison operator. That also follows the definition of reserved keywords
for the major SQL syntax definitions.</li>
<li>Fix regular expressions for string parsing.</li>
</ul>
<p>Other</p>
<ul>
<li>sqlparse now uses pyproject.toml instead of setup.cfg (issue685).</li>
</ul>
<h2>Release 0.4.3 (Sep 23, 2022)</h2>
<p>Enhancements</p>
<ul>
<li>Add support for DIV operator (pr664, by chezou).</li>
<li>Add support for additional SPARK keywords (pr643, by mrmasterplan).</li>
<li>Avoid tokens copy (pr622, by living180).</li>
<li>Add REGEXP as a comparision (pr647, by PeterSandwich).</li>
<li>Add DISTINCTROW keyword for MS Access (issue677).</li>
<li>Improve parsing of CREATE TABLE AS SELECT (pr662, by chezou).</li>
</ul>
<p>Bug Fixes</p>
<ul>
<li>Fix spelling of INDICATOR keyword (pr653, by ptld).</li>
<li>Fix formatting error in EXTRACT function (issue562, issue670, pr676, by ecederstrand).</li>
<li>Fix bad parsing of create table statements that use lower case (issue217, pr642, by mrmasterplan).</li>
<li>Handle backtick as valid quote char (issue628, pr629, by codenamelxl).</li>
<li>Allow any unicode character as valid identifier name (issue641).</li>
</ul>
<p>Other</p>
<ul>
<li>Update github actions to test on Python 3.10 as well (pr661, by cclaus).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/647d1457acf7d88614215841eb15d423df2a1895"><code>647d145</code></a> Update Changelog.</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/58dae6fcd2a51209aeccd4fff3b923bf37714e19"><code>58dae6f</code></a> Bump version.</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/d9d69f47ed13a583c81473211f44ae320470a58b"><code>d9d69f4</code></a> Removed test file</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/64bb91f4880b46f73b4cc9207ae9ccc180d56d1b"><code>64bb91f</code></a> Testing branch</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/c457abd5f097dd13fb21543381e7cfafe7d31cfb"><code>c457abd</code></a> Remove unnecessary parts in regex for bad escaping.</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/b949fdf9a1538f98b57612bef6306fc38f32aaf7"><code>b949fdf</code></a> CI: Use codecov action.</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/fc76056fb8f0ec713a3f2a2b6206a3336932c382"><code>fc76056</code></a> Cleanup regex for detecting keywords (fixes <a href="https://redirect.github.com/andialbrecht/sqlparse/issues/709">#709</a>).</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/7fdb2da82d51a9a02baaefb5c7fe5cbbaac4329e"><code>7fdb2da</code></a> Merge pull request <a href="https://redirect.github.com/andialbrecht/sqlparse/issues/633">#633</a> from shikanime/master</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/dd9d5b91d7aa30e4a000d5370f09dc99378891dc"><code>dd9d5b9</code></a> Fix get_type with comments between WITH keyword</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/907fb496f90f2719095a1f01fe24db1e5c0e15a8"><code>907fb49</code></a> change singleton behavior</li>
<li>Additional commits viewable in <a href="https://github.com/andialbrecht/sqlparse/compare/0.4.2...0.4.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=sqlparse&package-manager=pip&previous-version=0.4.2&new-version=0.4.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cello/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-21 21:46:44 +0000 UTC
    </div>
</div>

