---
layout: default
title: aries-acapy-plugins
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-plugins
---

# aries-acapy-plugins <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-plugins){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/732" class=".btn">#732</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.5.0 to 0.5.1 in /firebase_push_notifications
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.5.0 to 0.5.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>0.5.1</h2>
<h2>Release Notes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement mutable-contextvar-default (B039) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12113">#12113</a>)</li>
<li>[<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12140">#12140</a>)</li>
<li>[<code>pytest</code>] Reverse <code>PT001</code> and <code>PT0023</code> defaults (<a href="https://redirect.github.com/astral-sh/ruff/pull/12106">#12106</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>Enable token-based rules on source with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/11950">#11950</a>)</li>
<li>[<code>flake8-bandit</code>] Detect <code>httpx</code> for <code>S113</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12174">#12174</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY201</code> to include exception deprecations (<a href="https://redirect.github.com/astral-sh/ruff/pull/12065">#12065</a>)</li>
<li>[<code>pylint</code>] Generate autofix for <code>duplicate-bases</code> (<code>PLE0241</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12105">#12105</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Avoid syntax error notification for source code actions (<a href="https://redirect.github.com/astral-sh/ruff/pull/12148">#12148</a>)</li>
<li>Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/pull/12203">#12203</a>)</li>
<li>Fix replacement edit range computation (<a href="https://redirect.github.com/astral-sh/ruff/pull/12171">#12171</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Disable auto-fix when source has syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/12134">#12134</a>)</li>
<li>Fix cache key collisions for paths with separators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12159">#12159</a>)</li>
<li>Make <code>requires-python</code> inference robust to <code>==</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12091">#12091</a>)</li>
<li>Use char-wise width instead of <code>str</code>-width (<a href="https://redirect.github.com/astral-sh/ruff/pull/12135">#12135</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword followed by comma (<a href="https://redirect.github.com/astral-sh/ruff/pull/12136">#12136</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword is followed by a semicolon (<a href="https://redirect.github.com/astral-sh/ruff/pull/12095">#12095</a>)</li>
<li>[<code>pylint</code>] Skip <a href="https://docs.astral.sh/ruff/settings/#lint_dummy-variable-rgx">dummy variables</a> for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12190">#12190</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Remove allocation in <code>parse_identifier</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12103">#12103</a>)</li>
<li>Use <code>CompactString</code> for <code>Identifier</code> AST node (<a href="https://redirect.github.com/astral-sh/ruff/pull/12101">#12101</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/Peiffap"><code>@​Peiffap</code></a></li>
<li><a href="https://github.com/ThomasFaivre"><code>@​ThomasFaivre</code></a></li>
<li><a href="https://github.com/bersace"><code>@​bersace</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/github-actions"><code>@​github-actions</code></a></li>
<li><a href="https://github.com/jkauerl"><code>@​jkauerl</code></a></li>
<li><a href="https://github.com/mkniewallner"><code>@​mkniewallner</code></a></li>
<li><a href="https://github.com/mtsokol"><code>@​mtsokol</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.5.1</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement mutable-contextvar-default (B039) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12113">#12113</a>)</li>
<li>[<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12140">#12140</a>)</li>
<li>[<code>pytest</code>] Reverse <code>PT001</code> and <code>PT0023</code> defaults (<a href="https://redirect.github.com/astral-sh/ruff/pull/12106">#12106</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>Enable token-based rules on source with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/11950">#11950</a>)</li>
<li>[<code>flake8-bandit</code>] Detect <code>httpx</code> for <code>S113</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12174">#12174</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY201</code> to include exception deprecations (<a href="https://redirect.github.com/astral-sh/ruff/pull/12065">#12065</a>)</li>
<li>[<code>pylint</code>] Generate autofix for <code>duplicate-bases</code> (<code>PLE0241</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12105">#12105</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Avoid syntax error notification for source code actions (<a href="https://redirect.github.com/astral-sh/ruff/pull/12148">#12148</a>)</li>
<li>Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/pull/12203">#12203</a>)</li>
<li>Fix replacement edit range computation (<a href="https://redirect.github.com/astral-sh/ruff/pull/12171">#12171</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Disable auto-fix when source has syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/12134">#12134</a>)</li>
<li>Fix cache key collisions for paths with separators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12159">#12159</a>)</li>
<li>Make <code>requires-python</code> inference robust to <code>==</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12091">#12091</a>)</li>
<li>Use char-wise width instead of <code>str</code>-width (<a href="https://redirect.github.com/astral-sh/ruff/pull/12135">#12135</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword followed by comma (<a href="https://redirect.github.com/astral-sh/ruff/pull/12136">#12136</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword is followed by a semicolon (<a href="https://redirect.github.com/astral-sh/ruff/pull/12095">#12095</a>)</li>
<li>[<code>pylint</code>] Skip <a href="https://docs.astral.sh/ruff/settings/#lint_dummy-variable-rgx">dummy variables</a> for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12190">#12190</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Remove allocation in <code>parse_identifier</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12103">#12103</a>)</li>
<li>Use <code>CompactString</code> for <code>Identifier</code> AST node (<a href="https://redirect.github.com/astral-sh/ruff/pull/12101">#12101</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/3a72400202642f0bb340fb2b1d1c31da2b6524dd"><code>3a72400</code></a> Rename publish workflow file extension (<code>yaml</code> -&gt; <code>yml</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/12206">#12206</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1b3bff03300b2c48f0ad6c7bd6b1038e2f1fce5a"><code>1b3bff0</code></a> Bump version to 0.5.1 (<a href="https://redirect.github.com/astral-sh/ruff/issues/12205">#12205</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/0f6f73ecf3c2ebfe5b218edc0765886ccdca6f7f"><code>0f6f73e</code></a> [red-knot] Require that <code>FileSystem</code> objects implement <code>Debug</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12204">#12204</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/7910beecc42b2694890b10011c27a3cbb2db3335"><code>7910bee</code></a> Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/issues/12203">#12203</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f3ccd152e99d6bccfec58275c0b3b2ec3ffd5bdd"><code>f3ccd15</code></a> Revert &quot;Remove <code>--preview</code> as a required argument for <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12053">#12053</a>)&quot;...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1e07bfa3730db9461f51b877bf71ea31e7dd56e4"><code>1e07bfa</code></a> [<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/12140">#12140</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/5e7ba056128c8bc272ab1a2a22c9cb94a5079361"><code>5e7ba05</code></a> docs(*): fix a few typos, consistency issues and links (<a href="https://redirect.github.com/astral-sh/ruff/issues/12193">#12193</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d12570ea006d23a610e2410d9c70c3b3deae717c"><code>d12570e</code></a> docs(options): fix some typos and improve consistency (<a href="https://redirect.github.com/astral-sh/ruff/issues/12191">#12191</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2f3264e148b9cf31e32c3137feb0f5ce9532d85b"><code>2f3264e</code></a> fix(rules): skip dummy variables for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12190">#12190</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e2e0889a303e8ce9953a2eb8a426921d08176c5f"><code>e2e0889</code></a> [red-knot] Add very basic benchmark (<a href="https://redirect.github.com/astral-sh/ruff/issues/12182">#12182</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/0.5.0...0.5.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.5.0&new-version=0.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 12:03:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/731" class=".btn">#731</a>
            </td>
            <td>
                <b>
                    Bump google-auth from 2.29.0 to 2.31.0 in /firebase_push_notifications
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [google-auth](https://github.com/googleapis/google-auth-library-python) from 2.29.0 to 2.31.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/googleapis/google-auth-library-python/releases">google-auth's releases</a>.</em></p>
<blockquote>
<h2>v2.31.0</h2>
<h2><a href="https://github.com/googleapis/google-auth-library-python/compare/v2.30.0...v2.31.0">2.31.0</a> (2024-06-27)</h2>
<h3>Features</h3>
<ul>
<li>Adds X509 workload cert logic (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1527">#1527</a>) (<a href="https://github.com/googleapis/google-auth-library-python/commit/05220e06a23b3d4c398628918dab113abcce52db">05220e0</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>Added py.typed to MANIFEST.in (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1526">#1526</a>) (<a href="https://github.com/googleapis/google-auth-library-python/commit/1829a3be18aea5eca8b7272111d75eb61a6077b1">1829a3b</a>)</li>
<li>Pass trust_env kwarg to ClientSession (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1533">#1533</a>) (<a href="https://github.com/googleapis/google-auth-library-python/commit/6c15c9ad0ff90cf9bac044b38e72956aa3039cf6">6c15c9a</a>), closes <a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1530">#1530</a></li>
</ul>
<h2>v2.30.0</h2>
<h2><a href="https://github.com/googleapis/google-auth-library-python/compare/v2.29.0...v2.30.0">2.30.0</a> (2024-06-06)</h2>
<h3>Features</h3>
<ul>
<li>Add WebAuthn plugin component to handle WebAuthn get assertion request (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1464">#1464</a>) (<a href="https://github.com/googleapis/google-auth-library-python/commit/e25f336ab49c2018a222458a95ebe083e8a4eb2a">e25f336</a>)</li>
<li>ECP Provider drop cryptography requirement (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1524">#1524</a>) (<a href="https://github.com/googleapis/google-auth-library-python/commit/a821d719e2fc7bcdc21737fdf175d6f06aa9a56a">a821d71</a>)</li>
<li>Enable webauthn plugin for security keys (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1528">#1528</a>) (<a href="https://github.com/googleapis/google-auth-library-python/commit/e2d5e635da2cb2caf8240fb9e07fc381442a9d0c">e2d5e63</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>Fix id_token iam endpoint for non-gdu service credentials (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1506">#1506</a>) (<a href="https://github.com/googleapis/google-auth-library-python/commit/93d681e6cfb15eb4a3efada623be8ba73b302257">93d681e</a>)</li>
<li>Makes default token_url universe aware (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1514">#1514</a>) (<a href="https://github.com/googleapis/google-auth-library-python/commit/045776e5dfa3fb172ffaeb59bfe5c637778a5d34">045776e</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/googleapis/google-auth-library-python/blob/main/CHANGELOG.md">google-auth's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/googleapis/google-auth-library-python/compare/v2.30.0...v2.31.0">2.31.0</a> (2024-06-27)</h2>
<h3>Features</h3>
<ul>
<li>Adds X509 workload cert logic (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1527">#1527</a>) (<a href="https://github.com/googleapis/google-auth-library-python/commit/05220e06a23b3d4c398628918dab113abcce52db">05220e0</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>Added py.typed to MANIFEST.in (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1526">#1526</a>) (<a href="https://github.com/googleapis/google-auth-library-python/commit/1829a3be18aea5eca8b7272111d75eb61a6077b1">1829a3b</a>)</li>
<li>Pass trust_env kwarg to ClientSession (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1533">#1533</a>) (<a href="https://github.com/googleapis/google-auth-library-python/commit/6c15c9ad0ff90cf9bac044b38e72956aa3039cf6">6c15c9a</a>), closes <a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1530">#1530</a></li>
</ul>
<h2><a href="https://github.com/googleapis/google-auth-library-python/compare/v2.29.0...v2.30.0">2.30.0</a> (2024-06-06)</h2>
<h3>Features</h3>
<ul>
<li>Add WebAuthn plugin component to handle WebAuthn get assertion request (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1464">#1464</a>) (<a href="https://github.com/googleapis/google-auth-library-python/commit/e25f336ab49c2018a222458a95ebe083e8a4eb2a">e25f336</a>)</li>
<li>ECP Provider drop cryptography requirement (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1524">#1524</a>) (<a href="https://github.com/googleapis/google-auth-library-python/commit/a821d719e2fc7bcdc21737fdf175d6f06aa9a56a">a821d71</a>)</li>
<li>Enable webauthn plugin for security keys (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1528">#1528</a>) (<a href="https://github.com/googleapis/google-auth-library-python/commit/e2d5e635da2cb2caf8240fb9e07fc381442a9d0c">e2d5e63</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>Fix id_token iam endpoint for non-gdu service credentials (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1506">#1506</a>) (<a href="https://github.com/googleapis/google-auth-library-python/commit/93d681e6cfb15eb4a3efada623be8ba73b302257">93d681e</a>)</li>
<li>Makes default token_url universe aware (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1514">#1514</a>) (<a href="https://github.com/googleapis/google-auth-library-python/commit/045776e5dfa3fb172ffaeb59bfe5c637778a5d34">045776e</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/googleapis/google-auth-library-python/commit/2150bf2f1c62966a626fe90e07344be77c48fffe"><code>2150bf2</code></a> chore(main): release 2.31.0 (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1535">#1535</a>)</li>
<li><a href="https://github.com/googleapis/google-auth-library-python/commit/1829a3be18aea5eca8b7272111d75eb61a6077b1"><code>1829a3b</code></a> fix: Added py.typed to MANIFEST.in (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1526">#1526</a>)</li>
<li><a href="https://github.com/googleapis/google-auth-library-python/commit/cb982276e806c3f3c67faf85f009a9c688d084f4"><code>cb98227</code></a> chore: Use cryptography for the Provider as well. This is to have an easier t...</li>
<li><a href="https://github.com/googleapis/google-auth-library-python/commit/05220e06a23b3d4c398628918dab113abcce52db"><code>05220e0</code></a> feat: adds X509 workload cert logic (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1527">#1527</a>)</li>
<li><a href="https://github.com/googleapis/google-auth-library-python/commit/6c15c9ad0ff90cf9bac044b38e72956aa3039cf6"><code>6c15c9a</code></a> fix: pass trust_env kwarg to ClientSession (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1533">#1533</a>)</li>
<li><a href="https://github.com/googleapis/google-auth-library-python/commit/440f171e8e627516a4c6c14698a71ed0242f86e0"><code>440f171</code></a> chore: update token (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1534">#1534</a>)</li>
<li><a href="https://github.com/googleapis/google-auth-library-python/commit/48add44e98a44f08a0a099d4f75b0184f2d79e5b"><code>48add44</code></a> chore(main): release 2.30.0 (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1507">#1507</a>)</li>
<li><a href="https://github.com/googleapis/google-auth-library-python/commit/0d276da5e0615d13bc6867eb45badcbb1f08f7ed"><code>0d276da</code></a> chore: update sys test cred (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1532">#1532</a>)</li>
<li><a href="https://github.com/googleapis/google-auth-library-python/commit/e2d5e635da2cb2caf8240fb9e07fc381442a9d0c"><code>e2d5e63</code></a> feat: Enable webauthn plugin for security keys (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1528">#1528</a>)</li>
<li><a href="https://github.com/googleapis/google-auth-library-python/commit/adb94f7bd7d08213853c36311c96331dd426fbab"><code>adb94f7</code></a> chore: update sys test cred (<a href="https://redirect.github.com/googleapis/google-auth-library-python/issues/1531">#1531</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/googleapis/google-auth-library-python/compare/v2.29.0...v2.31.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google-auth&package-manager=pip&previous-version=2.29.0&new-version=2.31.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 12:03:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/730" class=".btn">#730</a>
            </td>
            <td>
                <b>
                    Bump aries-askar from 0.3.1 to 0.3.2 in /firebase_push_notifications
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [aries-askar](https://github.com/hyperledger/aries-askar) from 0.3.1 to 0.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperledger/aries-askar/releases">aries-askar's releases</a>.</em></p>
<blockquote>
<h2>v0.3.2</h2>
<h2>What's Changed</h2>
<ul>
<li>chore(js): update to stable 0.2.0 by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/222">hyperledger/aries-askar#222</a></li>
<li>Add Dependabot configuration by <a href="https://github.com/WadeBarnes"><code>@​WadeBarnes</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/223">hyperledger/aries-askar#223</a></li>
<li>build(deps): bump the all-actions group with 7 updates by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/224">hyperledger/aries-askar#224</a></li>
<li>build(deps): bump ip from 2.0.0 to 2.0.1 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/226">hyperledger/aries-askar#226</a></li>
<li>build(deps): bump es5-ext from 0.10.62 to 0.10.64 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/228">hyperledger/aries-askar#228</a></li>
<li>build(deps): bump mio from 0.8.10 to 0.8.11 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/229">hyperledger/aries-askar#229</a></li>
<li>build(deps): bump follow-redirects from 1.15.4 to 1.15.6 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/230">hyperledger/aries-askar#230</a></li>
<li>build(deps): bump the all-actions group with 1 update by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/231">hyperledger/aries-askar#231</a></li>
<li>fix(js): update ffi-napi by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/234">hyperledger/aries-askar#234</a></li>
<li>build(deps): bump a7ul/tar-action from 1.1.3 to 1.2.0 in the all-actions group by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/235">hyperledger/aries-askar#235</a></li>
<li>build(deps): bump whoami from 1.4.1 to 1.5.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/233">hyperledger/aries-askar#233</a></li>
<li>chore: update version for js wrapper by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/236">hyperledger/aries-askar#236</a></li>
<li>fix: correctly serliaize for buffer by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/238">hyperledger/aries-askar#238</a></li>
<li>Build Javascript on multiple platforms by <a href="https://github.com/brianorwhatever"><code>@​brianorwhatever</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/239">hyperledger/aries-askar#239</a></li>
<li>build(deps): bump rustls from 0.21.10 to 0.21.11 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/240">hyperledger/aries-askar#240</a></li>
<li>P256 keys using Secure Enclave and Android StrongBox by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/245">hyperledger/aries-askar#245</a></li>
<li>chore: update minSdkVersion to get the project version or fallback to 21 by <a href="https://github.com/ja-bravo"><code>@​ja-bravo</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/248">hyperledger/aries-askar#248</a></li>
<li>chore: updating dependabot to support gha, TS, JS and rust packages by <a href="https://github.com/rajpalc7"><code>@​rajpalc7</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/249">hyperledger/aries-askar#249</a></li>
<li>chore(js): update version to 0.2.2 by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/243">hyperledger/aries-askar#243</a></li>
<li>fix: Incorrect SQLite expire check by <a href="https://github.com/dkulic"><code>@​dkulic</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/261">hyperledger/aries-askar#261</a></li>
<li>Add python requirements file and update dependabot workflow by <a href="https://github.com/ff137"><code>@​ff137</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/262">hyperledger/aries-askar#262</a></li>
<li>chore(js): add expo example app and move to pnpm by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/247">hyperledger/aries-askar#247</a></li>
<li>build(deps-dev): update pytest requirement from ~=8.2.1 to ~=8.2.2 in /wrappers/python by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/265">hyperledger/aries-askar#265</a></li>
<li>chore: update library versions by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/271">hyperledger/aries-askar#271</a></li>
<li>build: allow action to create release by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/272">hyperledger/aries-askar#272</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/WadeBarnes"><code>@​WadeBarnes</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/223">hyperledger/aries-askar#223</a></li>
<li><a href="https://github.com/brianorwhatever"><code>@​brianorwhatever</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/239">hyperledger/aries-askar#239</a></li>
<li><a href="https://github.com/ja-bravo"><code>@​ja-bravo</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/248">hyperledger/aries-askar#248</a></li>
<li><a href="https://github.com/rajpalc7"><code>@​rajpalc7</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/249">hyperledger/aries-askar#249</a></li>
<li><a href="https://github.com/dkulic"><code>@​dkulic</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/261">hyperledger/aries-askar#261</a></li>
<li><a href="https://github.com/ff137"><code>@​ff137</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/262">hyperledger/aries-askar#262</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2">https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperledger/aries-askar/commit/10f58b3984bf6b2d370b8fb2cd07a0696bd93d2f"><code>10f58b3</code></a> build: allow action to create release</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/cf0586ed0cf28bc5197af40e4760158e79a77458"><code>cf0586e</code></a> chore: update library versions</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/c5ebacad74923a462ad754c5d726a0b069a62ca9"><code>c5ebaca</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/265">#265</a> from hyperledger/dependabot/pip/wrappers/python/pytes...</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/1a2f90a52dc336368334b7f14ebc2605e9f7ccf8"><code>1a2f90a</code></a> Merge branch 'main' into dependabot/pip/wrappers/python/pytest-approx-eq-8.2.2</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/9ff1271d36b73a765a3bd05c99376fa86d454973"><code>9ff1271</code></a> chore(js): add expo example app and move to pnpm (<a href="https://redirect.github.com/hyperledger/aries-askar/issues/247">#247</a>)</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/8923c50c2c7d6daf1cd856a060af2d9b672a258d"><code>8923c50</code></a> build(deps-dev): update pytest requirement in /wrappers/python</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/95a00366e78a5b504433576a8e31ad264dcc0d6f"><code>95a0036</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/262">#262</a> from ff137/add-python-requirements</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/594c2a1d7153cef38cf46e6fb5d41304e1a990da"><code>594c2a1</code></a> Merge branch 'main' into add-python-requirements</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/19034c97e9ab5e9b9d6fb459218c4c3894863836"><code>19034c9</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/261">#261</a> from dkulic/fix/sqlite_expire_check</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/ab33405ea58f37d8a6f68ad53205be2653ca4379"><code>ab33405</code></a> Merge branch 'main' into fix/sqlite_expire_check</li>
<li>Additional commits viewable in <a href="https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=aries-askar&package-manager=pip&previous-version=0.3.1&new-version=0.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 12:02:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/729" class=".btn">#729</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.5.0 to 0.5.1 in /oid4vci
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.5.0 to 0.5.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>0.5.1</h2>
<h2>Release Notes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement mutable-contextvar-default (B039) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12113">#12113</a>)</li>
<li>[<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12140">#12140</a>)</li>
<li>[<code>pytest</code>] Reverse <code>PT001</code> and <code>PT0023</code> defaults (<a href="https://redirect.github.com/astral-sh/ruff/pull/12106">#12106</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>Enable token-based rules on source with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/11950">#11950</a>)</li>
<li>[<code>flake8-bandit</code>] Detect <code>httpx</code> for <code>S113</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12174">#12174</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY201</code> to include exception deprecations (<a href="https://redirect.github.com/astral-sh/ruff/pull/12065">#12065</a>)</li>
<li>[<code>pylint</code>] Generate autofix for <code>duplicate-bases</code> (<code>PLE0241</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12105">#12105</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Avoid syntax error notification for source code actions (<a href="https://redirect.github.com/astral-sh/ruff/pull/12148">#12148</a>)</li>
<li>Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/pull/12203">#12203</a>)</li>
<li>Fix replacement edit range computation (<a href="https://redirect.github.com/astral-sh/ruff/pull/12171">#12171</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Disable auto-fix when source has syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/12134">#12134</a>)</li>
<li>Fix cache key collisions for paths with separators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12159">#12159</a>)</li>
<li>Make <code>requires-python</code> inference robust to <code>==</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12091">#12091</a>)</li>
<li>Use char-wise width instead of <code>str</code>-width (<a href="https://redirect.github.com/astral-sh/ruff/pull/12135">#12135</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword followed by comma (<a href="https://redirect.github.com/astral-sh/ruff/pull/12136">#12136</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword is followed by a semicolon (<a href="https://redirect.github.com/astral-sh/ruff/pull/12095">#12095</a>)</li>
<li>[<code>pylint</code>] Skip <a href="https://docs.astral.sh/ruff/settings/#lint_dummy-variable-rgx">dummy variables</a> for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12190">#12190</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Remove allocation in <code>parse_identifier</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12103">#12103</a>)</li>
<li>Use <code>CompactString</code> for <code>Identifier</code> AST node (<a href="https://redirect.github.com/astral-sh/ruff/pull/12101">#12101</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/Peiffap"><code>@​Peiffap</code></a></li>
<li><a href="https://github.com/ThomasFaivre"><code>@​ThomasFaivre</code></a></li>
<li><a href="https://github.com/bersace"><code>@​bersace</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/github-actions"><code>@​github-actions</code></a></li>
<li><a href="https://github.com/jkauerl"><code>@​jkauerl</code></a></li>
<li><a href="https://github.com/mkniewallner"><code>@​mkniewallner</code></a></li>
<li><a href="https://github.com/mtsokol"><code>@​mtsokol</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.5.1</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement mutable-contextvar-default (B039) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12113">#12113</a>)</li>
<li>[<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12140">#12140</a>)</li>
<li>[<code>pytest</code>] Reverse <code>PT001</code> and <code>PT0023</code> defaults (<a href="https://redirect.github.com/astral-sh/ruff/pull/12106">#12106</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>Enable token-based rules on source with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/11950">#11950</a>)</li>
<li>[<code>flake8-bandit</code>] Detect <code>httpx</code> for <code>S113</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12174">#12174</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY201</code> to include exception deprecations (<a href="https://redirect.github.com/astral-sh/ruff/pull/12065">#12065</a>)</li>
<li>[<code>pylint</code>] Generate autofix for <code>duplicate-bases</code> (<code>PLE0241</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12105">#12105</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Avoid syntax error notification for source code actions (<a href="https://redirect.github.com/astral-sh/ruff/pull/12148">#12148</a>)</li>
<li>Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/pull/12203">#12203</a>)</li>
<li>Fix replacement edit range computation (<a href="https://redirect.github.com/astral-sh/ruff/pull/12171">#12171</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Disable auto-fix when source has syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/12134">#12134</a>)</li>
<li>Fix cache key collisions for paths with separators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12159">#12159</a>)</li>
<li>Make <code>requires-python</code> inference robust to <code>==</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12091">#12091</a>)</li>
<li>Use char-wise width instead of <code>str</code>-width (<a href="https://redirect.github.com/astral-sh/ruff/pull/12135">#12135</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword followed by comma (<a href="https://redirect.github.com/astral-sh/ruff/pull/12136">#12136</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword is followed by a semicolon (<a href="https://redirect.github.com/astral-sh/ruff/pull/12095">#12095</a>)</li>
<li>[<code>pylint</code>] Skip <a href="https://docs.astral.sh/ruff/settings/#lint_dummy-variable-rgx">dummy variables</a> for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12190">#12190</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Remove allocation in <code>parse_identifier</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12103">#12103</a>)</li>
<li>Use <code>CompactString</code> for <code>Identifier</code> AST node (<a href="https://redirect.github.com/astral-sh/ruff/pull/12101">#12101</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/3a72400202642f0bb340fb2b1d1c31da2b6524dd"><code>3a72400</code></a> Rename publish workflow file extension (<code>yaml</code> -&gt; <code>yml</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/12206">#12206</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1b3bff03300b2c48f0ad6c7bd6b1038e2f1fce5a"><code>1b3bff0</code></a> Bump version to 0.5.1 (<a href="https://redirect.github.com/astral-sh/ruff/issues/12205">#12205</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/0f6f73ecf3c2ebfe5b218edc0765886ccdca6f7f"><code>0f6f73e</code></a> [red-knot] Require that <code>FileSystem</code> objects implement <code>Debug</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12204">#12204</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/7910beecc42b2694890b10011c27a3cbb2db3335"><code>7910bee</code></a> Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/issues/12203">#12203</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f3ccd152e99d6bccfec58275c0b3b2ec3ffd5bdd"><code>f3ccd15</code></a> Revert &quot;Remove <code>--preview</code> as a required argument for <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12053">#12053</a>)&quot;...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1e07bfa3730db9461f51b877bf71ea31e7dd56e4"><code>1e07bfa</code></a> [<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/12140">#12140</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/5e7ba056128c8bc272ab1a2a22c9cb94a5079361"><code>5e7ba05</code></a> docs(*): fix a few typos, consistency issues and links (<a href="https://redirect.github.com/astral-sh/ruff/issues/12193">#12193</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d12570ea006d23a610e2410d9c70c3b3deae717c"><code>d12570e</code></a> docs(options): fix some typos and improve consistency (<a href="https://redirect.github.com/astral-sh/ruff/issues/12191">#12191</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2f3264e148b9cf31e32c3137feb0f5ce9532d85b"><code>2f3264e</code></a> fix(rules): skip dummy variables for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12190">#12190</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e2e0889a303e8ce9953a2eb8a426921d08176c5f"><code>e2e0889</code></a> [red-knot] Add very basic benchmark (<a href="https://redirect.github.com/astral-sh/ruff/issues/12182">#12182</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/0.5.0...0.5.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.5.0&new-version=0.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 12:01:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/728" class=".btn">#728</a>
            </td>
            <td>
                <b>
                    Bump aries-askar from 0.3.1 to 0.3.2 in /oid4vci
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [aries-askar](https://github.com/hyperledger/aries-askar) from 0.3.1 to 0.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperledger/aries-askar/releases">aries-askar's releases</a>.</em></p>
<blockquote>
<h2>v0.3.2</h2>
<h2>What's Changed</h2>
<ul>
<li>chore(js): update to stable 0.2.0 by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/222">hyperledger/aries-askar#222</a></li>
<li>Add Dependabot configuration by <a href="https://github.com/WadeBarnes"><code>@​WadeBarnes</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/223">hyperledger/aries-askar#223</a></li>
<li>build(deps): bump the all-actions group with 7 updates by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/224">hyperledger/aries-askar#224</a></li>
<li>build(deps): bump ip from 2.0.0 to 2.0.1 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/226">hyperledger/aries-askar#226</a></li>
<li>build(deps): bump es5-ext from 0.10.62 to 0.10.64 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/228">hyperledger/aries-askar#228</a></li>
<li>build(deps): bump mio from 0.8.10 to 0.8.11 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/229">hyperledger/aries-askar#229</a></li>
<li>build(deps): bump follow-redirects from 1.15.4 to 1.15.6 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/230">hyperledger/aries-askar#230</a></li>
<li>build(deps): bump the all-actions group with 1 update by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/231">hyperledger/aries-askar#231</a></li>
<li>fix(js): update ffi-napi by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/234">hyperledger/aries-askar#234</a></li>
<li>build(deps): bump a7ul/tar-action from 1.1.3 to 1.2.0 in the all-actions group by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/235">hyperledger/aries-askar#235</a></li>
<li>build(deps): bump whoami from 1.4.1 to 1.5.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/233">hyperledger/aries-askar#233</a></li>
<li>chore: update version for js wrapper by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/236">hyperledger/aries-askar#236</a></li>
<li>fix: correctly serliaize for buffer by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/238">hyperledger/aries-askar#238</a></li>
<li>Build Javascript on multiple platforms by <a href="https://github.com/brianorwhatever"><code>@​brianorwhatever</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/239">hyperledger/aries-askar#239</a></li>
<li>build(deps): bump rustls from 0.21.10 to 0.21.11 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/240">hyperledger/aries-askar#240</a></li>
<li>P256 keys using Secure Enclave and Android StrongBox by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/245">hyperledger/aries-askar#245</a></li>
<li>chore: update minSdkVersion to get the project version or fallback to 21 by <a href="https://github.com/ja-bravo"><code>@​ja-bravo</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/248">hyperledger/aries-askar#248</a></li>
<li>chore: updating dependabot to support gha, TS, JS and rust packages by <a href="https://github.com/rajpalc7"><code>@​rajpalc7</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/249">hyperledger/aries-askar#249</a></li>
<li>chore(js): update version to 0.2.2 by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/243">hyperledger/aries-askar#243</a></li>
<li>fix: Incorrect SQLite expire check by <a href="https://github.com/dkulic"><code>@​dkulic</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/261">hyperledger/aries-askar#261</a></li>
<li>Add python requirements file and update dependabot workflow by <a href="https://github.com/ff137"><code>@​ff137</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/262">hyperledger/aries-askar#262</a></li>
<li>chore(js): add expo example app and move to pnpm by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/247">hyperledger/aries-askar#247</a></li>
<li>build(deps-dev): update pytest requirement from ~=8.2.1 to ~=8.2.2 in /wrappers/python by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/265">hyperledger/aries-askar#265</a></li>
<li>chore: update library versions by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/271">hyperledger/aries-askar#271</a></li>
<li>build: allow action to create release by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/272">hyperledger/aries-askar#272</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/WadeBarnes"><code>@​WadeBarnes</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/223">hyperledger/aries-askar#223</a></li>
<li><a href="https://github.com/brianorwhatever"><code>@​brianorwhatever</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/239">hyperledger/aries-askar#239</a></li>
<li><a href="https://github.com/ja-bravo"><code>@​ja-bravo</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/248">hyperledger/aries-askar#248</a></li>
<li><a href="https://github.com/rajpalc7"><code>@​rajpalc7</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/249">hyperledger/aries-askar#249</a></li>
<li><a href="https://github.com/dkulic"><code>@​dkulic</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/261">hyperledger/aries-askar#261</a></li>
<li><a href="https://github.com/ff137"><code>@​ff137</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/262">hyperledger/aries-askar#262</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2">https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperledger/aries-askar/commit/10f58b3984bf6b2d370b8fb2cd07a0696bd93d2f"><code>10f58b3</code></a> build: allow action to create release</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/cf0586ed0cf28bc5197af40e4760158e79a77458"><code>cf0586e</code></a> chore: update library versions</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/c5ebacad74923a462ad754c5d726a0b069a62ca9"><code>c5ebaca</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/265">#265</a> from hyperledger/dependabot/pip/wrappers/python/pytes...</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/1a2f90a52dc336368334b7f14ebc2605e9f7ccf8"><code>1a2f90a</code></a> Merge branch 'main' into dependabot/pip/wrappers/python/pytest-approx-eq-8.2.2</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/9ff1271d36b73a765a3bd05c99376fa86d454973"><code>9ff1271</code></a> chore(js): add expo example app and move to pnpm (<a href="https://redirect.github.com/hyperledger/aries-askar/issues/247">#247</a>)</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/8923c50c2c7d6daf1cd856a060af2d9b672a258d"><code>8923c50</code></a> build(deps-dev): update pytest requirement in /wrappers/python</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/95a00366e78a5b504433576a8e31ad264dcc0d6f"><code>95a0036</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/262">#262</a> from ff137/add-python-requirements</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/594c2a1d7153cef38cf46e6fb5d41304e1a990da"><code>594c2a1</code></a> Merge branch 'main' into add-python-requirements</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/19034c97e9ab5e9b9d6fb459218c4c3894863836"><code>19034c9</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/261">#261</a> from dkulic/fix/sqlite_expire_check</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/ab33405ea58f37d8a6f68ad53205be2653ca4379"><code>ab33405</code></a> Merge branch 'main' into fix/sqlite_expire_check</li>
<li>Additional commits viewable in <a href="https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=aries-askar&package-manager=pip&previous-version=0.3.1&new-version=0.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 12:00:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/727" class=".btn">#727</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.5.0 to 0.5.1 in /connection_update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.5.0 to 0.5.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>0.5.1</h2>
<h2>Release Notes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement mutable-contextvar-default (B039) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12113">#12113</a>)</li>
<li>[<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12140">#12140</a>)</li>
<li>[<code>pytest</code>] Reverse <code>PT001</code> and <code>PT0023</code> defaults (<a href="https://redirect.github.com/astral-sh/ruff/pull/12106">#12106</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>Enable token-based rules on source with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/11950">#11950</a>)</li>
<li>[<code>flake8-bandit</code>] Detect <code>httpx</code> for <code>S113</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12174">#12174</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY201</code> to include exception deprecations (<a href="https://redirect.github.com/astral-sh/ruff/pull/12065">#12065</a>)</li>
<li>[<code>pylint</code>] Generate autofix for <code>duplicate-bases</code> (<code>PLE0241</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12105">#12105</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Avoid syntax error notification for source code actions (<a href="https://redirect.github.com/astral-sh/ruff/pull/12148">#12148</a>)</li>
<li>Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/pull/12203">#12203</a>)</li>
<li>Fix replacement edit range computation (<a href="https://redirect.github.com/astral-sh/ruff/pull/12171">#12171</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Disable auto-fix when source has syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/12134">#12134</a>)</li>
<li>Fix cache key collisions for paths with separators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12159">#12159</a>)</li>
<li>Make <code>requires-python</code> inference robust to <code>==</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12091">#12091</a>)</li>
<li>Use char-wise width instead of <code>str</code>-width (<a href="https://redirect.github.com/astral-sh/ruff/pull/12135">#12135</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword followed by comma (<a href="https://redirect.github.com/astral-sh/ruff/pull/12136">#12136</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword is followed by a semicolon (<a href="https://redirect.github.com/astral-sh/ruff/pull/12095">#12095</a>)</li>
<li>[<code>pylint</code>] Skip <a href="https://docs.astral.sh/ruff/settings/#lint_dummy-variable-rgx">dummy variables</a> for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12190">#12190</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Remove allocation in <code>parse_identifier</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12103">#12103</a>)</li>
<li>Use <code>CompactString</code> for <code>Identifier</code> AST node (<a href="https://redirect.github.com/astral-sh/ruff/pull/12101">#12101</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/Peiffap"><code>@​Peiffap</code></a></li>
<li><a href="https://github.com/ThomasFaivre"><code>@​ThomasFaivre</code></a></li>
<li><a href="https://github.com/bersace"><code>@​bersace</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/github-actions"><code>@​github-actions</code></a></li>
<li><a href="https://github.com/jkauerl"><code>@​jkauerl</code></a></li>
<li><a href="https://github.com/mkniewallner"><code>@​mkniewallner</code></a></li>
<li><a href="https://github.com/mtsokol"><code>@​mtsokol</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.5.1</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement mutable-contextvar-default (B039) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12113">#12113</a>)</li>
<li>[<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12140">#12140</a>)</li>
<li>[<code>pytest</code>] Reverse <code>PT001</code> and <code>PT0023</code> defaults (<a href="https://redirect.github.com/astral-sh/ruff/pull/12106">#12106</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>Enable token-based rules on source with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/11950">#11950</a>)</li>
<li>[<code>flake8-bandit</code>] Detect <code>httpx</code> for <code>S113</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12174">#12174</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY201</code> to include exception deprecations (<a href="https://redirect.github.com/astral-sh/ruff/pull/12065">#12065</a>)</li>
<li>[<code>pylint</code>] Generate autofix for <code>duplicate-bases</code> (<code>PLE0241</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12105">#12105</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Avoid syntax error notification for source code actions (<a href="https://redirect.github.com/astral-sh/ruff/pull/12148">#12148</a>)</li>
<li>Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/pull/12203">#12203</a>)</li>
<li>Fix replacement edit range computation (<a href="https://redirect.github.com/astral-sh/ruff/pull/12171">#12171</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Disable auto-fix when source has syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/12134">#12134</a>)</li>
<li>Fix cache key collisions for paths with separators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12159">#12159</a>)</li>
<li>Make <code>requires-python</code> inference robust to <code>==</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12091">#12091</a>)</li>
<li>Use char-wise width instead of <code>str</code>-width (<a href="https://redirect.github.com/astral-sh/ruff/pull/12135">#12135</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword followed by comma (<a href="https://redirect.github.com/astral-sh/ruff/pull/12136">#12136</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword is followed by a semicolon (<a href="https://redirect.github.com/astral-sh/ruff/pull/12095">#12095</a>)</li>
<li>[<code>pylint</code>] Skip <a href="https://docs.astral.sh/ruff/settings/#lint_dummy-variable-rgx">dummy variables</a> for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12190">#12190</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Remove allocation in <code>parse_identifier</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12103">#12103</a>)</li>
<li>Use <code>CompactString</code> for <code>Identifier</code> AST node (<a href="https://redirect.github.com/astral-sh/ruff/pull/12101">#12101</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/3a72400202642f0bb340fb2b1d1c31da2b6524dd"><code>3a72400</code></a> Rename publish workflow file extension (<code>yaml</code> -&gt; <code>yml</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/12206">#12206</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1b3bff03300b2c48f0ad6c7bd6b1038e2f1fce5a"><code>1b3bff0</code></a> Bump version to 0.5.1 (<a href="https://redirect.github.com/astral-sh/ruff/issues/12205">#12205</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/0f6f73ecf3c2ebfe5b218edc0765886ccdca6f7f"><code>0f6f73e</code></a> [red-knot] Require that <code>FileSystem</code> objects implement <code>Debug</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12204">#12204</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/7910beecc42b2694890b10011c27a3cbb2db3335"><code>7910bee</code></a> Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/issues/12203">#12203</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f3ccd152e99d6bccfec58275c0b3b2ec3ffd5bdd"><code>f3ccd15</code></a> Revert &quot;Remove <code>--preview</code> as a required argument for <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12053">#12053</a>)&quot;...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1e07bfa3730db9461f51b877bf71ea31e7dd56e4"><code>1e07bfa</code></a> [<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/12140">#12140</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/5e7ba056128c8bc272ab1a2a22c9cb94a5079361"><code>5e7ba05</code></a> docs(*): fix a few typos, consistency issues and links (<a href="https://redirect.github.com/astral-sh/ruff/issues/12193">#12193</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d12570ea006d23a610e2410d9c70c3b3deae717c"><code>d12570e</code></a> docs(options): fix some typos and improve consistency (<a href="https://redirect.github.com/astral-sh/ruff/issues/12191">#12191</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2f3264e148b9cf31e32c3137feb0f5ce9532d85b"><code>2f3264e</code></a> fix(rules): skip dummy variables for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12190">#12190</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e2e0889a303e8ce9953a2eb8a426921d08176c5f"><code>e2e0889</code></a> [red-knot] Add very basic benchmark (<a href="https://redirect.github.com/astral-sh/ruff/issues/12182">#12182</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/0.5.0...0.5.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.5.0&new-version=0.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 11:59:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/726" class=".btn">#726</a>
            </td>
            <td>
                <b>
                    Bump aries-askar from 0.3.1 to 0.3.2 in /connection_update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [aries-askar](https://github.com/hyperledger/aries-askar) from 0.3.1 to 0.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperledger/aries-askar/releases">aries-askar's releases</a>.</em></p>
<blockquote>
<h2>v0.3.2</h2>
<h2>What's Changed</h2>
<ul>
<li>chore(js): update to stable 0.2.0 by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/222">hyperledger/aries-askar#222</a></li>
<li>Add Dependabot configuration by <a href="https://github.com/WadeBarnes"><code>@​WadeBarnes</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/223">hyperledger/aries-askar#223</a></li>
<li>build(deps): bump the all-actions group with 7 updates by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/224">hyperledger/aries-askar#224</a></li>
<li>build(deps): bump ip from 2.0.0 to 2.0.1 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/226">hyperledger/aries-askar#226</a></li>
<li>build(deps): bump es5-ext from 0.10.62 to 0.10.64 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/228">hyperledger/aries-askar#228</a></li>
<li>build(deps): bump mio from 0.8.10 to 0.8.11 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/229">hyperledger/aries-askar#229</a></li>
<li>build(deps): bump follow-redirects from 1.15.4 to 1.15.6 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/230">hyperledger/aries-askar#230</a></li>
<li>build(deps): bump the all-actions group with 1 update by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/231">hyperledger/aries-askar#231</a></li>
<li>fix(js): update ffi-napi by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/234">hyperledger/aries-askar#234</a></li>
<li>build(deps): bump a7ul/tar-action from 1.1.3 to 1.2.0 in the all-actions group by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/235">hyperledger/aries-askar#235</a></li>
<li>build(deps): bump whoami from 1.4.1 to 1.5.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/233">hyperledger/aries-askar#233</a></li>
<li>chore: update version for js wrapper by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/236">hyperledger/aries-askar#236</a></li>
<li>fix: correctly serliaize for buffer by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/238">hyperledger/aries-askar#238</a></li>
<li>Build Javascript on multiple platforms by <a href="https://github.com/brianorwhatever"><code>@​brianorwhatever</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/239">hyperledger/aries-askar#239</a></li>
<li>build(deps): bump rustls from 0.21.10 to 0.21.11 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/240">hyperledger/aries-askar#240</a></li>
<li>P256 keys using Secure Enclave and Android StrongBox by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/245">hyperledger/aries-askar#245</a></li>
<li>chore: update minSdkVersion to get the project version or fallback to 21 by <a href="https://github.com/ja-bravo"><code>@​ja-bravo</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/248">hyperledger/aries-askar#248</a></li>
<li>chore: updating dependabot to support gha, TS, JS and rust packages by <a href="https://github.com/rajpalc7"><code>@​rajpalc7</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/249">hyperledger/aries-askar#249</a></li>
<li>chore(js): update version to 0.2.2 by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/243">hyperledger/aries-askar#243</a></li>
<li>fix: Incorrect SQLite expire check by <a href="https://github.com/dkulic"><code>@​dkulic</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/261">hyperledger/aries-askar#261</a></li>
<li>Add python requirements file and update dependabot workflow by <a href="https://github.com/ff137"><code>@​ff137</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/262">hyperledger/aries-askar#262</a></li>
<li>chore(js): add expo example app and move to pnpm by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/247">hyperledger/aries-askar#247</a></li>
<li>build(deps-dev): update pytest requirement from ~=8.2.1 to ~=8.2.2 in /wrappers/python by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/265">hyperledger/aries-askar#265</a></li>
<li>chore: update library versions by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/271">hyperledger/aries-askar#271</a></li>
<li>build: allow action to create release by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/272">hyperledger/aries-askar#272</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/WadeBarnes"><code>@​WadeBarnes</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/223">hyperledger/aries-askar#223</a></li>
<li><a href="https://github.com/brianorwhatever"><code>@​brianorwhatever</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/239">hyperledger/aries-askar#239</a></li>
<li><a href="https://github.com/ja-bravo"><code>@​ja-bravo</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/248">hyperledger/aries-askar#248</a></li>
<li><a href="https://github.com/rajpalc7"><code>@​rajpalc7</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/249">hyperledger/aries-askar#249</a></li>
<li><a href="https://github.com/dkulic"><code>@​dkulic</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/261">hyperledger/aries-askar#261</a></li>
<li><a href="https://github.com/ff137"><code>@​ff137</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/262">hyperledger/aries-askar#262</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2">https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperledger/aries-askar/commit/10f58b3984bf6b2d370b8fb2cd07a0696bd93d2f"><code>10f58b3</code></a> build: allow action to create release</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/cf0586ed0cf28bc5197af40e4760158e79a77458"><code>cf0586e</code></a> chore: update library versions</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/c5ebacad74923a462ad754c5d726a0b069a62ca9"><code>c5ebaca</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/265">#265</a> from hyperledger/dependabot/pip/wrappers/python/pytes...</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/1a2f90a52dc336368334b7f14ebc2605e9f7ccf8"><code>1a2f90a</code></a> Merge branch 'main' into dependabot/pip/wrappers/python/pytest-approx-eq-8.2.2</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/9ff1271d36b73a765a3bd05c99376fa86d454973"><code>9ff1271</code></a> chore(js): add expo example app and move to pnpm (<a href="https://redirect.github.com/hyperledger/aries-askar/issues/247">#247</a>)</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/8923c50c2c7d6daf1cd856a060af2d9b672a258d"><code>8923c50</code></a> build(deps-dev): update pytest requirement in /wrappers/python</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/95a00366e78a5b504433576a8e31ad264dcc0d6f"><code>95a0036</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/262">#262</a> from ff137/add-python-requirements</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/594c2a1d7153cef38cf46e6fb5d41304e1a990da"><code>594c2a1</code></a> Merge branch 'main' into add-python-requirements</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/19034c97e9ab5e9b9d6fb459218c4c3894863836"><code>19034c9</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/261">#261</a> from dkulic/fix/sqlite_expire_check</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/ab33405ea58f37d8a6f68ad53205be2653ca4379"><code>ab33405</code></a> Merge branch 'main' into fix/sqlite_expire_check</li>
<li>Additional commits viewable in <a href="https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=aries-askar&package-manager=pip&previous-version=0.3.1&new-version=0.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 11:58:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/725" class=".btn">#725</a>
            </td>
            <td>
                <b>
                    Bump aries-askar from 0.3.1 to 0.3.2 in /multitenant_provider
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [aries-askar](https://github.com/hyperledger/aries-askar) from 0.3.1 to 0.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperledger/aries-askar/releases">aries-askar's releases</a>.</em></p>
<blockquote>
<h2>v0.3.2</h2>
<h2>What's Changed</h2>
<ul>
<li>chore(js): update to stable 0.2.0 by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/222">hyperledger/aries-askar#222</a></li>
<li>Add Dependabot configuration by <a href="https://github.com/WadeBarnes"><code>@​WadeBarnes</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/223">hyperledger/aries-askar#223</a></li>
<li>build(deps): bump the all-actions group with 7 updates by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/224">hyperledger/aries-askar#224</a></li>
<li>build(deps): bump ip from 2.0.0 to 2.0.1 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/226">hyperledger/aries-askar#226</a></li>
<li>build(deps): bump es5-ext from 0.10.62 to 0.10.64 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/228">hyperledger/aries-askar#228</a></li>
<li>build(deps): bump mio from 0.8.10 to 0.8.11 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/229">hyperledger/aries-askar#229</a></li>
<li>build(deps): bump follow-redirects from 1.15.4 to 1.15.6 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/230">hyperledger/aries-askar#230</a></li>
<li>build(deps): bump the all-actions group with 1 update by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/231">hyperledger/aries-askar#231</a></li>
<li>fix(js): update ffi-napi by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/234">hyperledger/aries-askar#234</a></li>
<li>build(deps): bump a7ul/tar-action from 1.1.3 to 1.2.0 in the all-actions group by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/235">hyperledger/aries-askar#235</a></li>
<li>build(deps): bump whoami from 1.4.1 to 1.5.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/233">hyperledger/aries-askar#233</a></li>
<li>chore: update version for js wrapper by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/236">hyperledger/aries-askar#236</a></li>
<li>fix: correctly serliaize for buffer by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/238">hyperledger/aries-askar#238</a></li>
<li>Build Javascript on multiple platforms by <a href="https://github.com/brianorwhatever"><code>@​brianorwhatever</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/239">hyperledger/aries-askar#239</a></li>
<li>build(deps): bump rustls from 0.21.10 to 0.21.11 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/240">hyperledger/aries-askar#240</a></li>
<li>P256 keys using Secure Enclave and Android StrongBox by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/245">hyperledger/aries-askar#245</a></li>
<li>chore: update minSdkVersion to get the project version or fallback to 21 by <a href="https://github.com/ja-bravo"><code>@​ja-bravo</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/248">hyperledger/aries-askar#248</a></li>
<li>chore: updating dependabot to support gha, TS, JS and rust packages by <a href="https://github.com/rajpalc7"><code>@​rajpalc7</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/249">hyperledger/aries-askar#249</a></li>
<li>chore(js): update version to 0.2.2 by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/243">hyperledger/aries-askar#243</a></li>
<li>fix: Incorrect SQLite expire check by <a href="https://github.com/dkulic"><code>@​dkulic</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/261">hyperledger/aries-askar#261</a></li>
<li>Add python requirements file and update dependabot workflow by <a href="https://github.com/ff137"><code>@​ff137</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/262">hyperledger/aries-askar#262</a></li>
<li>chore(js): add expo example app and move to pnpm by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/247">hyperledger/aries-askar#247</a></li>
<li>build(deps-dev): update pytest requirement from ~=8.2.1 to ~=8.2.2 in /wrappers/python by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/265">hyperledger/aries-askar#265</a></li>
<li>chore: update library versions by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/271">hyperledger/aries-askar#271</a></li>
<li>build: allow action to create release by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/272">hyperledger/aries-askar#272</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/WadeBarnes"><code>@​WadeBarnes</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/223">hyperledger/aries-askar#223</a></li>
<li><a href="https://github.com/brianorwhatever"><code>@​brianorwhatever</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/239">hyperledger/aries-askar#239</a></li>
<li><a href="https://github.com/ja-bravo"><code>@​ja-bravo</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/248">hyperledger/aries-askar#248</a></li>
<li><a href="https://github.com/rajpalc7"><code>@​rajpalc7</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/249">hyperledger/aries-askar#249</a></li>
<li><a href="https://github.com/dkulic"><code>@​dkulic</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/261">hyperledger/aries-askar#261</a></li>
<li><a href="https://github.com/ff137"><code>@​ff137</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/262">hyperledger/aries-askar#262</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2">https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperledger/aries-askar/commit/10f58b3984bf6b2d370b8fb2cd07a0696bd93d2f"><code>10f58b3</code></a> build: allow action to create release</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/cf0586ed0cf28bc5197af40e4760158e79a77458"><code>cf0586e</code></a> chore: update library versions</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/c5ebacad74923a462ad754c5d726a0b069a62ca9"><code>c5ebaca</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/265">#265</a> from hyperledger/dependabot/pip/wrappers/python/pytes...</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/1a2f90a52dc336368334b7f14ebc2605e9f7ccf8"><code>1a2f90a</code></a> Merge branch 'main' into dependabot/pip/wrappers/python/pytest-approx-eq-8.2.2</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/9ff1271d36b73a765a3bd05c99376fa86d454973"><code>9ff1271</code></a> chore(js): add expo example app and move to pnpm (<a href="https://redirect.github.com/hyperledger/aries-askar/issues/247">#247</a>)</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/8923c50c2c7d6daf1cd856a060af2d9b672a258d"><code>8923c50</code></a> build(deps-dev): update pytest requirement in /wrappers/python</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/95a00366e78a5b504433576a8e31ad264dcc0d6f"><code>95a0036</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/262">#262</a> from ff137/add-python-requirements</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/594c2a1d7153cef38cf46e6fb5d41304e1a990da"><code>594c2a1</code></a> Merge branch 'main' into add-python-requirements</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/19034c97e9ab5e9b9d6fb459218c4c3894863836"><code>19034c9</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/261">#261</a> from dkulic/fix/sqlite_expire_check</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/ab33405ea58f37d8a6f68ad53205be2653ca4379"><code>ab33405</code></a> Merge branch 'main' into fix/sqlite_expire_check</li>
<li>Additional commits viewable in <a href="https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=aries-askar&package-manager=pip&previous-version=0.3.1&new-version=0.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 11:48:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/724" class=".btn">#724</a>
            </td>
            <td>
                <b>
                    Bump aries-askar from 0.3.1 to 0.3.2 in /basicmessage_storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [aries-askar](https://github.com/hyperledger/aries-askar) from 0.3.1 to 0.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperledger/aries-askar/releases">aries-askar's releases</a>.</em></p>
<blockquote>
<h2>v0.3.2</h2>
<h2>What's Changed</h2>
<ul>
<li>chore(js): update to stable 0.2.0 by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/222">hyperledger/aries-askar#222</a></li>
<li>Add Dependabot configuration by <a href="https://github.com/WadeBarnes"><code>@​WadeBarnes</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/223">hyperledger/aries-askar#223</a></li>
<li>build(deps): bump the all-actions group with 7 updates by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/224">hyperledger/aries-askar#224</a></li>
<li>build(deps): bump ip from 2.0.0 to 2.0.1 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/226">hyperledger/aries-askar#226</a></li>
<li>build(deps): bump es5-ext from 0.10.62 to 0.10.64 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/228">hyperledger/aries-askar#228</a></li>
<li>build(deps): bump mio from 0.8.10 to 0.8.11 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/229">hyperledger/aries-askar#229</a></li>
<li>build(deps): bump follow-redirects from 1.15.4 to 1.15.6 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/230">hyperledger/aries-askar#230</a></li>
<li>build(deps): bump the all-actions group with 1 update by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/231">hyperledger/aries-askar#231</a></li>
<li>fix(js): update ffi-napi by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/234">hyperledger/aries-askar#234</a></li>
<li>build(deps): bump a7ul/tar-action from 1.1.3 to 1.2.0 in the all-actions group by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/235">hyperledger/aries-askar#235</a></li>
<li>build(deps): bump whoami from 1.4.1 to 1.5.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/233">hyperledger/aries-askar#233</a></li>
<li>chore: update version for js wrapper by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/236">hyperledger/aries-askar#236</a></li>
<li>fix: correctly serliaize for buffer by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/238">hyperledger/aries-askar#238</a></li>
<li>Build Javascript on multiple platforms by <a href="https://github.com/brianorwhatever"><code>@​brianorwhatever</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/239">hyperledger/aries-askar#239</a></li>
<li>build(deps): bump rustls from 0.21.10 to 0.21.11 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/240">hyperledger/aries-askar#240</a></li>
<li>P256 keys using Secure Enclave and Android StrongBox by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/245">hyperledger/aries-askar#245</a></li>
<li>chore: update minSdkVersion to get the project version or fallback to 21 by <a href="https://github.com/ja-bravo"><code>@​ja-bravo</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/248">hyperledger/aries-askar#248</a></li>
<li>chore: updating dependabot to support gha, TS, JS and rust packages by <a href="https://github.com/rajpalc7"><code>@​rajpalc7</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/249">hyperledger/aries-askar#249</a></li>
<li>chore(js): update version to 0.2.2 by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/243">hyperledger/aries-askar#243</a></li>
<li>fix: Incorrect SQLite expire check by <a href="https://github.com/dkulic"><code>@​dkulic</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/261">hyperledger/aries-askar#261</a></li>
<li>Add python requirements file and update dependabot workflow by <a href="https://github.com/ff137"><code>@​ff137</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/262">hyperledger/aries-askar#262</a></li>
<li>chore(js): add expo example app and move to pnpm by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/247">hyperledger/aries-askar#247</a></li>
<li>build(deps-dev): update pytest requirement from ~=8.2.1 to ~=8.2.2 in /wrappers/python by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/265">hyperledger/aries-askar#265</a></li>
<li>chore: update library versions by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/271">hyperledger/aries-askar#271</a></li>
<li>build: allow action to create release by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/272">hyperledger/aries-askar#272</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/WadeBarnes"><code>@​WadeBarnes</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/223">hyperledger/aries-askar#223</a></li>
<li><a href="https://github.com/brianorwhatever"><code>@​brianorwhatever</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/239">hyperledger/aries-askar#239</a></li>
<li><a href="https://github.com/ja-bravo"><code>@​ja-bravo</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/248">hyperledger/aries-askar#248</a></li>
<li><a href="https://github.com/rajpalc7"><code>@​rajpalc7</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/249">hyperledger/aries-askar#249</a></li>
<li><a href="https://github.com/dkulic"><code>@​dkulic</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/261">hyperledger/aries-askar#261</a></li>
<li><a href="https://github.com/ff137"><code>@​ff137</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/262">hyperledger/aries-askar#262</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2">https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperledger/aries-askar/commit/10f58b3984bf6b2d370b8fb2cd07a0696bd93d2f"><code>10f58b3</code></a> build: allow action to create release</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/cf0586ed0cf28bc5197af40e4760158e79a77458"><code>cf0586e</code></a> chore: update library versions</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/c5ebacad74923a462ad754c5d726a0b069a62ca9"><code>c5ebaca</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/265">#265</a> from hyperledger/dependabot/pip/wrappers/python/pytes...</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/1a2f90a52dc336368334b7f14ebc2605e9f7ccf8"><code>1a2f90a</code></a> Merge branch 'main' into dependabot/pip/wrappers/python/pytest-approx-eq-8.2.2</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/9ff1271d36b73a765a3bd05c99376fa86d454973"><code>9ff1271</code></a> chore(js): add expo example app and move to pnpm (<a href="https://redirect.github.com/hyperledger/aries-askar/issues/247">#247</a>)</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/8923c50c2c7d6daf1cd856a060af2d9b672a258d"><code>8923c50</code></a> build(deps-dev): update pytest requirement in /wrappers/python</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/95a00366e78a5b504433576a8e31ad264dcc0d6f"><code>95a0036</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/262">#262</a> from ff137/add-python-requirements</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/594c2a1d7153cef38cf46e6fb5d41304e1a990da"><code>594c2a1</code></a> Merge branch 'main' into add-python-requirements</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/19034c97e9ab5e9b9d6fb459218c4c3894863836"><code>19034c9</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/261">#261</a> from dkulic/fix/sqlite_expire_check</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/ab33405ea58f37d8a6f68ad53205be2653ca4379"><code>ab33405</code></a> Merge branch 'main' into fix/sqlite_expire_check</li>
<li>Additional commits viewable in <a href="https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=aries-askar&package-manager=pip&previous-version=0.3.1&new-version=0.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 11:39:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/723" class=".btn">#723</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.5.0 to 0.5.1 in /basicmessage_storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.5.0 to 0.5.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>0.5.1</h2>
<h2>Release Notes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement mutable-contextvar-default (B039) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12113">#12113</a>)</li>
<li>[<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12140">#12140</a>)</li>
<li>[<code>pytest</code>] Reverse <code>PT001</code> and <code>PT0023</code> defaults (<a href="https://redirect.github.com/astral-sh/ruff/pull/12106">#12106</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>Enable token-based rules on source with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/11950">#11950</a>)</li>
<li>[<code>flake8-bandit</code>] Detect <code>httpx</code> for <code>S113</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12174">#12174</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY201</code> to include exception deprecations (<a href="https://redirect.github.com/astral-sh/ruff/pull/12065">#12065</a>)</li>
<li>[<code>pylint</code>] Generate autofix for <code>duplicate-bases</code> (<code>PLE0241</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12105">#12105</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Avoid syntax error notification for source code actions (<a href="https://redirect.github.com/astral-sh/ruff/pull/12148">#12148</a>)</li>
<li>Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/pull/12203">#12203</a>)</li>
<li>Fix replacement edit range computation (<a href="https://redirect.github.com/astral-sh/ruff/pull/12171">#12171</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Disable auto-fix when source has syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/12134">#12134</a>)</li>
<li>Fix cache key collisions for paths with separators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12159">#12159</a>)</li>
<li>Make <code>requires-python</code> inference robust to <code>==</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12091">#12091</a>)</li>
<li>Use char-wise width instead of <code>str</code>-width (<a href="https://redirect.github.com/astral-sh/ruff/pull/12135">#12135</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword followed by comma (<a href="https://redirect.github.com/astral-sh/ruff/pull/12136">#12136</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword is followed by a semicolon (<a href="https://redirect.github.com/astral-sh/ruff/pull/12095">#12095</a>)</li>
<li>[<code>pylint</code>] Skip <a href="https://docs.astral.sh/ruff/settings/#lint_dummy-variable-rgx">dummy variables</a> for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12190">#12190</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Remove allocation in <code>parse_identifier</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12103">#12103</a>)</li>
<li>Use <code>CompactString</code> for <code>Identifier</code> AST node (<a href="https://redirect.github.com/astral-sh/ruff/pull/12101">#12101</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/Peiffap"><code>@​Peiffap</code></a></li>
<li><a href="https://github.com/ThomasFaivre"><code>@​ThomasFaivre</code></a></li>
<li><a href="https://github.com/bersace"><code>@​bersace</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/github-actions"><code>@​github-actions</code></a></li>
<li><a href="https://github.com/jkauerl"><code>@​jkauerl</code></a></li>
<li><a href="https://github.com/mkniewallner"><code>@​mkniewallner</code></a></li>
<li><a href="https://github.com/mtsokol"><code>@​mtsokol</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.5.1</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement mutable-contextvar-default (B039) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12113">#12113</a>)</li>
<li>[<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12140">#12140</a>)</li>
<li>[<code>pytest</code>] Reverse <code>PT001</code> and <code>PT0023</code> defaults (<a href="https://redirect.github.com/astral-sh/ruff/pull/12106">#12106</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>Enable token-based rules on source with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/11950">#11950</a>)</li>
<li>[<code>flake8-bandit</code>] Detect <code>httpx</code> for <code>S113</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12174">#12174</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY201</code> to include exception deprecations (<a href="https://redirect.github.com/astral-sh/ruff/pull/12065">#12065</a>)</li>
<li>[<code>pylint</code>] Generate autofix for <code>duplicate-bases</code> (<code>PLE0241</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12105">#12105</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Avoid syntax error notification for source code actions (<a href="https://redirect.github.com/astral-sh/ruff/pull/12148">#12148</a>)</li>
<li>Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/pull/12203">#12203</a>)</li>
<li>Fix replacement edit range computation (<a href="https://redirect.github.com/astral-sh/ruff/pull/12171">#12171</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Disable auto-fix when source has syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/12134">#12134</a>)</li>
<li>Fix cache key collisions for paths with separators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12159">#12159</a>)</li>
<li>Make <code>requires-python</code> inference robust to <code>==</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12091">#12091</a>)</li>
<li>Use char-wise width instead of <code>str</code>-width (<a href="https://redirect.github.com/astral-sh/ruff/pull/12135">#12135</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword followed by comma (<a href="https://redirect.github.com/astral-sh/ruff/pull/12136">#12136</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword is followed by a semicolon (<a href="https://redirect.github.com/astral-sh/ruff/pull/12095">#12095</a>)</li>
<li>[<code>pylint</code>] Skip <a href="https://docs.astral.sh/ruff/settings/#lint_dummy-variable-rgx">dummy variables</a> for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12190">#12190</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Remove allocation in <code>parse_identifier</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12103">#12103</a>)</li>
<li>Use <code>CompactString</code> for <code>Identifier</code> AST node (<a href="https://redirect.github.com/astral-sh/ruff/pull/12101">#12101</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/3a72400202642f0bb340fb2b1d1c31da2b6524dd"><code>3a72400</code></a> Rename publish workflow file extension (<code>yaml</code> -&gt; <code>yml</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/12206">#12206</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1b3bff03300b2c48f0ad6c7bd6b1038e2f1fce5a"><code>1b3bff0</code></a> Bump version to 0.5.1 (<a href="https://redirect.github.com/astral-sh/ruff/issues/12205">#12205</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/0f6f73ecf3c2ebfe5b218edc0765886ccdca6f7f"><code>0f6f73e</code></a> [red-knot] Require that <code>FileSystem</code> objects implement <code>Debug</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12204">#12204</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/7910beecc42b2694890b10011c27a3cbb2db3335"><code>7910bee</code></a> Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/issues/12203">#12203</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f3ccd152e99d6bccfec58275c0b3b2ec3ffd5bdd"><code>f3ccd15</code></a> Revert &quot;Remove <code>--preview</code> as a required argument for <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12053">#12053</a>)&quot;...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1e07bfa3730db9461f51b877bf71ea31e7dd56e4"><code>1e07bfa</code></a> [<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/12140">#12140</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/5e7ba056128c8bc272ab1a2a22c9cb94a5079361"><code>5e7ba05</code></a> docs(*): fix a few typos, consistency issues and links (<a href="https://redirect.github.com/astral-sh/ruff/issues/12193">#12193</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d12570ea006d23a610e2410d9c70c3b3deae717c"><code>d12570e</code></a> docs(options): fix some typos and improve consistency (<a href="https://redirect.github.com/astral-sh/ruff/issues/12191">#12191</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2f3264e148b9cf31e32c3137feb0f5ce9532d85b"><code>2f3264e</code></a> fix(rules): skip dummy variables for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12190">#12190</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e2e0889a303e8ce9953a2eb8a426921d08176c5f"><code>e2e0889</code></a> [red-knot] Add very basic benchmark (<a href="https://redirect.github.com/astral-sh/ruff/issues/12182">#12182</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/0.5.0...0.5.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.5.0&new-version=0.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 11:38:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/722" class=".btn">#722</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.5.0 to 0.5.1 in /oid4vci/integration/afj_runner
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.5.0 to 0.5.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>0.5.1</h2>
<h2>Release Notes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement mutable-contextvar-default (B039) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12113">#12113</a>)</li>
<li>[<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12140">#12140</a>)</li>
<li>[<code>pytest</code>] Reverse <code>PT001</code> and <code>PT0023</code> defaults (<a href="https://redirect.github.com/astral-sh/ruff/pull/12106">#12106</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>Enable token-based rules on source with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/11950">#11950</a>)</li>
<li>[<code>flake8-bandit</code>] Detect <code>httpx</code> for <code>S113</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12174">#12174</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY201</code> to include exception deprecations (<a href="https://redirect.github.com/astral-sh/ruff/pull/12065">#12065</a>)</li>
<li>[<code>pylint</code>] Generate autofix for <code>duplicate-bases</code> (<code>PLE0241</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12105">#12105</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Avoid syntax error notification for source code actions (<a href="https://redirect.github.com/astral-sh/ruff/pull/12148">#12148</a>)</li>
<li>Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/pull/12203">#12203</a>)</li>
<li>Fix replacement edit range computation (<a href="https://redirect.github.com/astral-sh/ruff/pull/12171">#12171</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Disable auto-fix when source has syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/12134">#12134</a>)</li>
<li>Fix cache key collisions for paths with separators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12159">#12159</a>)</li>
<li>Make <code>requires-python</code> inference robust to <code>==</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12091">#12091</a>)</li>
<li>Use char-wise width instead of <code>str</code>-width (<a href="https://redirect.github.com/astral-sh/ruff/pull/12135">#12135</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword followed by comma (<a href="https://redirect.github.com/astral-sh/ruff/pull/12136">#12136</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword is followed by a semicolon (<a href="https://redirect.github.com/astral-sh/ruff/pull/12095">#12095</a>)</li>
<li>[<code>pylint</code>] Skip <a href="https://docs.astral.sh/ruff/settings/#lint_dummy-variable-rgx">dummy variables</a> for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12190">#12190</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Remove allocation in <code>parse_identifier</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12103">#12103</a>)</li>
<li>Use <code>CompactString</code> for <code>Identifier</code> AST node (<a href="https://redirect.github.com/astral-sh/ruff/pull/12101">#12101</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/Peiffap"><code>@​Peiffap</code></a></li>
<li><a href="https://github.com/ThomasFaivre"><code>@​ThomasFaivre</code></a></li>
<li><a href="https://github.com/bersace"><code>@​bersace</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/github-actions"><code>@​github-actions</code></a></li>
<li><a href="https://github.com/jkauerl"><code>@​jkauerl</code></a></li>
<li><a href="https://github.com/mkniewallner"><code>@​mkniewallner</code></a></li>
<li><a href="https://github.com/mtsokol"><code>@​mtsokol</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.5.1</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement mutable-contextvar-default (B039) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12113">#12113</a>)</li>
<li>[<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12140">#12140</a>)</li>
<li>[<code>pytest</code>] Reverse <code>PT001</code> and <code>PT0023</code> defaults (<a href="https://redirect.github.com/astral-sh/ruff/pull/12106">#12106</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>Enable token-based rules on source with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/11950">#11950</a>)</li>
<li>[<code>flake8-bandit</code>] Detect <code>httpx</code> for <code>S113</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12174">#12174</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY201</code> to include exception deprecations (<a href="https://redirect.github.com/astral-sh/ruff/pull/12065">#12065</a>)</li>
<li>[<code>pylint</code>] Generate autofix for <code>duplicate-bases</code> (<code>PLE0241</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12105">#12105</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Avoid syntax error notification for source code actions (<a href="https://redirect.github.com/astral-sh/ruff/pull/12148">#12148</a>)</li>
<li>Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/pull/12203">#12203</a>)</li>
<li>Fix replacement edit range computation (<a href="https://redirect.github.com/astral-sh/ruff/pull/12171">#12171</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Disable auto-fix when source has syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/12134">#12134</a>)</li>
<li>Fix cache key collisions for paths with separators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12159">#12159</a>)</li>
<li>Make <code>requires-python</code> inference robust to <code>==</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12091">#12091</a>)</li>
<li>Use char-wise width instead of <code>str</code>-width (<a href="https://redirect.github.com/astral-sh/ruff/pull/12135">#12135</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword followed by comma (<a href="https://redirect.github.com/astral-sh/ruff/pull/12136">#12136</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword is followed by a semicolon (<a href="https://redirect.github.com/astral-sh/ruff/pull/12095">#12095</a>)</li>
<li>[<code>pylint</code>] Skip <a href="https://docs.astral.sh/ruff/settings/#lint_dummy-variable-rgx">dummy variables</a> for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12190">#12190</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Remove allocation in <code>parse_identifier</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12103">#12103</a>)</li>
<li>Use <code>CompactString</code> for <code>Identifier</code> AST node (<a href="https://redirect.github.com/astral-sh/ruff/pull/12101">#12101</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/3a72400202642f0bb340fb2b1d1c31da2b6524dd"><code>3a72400</code></a> Rename publish workflow file extension (<code>yaml</code> -&gt; <code>yml</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/12206">#12206</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1b3bff03300b2c48f0ad6c7bd6b1038e2f1fce5a"><code>1b3bff0</code></a> Bump version to 0.5.1 (<a href="https://redirect.github.com/astral-sh/ruff/issues/12205">#12205</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/0f6f73ecf3c2ebfe5b218edc0765886ccdca6f7f"><code>0f6f73e</code></a> [red-knot] Require that <code>FileSystem</code> objects implement <code>Debug</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12204">#12204</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/7910beecc42b2694890b10011c27a3cbb2db3335"><code>7910bee</code></a> Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/issues/12203">#12203</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f3ccd152e99d6bccfec58275c0b3b2ec3ffd5bdd"><code>f3ccd15</code></a> Revert &quot;Remove <code>--preview</code> as a required argument for <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12053">#12053</a>)&quot;...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1e07bfa3730db9461f51b877bf71ea31e7dd56e4"><code>1e07bfa</code></a> [<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/12140">#12140</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/5e7ba056128c8bc272ab1a2a22c9cb94a5079361"><code>5e7ba05</code></a> docs(*): fix a few typos, consistency issues and links (<a href="https://redirect.github.com/astral-sh/ruff/issues/12193">#12193</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d12570ea006d23a610e2410d9c70c3b3deae717c"><code>d12570e</code></a> docs(options): fix some typos and improve consistency (<a href="https://redirect.github.com/astral-sh/ruff/issues/12191">#12191</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2f3264e148b9cf31e32c3137feb0f5ce9532d85b"><code>2f3264e</code></a> fix(rules): skip dummy variables for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12190">#12190</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e2e0889a303e8ce9953a2eb8a426921d08176c5f"><code>e2e0889</code></a> [red-knot] Add very basic benchmark (<a href="https://redirect.github.com/astral-sh/ruff/issues/12182">#12182</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/0.5.0...0.5.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.5.0&new-version=0.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 11:35:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/721" class=".btn">#721</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.5.0 to 0.5.1 in /plugin_globals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.5.0 to 0.5.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>0.5.1</h2>
<h2>Release Notes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement mutable-contextvar-default (B039) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12113">#12113</a>)</li>
<li>[<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12140">#12140</a>)</li>
<li>[<code>pytest</code>] Reverse <code>PT001</code> and <code>PT0023</code> defaults (<a href="https://redirect.github.com/astral-sh/ruff/pull/12106">#12106</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>Enable token-based rules on source with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/11950">#11950</a>)</li>
<li>[<code>flake8-bandit</code>] Detect <code>httpx</code> for <code>S113</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12174">#12174</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY201</code> to include exception deprecations (<a href="https://redirect.github.com/astral-sh/ruff/pull/12065">#12065</a>)</li>
<li>[<code>pylint</code>] Generate autofix for <code>duplicate-bases</code> (<code>PLE0241</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12105">#12105</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Avoid syntax error notification for source code actions (<a href="https://redirect.github.com/astral-sh/ruff/pull/12148">#12148</a>)</li>
<li>Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/pull/12203">#12203</a>)</li>
<li>Fix replacement edit range computation (<a href="https://redirect.github.com/astral-sh/ruff/pull/12171">#12171</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Disable auto-fix when source has syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/12134">#12134</a>)</li>
<li>Fix cache key collisions for paths with separators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12159">#12159</a>)</li>
<li>Make <code>requires-python</code> inference robust to <code>==</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12091">#12091</a>)</li>
<li>Use char-wise width instead of <code>str</code>-width (<a href="https://redirect.github.com/astral-sh/ruff/pull/12135">#12135</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword followed by comma (<a href="https://redirect.github.com/astral-sh/ruff/pull/12136">#12136</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword is followed by a semicolon (<a href="https://redirect.github.com/astral-sh/ruff/pull/12095">#12095</a>)</li>
<li>[<code>pylint</code>] Skip <a href="https://docs.astral.sh/ruff/settings/#lint_dummy-variable-rgx">dummy variables</a> for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12190">#12190</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Remove allocation in <code>parse_identifier</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12103">#12103</a>)</li>
<li>Use <code>CompactString</code> for <code>Identifier</code> AST node (<a href="https://redirect.github.com/astral-sh/ruff/pull/12101">#12101</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/Peiffap"><code>@​Peiffap</code></a></li>
<li><a href="https://github.com/ThomasFaivre"><code>@​ThomasFaivre</code></a></li>
<li><a href="https://github.com/bersace"><code>@​bersace</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/github-actions"><code>@​github-actions</code></a></li>
<li><a href="https://github.com/jkauerl"><code>@​jkauerl</code></a></li>
<li><a href="https://github.com/mkniewallner"><code>@​mkniewallner</code></a></li>
<li><a href="https://github.com/mtsokol"><code>@​mtsokol</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.5.1</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement mutable-contextvar-default (B039) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12113">#12113</a>)</li>
<li>[<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12140">#12140</a>)</li>
<li>[<code>pytest</code>] Reverse <code>PT001</code> and <code>PT0023</code> defaults (<a href="https://redirect.github.com/astral-sh/ruff/pull/12106">#12106</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>Enable token-based rules on source with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/11950">#11950</a>)</li>
<li>[<code>flake8-bandit</code>] Detect <code>httpx</code> for <code>S113</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12174">#12174</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY201</code> to include exception deprecations (<a href="https://redirect.github.com/astral-sh/ruff/pull/12065">#12065</a>)</li>
<li>[<code>pylint</code>] Generate autofix for <code>duplicate-bases</code> (<code>PLE0241</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12105">#12105</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Avoid syntax error notification for source code actions (<a href="https://redirect.github.com/astral-sh/ruff/pull/12148">#12148</a>)</li>
<li>Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/pull/12203">#12203</a>)</li>
<li>Fix replacement edit range computation (<a href="https://redirect.github.com/astral-sh/ruff/pull/12171">#12171</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Disable auto-fix when source has syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/12134">#12134</a>)</li>
<li>Fix cache key collisions for paths with separators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12159">#12159</a>)</li>
<li>Make <code>requires-python</code> inference robust to <code>==</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12091">#12091</a>)</li>
<li>Use char-wise width instead of <code>str</code>-width (<a href="https://redirect.github.com/astral-sh/ruff/pull/12135">#12135</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword followed by comma (<a href="https://redirect.github.com/astral-sh/ruff/pull/12136">#12136</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword is followed by a semicolon (<a href="https://redirect.github.com/astral-sh/ruff/pull/12095">#12095</a>)</li>
<li>[<code>pylint</code>] Skip <a href="https://docs.astral.sh/ruff/settings/#lint_dummy-variable-rgx">dummy variables</a> for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12190">#12190</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Remove allocation in <code>parse_identifier</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12103">#12103</a>)</li>
<li>Use <code>CompactString</code> for <code>Identifier</code> AST node (<a href="https://redirect.github.com/astral-sh/ruff/pull/12101">#12101</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/3a72400202642f0bb340fb2b1d1c31da2b6524dd"><code>3a72400</code></a> Rename publish workflow file extension (<code>yaml</code> -&gt; <code>yml</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/12206">#12206</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1b3bff03300b2c48f0ad6c7bd6b1038e2f1fce5a"><code>1b3bff0</code></a> Bump version to 0.5.1 (<a href="https://redirect.github.com/astral-sh/ruff/issues/12205">#12205</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/0f6f73ecf3c2ebfe5b218edc0765886ccdca6f7f"><code>0f6f73e</code></a> [red-knot] Require that <code>FileSystem</code> objects implement <code>Debug</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12204">#12204</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/7910beecc42b2694890b10011c27a3cbb2db3335"><code>7910bee</code></a> Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/issues/12203">#12203</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f3ccd152e99d6bccfec58275c0b3b2ec3ffd5bdd"><code>f3ccd15</code></a> Revert &quot;Remove <code>--preview</code> as a required argument for <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12053">#12053</a>)&quot;...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1e07bfa3730db9461f51b877bf71ea31e7dd56e4"><code>1e07bfa</code></a> [<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/12140">#12140</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/5e7ba056128c8bc272ab1a2a22c9cb94a5079361"><code>5e7ba05</code></a> docs(*): fix a few typos, consistency issues and links (<a href="https://redirect.github.com/astral-sh/ruff/issues/12193">#12193</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d12570ea006d23a610e2410d9c70c3b3deae717c"><code>d12570e</code></a> docs(options): fix some typos and improve consistency (<a href="https://redirect.github.com/astral-sh/ruff/issues/12191">#12191</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2f3264e148b9cf31e32c3137feb0f5ce9532d85b"><code>2f3264e</code></a> fix(rules): skip dummy variables for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12190">#12190</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e2e0889a303e8ce9953a2eb8a426921d08176c5f"><code>e2e0889</code></a> [red-knot] Add very basic benchmark (<a href="https://redirect.github.com/astral-sh/ruff/issues/12182">#12182</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/0.5.0...0.5.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.5.0&new-version=0.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 11:34:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/720" class=".btn">#720</a>
            </td>
            <td>
                <b>
                    Bump aries-askar from 0.3.1 to 0.3.2 in /plugin_globals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [aries-askar](https://github.com/hyperledger/aries-askar) from 0.3.1 to 0.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperledger/aries-askar/releases">aries-askar's releases</a>.</em></p>
<blockquote>
<h2>v0.3.2</h2>
<h2>What's Changed</h2>
<ul>
<li>chore(js): update to stable 0.2.0 by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/222">hyperledger/aries-askar#222</a></li>
<li>Add Dependabot configuration by <a href="https://github.com/WadeBarnes"><code>@​WadeBarnes</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/223">hyperledger/aries-askar#223</a></li>
<li>build(deps): bump the all-actions group with 7 updates by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/224">hyperledger/aries-askar#224</a></li>
<li>build(deps): bump ip from 2.0.0 to 2.0.1 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/226">hyperledger/aries-askar#226</a></li>
<li>build(deps): bump es5-ext from 0.10.62 to 0.10.64 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/228">hyperledger/aries-askar#228</a></li>
<li>build(deps): bump mio from 0.8.10 to 0.8.11 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/229">hyperledger/aries-askar#229</a></li>
<li>build(deps): bump follow-redirects from 1.15.4 to 1.15.6 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/230">hyperledger/aries-askar#230</a></li>
<li>build(deps): bump the all-actions group with 1 update by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/231">hyperledger/aries-askar#231</a></li>
<li>fix(js): update ffi-napi by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/234">hyperledger/aries-askar#234</a></li>
<li>build(deps): bump a7ul/tar-action from 1.1.3 to 1.2.0 in the all-actions group by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/235">hyperledger/aries-askar#235</a></li>
<li>build(deps): bump whoami from 1.4.1 to 1.5.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/233">hyperledger/aries-askar#233</a></li>
<li>chore: update version for js wrapper by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/236">hyperledger/aries-askar#236</a></li>
<li>fix: correctly serliaize for buffer by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/238">hyperledger/aries-askar#238</a></li>
<li>Build Javascript on multiple platforms by <a href="https://github.com/brianorwhatever"><code>@​brianorwhatever</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/239">hyperledger/aries-askar#239</a></li>
<li>build(deps): bump rustls from 0.21.10 to 0.21.11 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/240">hyperledger/aries-askar#240</a></li>
<li>P256 keys using Secure Enclave and Android StrongBox by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/245">hyperledger/aries-askar#245</a></li>
<li>chore: update minSdkVersion to get the project version or fallback to 21 by <a href="https://github.com/ja-bravo"><code>@​ja-bravo</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/248">hyperledger/aries-askar#248</a></li>
<li>chore: updating dependabot to support gha, TS, JS and rust packages by <a href="https://github.com/rajpalc7"><code>@​rajpalc7</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/249">hyperledger/aries-askar#249</a></li>
<li>chore(js): update version to 0.2.2 by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/243">hyperledger/aries-askar#243</a></li>
<li>fix: Incorrect SQLite expire check by <a href="https://github.com/dkulic"><code>@​dkulic</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/261">hyperledger/aries-askar#261</a></li>
<li>Add python requirements file and update dependabot workflow by <a href="https://github.com/ff137"><code>@​ff137</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/262">hyperledger/aries-askar#262</a></li>
<li>chore(js): add expo example app and move to pnpm by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/247">hyperledger/aries-askar#247</a></li>
<li>build(deps-dev): update pytest requirement from ~=8.2.1 to ~=8.2.2 in /wrappers/python by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/265">hyperledger/aries-askar#265</a></li>
<li>chore: update library versions by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/271">hyperledger/aries-askar#271</a></li>
<li>build: allow action to create release by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/272">hyperledger/aries-askar#272</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/WadeBarnes"><code>@​WadeBarnes</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/223">hyperledger/aries-askar#223</a></li>
<li><a href="https://github.com/brianorwhatever"><code>@​brianorwhatever</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/239">hyperledger/aries-askar#239</a></li>
<li><a href="https://github.com/ja-bravo"><code>@​ja-bravo</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/248">hyperledger/aries-askar#248</a></li>
<li><a href="https://github.com/rajpalc7"><code>@​rajpalc7</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/249">hyperledger/aries-askar#249</a></li>
<li><a href="https://github.com/dkulic"><code>@​dkulic</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/261">hyperledger/aries-askar#261</a></li>
<li><a href="https://github.com/ff137"><code>@​ff137</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/262">hyperledger/aries-askar#262</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2">https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperledger/aries-askar/commit/10f58b3984bf6b2d370b8fb2cd07a0696bd93d2f"><code>10f58b3</code></a> build: allow action to create release</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/cf0586ed0cf28bc5197af40e4760158e79a77458"><code>cf0586e</code></a> chore: update library versions</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/c5ebacad74923a462ad754c5d726a0b069a62ca9"><code>c5ebaca</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/265">#265</a> from hyperledger/dependabot/pip/wrappers/python/pytes...</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/1a2f90a52dc336368334b7f14ebc2605e9f7ccf8"><code>1a2f90a</code></a> Merge branch 'main' into dependabot/pip/wrappers/python/pytest-approx-eq-8.2.2</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/9ff1271d36b73a765a3bd05c99376fa86d454973"><code>9ff1271</code></a> chore(js): add expo example app and move to pnpm (<a href="https://redirect.github.com/hyperledger/aries-askar/issues/247">#247</a>)</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/8923c50c2c7d6daf1cd856a060af2d9b672a258d"><code>8923c50</code></a> build(deps-dev): update pytest requirement in /wrappers/python</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/95a00366e78a5b504433576a8e31ad264dcc0d6f"><code>95a0036</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/262">#262</a> from ff137/add-python-requirements</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/594c2a1d7153cef38cf46e6fb5d41304e1a990da"><code>594c2a1</code></a> Merge branch 'main' into add-python-requirements</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/19034c97e9ab5e9b9d6fb459218c4c3894863836"><code>19034c9</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/261">#261</a> from dkulic/fix/sqlite_expire_check</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/ab33405ea58f37d8a6f68ad53205be2653ca4379"><code>ab33405</code></a> Merge branch 'main' into fix/sqlite_expire_check</li>
<li>Additional commits viewable in <a href="https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=aries-askar&package-manager=pip&previous-version=0.3.1&new-version=0.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 11:33:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/719" class=".btn">#719</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.5.0 to 0.5.1 in /rpc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.5.0 to 0.5.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>0.5.1</h2>
<h2>Release Notes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement mutable-contextvar-default (B039) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12113">#12113</a>)</li>
<li>[<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12140">#12140</a>)</li>
<li>[<code>pytest</code>] Reverse <code>PT001</code> and <code>PT0023</code> defaults (<a href="https://redirect.github.com/astral-sh/ruff/pull/12106">#12106</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>Enable token-based rules on source with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/11950">#11950</a>)</li>
<li>[<code>flake8-bandit</code>] Detect <code>httpx</code> for <code>S113</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12174">#12174</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY201</code> to include exception deprecations (<a href="https://redirect.github.com/astral-sh/ruff/pull/12065">#12065</a>)</li>
<li>[<code>pylint</code>] Generate autofix for <code>duplicate-bases</code> (<code>PLE0241</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12105">#12105</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Avoid syntax error notification for source code actions (<a href="https://redirect.github.com/astral-sh/ruff/pull/12148">#12148</a>)</li>
<li>Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/pull/12203">#12203</a>)</li>
<li>Fix replacement edit range computation (<a href="https://redirect.github.com/astral-sh/ruff/pull/12171">#12171</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Disable auto-fix when source has syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/12134">#12134</a>)</li>
<li>Fix cache key collisions for paths with separators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12159">#12159</a>)</li>
<li>Make <code>requires-python</code> inference robust to <code>==</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12091">#12091</a>)</li>
<li>Use char-wise width instead of <code>str</code>-width (<a href="https://redirect.github.com/astral-sh/ruff/pull/12135">#12135</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword followed by comma (<a href="https://redirect.github.com/astral-sh/ruff/pull/12136">#12136</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword is followed by a semicolon (<a href="https://redirect.github.com/astral-sh/ruff/pull/12095">#12095</a>)</li>
<li>[<code>pylint</code>] Skip <a href="https://docs.astral.sh/ruff/settings/#lint_dummy-variable-rgx">dummy variables</a> for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12190">#12190</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Remove allocation in <code>parse_identifier</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12103">#12103</a>)</li>
<li>Use <code>CompactString</code> for <code>Identifier</code> AST node (<a href="https://redirect.github.com/astral-sh/ruff/pull/12101">#12101</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/Peiffap"><code>@​Peiffap</code></a></li>
<li><a href="https://github.com/ThomasFaivre"><code>@​ThomasFaivre</code></a></li>
<li><a href="https://github.com/bersace"><code>@​bersace</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/github-actions"><code>@​github-actions</code></a></li>
<li><a href="https://github.com/jkauerl"><code>@​jkauerl</code></a></li>
<li><a href="https://github.com/mkniewallner"><code>@​mkniewallner</code></a></li>
<li><a href="https://github.com/mtsokol"><code>@​mtsokol</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.5.1</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement mutable-contextvar-default (B039) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12113">#12113</a>)</li>
<li>[<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12140">#12140</a>)</li>
<li>[<code>pytest</code>] Reverse <code>PT001</code> and <code>PT0023</code> defaults (<a href="https://redirect.github.com/astral-sh/ruff/pull/12106">#12106</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>Enable token-based rules on source with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/11950">#11950</a>)</li>
<li>[<code>flake8-bandit</code>] Detect <code>httpx</code> for <code>S113</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12174">#12174</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY201</code> to include exception deprecations (<a href="https://redirect.github.com/astral-sh/ruff/pull/12065">#12065</a>)</li>
<li>[<code>pylint</code>] Generate autofix for <code>duplicate-bases</code> (<code>PLE0241</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12105">#12105</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Avoid syntax error notification for source code actions (<a href="https://redirect.github.com/astral-sh/ruff/pull/12148">#12148</a>)</li>
<li>Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/pull/12203">#12203</a>)</li>
<li>Fix replacement edit range computation (<a href="https://redirect.github.com/astral-sh/ruff/pull/12171">#12171</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Disable auto-fix when source has syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/12134">#12134</a>)</li>
<li>Fix cache key collisions for paths with separators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12159">#12159</a>)</li>
<li>Make <code>requires-python</code> inference robust to <code>==</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12091">#12091</a>)</li>
<li>Use char-wise width instead of <code>str</code>-width (<a href="https://redirect.github.com/astral-sh/ruff/pull/12135">#12135</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword followed by comma (<a href="https://redirect.github.com/astral-sh/ruff/pull/12136">#12136</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword is followed by a semicolon (<a href="https://redirect.github.com/astral-sh/ruff/pull/12095">#12095</a>)</li>
<li>[<code>pylint</code>] Skip <a href="https://docs.astral.sh/ruff/settings/#lint_dummy-variable-rgx">dummy variables</a> for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12190">#12190</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Remove allocation in <code>parse_identifier</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12103">#12103</a>)</li>
<li>Use <code>CompactString</code> for <code>Identifier</code> AST node (<a href="https://redirect.github.com/astral-sh/ruff/pull/12101">#12101</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/3a72400202642f0bb340fb2b1d1c31da2b6524dd"><code>3a72400</code></a> Rename publish workflow file extension (<code>yaml</code> -&gt; <code>yml</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/12206">#12206</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1b3bff03300b2c48f0ad6c7bd6b1038e2f1fce5a"><code>1b3bff0</code></a> Bump version to 0.5.1 (<a href="https://redirect.github.com/astral-sh/ruff/issues/12205">#12205</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/0f6f73ecf3c2ebfe5b218edc0765886ccdca6f7f"><code>0f6f73e</code></a> [red-knot] Require that <code>FileSystem</code> objects implement <code>Debug</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12204">#12204</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/7910beecc42b2694890b10011c27a3cbb2db3335"><code>7910bee</code></a> Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/issues/12203">#12203</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f3ccd152e99d6bccfec58275c0b3b2ec3ffd5bdd"><code>f3ccd15</code></a> Revert &quot;Remove <code>--preview</code> as a required argument for <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12053">#12053</a>)&quot;...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1e07bfa3730db9461f51b877bf71ea31e7dd56e4"><code>1e07bfa</code></a> [<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/12140">#12140</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/5e7ba056128c8bc272ab1a2a22c9cb94a5079361"><code>5e7ba05</code></a> docs(*): fix a few typos, consistency issues and links (<a href="https://redirect.github.com/astral-sh/ruff/issues/12193">#12193</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d12570ea006d23a610e2410d9c70c3b3deae717c"><code>d12570e</code></a> docs(options): fix some typos and improve consistency (<a href="https://redirect.github.com/astral-sh/ruff/issues/12191">#12191</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2f3264e148b9cf31e32c3137feb0f5ce9532d85b"><code>2f3264e</code></a> fix(rules): skip dummy variables for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12190">#12190</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e2e0889a303e8ce9953a2eb8a426921d08176c5f"><code>e2e0889</code></a> [red-knot] Add very basic benchmark (<a href="https://redirect.github.com/astral-sh/ruff/issues/12182">#12182</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/0.5.0...0.5.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.5.0&new-version=0.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 11:28:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/718" class=".btn">#718</a>
            </td>
            <td>
                <b>
                    Bump aries-askar from 0.3.1 to 0.3.2 in /rpc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [aries-askar](https://github.com/hyperledger/aries-askar) from 0.3.1 to 0.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperledger/aries-askar/releases">aries-askar's releases</a>.</em></p>
<blockquote>
<h2>v0.3.2</h2>
<h2>What's Changed</h2>
<ul>
<li>chore(js): update to stable 0.2.0 by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/222">hyperledger/aries-askar#222</a></li>
<li>Add Dependabot configuration by <a href="https://github.com/WadeBarnes"><code>@​WadeBarnes</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/223">hyperledger/aries-askar#223</a></li>
<li>build(deps): bump the all-actions group with 7 updates by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/224">hyperledger/aries-askar#224</a></li>
<li>build(deps): bump ip from 2.0.0 to 2.0.1 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/226">hyperledger/aries-askar#226</a></li>
<li>build(deps): bump es5-ext from 0.10.62 to 0.10.64 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/228">hyperledger/aries-askar#228</a></li>
<li>build(deps): bump mio from 0.8.10 to 0.8.11 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/229">hyperledger/aries-askar#229</a></li>
<li>build(deps): bump follow-redirects from 1.15.4 to 1.15.6 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/230">hyperledger/aries-askar#230</a></li>
<li>build(deps): bump the all-actions group with 1 update by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/231">hyperledger/aries-askar#231</a></li>
<li>fix(js): update ffi-napi by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/234">hyperledger/aries-askar#234</a></li>
<li>build(deps): bump a7ul/tar-action from 1.1.3 to 1.2.0 in the all-actions group by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/235">hyperledger/aries-askar#235</a></li>
<li>build(deps): bump whoami from 1.4.1 to 1.5.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/233">hyperledger/aries-askar#233</a></li>
<li>chore: update version for js wrapper by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/236">hyperledger/aries-askar#236</a></li>
<li>fix: correctly serliaize for buffer by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/238">hyperledger/aries-askar#238</a></li>
<li>Build Javascript on multiple platforms by <a href="https://github.com/brianorwhatever"><code>@​brianorwhatever</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/239">hyperledger/aries-askar#239</a></li>
<li>build(deps): bump rustls from 0.21.10 to 0.21.11 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/240">hyperledger/aries-askar#240</a></li>
<li>P256 keys using Secure Enclave and Android StrongBox by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/245">hyperledger/aries-askar#245</a></li>
<li>chore: update minSdkVersion to get the project version or fallback to 21 by <a href="https://github.com/ja-bravo"><code>@​ja-bravo</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/248">hyperledger/aries-askar#248</a></li>
<li>chore: updating dependabot to support gha, TS, JS and rust packages by <a href="https://github.com/rajpalc7"><code>@​rajpalc7</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/249">hyperledger/aries-askar#249</a></li>
<li>chore(js): update version to 0.2.2 by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/243">hyperledger/aries-askar#243</a></li>
<li>fix: Incorrect SQLite expire check by <a href="https://github.com/dkulic"><code>@​dkulic</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/261">hyperledger/aries-askar#261</a></li>
<li>Add python requirements file and update dependabot workflow by <a href="https://github.com/ff137"><code>@​ff137</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/262">hyperledger/aries-askar#262</a></li>
<li>chore(js): add expo example app and move to pnpm by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/247">hyperledger/aries-askar#247</a></li>
<li>build(deps-dev): update pytest requirement from ~=8.2.1 to ~=8.2.2 in /wrappers/python by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/265">hyperledger/aries-askar#265</a></li>
<li>chore: update library versions by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/271">hyperledger/aries-askar#271</a></li>
<li>build: allow action to create release by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/272">hyperledger/aries-askar#272</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/WadeBarnes"><code>@​WadeBarnes</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/223">hyperledger/aries-askar#223</a></li>
<li><a href="https://github.com/brianorwhatever"><code>@​brianorwhatever</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/239">hyperledger/aries-askar#239</a></li>
<li><a href="https://github.com/ja-bravo"><code>@​ja-bravo</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/248">hyperledger/aries-askar#248</a></li>
<li><a href="https://github.com/rajpalc7"><code>@​rajpalc7</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/249">hyperledger/aries-askar#249</a></li>
<li><a href="https://github.com/dkulic"><code>@​dkulic</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/261">hyperledger/aries-askar#261</a></li>
<li><a href="https://github.com/ff137"><code>@​ff137</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/262">hyperledger/aries-askar#262</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2">https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperledger/aries-askar/commit/10f58b3984bf6b2d370b8fb2cd07a0696bd93d2f"><code>10f58b3</code></a> build: allow action to create release</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/cf0586ed0cf28bc5197af40e4760158e79a77458"><code>cf0586e</code></a> chore: update library versions</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/c5ebacad74923a462ad754c5d726a0b069a62ca9"><code>c5ebaca</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/265">#265</a> from hyperledger/dependabot/pip/wrappers/python/pytes...</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/1a2f90a52dc336368334b7f14ebc2605e9f7ccf8"><code>1a2f90a</code></a> Merge branch 'main' into dependabot/pip/wrappers/python/pytest-approx-eq-8.2.2</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/9ff1271d36b73a765a3bd05c99376fa86d454973"><code>9ff1271</code></a> chore(js): add expo example app and move to pnpm (<a href="https://redirect.github.com/hyperledger/aries-askar/issues/247">#247</a>)</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/8923c50c2c7d6daf1cd856a060af2d9b672a258d"><code>8923c50</code></a> build(deps-dev): update pytest requirement in /wrappers/python</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/95a00366e78a5b504433576a8e31ad264dcc0d6f"><code>95a0036</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/262">#262</a> from ff137/add-python-requirements</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/594c2a1d7153cef38cf46e6fb5d41304e1a990da"><code>594c2a1</code></a> Merge branch 'main' into add-python-requirements</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/19034c97e9ab5e9b9d6fb459218c4c3894863836"><code>19034c9</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/261">#261</a> from dkulic/fix/sqlite_expire_check</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/ab33405ea58f37d8a6f68ad53205be2653ca4379"><code>ab33405</code></a> Merge branch 'main' into fix/sqlite_expire_check</li>
<li>Additional commits viewable in <a href="https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=aries-askar&package-manager=pip&previous-version=0.3.1&new-version=0.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 11:27:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/717" class=".btn">#717</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.5.0 to 0.5.1 in /redis_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.5.0 to 0.5.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>0.5.1</h2>
<h2>Release Notes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement mutable-contextvar-default (B039) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12113">#12113</a>)</li>
<li>[<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12140">#12140</a>)</li>
<li>[<code>pytest</code>] Reverse <code>PT001</code> and <code>PT0023</code> defaults (<a href="https://redirect.github.com/astral-sh/ruff/pull/12106">#12106</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>Enable token-based rules on source with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/11950">#11950</a>)</li>
<li>[<code>flake8-bandit</code>] Detect <code>httpx</code> for <code>S113</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12174">#12174</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY201</code> to include exception deprecations (<a href="https://redirect.github.com/astral-sh/ruff/pull/12065">#12065</a>)</li>
<li>[<code>pylint</code>] Generate autofix for <code>duplicate-bases</code> (<code>PLE0241</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12105">#12105</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Avoid syntax error notification for source code actions (<a href="https://redirect.github.com/astral-sh/ruff/pull/12148">#12148</a>)</li>
<li>Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/pull/12203">#12203</a>)</li>
<li>Fix replacement edit range computation (<a href="https://redirect.github.com/astral-sh/ruff/pull/12171">#12171</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Disable auto-fix when source has syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/12134">#12134</a>)</li>
<li>Fix cache key collisions for paths with separators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12159">#12159</a>)</li>
<li>Make <code>requires-python</code> inference robust to <code>==</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12091">#12091</a>)</li>
<li>Use char-wise width instead of <code>str</code>-width (<a href="https://redirect.github.com/astral-sh/ruff/pull/12135">#12135</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword followed by comma (<a href="https://redirect.github.com/astral-sh/ruff/pull/12136">#12136</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword is followed by a semicolon (<a href="https://redirect.github.com/astral-sh/ruff/pull/12095">#12095</a>)</li>
<li>[<code>pylint</code>] Skip <a href="https://docs.astral.sh/ruff/settings/#lint_dummy-variable-rgx">dummy variables</a> for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12190">#12190</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Remove allocation in <code>parse_identifier</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12103">#12103</a>)</li>
<li>Use <code>CompactString</code> for <code>Identifier</code> AST node (<a href="https://redirect.github.com/astral-sh/ruff/pull/12101">#12101</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/Peiffap"><code>@​Peiffap</code></a></li>
<li><a href="https://github.com/ThomasFaivre"><code>@​ThomasFaivre</code></a></li>
<li><a href="https://github.com/bersace"><code>@​bersace</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/github-actions"><code>@​github-actions</code></a></li>
<li><a href="https://github.com/jkauerl"><code>@​jkauerl</code></a></li>
<li><a href="https://github.com/mkniewallner"><code>@​mkniewallner</code></a></li>
<li><a href="https://github.com/mtsokol"><code>@​mtsokol</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.5.1</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement mutable-contextvar-default (B039) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12113">#12113</a>)</li>
<li>[<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12140">#12140</a>)</li>
<li>[<code>pytest</code>] Reverse <code>PT001</code> and <code>PT0023</code> defaults (<a href="https://redirect.github.com/astral-sh/ruff/pull/12106">#12106</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>Enable token-based rules on source with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/11950">#11950</a>)</li>
<li>[<code>flake8-bandit</code>] Detect <code>httpx</code> for <code>S113</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12174">#12174</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY201</code> to include exception deprecations (<a href="https://redirect.github.com/astral-sh/ruff/pull/12065">#12065</a>)</li>
<li>[<code>pylint</code>] Generate autofix for <code>duplicate-bases</code> (<code>PLE0241</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12105">#12105</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Avoid syntax error notification for source code actions (<a href="https://redirect.github.com/astral-sh/ruff/pull/12148">#12148</a>)</li>
<li>Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/pull/12203">#12203</a>)</li>
<li>Fix replacement edit range computation (<a href="https://redirect.github.com/astral-sh/ruff/pull/12171">#12171</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Disable auto-fix when source has syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/12134">#12134</a>)</li>
<li>Fix cache key collisions for paths with separators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12159">#12159</a>)</li>
<li>Make <code>requires-python</code> inference robust to <code>==</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12091">#12091</a>)</li>
<li>Use char-wise width instead of <code>str</code>-width (<a href="https://redirect.github.com/astral-sh/ruff/pull/12135">#12135</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword followed by comma (<a href="https://redirect.github.com/astral-sh/ruff/pull/12136">#12136</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword is followed by a semicolon (<a href="https://redirect.github.com/astral-sh/ruff/pull/12095">#12095</a>)</li>
<li>[<code>pylint</code>] Skip <a href="https://docs.astral.sh/ruff/settings/#lint_dummy-variable-rgx">dummy variables</a> for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12190">#12190</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Remove allocation in <code>parse_identifier</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12103">#12103</a>)</li>
<li>Use <code>CompactString</code> for <code>Identifier</code> AST node (<a href="https://redirect.github.com/astral-sh/ruff/pull/12101">#12101</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/3a72400202642f0bb340fb2b1d1c31da2b6524dd"><code>3a72400</code></a> Rename publish workflow file extension (<code>yaml</code> -&gt; <code>yml</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/12206">#12206</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1b3bff03300b2c48f0ad6c7bd6b1038e2f1fce5a"><code>1b3bff0</code></a> Bump version to 0.5.1 (<a href="https://redirect.github.com/astral-sh/ruff/issues/12205">#12205</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/0f6f73ecf3c2ebfe5b218edc0765886ccdca6f7f"><code>0f6f73e</code></a> [red-knot] Require that <code>FileSystem</code> objects implement <code>Debug</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12204">#12204</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/7910beecc42b2694890b10011c27a3cbb2db3335"><code>7910bee</code></a> Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/issues/12203">#12203</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f3ccd152e99d6bccfec58275c0b3b2ec3ffd5bdd"><code>f3ccd15</code></a> Revert &quot;Remove <code>--preview</code> as a required argument for <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12053">#12053</a>)&quot;...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1e07bfa3730db9461f51b877bf71ea31e7dd56e4"><code>1e07bfa</code></a> [<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/12140">#12140</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/5e7ba056128c8bc272ab1a2a22c9cb94a5079361"><code>5e7ba05</code></a> docs(*): fix a few typos, consistency issues and links (<a href="https://redirect.github.com/astral-sh/ruff/issues/12193">#12193</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d12570ea006d23a610e2410d9c70c3b3deae717c"><code>d12570e</code></a> docs(options): fix some typos and improve consistency (<a href="https://redirect.github.com/astral-sh/ruff/issues/12191">#12191</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2f3264e148b9cf31e32c3137feb0f5ce9532d85b"><code>2f3264e</code></a> fix(rules): skip dummy variables for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12190">#12190</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e2e0889a303e8ce9953a2eb8a426921d08176c5f"><code>e2e0889</code></a> [red-knot] Add very basic benchmark (<a href="https://redirect.github.com/astral-sh/ruff/issues/12182">#12182</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/0.5.0...0.5.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.5.0&new-version=0.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 11:23:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/716" class=".btn">#716</a>
            </td>
            <td>
                <b>
                    Bump aries-askar from 0.3.1 to 0.3.2 in /kafka_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [aries-askar](https://github.com/hyperledger/aries-askar) from 0.3.1 to 0.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperledger/aries-askar/releases">aries-askar's releases</a>.</em></p>
<blockquote>
<h2>v0.3.2</h2>
<h2>What's Changed</h2>
<ul>
<li>chore(js): update to stable 0.2.0 by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/222">hyperledger/aries-askar#222</a></li>
<li>Add Dependabot configuration by <a href="https://github.com/WadeBarnes"><code>@​WadeBarnes</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/223">hyperledger/aries-askar#223</a></li>
<li>build(deps): bump the all-actions group with 7 updates by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/224">hyperledger/aries-askar#224</a></li>
<li>build(deps): bump ip from 2.0.0 to 2.0.1 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/226">hyperledger/aries-askar#226</a></li>
<li>build(deps): bump es5-ext from 0.10.62 to 0.10.64 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/228">hyperledger/aries-askar#228</a></li>
<li>build(deps): bump mio from 0.8.10 to 0.8.11 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/229">hyperledger/aries-askar#229</a></li>
<li>build(deps): bump follow-redirects from 1.15.4 to 1.15.6 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/230">hyperledger/aries-askar#230</a></li>
<li>build(deps): bump the all-actions group with 1 update by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/231">hyperledger/aries-askar#231</a></li>
<li>fix(js): update ffi-napi by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/234">hyperledger/aries-askar#234</a></li>
<li>build(deps): bump a7ul/tar-action from 1.1.3 to 1.2.0 in the all-actions group by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/235">hyperledger/aries-askar#235</a></li>
<li>build(deps): bump whoami from 1.4.1 to 1.5.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/233">hyperledger/aries-askar#233</a></li>
<li>chore: update version for js wrapper by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/236">hyperledger/aries-askar#236</a></li>
<li>fix: correctly serliaize for buffer by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/238">hyperledger/aries-askar#238</a></li>
<li>Build Javascript on multiple platforms by <a href="https://github.com/brianorwhatever"><code>@​brianorwhatever</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/239">hyperledger/aries-askar#239</a></li>
<li>build(deps): bump rustls from 0.21.10 to 0.21.11 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/240">hyperledger/aries-askar#240</a></li>
<li>P256 keys using Secure Enclave and Android StrongBox by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/245">hyperledger/aries-askar#245</a></li>
<li>chore: update minSdkVersion to get the project version or fallback to 21 by <a href="https://github.com/ja-bravo"><code>@​ja-bravo</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/248">hyperledger/aries-askar#248</a></li>
<li>chore: updating dependabot to support gha, TS, JS and rust packages by <a href="https://github.com/rajpalc7"><code>@​rajpalc7</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/249">hyperledger/aries-askar#249</a></li>
<li>chore(js): update version to 0.2.2 by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/243">hyperledger/aries-askar#243</a></li>
<li>fix: Incorrect SQLite expire check by <a href="https://github.com/dkulic"><code>@​dkulic</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/261">hyperledger/aries-askar#261</a></li>
<li>Add python requirements file and update dependabot workflow by <a href="https://github.com/ff137"><code>@​ff137</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/262">hyperledger/aries-askar#262</a></li>
<li>chore(js): add expo example app and move to pnpm by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/247">hyperledger/aries-askar#247</a></li>
<li>build(deps-dev): update pytest requirement from ~=8.2.1 to ~=8.2.2 in /wrappers/python by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/265">hyperledger/aries-askar#265</a></li>
<li>chore: update library versions by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/271">hyperledger/aries-askar#271</a></li>
<li>build: allow action to create release by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/272">hyperledger/aries-askar#272</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/WadeBarnes"><code>@​WadeBarnes</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/223">hyperledger/aries-askar#223</a></li>
<li><a href="https://github.com/brianorwhatever"><code>@​brianorwhatever</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/239">hyperledger/aries-askar#239</a></li>
<li><a href="https://github.com/ja-bravo"><code>@​ja-bravo</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/248">hyperledger/aries-askar#248</a></li>
<li><a href="https://github.com/rajpalc7"><code>@​rajpalc7</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/249">hyperledger/aries-askar#249</a></li>
<li><a href="https://github.com/dkulic"><code>@​dkulic</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/261">hyperledger/aries-askar#261</a></li>
<li><a href="https://github.com/ff137"><code>@​ff137</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/262">hyperledger/aries-askar#262</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2">https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperledger/aries-askar/commit/10f58b3984bf6b2d370b8fb2cd07a0696bd93d2f"><code>10f58b3</code></a> build: allow action to create release</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/cf0586ed0cf28bc5197af40e4760158e79a77458"><code>cf0586e</code></a> chore: update library versions</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/c5ebacad74923a462ad754c5d726a0b069a62ca9"><code>c5ebaca</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/265">#265</a> from hyperledger/dependabot/pip/wrappers/python/pytes...</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/1a2f90a52dc336368334b7f14ebc2605e9f7ccf8"><code>1a2f90a</code></a> Merge branch 'main' into dependabot/pip/wrappers/python/pytest-approx-eq-8.2.2</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/9ff1271d36b73a765a3bd05c99376fa86d454973"><code>9ff1271</code></a> chore(js): add expo example app and move to pnpm (<a href="https://redirect.github.com/hyperledger/aries-askar/issues/247">#247</a>)</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/8923c50c2c7d6daf1cd856a060af2d9b672a258d"><code>8923c50</code></a> build(deps-dev): update pytest requirement in /wrappers/python</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/95a00366e78a5b504433576a8e31ad264dcc0d6f"><code>95a0036</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/262">#262</a> from ff137/add-python-requirements</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/594c2a1d7153cef38cf46e6fb5d41304e1a990da"><code>594c2a1</code></a> Merge branch 'main' into add-python-requirements</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/19034c97e9ab5e9b9d6fb459218c4c3894863836"><code>19034c9</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/261">#261</a> from dkulic/fix/sqlite_expire_check</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/ab33405ea58f37d8a6f68ad53205be2653ca4379"><code>ab33405</code></a> Merge branch 'main' into fix/sqlite_expire_check</li>
<li>Additional commits viewable in <a href="https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=aries-askar&package-manager=pip&previous-version=0.3.1&new-version=0.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 11:23:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/715" class=".btn">#715</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.5.0 to 0.5.1 in /kafka_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.5.0 to 0.5.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>0.5.1</h2>
<h2>Release Notes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement mutable-contextvar-default (B039) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12113">#12113</a>)</li>
<li>[<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12140">#12140</a>)</li>
<li>[<code>pytest</code>] Reverse <code>PT001</code> and <code>PT0023</code> defaults (<a href="https://redirect.github.com/astral-sh/ruff/pull/12106">#12106</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>Enable token-based rules on source with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/11950">#11950</a>)</li>
<li>[<code>flake8-bandit</code>] Detect <code>httpx</code> for <code>S113</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12174">#12174</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY201</code> to include exception deprecations (<a href="https://redirect.github.com/astral-sh/ruff/pull/12065">#12065</a>)</li>
<li>[<code>pylint</code>] Generate autofix for <code>duplicate-bases</code> (<code>PLE0241</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12105">#12105</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Avoid syntax error notification for source code actions (<a href="https://redirect.github.com/astral-sh/ruff/pull/12148">#12148</a>)</li>
<li>Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/pull/12203">#12203</a>)</li>
<li>Fix replacement edit range computation (<a href="https://redirect.github.com/astral-sh/ruff/pull/12171">#12171</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Disable auto-fix when source has syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/12134">#12134</a>)</li>
<li>Fix cache key collisions for paths with separators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12159">#12159</a>)</li>
<li>Make <code>requires-python</code> inference robust to <code>==</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12091">#12091</a>)</li>
<li>Use char-wise width instead of <code>str</code>-width (<a href="https://redirect.github.com/astral-sh/ruff/pull/12135">#12135</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword followed by comma (<a href="https://redirect.github.com/astral-sh/ruff/pull/12136">#12136</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword is followed by a semicolon (<a href="https://redirect.github.com/astral-sh/ruff/pull/12095">#12095</a>)</li>
<li>[<code>pylint</code>] Skip <a href="https://docs.astral.sh/ruff/settings/#lint_dummy-variable-rgx">dummy variables</a> for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12190">#12190</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Remove allocation in <code>parse_identifier</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12103">#12103</a>)</li>
<li>Use <code>CompactString</code> for <code>Identifier</code> AST node (<a href="https://redirect.github.com/astral-sh/ruff/pull/12101">#12101</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/Peiffap"><code>@​Peiffap</code></a></li>
<li><a href="https://github.com/ThomasFaivre"><code>@​ThomasFaivre</code></a></li>
<li><a href="https://github.com/bersace"><code>@​bersace</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/github-actions"><code>@​github-actions</code></a></li>
<li><a href="https://github.com/jkauerl"><code>@​jkauerl</code></a></li>
<li><a href="https://github.com/mkniewallner"><code>@​mkniewallner</code></a></li>
<li><a href="https://github.com/mtsokol"><code>@​mtsokol</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.5.1</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement mutable-contextvar-default (B039) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12113">#12113</a>)</li>
<li>[<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12140">#12140</a>)</li>
<li>[<code>pytest</code>] Reverse <code>PT001</code> and <code>PT0023</code> defaults (<a href="https://redirect.github.com/astral-sh/ruff/pull/12106">#12106</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>Enable token-based rules on source with syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/11950">#11950</a>)</li>
<li>[<code>flake8-bandit</code>] Detect <code>httpx</code> for <code>S113</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12174">#12174</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY201</code> to include exception deprecations (<a href="https://redirect.github.com/astral-sh/ruff/pull/12065">#12065</a>)</li>
<li>[<code>pylint</code>] Generate autofix for <code>duplicate-bases</code> (<code>PLE0241</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12105">#12105</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Avoid syntax error notification for source code actions (<a href="https://redirect.github.com/astral-sh/ruff/pull/12148">#12148</a>)</li>
<li>Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/pull/12203">#12203</a>)</li>
<li>Fix replacement edit range computation (<a href="https://redirect.github.com/astral-sh/ruff/pull/12171">#12171</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Disable auto-fix when source has syntax errors (<a href="https://redirect.github.com/astral-sh/ruff/pull/12134">#12134</a>)</li>
<li>Fix cache key collisions for paths with separators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12159">#12159</a>)</li>
<li>Make <code>requires-python</code> inference robust to <code>==</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12091">#12091</a>)</li>
<li>Use char-wise width instead of <code>str</code>-width (<a href="https://redirect.github.com/astral-sh/ruff/pull/12135">#12135</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword followed by comma (<a href="https://redirect.github.com/astral-sh/ruff/pull/12136">#12136</a>)</li>
<li>[<code>pycodestyle</code>] Avoid <code>E275</code> if keyword is followed by a semicolon (<a href="https://redirect.github.com/astral-sh/ruff/pull/12095">#12095</a>)</li>
<li>[<code>pylint</code>] Skip <a href="https://docs.astral.sh/ruff/settings/#lint_dummy-variable-rgx">dummy variables</a> for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12190">#12190</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Remove allocation in <code>parse_identifier</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12103">#12103</a>)</li>
<li>Use <code>CompactString</code> for <code>Identifier</code> AST node (<a href="https://redirect.github.com/astral-sh/ruff/pull/12101">#12101</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/3a72400202642f0bb340fb2b1d1c31da2b6524dd"><code>3a72400</code></a> Rename publish workflow file extension (<code>yaml</code> -&gt; <code>yml</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/12206">#12206</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1b3bff03300b2c48f0ad6c7bd6b1038e2f1fce5a"><code>1b3bff0</code></a> Bump version to 0.5.1 (<a href="https://redirect.github.com/astral-sh/ruff/issues/12205">#12205</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/0f6f73ecf3c2ebfe5b218edc0765886ccdca6f7f"><code>0f6f73e</code></a> [red-knot] Require that <code>FileSystem</code> objects implement <code>Debug</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12204">#12204</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/7910beecc42b2694890b10011c27a3cbb2db3335"><code>7910bee</code></a> Consider the content of the new cells during notebook sync (<a href="https://redirect.github.com/astral-sh/ruff/issues/12203">#12203</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f3ccd152e99d6bccfec58275c0b3b2ec3ffd5bdd"><code>f3ccd15</code></a> Revert &quot;Remove <code>--preview</code> as a required argument for <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12053">#12053</a>)&quot;...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1e07bfa3730db9461f51b877bf71ea31e7dd56e4"><code>1e07bfa</code></a> [<code>pycodestyle</code>] Whitespace after decorator (<code>E204</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/12140">#12140</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/5e7ba056128c8bc272ab1a2a22c9cb94a5079361"><code>5e7ba05</code></a> docs(*): fix a few typos, consistency issues and links (<a href="https://redirect.github.com/astral-sh/ruff/issues/12193">#12193</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d12570ea006d23a610e2410d9c70c3b3deae717c"><code>d12570e</code></a> docs(options): fix some typos and improve consistency (<a href="https://redirect.github.com/astral-sh/ruff/issues/12191">#12191</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2f3264e148b9cf31e32c3137feb0f5ce9532d85b"><code>2f3264e</code></a> fix(rules): skip dummy variables for <code>PLR1704</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/12190">#12190</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e2e0889a303e8ce9953a2eb8a426921d08176c5f"><code>e2e0889</code></a> [red-knot] Add very basic benchmark (<a href="https://redirect.github.com/astral-sh/ruff/issues/12182">#12182</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/0.5.0...0.5.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.5.0&new-version=0.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 11:22:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/714" class=".btn">#714</a>
            </td>
            <td>
                <b>
                    Bump aries-askar from 0.3.1 to 0.3.2 in /redis_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [aries-askar](https://github.com/hyperledger/aries-askar) from 0.3.1 to 0.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperledger/aries-askar/releases">aries-askar's releases</a>.</em></p>
<blockquote>
<h2>v0.3.2</h2>
<h2>What's Changed</h2>
<ul>
<li>chore(js): update to stable 0.2.0 by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/222">hyperledger/aries-askar#222</a></li>
<li>Add Dependabot configuration by <a href="https://github.com/WadeBarnes"><code>@​WadeBarnes</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/223">hyperledger/aries-askar#223</a></li>
<li>build(deps): bump the all-actions group with 7 updates by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/224">hyperledger/aries-askar#224</a></li>
<li>build(deps): bump ip from 2.0.0 to 2.0.1 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/226">hyperledger/aries-askar#226</a></li>
<li>build(deps): bump es5-ext from 0.10.62 to 0.10.64 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/228">hyperledger/aries-askar#228</a></li>
<li>build(deps): bump mio from 0.8.10 to 0.8.11 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/229">hyperledger/aries-askar#229</a></li>
<li>build(deps): bump follow-redirects from 1.15.4 to 1.15.6 in /wrappers/javascript by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/230">hyperledger/aries-askar#230</a></li>
<li>build(deps): bump the all-actions group with 1 update by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/231">hyperledger/aries-askar#231</a></li>
<li>fix(js): update ffi-napi by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/234">hyperledger/aries-askar#234</a></li>
<li>build(deps): bump a7ul/tar-action from 1.1.3 to 1.2.0 in the all-actions group by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/235">hyperledger/aries-askar#235</a></li>
<li>build(deps): bump whoami from 1.4.1 to 1.5.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/233">hyperledger/aries-askar#233</a></li>
<li>chore: update version for js wrapper by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/236">hyperledger/aries-askar#236</a></li>
<li>fix: correctly serliaize for buffer by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/238">hyperledger/aries-askar#238</a></li>
<li>Build Javascript on multiple platforms by <a href="https://github.com/brianorwhatever"><code>@​brianorwhatever</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/239">hyperledger/aries-askar#239</a></li>
<li>build(deps): bump rustls from 0.21.10 to 0.21.11 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/240">hyperledger/aries-askar#240</a></li>
<li>P256 keys using Secure Enclave and Android StrongBox by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/245">hyperledger/aries-askar#245</a></li>
<li>chore: update minSdkVersion to get the project version or fallback to 21 by <a href="https://github.com/ja-bravo"><code>@​ja-bravo</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/248">hyperledger/aries-askar#248</a></li>
<li>chore: updating dependabot to support gha, TS, JS and rust packages by <a href="https://github.com/rajpalc7"><code>@​rajpalc7</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/249">hyperledger/aries-askar#249</a></li>
<li>chore(js): update version to 0.2.2 by <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/243">hyperledger/aries-askar#243</a></li>
<li>fix: Incorrect SQLite expire check by <a href="https://github.com/dkulic"><code>@​dkulic</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/261">hyperledger/aries-askar#261</a></li>
<li>Add python requirements file and update dependabot workflow by <a href="https://github.com/ff137"><code>@​ff137</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/262">hyperledger/aries-askar#262</a></li>
<li>chore(js): add expo example app and move to pnpm by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/247">hyperledger/aries-askar#247</a></li>
<li>build(deps-dev): update pytest requirement from ~=8.2.1 to ~=8.2.2 in /wrappers/python by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/265">hyperledger/aries-askar#265</a></li>
<li>chore: update library versions by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/271">hyperledger/aries-askar#271</a></li>
<li>build: allow action to create release by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/272">hyperledger/aries-askar#272</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/WadeBarnes"><code>@​WadeBarnes</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/223">hyperledger/aries-askar#223</a></li>
<li><a href="https://github.com/brianorwhatever"><code>@​brianorwhatever</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/239">hyperledger/aries-askar#239</a></li>
<li><a href="https://github.com/ja-bravo"><code>@​ja-bravo</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/248">hyperledger/aries-askar#248</a></li>
<li><a href="https://github.com/rajpalc7"><code>@​rajpalc7</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/249">hyperledger/aries-askar#249</a></li>
<li><a href="https://github.com/dkulic"><code>@​dkulic</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/261">hyperledger/aries-askar#261</a></li>
<li><a href="https://github.com/ff137"><code>@​ff137</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/aries-askar/pull/262">hyperledger/aries-askar#262</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2">https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperledger/aries-askar/commit/10f58b3984bf6b2d370b8fb2cd07a0696bd93d2f"><code>10f58b3</code></a> build: allow action to create release</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/cf0586ed0cf28bc5197af40e4760158e79a77458"><code>cf0586e</code></a> chore: update library versions</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/c5ebacad74923a462ad754c5d726a0b069a62ca9"><code>c5ebaca</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/265">#265</a> from hyperledger/dependabot/pip/wrappers/python/pytes...</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/1a2f90a52dc336368334b7f14ebc2605e9f7ccf8"><code>1a2f90a</code></a> Merge branch 'main' into dependabot/pip/wrappers/python/pytest-approx-eq-8.2.2</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/9ff1271d36b73a765a3bd05c99376fa86d454973"><code>9ff1271</code></a> chore(js): add expo example app and move to pnpm (<a href="https://redirect.github.com/hyperledger/aries-askar/issues/247">#247</a>)</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/8923c50c2c7d6daf1cd856a060af2d9b672a258d"><code>8923c50</code></a> build(deps-dev): update pytest requirement in /wrappers/python</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/95a00366e78a5b504433576a8e31ad264dcc0d6f"><code>95a0036</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/262">#262</a> from ff137/add-python-requirements</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/594c2a1d7153cef38cf46e6fb5d41304e1a990da"><code>594c2a1</code></a> Merge branch 'main' into add-python-requirements</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/19034c97e9ab5e9b9d6fb459218c4c3894863836"><code>19034c9</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/aries-askar/issues/261">#261</a> from dkulic/fix/sqlite_expire_check</li>
<li><a href="https://github.com/hyperledger/aries-askar/commit/ab33405ea58f37d8a6f68ad53205be2653ca4379"><code>ab33405</code></a> Merge branch 'main' into fix/sqlite_expire_check</li>
<li>Additional commits viewable in <a href="https://github.com/hyperledger/aries-askar/compare/v0.3.1...v0.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=aries-askar&package-manager=pip&previous-version=0.3.1&new-version=0.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 11:22:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/713" class=".btn">#713</a>
            </td>
            <td>
                <b>
                    Bump aiokafka from 0.7.2 to 0.9.0 in /kafka_events/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [aiokafka](https://github.com/aio-libs/aiokafka) from 0.7.2 to 0.9.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/aio-libs/aiokafka/releases">aiokafka's releases</a>.</em></p>
<blockquote>
<h2>v0.9.0</h2>
<p>New features:</p>
<ul>
<li>Include <code>kafka-python</code> into <code>aiokafka</code>'s code base (issue <a href="https://redirect.github.com/aio-libs/aiokafka/issues/928">#928</a> and others)</li>
<li>Replace <code>python-snappy</code> and <code>zstandard</code> with <code>cramjam</code> (issue <a href="https://redirect.github.com/aio-libs/aiokafka/issues/930">#930</a>)</li>
<li>PEP518 compliant <code>pyproject.toml</code></li>
<li>Python 3.12 support</li>
</ul>
<p>Bugfixes:</p>
<ul>
<li>Fix type annotation for <code>ConsumerRecord</code> (pr <a href="https://redirect.github.com/aio-libs/aiokafka/issues/912">#912</a> by <a href="https://github.com/zschumacher"><code>@​zschumacher</code></a>)</li>
<li>Improve send performance (issue <a href="https://redirect.github.com/aio-libs/aiokafka/issues/943">#943</a>)</li>
</ul>
<p>Improved Documentation:</p>
<ul>
<li>Fix <code>AbstractTokenProvider.token</code> example (pr <a href="https://redirect.github.com/aio-libs/aiokafka/issues/919">#919</a> by <a href="https://github.com/mtomilov"><code>@​mtomilov</code></a>)</li>
</ul>
<h2>v0.9.0.rc1</h2>
<p>New features:</p>
<ul>
<li>Include <code>kafka-python</code> into <code>aiokafka</code>'s code base</li>
<li>Replace <code>python-snappy</code> and <code>zstandard</code> with <code>cramjam</code></li>
<li>PEP518 compliant <code>pyproject.toml</code></li>
<li>Python 3.12 support</li>
</ul>
<p>Bugfixes:</p>
<ul>
<li>Fix type annotation for <code>ConsumerRecord</code> (pr <a href="https://redirect.github.com/aio-libs/aiokafka/issues/912">#912</a> by <a href="https://github.com/zschumacher"><code>@​zschumacher</code></a>)</li>
<li>Improve send performance (issue <a href="https://redirect.github.com/aio-libs/aiokafka/issues/943">#943</a>)</li>
</ul>
<p>Improved Documentation:</p>
<ul>
<li>Fix <code>AbstractTokenProvider.token</code> example (pr <a href="https://redirect.github.com/aio-libs/aiokafka/issues/919">#919</a> by <a href="https://github.com/mtomilov"><code>@​mtomilov</code></a>)</li>
</ul>
<h2>v0.9.0.rc0</h2>
<p>New features:</p>
<ul>
<li>Include <code>kafka-python</code> into <code>aiokafka</code>'s code base</li>
<li>Replace <code>python-snappy</code> and <code>zstandard</code> with <code>cramjam</code></li>
<li>PEP518 compliant <code>pyproject.toml</code></li>
<li>Python 3.12 support</li>
</ul>
<p>Bugfixes:</p>
<ul>
<li>Fix type annotation for <code>ConsumerRecord</code> (pr <a href="https://redirect.github.com/aio-libs/aiokafka/issues/912">#912</a> by <a href="https://github.com/zschumacher"><code>@​zschumacher</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/aio-libs/aiokafka/blob/master/CHANGES.rst">aiokafka's changelog</a>.</em></p>
<blockquote>
<h1>0.9.0 (2023-12-04)</h1>
<p>New features:</p>
<ul>
<li>Include <code>kafka-python</code> into <code>aiokafka</code>'s code base (issue <a href="https://redirect.github.com/aio-libs/aiokafka/issues/928">#928</a> and others)</li>
<li>Replace <code>python-snappy</code> and <code>zstandard</code> with <code>cramjam</code> (issue <a href="https://redirect.github.com/aio-libs/aiokafka/issues/930">#930</a>)</li>
<li>PEP518 compliant <code>pyproject.toml</code></li>
<li>Python 3.12 support</li>
</ul>
<p>Bugfixes:</p>
<ul>
<li>Fix type annotation for <code>ConsumerRecord</code> (pr <a href="https://redirect.github.com/aio-libs/aiokafka/issues/912">#912</a> by <a href="https://github.com/zschumacher"><code>@​zschumacher</code></a>)</li>
<li>Improve send performance (issue <a href="https://redirect.github.com/aio-libs/aiokafka/issues/943">#943</a>)</li>
<li>Fix <code>DescribeConfigsResponse_v1</code></li>
</ul>
<p>Improved Documentation:</p>
<ul>
<li>Fix <code>AbstractTokenProvider.token</code> example (pr <a href="https://redirect.github.com/aio-libs/aiokafka/issues/919">#919</a> by <a href="https://github.com/mtomilov"><code>@​mtomilov</code></a>)</li>
</ul>
<h1>0.8.1 (2023-05-31)</h1>
<p>New features:</p>
<ul>
<li>Drop support for Python 3.7 due to end of life (pr <a href="https://redirect.github.com/aio-libs/aiokafka/issues/893">#893</a>)</li>
</ul>
<p>Bugfixes:</p>
<ul>
<li>Add SASL authentication support to <code>AIOKafkaAdminClient</code> (issue <a href="https://redirect.github.com/aio-libs/aiokafka/issues/889">#889</a>,
pr <a href="https://redirect.github.com/aio-libs/aiokafka/issues/890">#890</a> by <a href="https://github.com/selevit"><code>@​selevit</code></a>)</li>
</ul>
<p>Improved Documentation:</p>
<ul>
<li>Update <code>security_protocol</code> argument docstring (issue <a href="https://redirect.github.com/aio-libs/aiokafka/issues/883">#883</a>, pr <a href="https://redirect.github.com/aio-libs/aiokafka/issues/884">#884</a> by
<a href="https://github.com/gabrielmbmb"><code>@​gabrielmbmb</code></a>)</li>
<li>Remove incorrect <code>await</code> for <code>AIOKafkaConsumer.highwater()</code> (pr <a href="https://redirect.github.com/aio-libs/aiokafka/issues/858">#858</a> by
<a href="https://github.com/yi-jiayu"><code>@​yi-jiayu</code></a>)</li>
</ul>
<h1>0.8.0 (2022-11-21)</h1>
<p>New features:</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/aio-libs/aiokafka/commit/881851783673e927591ba274a7703c9b52d387ac"><code>8818517</code></a> Prepare 0.9.0 release</li>
<li><a href="https://github.com/aio-libs/aiokafka/commit/d7201c1e26fd2f3e51f15a2cdeda9753d4fd3a1a"><code>d7201c1</code></a> Prepare 0.9.0.rc1 release</li>
<li><a href="https://github.com/aio-libs/aiokafka/commit/a25e5c2294ab5967dc4480a71dd07244cbca468d"><code>a25e5c2</code></a> Merge pull request <a href="https://redirect.github.com/aio-libs/aiokafka/issues/947">#947</a> from ods/kafka-python-cleanup</li>
<li><a href="https://github.com/aio-libs/aiokafka/commit/fdba76455bfeb91ec349201e396e9840ddda2f90"><code>fdba764</code></a> Fix docstrings</li>
<li><a href="https://github.com/aio-libs/aiokafka/commit/170834fa9f5abbef64e3157860ebb873a3aff428"><code>170834f</code></a> Drop unused KafkaBytes</li>
<li><a href="https://github.com/aio-libs/aiokafka/commit/2e3ed6460dd561d6bc26f71a217dd0b0ee25c902"><code>2e3ed64</code></a> Remove unused modules</li>
<li><a href="https://github.com/aio-libs/aiokafka/commit/702b31f3495295d3ef774bb4dc2a2c2afb2c0f5e"><code>702b31f</code></a> Configure coverage</li>
<li><a href="https://github.com/aio-libs/aiokafka/commit/8814e7b8cac108527d98ff5378eab9a0519a8528"><code>8814e7b</code></a> Merge pull request <a href="https://redirect.github.com/aio-libs/aiokafka/issues/946">#946</a> from ods/issue943-send-perfomance</li>
<li><a href="https://github.com/aio-libs/aiokafka/commit/3554731f74f936cc004ab4479f9443ed9576b5ae"><code>3554731</code></a> Improve send performance</li>
<li><a href="https://github.com/aio-libs/aiokafka/commit/b029fa292a95540ce06157324faa4e837f719b59"><code>b029fa2</code></a> Prepare 0.9.0.rc0 release</li>
<li>Additional commits viewable in <a href="https://github.com/aio-libs/aiokafka/compare/v0.7.2...v0.9.0">compare view</a></li>
</ul>
</details>
<br />

<details>
<summary>Most Recent Ignore Conditions Applied to This Pull Request</summary>

| Dependency Name | Ignore Conditions |
| --- | --- |
| aiokafka | [>= 0.10.a, < 0.11] |
| aiokafka | [>= 0.11.a, < 0.12] |
</details>


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=aiokafka&package-manager=pip&previous-version=0.7.2&new-version=0.9.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 11:16:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/712" class=".btn">#712</a>
            </td>
            <td>
                <b>
                    Bump certifi from 2024.2.2 to 2024.7.4 in /oid4vci in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /oid4vci with 1 update: [certifi](https://github.com/certifi/python-certifi).

Updates `certifi` from 2024.2.2 to 2024.7.4
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/bd8153872e9c6fc98f4023df9c2deaffea2fa463"><code>bd81538</code></a> 2024.07.04 (<a href="https://redirect.github.com/certifi/python-certifi/issues/295">#295</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/06a2cbf21f345563dde6c28b60e29d57e9b210b3"><code>06a2cbf</code></a> Bump peter-evans/create-pull-request from 6.0.5 to 6.1.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/294">#294</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/13bba02b72bac97c432c277158bc04b4d2a6bc23"><code>13bba02</code></a> Bump actions/checkout from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/293">#293</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e8abcd0e62b334c164b95d49fcabdc9ecbca0554"><code>e8abcd0</code></a> Bump pypa/gh-action-pypi-publish from 1.8.14 to 1.9.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/292">#292</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/124f4adf171e15cd9a91a8b6e0325ecc97be8fe1"><code>124f4ad</code></a> 2024.06.02 (<a href="https://redirect.github.com/certifi/python-certifi/issues/291">#291</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c2196ce5d6ee675b27755a19948480a7823e2c6a"><code>c2196ce</code></a> --- (<a href="https://redirect.github.com/certifi/python-certifi/issues/290">#290</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/fefdeec7588ff1c05214b85a552afcad5fdb51b2"><code>fefdeec</code></a> Bump actions/checkout from 4.1.4 to 4.1.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/289">#289</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/3c5fb1560b826a7f83f1f9750173ff766492c9cf"><code>3c5fb15</code></a> Bump actions/download-artifact from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/286">#286</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/4a9569a3eb58db8548536fc16c5c5c7af946a5b1"><code>4a9569a</code></a> Bump actions/checkout from 4.1.2 to 4.1.4 (<a href="https://redirect.github.com/certifi/python-certifi/issues/287">#287</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/1fc808626a895a916b1e4c2b63abae6c5eafdbe3"><code>1fc8086</code></a> Bump peter-evans/create-pull-request from 6.0.4 to 6.0.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/288">#288</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/certifi/python-certifi/compare/2024.02.02...2024.07.04">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2024.2.2&new-version=2024.7.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-06 02:03:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/711" class=".btn">#711</a>
            </td>
            <td>
                <b>
                    Bump certifi from 2024.2.2 to 2024.7.4 in /kafka_events/demo/setup in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /kafka_events/demo/setup with 1 update: [certifi](https://github.com/certifi/python-certifi).

Updates `certifi` from 2024.2.2 to 2024.7.4
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/bd8153872e9c6fc98f4023df9c2deaffea2fa463"><code>bd81538</code></a> 2024.07.04 (<a href="https://redirect.github.com/certifi/python-certifi/issues/295">#295</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/06a2cbf21f345563dde6c28b60e29d57e9b210b3"><code>06a2cbf</code></a> Bump peter-evans/create-pull-request from 6.0.5 to 6.1.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/294">#294</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/13bba02b72bac97c432c277158bc04b4d2a6bc23"><code>13bba02</code></a> Bump actions/checkout from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/293">#293</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e8abcd0e62b334c164b95d49fcabdc9ecbca0554"><code>e8abcd0</code></a> Bump pypa/gh-action-pypi-publish from 1.8.14 to 1.9.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/292">#292</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/124f4adf171e15cd9a91a8b6e0325ecc97be8fe1"><code>124f4ad</code></a> 2024.06.02 (<a href="https://redirect.github.com/certifi/python-certifi/issues/291">#291</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c2196ce5d6ee675b27755a19948480a7823e2c6a"><code>c2196ce</code></a> --- (<a href="https://redirect.github.com/certifi/python-certifi/issues/290">#290</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/fefdeec7588ff1c05214b85a552afcad5fdb51b2"><code>fefdeec</code></a> Bump actions/checkout from 4.1.4 to 4.1.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/289">#289</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/3c5fb1560b826a7f83f1f9750173ff766492c9cf"><code>3c5fb15</code></a> Bump actions/download-artifact from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/286">#286</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/4a9569a3eb58db8548536fc16c5c5c7af946a5b1"><code>4a9569a</code></a> Bump actions/checkout from 4.1.2 to 4.1.4 (<a href="https://redirect.github.com/certifi/python-certifi/issues/287">#287</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/1fc808626a895a916b1e4c2b63abae6c5eafdbe3"><code>1fc8086</code></a> Bump peter-evans/create-pull-request from 6.0.4 to 6.0.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/288">#288</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/certifi/python-certifi/compare/2024.02.02...2024.07.04">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2024.2.2&new-version=2024.7.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-06 02:03:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/710" class=".btn">#710</a>
            </td>
            <td>
                <b>
                    Bump certifi from 2024.2.2 to 2024.7.4 in /plugin_globals in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /plugin_globals with 1 update: [certifi](https://github.com/certifi/python-certifi).

Updates `certifi` from 2024.2.2 to 2024.7.4
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/bd8153872e9c6fc98f4023df9c2deaffea2fa463"><code>bd81538</code></a> 2024.07.04 (<a href="https://redirect.github.com/certifi/python-certifi/issues/295">#295</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/06a2cbf21f345563dde6c28b60e29d57e9b210b3"><code>06a2cbf</code></a> Bump peter-evans/create-pull-request from 6.0.5 to 6.1.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/294">#294</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/13bba02b72bac97c432c277158bc04b4d2a6bc23"><code>13bba02</code></a> Bump actions/checkout from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/293">#293</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e8abcd0e62b334c164b95d49fcabdc9ecbca0554"><code>e8abcd0</code></a> Bump pypa/gh-action-pypi-publish from 1.8.14 to 1.9.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/292">#292</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/124f4adf171e15cd9a91a8b6e0325ecc97be8fe1"><code>124f4ad</code></a> 2024.06.02 (<a href="https://redirect.github.com/certifi/python-certifi/issues/291">#291</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c2196ce5d6ee675b27755a19948480a7823e2c6a"><code>c2196ce</code></a> --- (<a href="https://redirect.github.com/certifi/python-certifi/issues/290">#290</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/fefdeec7588ff1c05214b85a552afcad5fdb51b2"><code>fefdeec</code></a> Bump actions/checkout from 4.1.4 to 4.1.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/289">#289</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/3c5fb1560b826a7f83f1f9750173ff766492c9cf"><code>3c5fb15</code></a> Bump actions/download-artifact from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/286">#286</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/4a9569a3eb58db8548536fc16c5c5c7af946a5b1"><code>4a9569a</code></a> Bump actions/checkout from 4.1.2 to 4.1.4 (<a href="https://redirect.github.com/certifi/python-certifi/issues/287">#287</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/1fc808626a895a916b1e4c2b63abae6c5eafdbe3"><code>1fc8086</code></a> Bump peter-evans/create-pull-request from 6.0.4 to 6.0.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/288">#288</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/certifi/python-certifi/compare/2024.02.02...2024.07.04">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2024.2.2&new-version=2024.7.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-06 02:00:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/709" class=".btn">#709</a>
            </td>
            <td>
                <b>
                    Bump certifi from 2024.2.2 to 2024.7.4 in /firebase_push_notifications in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /firebase_push_notifications with 1 update: [certifi](https://github.com/certifi/python-certifi).

Updates `certifi` from 2024.2.2 to 2024.7.4
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/bd8153872e9c6fc98f4023df9c2deaffea2fa463"><code>bd81538</code></a> 2024.07.04 (<a href="https://redirect.github.com/certifi/python-certifi/issues/295">#295</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/06a2cbf21f345563dde6c28b60e29d57e9b210b3"><code>06a2cbf</code></a> Bump peter-evans/create-pull-request from 6.0.5 to 6.1.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/294">#294</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/13bba02b72bac97c432c277158bc04b4d2a6bc23"><code>13bba02</code></a> Bump actions/checkout from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/293">#293</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e8abcd0e62b334c164b95d49fcabdc9ecbca0554"><code>e8abcd0</code></a> Bump pypa/gh-action-pypi-publish from 1.8.14 to 1.9.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/292">#292</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/124f4adf171e15cd9a91a8b6e0325ecc97be8fe1"><code>124f4ad</code></a> 2024.06.02 (<a href="https://redirect.github.com/certifi/python-certifi/issues/291">#291</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c2196ce5d6ee675b27755a19948480a7823e2c6a"><code>c2196ce</code></a> --- (<a href="https://redirect.github.com/certifi/python-certifi/issues/290">#290</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/fefdeec7588ff1c05214b85a552afcad5fdb51b2"><code>fefdeec</code></a> Bump actions/checkout from 4.1.4 to 4.1.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/289">#289</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/3c5fb1560b826a7f83f1f9750173ff766492c9cf"><code>3c5fb15</code></a> Bump actions/download-artifact from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/286">#286</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/4a9569a3eb58db8548536fc16c5c5c7af946a5b1"><code>4a9569a</code></a> Bump actions/checkout from 4.1.2 to 4.1.4 (<a href="https://redirect.github.com/certifi/python-certifi/issues/287">#287</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/1fc808626a895a916b1e4c2b63abae6c5eafdbe3"><code>1fc8086</code></a> Bump peter-evans/create-pull-request from 6.0.4 to 6.0.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/288">#288</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/certifi/python-certifi/compare/2024.02.02...2024.07.04">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2024.2.2&new-version=2024.7.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-06 01:45:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/708" class=".btn">#708</a>
            </td>
            <td>
                <b>
                    Bump certifi from 2024.2.2 to 2024.7.4 in /firebase_push_notifications/integration in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /firebase_push_notifications/integration with 1 update: [certifi](https://github.com/certifi/python-certifi).

Updates `certifi` from 2024.2.2 to 2024.7.4
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/bd8153872e9c6fc98f4023df9c2deaffea2fa463"><code>bd81538</code></a> 2024.07.04 (<a href="https://redirect.github.com/certifi/python-certifi/issues/295">#295</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/06a2cbf21f345563dde6c28b60e29d57e9b210b3"><code>06a2cbf</code></a> Bump peter-evans/create-pull-request from 6.0.5 to 6.1.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/294">#294</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/13bba02b72bac97c432c277158bc04b4d2a6bc23"><code>13bba02</code></a> Bump actions/checkout from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/293">#293</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e8abcd0e62b334c164b95d49fcabdc9ecbca0554"><code>e8abcd0</code></a> Bump pypa/gh-action-pypi-publish from 1.8.14 to 1.9.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/292">#292</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/124f4adf171e15cd9a91a8b6e0325ecc97be8fe1"><code>124f4ad</code></a> 2024.06.02 (<a href="https://redirect.github.com/certifi/python-certifi/issues/291">#291</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c2196ce5d6ee675b27755a19948480a7823e2c6a"><code>c2196ce</code></a> --- (<a href="https://redirect.github.com/certifi/python-certifi/issues/290">#290</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/fefdeec7588ff1c05214b85a552afcad5fdb51b2"><code>fefdeec</code></a> Bump actions/checkout from 4.1.4 to 4.1.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/289">#289</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/3c5fb1560b826a7f83f1f9750173ff766492c9cf"><code>3c5fb15</code></a> Bump actions/download-artifact from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/286">#286</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/4a9569a3eb58db8548536fc16c5c5c7af946a5b1"><code>4a9569a</code></a> Bump actions/checkout from 4.1.2 to 4.1.4 (<a href="https://redirect.github.com/certifi/python-certifi/issues/287">#287</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/1fc808626a895a916b1e4c2b63abae6c5eafdbe3"><code>1fc8086</code></a> Bump peter-evans/create-pull-request from 6.0.4 to 6.0.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/288">#288</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/certifi/python-certifi/compare/2024.02.02...2024.07.04">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2024.2.2&new-version=2024.7.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-06 01:44:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/707" class=".btn">#707</a>
            </td>
            <td>
                <b>
                    Bump certifi from 2024.2.2 to 2024.7.4 in /multitenant_provider in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /multitenant_provider with 1 update: [certifi](https://github.com/certifi/python-certifi).

Updates `certifi` from 2024.2.2 to 2024.7.4
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/bd8153872e9c6fc98f4023df9c2deaffea2fa463"><code>bd81538</code></a> 2024.07.04 (<a href="https://redirect.github.com/certifi/python-certifi/issues/295">#295</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/06a2cbf21f345563dde6c28b60e29d57e9b210b3"><code>06a2cbf</code></a> Bump peter-evans/create-pull-request from 6.0.5 to 6.1.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/294">#294</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/13bba02b72bac97c432c277158bc04b4d2a6bc23"><code>13bba02</code></a> Bump actions/checkout from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/293">#293</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e8abcd0e62b334c164b95d49fcabdc9ecbca0554"><code>e8abcd0</code></a> Bump pypa/gh-action-pypi-publish from 1.8.14 to 1.9.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/292">#292</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/124f4adf171e15cd9a91a8b6e0325ecc97be8fe1"><code>124f4ad</code></a> 2024.06.02 (<a href="https://redirect.github.com/certifi/python-certifi/issues/291">#291</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c2196ce5d6ee675b27755a19948480a7823e2c6a"><code>c2196ce</code></a> --- (<a href="https://redirect.github.com/certifi/python-certifi/issues/290">#290</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/fefdeec7588ff1c05214b85a552afcad5fdb51b2"><code>fefdeec</code></a> Bump actions/checkout from 4.1.4 to 4.1.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/289">#289</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/3c5fb1560b826a7f83f1f9750173ff766492c9cf"><code>3c5fb15</code></a> Bump actions/download-artifact from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/286">#286</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/4a9569a3eb58db8548536fc16c5c5c7af946a5b1"><code>4a9569a</code></a> Bump actions/checkout from 4.1.2 to 4.1.4 (<a href="https://redirect.github.com/certifi/python-certifi/issues/287">#287</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/1fc808626a895a916b1e4c2b63abae6c5eafdbe3"><code>1fc8086</code></a> Bump peter-evans/create-pull-request from 6.0.4 to 6.0.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/288">#288</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/certifi/python-certifi/compare/2024.02.02...2024.07.04">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2024.2.2&new-version=2024.7.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-06 01:42:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/706" class=".btn">#706</a>
            </td>
            <td>
                <b>
                    Bump certifi from 2024.2.2 to 2024.7.4 in /multitenant_provider/integration in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /multitenant_provider/integration with 1 update: [certifi](https://github.com/certifi/python-certifi).

Updates `certifi` from 2024.2.2 to 2024.7.4
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/bd8153872e9c6fc98f4023df9c2deaffea2fa463"><code>bd81538</code></a> 2024.07.04 (<a href="https://redirect.github.com/certifi/python-certifi/issues/295">#295</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/06a2cbf21f345563dde6c28b60e29d57e9b210b3"><code>06a2cbf</code></a> Bump peter-evans/create-pull-request from 6.0.5 to 6.1.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/294">#294</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/13bba02b72bac97c432c277158bc04b4d2a6bc23"><code>13bba02</code></a> Bump actions/checkout from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/293">#293</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e8abcd0e62b334c164b95d49fcabdc9ecbca0554"><code>e8abcd0</code></a> Bump pypa/gh-action-pypi-publish from 1.8.14 to 1.9.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/292">#292</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/124f4adf171e15cd9a91a8b6e0325ecc97be8fe1"><code>124f4ad</code></a> 2024.06.02 (<a href="https://redirect.github.com/certifi/python-certifi/issues/291">#291</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c2196ce5d6ee675b27755a19948480a7823e2c6a"><code>c2196ce</code></a> --- (<a href="https://redirect.github.com/certifi/python-certifi/issues/290">#290</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/fefdeec7588ff1c05214b85a552afcad5fdb51b2"><code>fefdeec</code></a> Bump actions/checkout from 4.1.4 to 4.1.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/289">#289</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/3c5fb1560b826a7f83f1f9750173ff766492c9cf"><code>3c5fb15</code></a> Bump actions/download-artifact from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/286">#286</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/4a9569a3eb58db8548536fc16c5c5c7af946a5b1"><code>4a9569a</code></a> Bump actions/checkout from 4.1.2 to 4.1.4 (<a href="https://redirect.github.com/certifi/python-certifi/issues/287">#287</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/1fc808626a895a916b1e4c2b63abae6c5eafdbe3"><code>1fc8086</code></a> Bump peter-evans/create-pull-request from 6.0.4 to 6.0.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/288">#288</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/certifi/python-certifi/compare/2024.02.02...2024.07.04">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2024.2.2&new-version=2024.7.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-06 01:41:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/705" class=".btn">#705</a>
            </td>
            <td>
                <b>
                    Bump certifi from 2024.2.2 to 2024.7.4 in /redis_events in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /redis_events with 1 update: [certifi](https://github.com/certifi/python-certifi).

Updates `certifi` from 2024.2.2 to 2024.7.4
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/bd8153872e9c6fc98f4023df9c2deaffea2fa463"><code>bd81538</code></a> 2024.07.04 (<a href="https://redirect.github.com/certifi/python-certifi/issues/295">#295</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/06a2cbf21f345563dde6c28b60e29d57e9b210b3"><code>06a2cbf</code></a> Bump peter-evans/create-pull-request from 6.0.5 to 6.1.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/294">#294</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/13bba02b72bac97c432c277158bc04b4d2a6bc23"><code>13bba02</code></a> Bump actions/checkout from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/293">#293</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e8abcd0e62b334c164b95d49fcabdc9ecbca0554"><code>e8abcd0</code></a> Bump pypa/gh-action-pypi-publish from 1.8.14 to 1.9.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/292">#292</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/124f4adf171e15cd9a91a8b6e0325ecc97be8fe1"><code>124f4ad</code></a> 2024.06.02 (<a href="https://redirect.github.com/certifi/python-certifi/issues/291">#291</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c2196ce5d6ee675b27755a19948480a7823e2c6a"><code>c2196ce</code></a> --- (<a href="https://redirect.github.com/certifi/python-certifi/issues/290">#290</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/fefdeec7588ff1c05214b85a552afcad5fdb51b2"><code>fefdeec</code></a> Bump actions/checkout from 4.1.4 to 4.1.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/289">#289</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/3c5fb1560b826a7f83f1f9750173ff766492c9cf"><code>3c5fb15</code></a> Bump actions/download-artifact from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/286">#286</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/4a9569a3eb58db8548536fc16c5c5c7af946a5b1"><code>4a9569a</code></a> Bump actions/checkout from 4.1.2 to 4.1.4 (<a href="https://redirect.github.com/certifi/python-certifi/issues/287">#287</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/1fc808626a895a916b1e4c2b63abae6c5eafdbe3"><code>1fc8086</code></a> Bump peter-evans/create-pull-request from 6.0.4 to 6.0.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/288">#288</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/certifi/python-certifi/compare/2024.02.02...2024.07.04">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2024.2.2&new-version=2024.7.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-06 01:41:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/704" class=".btn">#704</a>
            </td>
            <td>
                <b>
                    Bump certifi from 2024.2.2 to 2024.7.4 in /kafka_events in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /kafka_events with 1 update: [certifi](https://github.com/certifi/python-certifi).

Updates `certifi` from 2024.2.2 to 2024.7.4
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/bd8153872e9c6fc98f4023df9c2deaffea2fa463"><code>bd81538</code></a> 2024.07.04 (<a href="https://redirect.github.com/certifi/python-certifi/issues/295">#295</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/06a2cbf21f345563dde6c28b60e29d57e9b210b3"><code>06a2cbf</code></a> Bump peter-evans/create-pull-request from 6.0.5 to 6.1.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/294">#294</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/13bba02b72bac97c432c277158bc04b4d2a6bc23"><code>13bba02</code></a> Bump actions/checkout from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/293">#293</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e8abcd0e62b334c164b95d49fcabdc9ecbca0554"><code>e8abcd0</code></a> Bump pypa/gh-action-pypi-publish from 1.8.14 to 1.9.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/292">#292</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/124f4adf171e15cd9a91a8b6e0325ecc97be8fe1"><code>124f4ad</code></a> 2024.06.02 (<a href="https://redirect.github.com/certifi/python-certifi/issues/291">#291</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c2196ce5d6ee675b27755a19948480a7823e2c6a"><code>c2196ce</code></a> --- (<a href="https://redirect.github.com/certifi/python-certifi/issues/290">#290</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/fefdeec7588ff1c05214b85a552afcad5fdb51b2"><code>fefdeec</code></a> Bump actions/checkout from 4.1.4 to 4.1.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/289">#289</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/3c5fb1560b826a7f83f1f9750173ff766492c9cf"><code>3c5fb15</code></a> Bump actions/download-artifact from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/286">#286</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/4a9569a3eb58db8548536fc16c5c5c7af946a5b1"><code>4a9569a</code></a> Bump actions/checkout from 4.1.2 to 4.1.4 (<a href="https://redirect.github.com/certifi/python-certifi/issues/287">#287</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/1fc808626a895a916b1e4c2b63abae6c5eafdbe3"><code>1fc8086</code></a> Bump peter-evans/create-pull-request from 6.0.4 to 6.0.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/288">#288</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/certifi/python-certifi/compare/2024.02.02...2024.07.04">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2024.2.2&new-version=2024.7.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-06 01:41:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/703" class=".btn">#703</a>
            </td>
            <td>
                <b>
                    Bump certifi from 2024.2.2 to 2024.7.4 in /connection_update in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /connection_update with 1 update: [certifi](https://github.com/certifi/python-certifi).

Updates `certifi` from 2024.2.2 to 2024.7.4
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/bd8153872e9c6fc98f4023df9c2deaffea2fa463"><code>bd81538</code></a> 2024.07.04 (<a href="https://redirect.github.com/certifi/python-certifi/issues/295">#295</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/06a2cbf21f345563dde6c28b60e29d57e9b210b3"><code>06a2cbf</code></a> Bump peter-evans/create-pull-request from 6.0.5 to 6.1.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/294">#294</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/13bba02b72bac97c432c277158bc04b4d2a6bc23"><code>13bba02</code></a> Bump actions/checkout from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/293">#293</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e8abcd0e62b334c164b95d49fcabdc9ecbca0554"><code>e8abcd0</code></a> Bump pypa/gh-action-pypi-publish from 1.8.14 to 1.9.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/292">#292</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/124f4adf171e15cd9a91a8b6e0325ecc97be8fe1"><code>124f4ad</code></a> 2024.06.02 (<a href="https://redirect.github.com/certifi/python-certifi/issues/291">#291</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c2196ce5d6ee675b27755a19948480a7823e2c6a"><code>c2196ce</code></a> --- (<a href="https://redirect.github.com/certifi/python-certifi/issues/290">#290</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/fefdeec7588ff1c05214b85a552afcad5fdb51b2"><code>fefdeec</code></a> Bump actions/checkout from 4.1.4 to 4.1.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/289">#289</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/3c5fb1560b826a7f83f1f9750173ff766492c9cf"><code>3c5fb15</code></a> Bump actions/download-artifact from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/286">#286</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/4a9569a3eb58db8548536fc16c5c5c7af946a5b1"><code>4a9569a</code></a> Bump actions/checkout from 4.1.2 to 4.1.4 (<a href="https://redirect.github.com/certifi/python-certifi/issues/287">#287</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/1fc808626a895a916b1e4c2b63abae6c5eafdbe3"><code>1fc8086</code></a> Bump peter-evans/create-pull-request from 6.0.4 to 6.0.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/288">#288</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/certifi/python-certifi/compare/2024.02.02...2024.07.04">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2024.2.2&new-version=2024.7.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-06 01:41:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/702" class=".btn">#702</a>
            </td>
            <td>
                <b>
                    Bump certifi from 2024.2.2 to 2024.7.4 in /basicmessage_storage in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /basicmessage_storage with 1 update: [certifi](https://github.com/certifi/python-certifi).

Updates `certifi` from 2024.2.2 to 2024.7.4
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/bd8153872e9c6fc98f4023df9c2deaffea2fa463"><code>bd81538</code></a> 2024.07.04 (<a href="https://redirect.github.com/certifi/python-certifi/issues/295">#295</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/06a2cbf21f345563dde6c28b60e29d57e9b210b3"><code>06a2cbf</code></a> Bump peter-evans/create-pull-request from 6.0.5 to 6.1.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/294">#294</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/13bba02b72bac97c432c277158bc04b4d2a6bc23"><code>13bba02</code></a> Bump actions/checkout from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/293">#293</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e8abcd0e62b334c164b95d49fcabdc9ecbca0554"><code>e8abcd0</code></a> Bump pypa/gh-action-pypi-publish from 1.8.14 to 1.9.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/292">#292</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/124f4adf171e15cd9a91a8b6e0325ecc97be8fe1"><code>124f4ad</code></a> 2024.06.02 (<a href="https://redirect.github.com/certifi/python-certifi/issues/291">#291</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c2196ce5d6ee675b27755a19948480a7823e2c6a"><code>c2196ce</code></a> --- (<a href="https://redirect.github.com/certifi/python-certifi/issues/290">#290</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/fefdeec7588ff1c05214b85a552afcad5fdb51b2"><code>fefdeec</code></a> Bump actions/checkout from 4.1.4 to 4.1.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/289">#289</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/3c5fb1560b826a7f83f1f9750173ff766492c9cf"><code>3c5fb15</code></a> Bump actions/download-artifact from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/286">#286</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/4a9569a3eb58db8548536fc16c5c5c7af946a5b1"><code>4a9569a</code></a> Bump actions/checkout from 4.1.2 to 4.1.4 (<a href="https://redirect.github.com/certifi/python-certifi/issues/287">#287</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/1fc808626a895a916b1e4c2b63abae6c5eafdbe3"><code>1fc8086</code></a> Bump peter-evans/create-pull-request from 6.0.4 to 6.0.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/288">#288</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/certifi/python-certifi/compare/2024.02.02...2024.07.04">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2024.2.2&new-version=2024.7.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-06 01:41:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/701" class=".btn">#701</a>
            </td>
            <td>
                <b>
                    Bump certifi from 2024.2.2 to 2024.7.4 in /basicmessage_storage/integration in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /basicmessage_storage/integration with 1 update: [certifi](https://github.com/certifi/python-certifi).

Updates `certifi` from 2024.2.2 to 2024.7.4
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/bd8153872e9c6fc98f4023df9c2deaffea2fa463"><code>bd81538</code></a> 2024.07.04 (<a href="https://redirect.github.com/certifi/python-certifi/issues/295">#295</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/06a2cbf21f345563dde6c28b60e29d57e9b210b3"><code>06a2cbf</code></a> Bump peter-evans/create-pull-request from 6.0.5 to 6.1.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/294">#294</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/13bba02b72bac97c432c277158bc04b4d2a6bc23"><code>13bba02</code></a> Bump actions/checkout from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/293">#293</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e8abcd0e62b334c164b95d49fcabdc9ecbca0554"><code>e8abcd0</code></a> Bump pypa/gh-action-pypi-publish from 1.8.14 to 1.9.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/292">#292</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/124f4adf171e15cd9a91a8b6e0325ecc97be8fe1"><code>124f4ad</code></a> 2024.06.02 (<a href="https://redirect.github.com/certifi/python-certifi/issues/291">#291</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c2196ce5d6ee675b27755a19948480a7823e2c6a"><code>c2196ce</code></a> --- (<a href="https://redirect.github.com/certifi/python-certifi/issues/290">#290</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/fefdeec7588ff1c05214b85a552afcad5fdb51b2"><code>fefdeec</code></a> Bump actions/checkout from 4.1.4 to 4.1.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/289">#289</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/3c5fb1560b826a7f83f1f9750173ff766492c9cf"><code>3c5fb15</code></a> Bump actions/download-artifact from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/286">#286</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/4a9569a3eb58db8548536fc16c5c5c7af946a5b1"><code>4a9569a</code></a> Bump actions/checkout from 4.1.2 to 4.1.4 (<a href="https://redirect.github.com/certifi/python-certifi/issues/287">#287</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/1fc808626a895a916b1e4c2b63abae6c5eafdbe3"><code>1fc8086</code></a> Bump peter-evans/create-pull-request from 6.0.4 to 6.0.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/288">#288</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/certifi/python-certifi/compare/2024.02.02...2024.07.04">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2024.2.2&new-version=2024.7.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-06 01:40:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/700" class=".btn">#700</a>
            </td>
            <td>
                <b>
                    Bump certifi from 2024.2.2 to 2024.7.4 in /connection_update/integration in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /connection_update/integration with 1 update: [certifi](https://github.com/certifi/python-certifi).

Updates `certifi` from 2024.2.2 to 2024.7.4
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/bd8153872e9c6fc98f4023df9c2deaffea2fa463"><code>bd81538</code></a> 2024.07.04 (<a href="https://redirect.github.com/certifi/python-certifi/issues/295">#295</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/06a2cbf21f345563dde6c28b60e29d57e9b210b3"><code>06a2cbf</code></a> Bump peter-evans/create-pull-request from 6.0.5 to 6.1.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/294">#294</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/13bba02b72bac97c432c277158bc04b4d2a6bc23"><code>13bba02</code></a> Bump actions/checkout from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/293">#293</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e8abcd0e62b334c164b95d49fcabdc9ecbca0554"><code>e8abcd0</code></a> Bump pypa/gh-action-pypi-publish from 1.8.14 to 1.9.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/292">#292</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/124f4adf171e15cd9a91a8b6e0325ecc97be8fe1"><code>124f4ad</code></a> 2024.06.02 (<a href="https://redirect.github.com/certifi/python-certifi/issues/291">#291</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c2196ce5d6ee675b27755a19948480a7823e2c6a"><code>c2196ce</code></a> --- (<a href="https://redirect.github.com/certifi/python-certifi/issues/290">#290</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/fefdeec7588ff1c05214b85a552afcad5fdb51b2"><code>fefdeec</code></a> Bump actions/checkout from 4.1.4 to 4.1.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/289">#289</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/3c5fb1560b826a7f83f1f9750173ff766492c9cf"><code>3c5fb15</code></a> Bump actions/download-artifact from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/286">#286</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/4a9569a3eb58db8548536fc16c5c5c7af946a5b1"><code>4a9569a</code></a> Bump actions/checkout from 4.1.2 to 4.1.4 (<a href="https://redirect.github.com/certifi/python-certifi/issues/287">#287</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/1fc808626a895a916b1e4c2b63abae6c5eafdbe3"><code>1fc8086</code></a> Bump peter-evans/create-pull-request from 6.0.4 to 6.0.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/288">#288</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/certifi/python-certifi/compare/2024.02.02...2024.07.04">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2024.2.2&new-version=2024.7.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-06 01:40:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/699" class=".btn">#699</a>
            </td>
            <td>
                <b>
                    Bump certifi from 2024.2.2 to 2024.7.4 in /redis_events/integration in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /redis_events/integration with 1 update: [certifi](https://github.com/certifi/python-certifi).

Updates `certifi` from 2024.2.2 to 2024.7.4
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/bd8153872e9c6fc98f4023df9c2deaffea2fa463"><code>bd81538</code></a> 2024.07.04 (<a href="https://redirect.github.com/certifi/python-certifi/issues/295">#295</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/06a2cbf21f345563dde6c28b60e29d57e9b210b3"><code>06a2cbf</code></a> Bump peter-evans/create-pull-request from 6.0.5 to 6.1.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/294">#294</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/13bba02b72bac97c432c277158bc04b4d2a6bc23"><code>13bba02</code></a> Bump actions/checkout from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/293">#293</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e8abcd0e62b334c164b95d49fcabdc9ecbca0554"><code>e8abcd0</code></a> Bump pypa/gh-action-pypi-publish from 1.8.14 to 1.9.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/292">#292</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/124f4adf171e15cd9a91a8b6e0325ecc97be8fe1"><code>124f4ad</code></a> 2024.06.02 (<a href="https://redirect.github.com/certifi/python-certifi/issues/291">#291</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c2196ce5d6ee675b27755a19948480a7823e2c6a"><code>c2196ce</code></a> --- (<a href="https://redirect.github.com/certifi/python-certifi/issues/290">#290</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/fefdeec7588ff1c05214b85a552afcad5fdb51b2"><code>fefdeec</code></a> Bump actions/checkout from 4.1.4 to 4.1.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/289">#289</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/3c5fb1560b826a7f83f1f9750173ff766492c9cf"><code>3c5fb15</code></a> Bump actions/download-artifact from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/286">#286</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/4a9569a3eb58db8548536fc16c5c5c7af946a5b1"><code>4a9569a</code></a> Bump actions/checkout from 4.1.2 to 4.1.4 (<a href="https://redirect.github.com/certifi/python-certifi/issues/287">#287</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/1fc808626a895a916b1e4c2b63abae6c5eafdbe3"><code>1fc8086</code></a> Bump peter-evans/create-pull-request from 6.0.4 to 6.0.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/288">#288</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/certifi/python-certifi/compare/2024.02.02...2024.07.04">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2024.2.2&new-version=2024.7.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-06 01:40:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/698" class=".btn">#698</a>
            </td>
            <td>
                <b>
                    Bump certifi from 2024.2.2 to 2024.7.4 in /kafka_events/integration in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /kafka_events/integration with 1 update: [certifi](https://github.com/certifi/python-certifi).

Updates `certifi` from 2024.2.2 to 2024.7.4
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/bd8153872e9c6fc98f4023df9c2deaffea2fa463"><code>bd81538</code></a> 2024.07.04 (<a href="https://redirect.github.com/certifi/python-certifi/issues/295">#295</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/06a2cbf21f345563dde6c28b60e29d57e9b210b3"><code>06a2cbf</code></a> Bump peter-evans/create-pull-request from 6.0.5 to 6.1.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/294">#294</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/13bba02b72bac97c432c277158bc04b4d2a6bc23"><code>13bba02</code></a> Bump actions/checkout from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/293">#293</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e8abcd0e62b334c164b95d49fcabdc9ecbca0554"><code>e8abcd0</code></a> Bump pypa/gh-action-pypi-publish from 1.8.14 to 1.9.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/292">#292</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/124f4adf171e15cd9a91a8b6e0325ecc97be8fe1"><code>124f4ad</code></a> 2024.06.02 (<a href="https://redirect.github.com/certifi/python-certifi/issues/291">#291</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c2196ce5d6ee675b27755a19948480a7823e2c6a"><code>c2196ce</code></a> --- (<a href="https://redirect.github.com/certifi/python-certifi/issues/290">#290</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/fefdeec7588ff1c05214b85a552afcad5fdb51b2"><code>fefdeec</code></a> Bump actions/checkout from 4.1.4 to 4.1.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/289">#289</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/3c5fb1560b826a7f83f1f9750173ff766492c9cf"><code>3c5fb15</code></a> Bump actions/download-artifact from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/286">#286</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/4a9569a3eb58db8548536fc16c5c5c7af946a5b1"><code>4a9569a</code></a> Bump actions/checkout from 4.1.2 to 4.1.4 (<a href="https://redirect.github.com/certifi/python-certifi/issues/287">#287</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/1fc808626a895a916b1e4c2b63abae6c5eafdbe3"><code>1fc8086</code></a> Bump peter-evans/create-pull-request from 6.0.4 to 6.0.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/288">#288</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/certifi/python-certifi/compare/2024.02.02...2024.07.04">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2024.2.2&new-version=2024.7.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-06 01:40:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/697" class=".btn">#697</a>
            </td>
            <td>
                <b>
                    Bump certifi from 2024.2.2 to 2024.7.4 in /rpc/integration in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /rpc/integration with 1 update: [certifi](https://github.com/certifi/python-certifi).

Updates `certifi` from 2024.2.2 to 2024.7.4
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/bd8153872e9c6fc98f4023df9c2deaffea2fa463"><code>bd81538</code></a> 2024.07.04 (<a href="https://redirect.github.com/certifi/python-certifi/issues/295">#295</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/06a2cbf21f345563dde6c28b60e29d57e9b210b3"><code>06a2cbf</code></a> Bump peter-evans/create-pull-request from 6.0.5 to 6.1.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/294">#294</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/13bba02b72bac97c432c277158bc04b4d2a6bc23"><code>13bba02</code></a> Bump actions/checkout from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/293">#293</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e8abcd0e62b334c164b95d49fcabdc9ecbca0554"><code>e8abcd0</code></a> Bump pypa/gh-action-pypi-publish from 1.8.14 to 1.9.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/292">#292</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/124f4adf171e15cd9a91a8b6e0325ecc97be8fe1"><code>124f4ad</code></a> 2024.06.02 (<a href="https://redirect.github.com/certifi/python-certifi/issues/291">#291</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c2196ce5d6ee675b27755a19948480a7823e2c6a"><code>c2196ce</code></a> --- (<a href="https://redirect.github.com/certifi/python-certifi/issues/290">#290</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/fefdeec7588ff1c05214b85a552afcad5fdb51b2"><code>fefdeec</code></a> Bump actions/checkout from 4.1.4 to 4.1.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/289">#289</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/3c5fb1560b826a7f83f1f9750173ff766492c9cf"><code>3c5fb15</code></a> Bump actions/download-artifact from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/286">#286</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/4a9569a3eb58db8548536fc16c5c5c7af946a5b1"><code>4a9569a</code></a> Bump actions/checkout from 4.1.2 to 4.1.4 (<a href="https://redirect.github.com/certifi/python-certifi/issues/287">#287</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/1fc808626a895a916b1e4c2b63abae6c5eafdbe3"><code>1fc8086</code></a> Bump peter-evans/create-pull-request from 6.0.4 to 6.0.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/288">#288</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/certifi/python-certifi/compare/2024.02.02...2024.07.04">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2024.2.2&new-version=2024.7.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-06 01:40:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/696" class=".btn">#696</a>
            </td>
            <td>
                <b>
                    Bump certifi from 2024.2.2 to 2024.7.4 in /rpc in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /rpc with 1 update: [certifi](https://github.com/certifi/python-certifi).

Updates `certifi` from 2024.2.2 to 2024.7.4
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/bd8153872e9c6fc98f4023df9c2deaffea2fa463"><code>bd81538</code></a> 2024.07.04 (<a href="https://redirect.github.com/certifi/python-certifi/issues/295">#295</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/06a2cbf21f345563dde6c28b60e29d57e9b210b3"><code>06a2cbf</code></a> Bump peter-evans/create-pull-request from 6.0.5 to 6.1.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/294">#294</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/13bba02b72bac97c432c277158bc04b4d2a6bc23"><code>13bba02</code></a> Bump actions/checkout from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/293">#293</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e8abcd0e62b334c164b95d49fcabdc9ecbca0554"><code>e8abcd0</code></a> Bump pypa/gh-action-pypi-publish from 1.8.14 to 1.9.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/292">#292</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/124f4adf171e15cd9a91a8b6e0325ecc97be8fe1"><code>124f4ad</code></a> 2024.06.02 (<a href="https://redirect.github.com/certifi/python-certifi/issues/291">#291</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c2196ce5d6ee675b27755a19948480a7823e2c6a"><code>c2196ce</code></a> --- (<a href="https://redirect.github.com/certifi/python-certifi/issues/290">#290</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/fefdeec7588ff1c05214b85a552afcad5fdb51b2"><code>fefdeec</code></a> Bump actions/checkout from 4.1.4 to 4.1.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/289">#289</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/3c5fb1560b826a7f83f1f9750173ff766492c9cf"><code>3c5fb15</code></a> Bump actions/download-artifact from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/286">#286</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/4a9569a3eb58db8548536fc16c5c5c7af946a5b1"><code>4a9569a</code></a> Bump actions/checkout from 4.1.2 to 4.1.4 (<a href="https://redirect.github.com/certifi/python-certifi/issues/287">#287</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/1fc808626a895a916b1e4c2b63abae6c5eafdbe3"><code>1fc8086</code></a> Bump peter-evans/create-pull-request from 6.0.4 to 6.0.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/288">#288</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/certifi/python-certifi/compare/2024.02.02...2024.07.04">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2024.2.2&new-version=2024.7.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-06 01:39:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/695" class=".btn">#695</a>
            </td>
            <td>
                <b>
                    General upgrades ruff, redis, google-api-python-client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some weekly upgrade. Ruff from 4 --> 5 had some breaking changes but I don't think they affect us. See https://github.com/astral-sh/ruff/releases/tag/0.5.0

Will do the others individually.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-02 22:04:44 +0000 UTC
    </div>
</div>

