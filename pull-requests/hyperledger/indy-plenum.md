---
layout: default
title: indy-plenum
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-plenum
---

# indy-plenum <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-plenum){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-plenum/pull/1655" class=".btn">#1655</a>
            </td>
            <td>
                <b>
                    Bump the all-actions group with 1 update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps the all-actions group with 1 update: [softprops/action-gh-release](https://github.com/softprops/action-gh-release).

Updates `softprops/action-gh-release` from 1 to 2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/softprops/action-gh-release/releases">softprops/action-gh-release's releases</a>.</em></p>
<blockquote>
<h2>v2.0.0</h2>
<ul>
<li>update actions.yml declaration to node20 to address warnings</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/softprops/action-gh-release/blob/master/CHANGELOG.md">softprops/action-gh-release's changelog</a>.</em></p>
<blockquote>
<h2>0.1.12</h2>
<ul>
<li>fix bug leading to empty strings subsituted for inputs users don't provide breaking api calls <a href="https://redirect.github.com/softprops/action-gh-release/pull/144">#144</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/softprops/action-gh-release/commit/d99959edae48b5ffffd7b00da66dcdb0a33a52ee"><code>d99959e</code></a> prep release</li>
<li><a href="https://github.com/softprops/action-gh-release/commit/0e39c679e8bac647fe5ad41070fe2295b0393d58"><code>0e39c67</code></a> make pattern error opt in (<a href="https://redirect.github.com/softprops/action-gh-release/issues/417">#417</a>)</li>
<li><a href="https://github.com/softprops/action-gh-release/commit/20e085ccc73308c2c8e43ab8da4f8d7ecbb94d4e"><code>20e085c</code></a> kick off 2.0.1 release</li>
<li><a href="https://github.com/softprops/action-gh-release/commit/9f5c4d39bc56b5ed07f92f260dd05d33000058a6"><code>9f5c4d3</code></a> update changelog</li>
<li><a href="https://github.com/softprops/action-gh-release/commit/0bea76b22707a1871a52b97e07c80657071adb76"><code>0bea76b</code></a> Add support for make_latest property (<a href="https://redirect.github.com/softprops/action-gh-release/issues/304">#304</a>)</li>
<li><a href="https://github.com/softprops/action-gh-release/commit/762fe13dfbc8921c36ebb81da5626a394a6a5b95"><code>762fe13</code></a> typo in changelog</li>
<li><a href="https://github.com/softprops/action-gh-release/commit/c0f2569fb90b35a0e2b043535a5778f437ec86ea"><code>c0f2569</code></a> remove unused script</li>
<li><a href="https://github.com/softprops/action-gh-release/commit/5743e060246b253faba6cb8e051511b63e7639c9"><code>5743e06</code></a> update changelog</li>
<li><a href="https://github.com/softprops/action-gh-release/commit/fe71fd3b919b0ad8636bb9a2930b15466814fbb7"><code>fe71fd3</code></a> Don't swallow errors (<a href="https://redirect.github.com/softprops/action-gh-release/issues/384">#384</a>)</li>
<li><a href="https://github.com/softprops/action-gh-release/commit/9150ab13f3b0f0b7df0b9979d0e04968f5844d96"><code>9150ab1</code></a> rebuild and update changelog</li>
<li>Additional commits viewable in <a href="https://github.com/softprops/action-gh-release/compare/v1...v2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=softprops/action-gh-release&package-manager=github_actions&previous-version=1&new-version=2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-11 11:31:54 +0000 UTC
    </div>
</div>

