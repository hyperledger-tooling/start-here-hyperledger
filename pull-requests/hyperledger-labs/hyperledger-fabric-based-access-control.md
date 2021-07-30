---
layout: default
title: hyperledger-fabric-based-access-control
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/hyperledger-fabric-based-access-control
---

# hyperledger-fabric-based-access-control <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/hyperledger-fabric-based-access-control){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hyperledger-fabric-based-access-control/pull/30" class=".btn">#30</a>
            </td>
            <td>
                <b>
                    Bump color-string from 1.5.3 to 1.6.0 in /attributebased/javascript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [color-string](https://github.com/Qix-/color-string) from 1.5.3 to 1.6.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/Qix-/color-string/releases">color-string's releases</a>.</em></p>
<blockquote>
<h2>1.6.0</h2>
<h1>Minor release 1.6.0</h1>
<ul>
<li><a href="https://github.com/Qix-/color-string/issues/55">#55</a> - Add support for space-separated HSL</li>
</ul>
<p>Thanks <a href="https://github.com/htunnicliff"><code>@​htunnicliff</code></a> for the contribution :)</p>
<h2>1.5.5 (Patch/Security Release) - hwb() ReDos patch (low-severity)</h2>
<blockquote>
<p>Release notes copied verbatim from the commit message, which can be found here: 0789e21284c33d89ebc4ab4ca6f759b9375ac9d3</p>
</blockquote>
<pre><code>Discovered by Yeting Li, c/o Colin Ife via Snyk.io.
<p>A ReDos (Regular Expression Denial of Service) vulnerability
was responsibly disclosed to me via email by Colin on
Mar 5 2021 regarding an exponential time complexity for
linearly increasing input lengths for <code>hwb()</code> color strings.</p>
<p>Strings reaching more than 5000 characters would see several
milliseconds of processing time; strings reaching more than
50,000 characters began seeing 1500ms (1.5s) of processing time.</p>
<p>The cause was due to a the regular expression that parses
hwb() strings - specifically, the hue value - where
the integer portion of the hue value used a 0-or-more quantifier
shortly thereafter followed by a 1-or-more quantifier.</p>
<p>This caused excessive backtracking and a cartesian scan,
resulting in exponential time complexity given a linear
increase in input length.</p>
<p>Thank you Yeting Li and Colin Ife for bringing this to my
attention in a secure, responsible and professional manner.</p>
<p>A CVE will not be assigned for this vulnerability.
</code></pre></p>
<h2>1.5.4 (Patch Release)</h2>
<ul>
<li>Removes rounding of alpha values in RGBA hex (<code>#rrggbbaa</code>) and condensed-hex (<code>#rgba</code>) parsers, which caused certain unique inputs to result in identical outputs (see <a href="https://github.com/qix-/color/issues/174">https://github.com/qix-/color/issues/174</a>).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/Qix-/color-string/commits/1.6.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=color-string&package-manager=npm_and_yarn&previous-version=1.5.3&new-version=1.6.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/hyperledger-fabric-based-access-control/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-29 19:49:48 +0000 UTC
    </div>
</div>

