---
layout: default
title: aries-endorser-service
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-endorser-service
---

# aries-endorser-service <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-endorser-service){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-endorser-service/pull/113" class=".btn">#113</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.4.4 to 0.5.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.4.4 to 0.5.1.
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
<h2>0.5.0</h2>
<p>Check out the <a href="https://astral.sh/blog/ruff-v0.5.0">blog post</a> for a migration guide and overview of the changes!</p>
<h3>Breaking changes</h3>
<p>See also, the &quot;Remapped rules&quot; section which may result in disabled rules.</p>
<ul>
<li>Follow the XDG specification to discover user-level configurations on macOS (same as on other Unix platforms)</li>
<li>Selecting <code>ALL</code> now excludes deprecated rules</li>
<li>The released archives now include an extra level of nesting, which can be removed with <code>--strip-components=1</code> when untarring.</li>
<li>The release artifact's file name no longer includes the version tag. This enables users to install via <code>/latest</code> URLs on GitHub.</li>
<li>The diagnostic ranges for some <code>flake8-bandit</code> rules were modified (<a href="https://redirect.github.com/astral-sh/ruff/pull/10667">#10667</a>).</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.4.4...0.5.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.4.4&new-version=0.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-08 11:19:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-endorser-service/pull/112" class=".btn">#112</a>
            </td>
            <td>
                <b>
                    Bump the pip group with 2 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group with 2 updates: [certifi](https://github.com/certifi/python-certifi) and [urllib3](https://github.com/urllib3/urllib3).

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

Updates `urllib3` from 2.2.1 to 2.2.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/releases">urllib3's releases</a>.</em></p>
<blockquote>
<h2>2.2.2</h2>
<h2>🚀 urllib3 is fundraising for HTTP/2 support</h2>
<p><a href="https://sethmlarson.dev/urllib3-is-fundraising-for-http2-support">urllib3 is raising ~$40,000 USD</a> to release HTTP/2 support and ensure long-term sustainable maintenance of the project after a sharp decline in financial support for 2023. If your company or organization uses Python and would benefit from HTTP/2 support in Requests, pip, cloud SDKs, and thousands of other projects <a href="https://opencollective.com/urllib3">please consider contributing financially</a> to ensure HTTP/2 support is developed sustainably and maintained for the long-haul.</p>
<p>Thank you for your support.</p>
<h2>Changes</h2>
<ul>
<li>Added the <code>Proxy-Authorization</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>.</li>
<li>Allowed passing negative integers as <code>amt</code> to read methods of <code>http.client.HTTPResponse</code> as an alternative to <code>None</code>. (<a href="https://redirect.github.com/urllib3/urllib3/issues/3122">#3122</a>)</li>
<li>Fixed return types representing copying actions to use <code>typing.Self</code>. (<a href="https://redirect.github.com/urllib3/urllib3/issues/3363">#3363</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/urllib3/urllib3/compare/2.2.1...2.2.2">https://github.com/urllib3/urllib3/compare/2.2.1...2.2.2</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/blob/main/CHANGES.rst">urllib3's changelog</a>.</em></p>
<blockquote>
<h1>2.2.2 (2024-06-17)</h1>
<ul>
<li>Added the <code>Proxy-Authorization</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>.</li>
<li>Allowed passing negative integers as <code>amt</code> to read methods of <code>http.client.HTTPResponse</code> as an alternative to <code>None</code>. (<code>[#3122](https://github.com/urllib3/urllib3/issues/3122) &lt;https://github.com/urllib3/urllib3/issues/3122&gt;</code>__)</li>
<li>Fixed return types representing copying actions to use <code>typing.Self</code>. (<code>[#3363](https://github.com/urllib3/urllib3/issues/3363) &lt;https://github.com/urllib3/urllib3/issues/3363&gt;</code>__)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/urllib3/urllib3/commit/27e2a5c5a7ab6a517252cc8dcef3ffa6ffb8f61a"><code>27e2a5c</code></a> Release 2.2.2 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3406">#3406</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/accff72ecc2f6cf5a76d9570198a93ac7c90270e"><code>accff72</code></a> Merge pull request from GHSA-34jh-p97f-mpxf</li>
<li><a href="https://github.com/urllib3/urllib3/commit/34be4a57e59eb7365bcc37d52e9f8271b5b8d0d3"><code>34be4a5</code></a> Pin CFFI to a new release candidate instead of a Git commit (<a href="https://redirect.github.com/urllib3/urllib3/issues/3398">#3398</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/da410581b6b3df73da976b5ce5eb20a4bd030437"><code>da41058</code></a> Bump browser-actions/setup-chrome from 1.6.0 to 1.7.1 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3399">#3399</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/b07a669bd970d69847801148286b726f0570b625"><code>b07a669</code></a> Bump github/codeql-action from 2.13.4 to 3.25.6 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3396">#3396</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/b8589ec9f8c4da91511e601b632ac06af7e7c10e"><code>b8589ec</code></a> Measure coverage with v4 of artifact actions (<a href="https://redirect.github.com/urllib3/urllib3/issues/3394">#3394</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/f3bdc5585111429e22c81b5fb26c3ec164d98b81"><code>f3bdc55</code></a> Allow triggering CI manually (<a href="https://redirect.github.com/urllib3/urllib3/issues/3391">#3391</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/52392654b30183129cf3ec06010306f517d9c146"><code>5239265</code></a> Fix HTTP version in debug log (<a href="https://redirect.github.com/urllib3/urllib3/issues/3316">#3316</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/b34619f94ece0c40e691a5aaf1304953d88089de"><code>b34619f</code></a> Bump actions/checkout to 4.1.4 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3387">#3387</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/9961d14de7c920091d42d42ed76d5d479b80064d"><code>9961d14</code></a> Bump browser-actions/setup-chrome from 1.5.0 to 1.6.0 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3386">#3386</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/urllib3/urllib3/compare/2.2.1...2.2.2">compare view</a></li>
</ul>
</details>
<br />


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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-endorser-service/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-06 02:14:21 +0000 UTC
    </div>
</div>

