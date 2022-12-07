---
layout: default
title: indy-did-method
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-did-method
---

# indy-did-method <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-did-method){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-did-method/pull/75" class=".btn">#75</a>
            </td>
            <td>
                <b>
                    Bump decode-uri-component from 0.2.0 to 0.2.2
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-did-method/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-07 11:06:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-did-method/pull/74" class=".btn">#74</a>
            </td>
            <td>
                <b>
                    Bump qs from 6.9.4 to 6.11.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [qs](https://github.com/ljharb/qs) from 6.9.4 to 6.11.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ljharb/qs/blob/main/CHANGELOG.md">qs's changelog</a>.</em></p>
<blockquote>
<h2><strong>6.11.0</strong></h2>
<ul>
<li>[New] [Fix] <code>stringify</code>: revert 0e903c0; add <code>commaRoundTrip</code> option (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/442">#442</a>)</li>
<li>[readme] fix version badge</li>
</ul>
<h2><strong>6.10.5</strong></h2>
<ul>
<li>[Fix] <code>stringify</code>: with <code>arrayFormat: comma</code>, properly include an explicit <code>[]</code> on a single-item array (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/434">#434</a>)</li>
</ul>
<h2><strong>6.10.4</strong></h2>
<ul>
<li>[Fix] <code>stringify</code>: with <code>arrayFormat: comma</code>, include an explicit <code>[]</code> on a single-item array (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/441">#441</a>)</li>
<li>[meta] use <code>npmignore</code> to autogenerate an npmignore file</li>
<li>[Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>aud</code>, <code>has-symbol</code>, <code>object-inspect</code>, <code>tape</code></li>
</ul>
<h2><strong>6.10.3</strong></h2>
<ul>
<li>[Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/428">#428</a>)</li>
<li>[Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/427">#427</a>)</li>
<li>[actions] reuse common workflows</li>
<li>[Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>object-inspect</code>, <code>tape</code></li>
</ul>
<h2><strong>6.10.2</strong></h2>
<ul>
<li>[Fix] <code>stringify</code>: actually fix cyclic references (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/426">#426</a>)</li>
<li>[Fix] <code>stringify</code>: avoid encoding arrayformat comma when <code>encodeValuesOnly = true</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/424">#424</a>)</li>
<li>[readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li>[Docs] add note and links for coercing primitive values (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/408">#408</a>)</li>
<li>[actions] update codecov uploader</li>
<li>[actions] update workflows</li>
<li>[Tests] clean up stringify tests slightly</li>
<li>[Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>aud</code>, <code>object-inspect</code>, <code>safe-publish-latest</code>, <code>tape</code></li>
</ul>
<h2><strong>6.10.1</strong></h2>
<ul>
<li>[Fix] <code>stringify</code>: avoid exception on repeated object values (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/402">#402</a>)</li>
</ul>
<h2><strong>6.10.0</strong></h2>
<ul>
<li>[New] <code>stringify</code>: throw on cycles, instead of an infinite loop (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/395">#395</a>, <a href="https://github-redirect.dependabot.com/ljharb/qs/issues/394">#394</a>, <a href="https://github-redirect.dependabot.com/ljharb/qs/issues/393">#393</a>)</li>
<li>[New] <code>parse</code>: add <code>allowSparse</code> option for collapsing arrays with missing indices (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/312">#312</a>)</li>
<li>[meta] fix README.md (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/399">#399</a>)</li>
<li>[meta] only run <code>npm run dist</code> in publish, not install</li>
<li>[Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>aud</code>, <code>has-symbols</code>, <code>tape</code></li>
<li>[Tests] fix tests on node v0.6</li>
<li>[Tests] use <code>ljharb/actions/node/install</code> instead of <code>ljharb/actions/node/run</code></li>
<li>[Tests] Revert &quot;[meta] ignore eclint transitive audit warning&quot;</li>
</ul>
<h2><strong>6.9.7</strong></h2>
<ul>
<li>[Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/428">#428</a>)</li>
<li>[Fix] <code>stringify</code>: avoid encoding arrayformat comma when <code>encodeValuesOnly = true</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/424">#424</a>)</li>
<li>[Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/427">#427</a>)</li>
<li>[readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li>[Docs] add note and links for coercing primitive values (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/408">#408</a>)</li>
<li>[Tests] clean up stringify tests slightly</li>
<li>[meta] fix README.md (<a href="https://github-redirect.dependabot.com/ljharb/qs/issues/399">#399</a>)</li>
<li>Revert &quot;[meta] ignore eclint transitive audit warning&quot;</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ljharb/qs/commit/56763c12ec4fbf723333cbb32371cbd386c33cbb"><code>56763c1</code></a> v6.11.0</li>
<li><a href="https://github.com/ljharb/qs/commit/ddd3e293b801df7a06cb7f2746462a6ca1dd3fb2"><code>ddd3e29</code></a> [readme] fix version badge</li>
<li><a href="https://github.com/ljharb/qs/commit/c31347299f34afca90e8b5ff793eb4d0f77cfa56"><code>c313472</code></a> [New] [Fix] <code>stringify</code>: revert 0e903c0; add <code>commaRoundTrip</code> option</li>
<li><a href="https://github.com/ljharb/qs/commit/95bc0185e157d400da4f43f1fcf1c7f008fd847e"><code>95bc018</code></a> v6.10.5</li>
<li><a href="https://github.com/ljharb/qs/commit/0e903c0a9092618756b0962f1b80655ac0da436a"><code>0e903c0</code></a> [Fix] <code>stringify</code>: with <code>arrayFormat: comma</code>, properly include an explicit `[...</li>
<li><a href="https://github.com/ljharb/qs/commit/ba9703c0340dfdeb73cb4387d6ab32c37768aa5b"><code>ba9703c</code></a> v6.10.4</li>
<li><a href="https://github.com/ljharb/qs/commit/4e440195c7647f21c20bb76340774cb3a0cb6eac"><code>4e44019</code></a> [Fix] <code>stringify</code>: with <code>arrayFormat: comma</code>, include an explicit <code>[]</code> on a s...</li>
<li><a href="https://github.com/ljharb/qs/commit/113b990ed23ae8d6f670eb879e16ed105cd9081b"><code>113b990</code></a> [Dev Deps] update <code>object-inspect</code></li>
<li><a href="https://github.com/ljharb/qs/commit/c77f38f7174b9f10e8937e0f601fa1e6f0373b33"><code>c77f38f</code></a> [Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>aud</code>, <code>has-symbol</code>, <code>tape</code></li>
<li><a href="https://github.com/ljharb/qs/commit/2cf45b2dcd31a6d5c7fc16f33c7148fade0eef1e"><code>2cf45b2</code></a> [meta] use <code>npmignore</code> to autogenerate an npmignore file</li>
<li>Additional commits viewable in <a href="https://github.com/ljharb/qs/compare/v6.9.4...v6.11.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=qs&package-manager=npm_and_yarn&previous-version=6.9.4&new-version=6.11.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-did-method/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-06 23:50:15 +0000 UTC
    </div>
</div>

