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
                PR <a href="https://github.com/hyperledger/aries-staticagent-python/pull/101" class=".btn">#101</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump activesupport from 6.0.3.2 to 6.0.6.1 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">ruby</span>
            </td>
            <td>
                Bumps [activesupport](https://github.com/rails/rails) from 6.0.3.2 to 6.0.6.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/rails/rails/releases">activesupport's releases</a>.</em></p>
<blockquote>
<h2>v6.0.6.1</h2>
<h2>Active Support</h2>
<ul>
<li>No changes.</li>
</ul>
<h2>Active Model</h2>
<ul>
<li>No changes.</li>
</ul>
<h2>Active Record</h2>
<ul>
<li>
<p>Make <code>sanitize_as_sql_comment</code> more strict</p>
<p>Though this method was likely never meant to take user input, it was
attempting sanitization. That sanitization could be bypassed with
carefully crafted input.</p>
<p>This commit makes the sanitization more robust by replacing any
occurrances of &quot;/<em>&quot; or &quot;</em>/&quot; with &quot;/ <em>&quot; or &quot;</em> /&quot;. It also performs a
first pass to remove one surrounding comment to avoid compatibility
issues for users relying on the existing removal.</p>
<p>This also clarifies in the documentation of annotate that it should not
be provided user input.</p>
<p>[CVE-2023-22794]</p>
</li>
</ul>
<h2>Action View</h2>
<ul>
<li>No changes.</li>
</ul>
<h2>Action Pack</h2>
<ul>
<li>No changes.</li>
</ul>
<h2>Active Job</h2>
<ul>
<li>No changes.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rails/rails/commit/28bb76d3efc39b2ef663dfe2346f7c2621343cd6"><code>28bb76d</code></a> Version 6.0.6.1</li>
<li><a href="https://github.com/rails/rails/commit/91cf62e7b43c33ae6263adf3d7563da9b68ff21d"><code>91cf62e</code></a> Version 6.0.6</li>
<li><a href="https://github.com/rails/rails/commit/c7d64e91b65d3633146e37c65ad5211352d60a69"><code>c7d64e9</code></a> Preparing for 6.0.5.1 release</li>
<li><a href="https://github.com/rails/rails/commit/c177e45858ebecbdb0782b6f25e538054794277b"><code>c177e45</code></a> updating version and changelog</li>
<li><a href="https://github.com/rails/rails/commit/433115554d3ea0b4dab9df99548c47707cadb20d"><code>4331155</code></a> Preparing for 6.0.5 release</li>
<li><a href="https://github.com/rails/rails/commit/1b5df893d82a27da907e9b8b75deff13179d1df3"><code>1b5df89</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/rails/rails/issues/45027">#45027</a> from rails/fix-tag-helper-regression</li>
<li><a href="https://github.com/rails/rails/commit/23f8485dced9be73877ae98a6554c7d34156866b"><code>23f8485</code></a> Merge branch '6-0-sec' into 6-0-stable</li>
<li><a href="https://github.com/rails/rails/commit/27a5ec76eed1e5d0bc5649b0e92097267c0b4338"><code>27a5ec7</code></a> Preparing for 6.0.4.8 release</li>
<li><a href="https://github.com/rails/rails/commit/636ee650d4a4edfca8ab6f2e982b543951976a59"><code>636ee65</code></a> updating changelog for release</li>
<li><a href="https://github.com/rails/rails/commit/36a6dad07d572a0098c29d6d96a226638a7caa38"><code>36a6dad</code></a> Fix and add protections for XSS in names.</li>
<li>Additional commits viewable in <a href="https://github.com/rails/rails/compare/v6.0.3.2...v6.0.6.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=activesupport&package-manager=bundler&previous-version=6.0.3.2&new-version=6.0.6.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-01-31 01:15:30 +0000 UTC
    </div>
</div>

