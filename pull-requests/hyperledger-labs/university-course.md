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
                PR <a href="https://github.com/hyperledger-labs/university-course/pull/88" class=".btn">#88</a>
            </td>
            <td>
                <b>
                    chore(deps): bump qs from 6.5.2 to 6.5.3 in /support/Lab06/b4s/organization/university/user-interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [qs](https://github.com/ljharb/qs) from 6.5.2 to 6.5.3.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ljharb/qs/blob/main/CHANGELOG.md">qs's changelog</a>.</em></p>
<blockquote>
<h2><strong>6.5.3</strong></h2>
<ul>
<li>[Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/428">#428</a>)</li>
<li>[Fix] <code>utils.merge</code>: avoid a crash with a null target and a truthy non-array source</li>
<li>[Fix] correctly parse nested arrays</li>
<li>[Fix] <code>stringify</code>: fix a crash with <code>strictNullHandling</code> and a custom <code>filter</code>/<code>serializeDate</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/279">#279</a>)</li>
<li>[Fix] <code>utils</code>: <code>merge</code>: fix crash when <code>source</code> is a truthy primitive &amp; no options are provided</li>
<li>[Fix] when <code>parseArrays</code> is false, properly handle keys ending in <code>[]</code></li>
<li>[Fix] fix for an impossible situation: when the formatter is called with a non-string value</li>
<li>[Fix] <code>utils.merge</code>: avoid a crash with a null target and an array source</li>
<li>[Refactor] <code>utils</code>: reduce observable [[Get]]s</li>
<li>[Refactor] use cached <code>Array.isArray</code></li>
<li>[Refactor] <code>stringify</code>: Avoid arr = arr.concat(...), push to the existing instance (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/269">#269</a>)</li>
<li>[Refactor] <code>parse</code>: only need to reassign the var once</li>
<li>[Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/427">#427</a>)</li>
<li>[readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li>[Docs] Clean up license text so it’s properly detected as BSD-3-Clause</li>
<li>[Docs] Clarify the need for &quot;arrayLimit&quot; option</li>
<li>[meta] fix README.md (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/399">#399</a>)</li>
<li>[meta] add FUNDING.yml</li>
<li>[actions] backport actions from main</li>
<li>[Tests] always use <code>String(x)</code> over <code>x.toString()</code></li>
<li>[Tests] remove nonexistent tape option</li>
<li>[Dev Deps] backport from main</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ljharb/qs/commit/298bfa55d6db00ddea78dd0333509aadf9bb3077"><code>298bfa5</code></a> v6.5.3</li>
<li><a href="https://github.com/ljharb/qs/commit/ed0f5dcbef4b168a8ae299d78b1e4a2e9b1baf1f"><code>ed0f5dc</code></a> [Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/428">#428</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/691e739cfa40cd42604dc05a54e6154371a429ab"><code>691e739</code></a> [Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/427">#427</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/1072d57d38a690e1ad7616dced44390bffedcbb2"><code>1072d57</code></a> [readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li><a href="https://github.com/ljharb/qs/commit/12ac1c403aaa04d1a34844f514ed9f9abfb76e64"><code>12ac1c4</code></a> [meta] fix README.md (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/399">#399</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/0338716b09fdbd4711823eeb0a14e556a2498e7a"><code>0338716</code></a> [actions] backport actions from main</li>
<li><a href="https://github.com/ljharb/qs/commit/5639c20ce0a7c1332200a3181339331483e5a3a1"><code>5639c20</code></a> Clean up license text so it’s properly detected as BSD-3-Clause</li>
<li><a href="https://github.com/ljharb/qs/commit/51b8a0b1b213596dd1702b837f5e7dec2229793d"><code>51b8a0b</code></a> add FUNDING.yml</li>
<li><a href="https://github.com/ljharb/qs/commit/45f675936e742d92fac8d4dae5cfc385c576a977"><code>45f6759</code></a> [Fix] fix for an impossible situation: when the formatter is called with a no...</li>
<li><a href="https://github.com/ljharb/qs/commit/f814a7f8f2af059f8158f7e4b2bf8b46aeb62cd3"><code>f814a7f</code></a> [Dev Deps] backport from main</li>
<li>Additional commits viewable in <a href="https://github.com/ljharb/qs/compare/v6.5.2...v6.5.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=qs&package-manager=npm_and_yarn&previous-version=6.5.2&new-version=6.5.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-12-08 23:04:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/university-course/pull/87" class=".btn">#87</a>
            </td>
            <td>
                <b>
                    chore(deps): bump decode-uri-component from 0.2.0 to 0.2.2 in /support/Lab06/b4s/organization/university/user-interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [decode-uri-component](https://github.com/SamVerschueren/decode-uri-component) from 0.2.0 to 0.2.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/SamVerschueren/decode-uri-component/releases">decode-uri-component's releases</a>.</em></p>
<blockquote>
<h2>v0.2.2</h2>
<ul>
<li>Prevent overwriting previously decoded tokens  980e0bf</li>
</ul>
<p><a href="https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.1...v0.2.2">https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.1...v0.2.2</a></p>
<h2>v0.2.1</h2>
<ul>
<li>Switch to GitHub workflows  76abc93</li>
<li>Fix issue where decode throws - fixes <a href="https://github-redirect.dependabot.com/SamVerschueren/decode-uri-component/issues/6">#6</a>  746ca5d</li>
<li>Update license (<a href="https://github-redirect.dependabot.com/SamVerschueren/decode-uri-component/issues/1">#1</a>)  486d7e2</li>
<li>Tidelift tasks  a650457</li>
<li>Meta tweaks  66e1c28</li>
</ul>
<p><a href="https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.0...v0.2.1">https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.0...v0.2.1</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/a0eea469d26eb0df668b081672cdb9581feb78eb"><code>a0eea46</code></a> 0.2.2</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/980e0bf09b64d94f1aa79012f895816c30ffd152"><code>980e0bf</code></a> Prevent overwriting previously decoded tokens</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/3c8a373dd4837e89b3f970e01295dd03e1405a33"><code>3c8a373</code></a> 0.2.1</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/76abc939783fe3900fadb7d384a74d324d5557f3"><code>76abc93</code></a> Switch to GitHub workflows</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/746ca5dcb6667c5d364e782d53c542830e4c10b9"><code>746ca5d</code></a> Fix issue where decode throws - fixes <a href="https://github-redirect.dependabot.com/SamVerschueren/decode-uri-component/issues/6">#6</a></li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/486d7e26d3a8c0fbe860fb651fe1bc98c2f2be30"><code>486d7e2</code></a> Update license (<a href="https://github-redirect.dependabot.com/SamVerschueren/decode-uri-component/issues/1">#1</a>)</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/a65045724e6234acef87f31da499d4807b20b134"><code>a650457</code></a> Tidelift tasks</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/66e1c2834c0e189201cb65196ec3101372459b02"><code>66e1c28</code></a> Meta tweaks</li>
<li>See full diff in <a href="https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.0...v0.2.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=decode-uri-component&package-manager=npm_and_yarn&previous-version=0.2.0&new-version=0.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-12-06 21:50:41 +0000 UTC
    </div>
</div>

