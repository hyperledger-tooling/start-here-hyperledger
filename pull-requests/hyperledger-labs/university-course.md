---
layout: default
title: university-course
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/university-course
---

# university-course <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/university-course){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/university-course/pull/84" class=".btn">#84</a>
            </td>
            <td>
                <b>
                    chore(deps): bump terser from 4.6.11 to 4.8.1 in /support/Lab06/b4s/organization/university/user-interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [terser](https://github.com/terser/terser) from 4.6.11 to 4.8.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/terser/terser/blob/master/CHANGELOG.md">terser's changelog</a>.</em></p>
<blockquote>
<h2>v4.8.1 (backport)</h2>
<ul>
<li>Security fix for RegExps that should not be evaluated (regexp DDOS)</li>
</ul>
<h2>v4.8.0</h2>
<ul>
<li>Support for numeric separators (<code>million = 1_000_000</code>) was added.</li>
<li>Assigning properties to a class is now assumed to be pure.</li>
<li>Fixed bug where <code>yield</code> wasn't considered a valid property key in generators.</li>
</ul>
<h2>v4.7.0</h2>
<ul>
<li>A bug was fixed where an arrow function would have the wrong size</li>
<li><code>arguments</code> object is now considered safe to retrieve properties from (useful for <code>length</code>, or <code>0</code>) even when <code>pure_getters</code> is not set.</li>
<li>Fixed erroneous <code>const</code> declarations without value (which is invalid) in some corner cases when using <code>collapse_vars</code>.</li>
</ul>
<h2>v4.6.13</h2>
<ul>
<li>Fixed issue where ES5 object properties were being turned into ES6 object properties due to more lax unicode rules.</li>
<li>Fixed parsing of BigInt with lowercase <code>e</code> in them.</li>
</ul>
<h2>v4.6.12</h2>
<ul>
<li>Fixed subtree comparison code, making it see that <code>[1,[2, 3]]</code> is different from <code>[1, 2, [3]]</code></li>
<li>Printing of unicode identifiers has been improved</li>
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


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=terser&package-manager=npm_and_yarn&previous-version=4.6.11&new-version=4.8.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/university-course/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-21 07:05:35 +0000 UTC
    </div>
</div>

