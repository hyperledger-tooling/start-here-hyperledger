---
layout: default
title: fabric-ca
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-ca
---

# fabric-ca <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-ca){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/377" class=".btn">#377</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 1.26.16 to 1.26.17 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [urllib3](https://github.com/urllib3/urllib3) from 1.26.16 to 1.26.17.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/releases">urllib3's releases</a>.</em></p>
<blockquote>
<h2>1.26.17</h2>
<ul>
<li>Added the <code>Cookie</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>. (GHSA-v845-jxx5-vc9f)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/blob/main/CHANGES.rst">urllib3's changelog</a>.</em></p>
<blockquote>
<h1>1.26.17 (2023-10-02)</h1>
<ul>
<li>Added the <code>Cookie</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>. (<code>[#3139](https://github.com/urllib3/urllib3/issues/3139) &lt;https://github.com/urllib3/urllib3/pull/3139&gt;</code>_)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/urllib3/urllib3/commit/c9016bf464751a02b7e46f8b86504f47d4238784"><code>c9016bf</code></a> Release 1.26.17</li>
<li><a href="https://github.com/urllib3/urllib3/commit/01220354d389cd05474713f8c982d05c9b17aafb"><code>0122035</code></a> Backport GHSA-v845-jxx5-vc9f (<a href="https://redirect.github.com/urllib3/urllib3/issues/3139">#3139</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/e63989f97d206e839ab9170c8a76e3e097cc60e8"><code>e63989f</code></a> Fix installing <code>brotli</code> extra on Python 2.7</li>
<li><a href="https://github.com/urllib3/urllib3/commit/2e7a24d08713a0131f0b3c7197889466d645cc49"><code>2e7a24d</code></a> [1.26] Configure OS for RTD to fix building docs</li>
<li><a href="https://github.com/urllib3/urllib3/commit/57181d6ea910ac7cb2ff83345d9e5e0eb816a0d0"><code>57181d6</code></a> [1.26] Improve error message when calling urllib3.request() (<a href="https://redirect.github.com/urllib3/urllib3/issues/3058">#3058</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/3c0148048a523325819377b23fc67f8d46afc3aa"><code>3c01480</code></a> [1.26] Run coverage even with failed jobs</li>
<li>See full diff in <a href="https://github.com/urllib3/urllib3/compare/1.26.16...1.26.17">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=urllib3&package-manager=pip&previous-version=1.26.16&new-version=1.26.17)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-ca/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 04:02:13 +0000 UTC
    </div>
</div>

