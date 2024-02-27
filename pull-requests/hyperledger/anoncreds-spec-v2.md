---
layout: default
title: anoncreds-spec-v2
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/anoncreds-spec-v2
---

# anoncreds-spec-v2 <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/anoncreds-spec-v2){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-spec-v2/pull/8" class=".btn">#8</a>
            </td>
            <td>
                <b>
                    Bump es5-ext from 0.10.62 to 0.10.64
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [es5-ext](https://github.com/medikoo/es5-ext) from 0.10.62 to 0.10.64.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/medikoo/es5-ext/releases">es5-ext's releases</a>.</em></p>
<blockquote>
<h2>0.10.64 (2024-02-27)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>Revert update to postinstall script meant to fix Powershell issue, as it's a regression for some Linux terminals (<a href="https://github.com/medikoo/es5-ext/commit/c2e2bb90c295c4c582445a6f03b2a3ad0b22550a">c2e2bb9</a>)</li>
</ul>
<hr />
<p><a href="https://github.com/medikoo/es5-ext/compare/v0.10.63...v0.10.64">Comparison since last release</a></p>
<h2>0.10.63 (2024-02-23)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>Do not rely on problematic regex (<a href="https://github.com/medikoo/es5-ext/commit/3551cdd7b2db08b1632841f819d008757d28e8e2">3551cdd</a>), addresses <a href="https://redirect.github.com/medikoo/es5-ext/issues/201">#201</a></li>
<li>Support ES2015+ function definitions in <code>function#toStringTokens()</code> (<a href="https://github.com/medikoo/es5-ext/commit/a52e95736690ad1d465ebcd9791d54570e294602">a52e957</a>), addresses <a href="https://redirect.github.com/medikoo/es5-ext/issues/021">#021</a></li>
<li>Ensure postinstall script does not crash on Windows, fixes <a href="https://redirect.github.com/medikoo/es5-ext/issues/181">#181</a> (<a href="https://github.com/medikoo/es5-ext/commit/bf8ed799d57df53096da9d908ff577f305e1366f">bf8ed79</a>)</li>
</ul>
<h3>Maintenance Improvements</h3>
<ul>
<li>Simplify the manifest message (<a href="https://github.com/medikoo/es5-ext/commit/7855319f41b9736639cf4555bd2c419f17addf55">7855319</a>)</li>
</ul>
<hr />
<p><a href="https://github.com/medikoo/es5-ext/compare/v0.10.62...v0.10.63">Comparison since last release</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/medikoo/es5-ext/blob/main/CHANGELOG.md">es5-ext's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/medikoo/es5-ext/compare/v0.10.63...v0.10.64">0.10.64</a> (2024-02-27)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>Revert update to postinstall script meant to fix Powershell issue, as it's a regression for some Linux terminals (<a href="https://github.com/medikoo/es5-ext/commit/c2e2bb90c295c4c582445a6f03b2a3ad0b22550a">c2e2bb9</a>)</li>
</ul>
<h3><a href="https://github.com/medikoo/es5-ext/compare/v0.10.62...v0.10.63">0.10.63</a> (2024-02-23)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>Do not rely on problematic regex (<a href="https://github.com/medikoo/es5-ext/commit/3551cdd7b2db08b1632841f819d008757d28e8e2">3551cdd</a>), addresses <a href="https://redirect.github.com/medikoo/es5-ext/issues/201">#201</a></li>
<li>Support ES2015+ function definitions in <code>function#toStringTokens()</code> (<a href="https://github.com/medikoo/es5-ext/commit/a52e95736690ad1d465ebcd9791d54570e294602">a52e957</a>), addresses <a href="https://redirect.github.com/medikoo/es5-ext/issues/021">#021</a></li>
<li>Ensure postinstall script does not crash on Windows, fixes <a href="https://redirect.github.com/medikoo/es5-ext/issues/181">#181</a> (<a href="https://github.com/medikoo/es5-ext/commit/bf8ed799d57df53096da9d908ff577f305e1366f">bf8ed79</a>)</li>
</ul>
<h3>Maintenance Improvements</h3>
<ul>
<li>Simplify the manifest message (<a href="https://github.com/medikoo/es5-ext/commit/7855319f41b9736639cf4555bd2c419f17addf55">7855319</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/medikoo/es5-ext/commit/f76b03d8c49ce4871f37f428c0e1d3ee6637fcc4"><code>f76b03d</code></a> chore: Release v0.10.64</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/2881acda50de0848b456690769919ed4b86be489"><code>2881acd</code></a> chore: Bump dependencies</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/c2e2bb90c295c4c582445a6f03b2a3ad0b22550a"><code>c2e2bb9</code></a> fix: Revert update meant to fix Powershell issue, as it's a regression</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/16f2b7253d3d8d499d8cf1d3ca76c585da7f08d3"><code>16f2b72</code></a> docs: Fix date in the changelog</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/de4e03c4776a303284142f73f3f181a070615817"><code>de4e03c</code></a> chore: Release v0.10.63</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/3fd53b755ec883be8f119c747f0b04130741e456"><code>3fd53b7</code></a> chore: Upgrade<code> lint-staged</code> to v13</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/bf8ed799d57df53096da9d908ff577f305e1366f"><code>bf8ed79</code></a> chore: Ensure postinstall script does not crash on Windows</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/2cbbb0717bd8de6e38fcba1f0d45bc876e7a1951"><code>2cbbb07</code></a> chore: Bump dependencies</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/22d0416ea170000a115609f22a560dfa9193ebb0"><code>22d0416</code></a> chore: Bump LICENSE year</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/a52e95736690ad1d465ebcd9791d54570e294602"><code>a52e957</code></a> fix: Support ES2015+ function definitions in <code>function#toStringTokens()</code></li>
<li>Additional commits viewable in <a href="https://github.com/medikoo/es5-ext/compare/v0.10.62...v0.10.64">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=es5-ext&package-manager=npm_and_yarn&previous-version=0.10.62&new-version=0.10.64)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/anoncreds-spec-v2/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-27 17:44:41 +0000 UTC
    </div>
</div>

