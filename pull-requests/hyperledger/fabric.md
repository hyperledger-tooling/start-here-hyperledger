---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4924" class=".btn">#4924</a>
            </td>
            <td>
                <b>
                    Bump zipp from 3.15.0 to 3.19.1 in /docs in the pip group across 1 directory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group with 1 update in the /docs directory: [zipp](https://github.com/jaraco/zipp).

Updates `zipp` from 3.15.0 to 3.19.1
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/jaraco/zipp/blob/main/NEWS.rst">zipp's changelog</a>.</em></p>
<blockquote>
<h1>v3.19.1</h1>
<h2>Bugfixes</h2>
<ul>
<li>Improved handling of malformed zip files. (<a href="https://redirect.github.com/jaraco/zipp/issues/119">#119</a>)</li>
</ul>
<h1>v3.19.0</h1>
<h2>Features</h2>
<ul>
<li>Implement is_symlink. (<a href="https://redirect.github.com/jaraco/zipp/issues/117">#117</a>)</li>
</ul>
<h1>v3.18.2</h1>
<p>No significant changes.</p>
<h1>v3.18.1</h1>
<p>No significant changes.</p>
<h1>v3.18.0</h1>
<h2>Features</h2>
<ul>
<li>Bypass ZipFile.namelist in glob for better performance. (<a href="https://redirect.github.com/jaraco/zipp/issues/106">#106</a>)</li>
<li>Refactored glob functionality to support a more generalized solution with support for platform-specific path separators. (<a href="https://redirect.github.com/jaraco/zipp/issues/108">#108</a>)</li>
</ul>
<h2>Bugfixes</h2>
<ul>
<li>Add special accounting for pypy when computing the stack level for text encoding warnings. (<a href="https://redirect.github.com/jaraco/zipp/issues/114">#114</a>)</li>
</ul>
<h1>v3.17.0</h1>
<p>Features</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jaraco/zipp/commit/6d1cb72aa55e0536f35d2af128994b5a61ca4c1a"><code>6d1cb72</code></a> Finalize</li>
<li><a href="https://github.com/jaraco/zipp/commit/fd604bd34f0343472521a36da1fbd22e793e14fd"><code>fd604bd</code></a> Merge pull request <a href="https://redirect.github.com/jaraco/zipp/issues/120">#120</a> from jaraco/bugfix/119-malformed-paths</li>
<li><a href="https://github.com/jaraco/zipp/commit/c18417ed2953e181728a7dac07bff88a2190abf7"><code>c18417e</code></a> Add news fragment.</li>
<li><a href="https://github.com/jaraco/zipp/commit/58115d2be968644ce71ce6bcc9b79826c82a1806"><code>58115d2</code></a> Employ SanitizedNames in CompleteDirs. Fixes broken test.</li>
<li><a href="https://github.com/jaraco/zipp/commit/564fcc10cdbfdaecdb33688e149827465931c9e0"><code>564fcc1</code></a> Add SanitizedNames mixin.</li>
<li><a href="https://github.com/jaraco/zipp/commit/79a309fe54dc6b7934fb72e9f31bcb58f2e9f547"><code>79a309f</code></a> Add some assertions about malformed paths.</li>
<li><a href="https://github.com/jaraco/zipp/commit/2d015c22348fab46ca765339f55f84fe9d6e8115"><code>2d015c2</code></a> Merge <a href="https://github.com/jaraco/skeleton">https://github.com/jaraco/skeleton</a></li>
<li><a href="https://github.com/jaraco/zipp/commit/a595a0fad054cd20b69d3e954c99174e3a548938"><code>a595a0f</code></a> Rename extras to align with core metadata spec.</li>
<li><a href="https://github.com/jaraco/zipp/commit/608f90a6e74919501577a1312dc5c7d8e1d391d7"><code>608f90a</code></a> Finalize</li>
<li><a href="https://github.com/jaraco/zipp/commit/3a22d724acf874111b43f87f7110225122ec3de5"><code>3a22d72</code></a> Merge pull request <a href="https://redirect.github.com/jaraco/zipp/issues/118">#118</a> from jaraco/feature/is-symlink</li>
<li>Additional commits viewable in <a href="https://github.com/jaraco/zipp/compare/v3.15.0...v3.19.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=zipp&package-manager=pip&previous-version=3.15.0&new-version=3.19.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot ignore <dependency name> major version` will close this group update PR and stop Dependabot creating any more for the specific dependency's major version (unless you unignore this specific dependency's major version or upgrade to it yourself)
- `@dependabot ignore <dependency name> minor version` will close this group update PR and stop Dependabot creating any more for the specific dependency's minor version (unless you unignore this specific dependency's minor version or upgrade to it yourself)
- `@dependabot ignore <dependency name>` will close this group update PR and stop Dependabot creating any more for the specific dependency (unless you unignore this specific dependency or upgrade to it yourself)
- `@dependabot unignore <dependency name>` will remove all of the ignore conditions of the specified dependency
- `@dependabot unignore <dependency name> <ignore condition>` will remove the ignore condition of the specified dependency and ignore conditions
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-09 18:12:41 +0000 UTC
    </div>
</div>

