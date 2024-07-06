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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-endorser-service/pull/111" class=".btn">#111</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.4.4 to 0.5.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.4.4 to 0.5.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>0.5.0</h2>
<h2>Release Notes</h2>
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
<h3>Deprecations</h3>
<p>The following rules are now deprecated:</p>
<ul>
<li><a href="https://docs.astral.sh/ruff/rules/syntax-error/"><code>syntax-error</code></a> (<code>E999</code>): Syntax errors are now always shown</li>
</ul>
<h3>Remapped rules</h3>
<p>The following rules have been remapped to new rule codes:</p>
<ul>
<li><a href="https://docs.astral.sh/ruff/rules/blocking-http-call-in-async-function/"><code>blocking-http-call-in-async-function</code></a>: <code>ASYNC100</code> to <code>ASYNC210</code></li>
<li><a href="https://docs.astral.sh/ruff/rules/open-sleep-or-subprocess-in-async-function/"><code>open-sleep-or-subprocess-in-async-function</code></a>: <code>ASYNC101</code> split into <code>ASYNC220</code>, <code>ASYNC221</code>, <code>ASYNC230</code>, and <code>ASYNC251</code></li>
<li><a href="https://docs.astral.sh/ruff/rules/blocking-os-call-in-async-function/"><code>blocking-os-call-in-async-function</code></a>: <code>ASYNC102</code> has been merged into <code>ASYNC220</code> and <code>ASYNC221</code></li>
<li><a href="https://docs.astral.sh/ruff/rules/trio-timeout-without-await/"><code>trio-timeout-without-await</code></a>: <code>TRIO100</code> to <code>ASYNC100</code></li>
<li><a href="https://docs.astral.sh/ruff/rules/trio-sync-call/"><code>trio-sync-call</code></a>: <code>TRIO105</code> to <code>ASYNC105</code></li>
<li><a href="https://docs.astral.sh/ruff/rules/trio-async-function-with-timeout/"><code>trio-async-function-with-timeout</code></a>: <code>TRIO109</code> to <code>ASYNC109</code></li>
<li><a href="https://docs.astral.sh/ruff/rules/trio-unneeded-sleep/"><code>trio-unneeded-sleep</code></a>: <code>TRIO110</code> to <code>ASYNC110</code></li>
<li><a href="https://docs.astral.sh/ruff/rules/trio-zero-sleep-call/"><code>trio-zero-sleep-call</code></a>: <code>TRIO115</code> to <code>ASYNC115</code></li>
<li><a href="https://docs.astral.sh/ruff/rules/repeated-isinstance-calls/"><code>repeated-isinstance-calls</code></a>: <code>PLR1701</code> to <code>SIM101</code></li>
</ul>
<h3>Stabilization</h3>
<p>The following rules have been stabilized and are no longer in preview:</p>
<ul>
<li><a href="https://docs.astral.sh/ruff/rules/mutable-fromkeys-value/"><code>mutable-fromkeys-value</code></a> (<code>RUF024</code>)</li>
<li><a href="https://docs.astral.sh/ruff/rules/default-factory-kwarg/"><code>default-factory-kwarg</code></a> (<code>RUF026</code>)</li>
<li><a href="https://docs.astral.sh/ruff/rules/django-extra/"><code>django-extra</code></a> (<code>S610</code>)</li>
<li><a href="https://docs.astral.sh/ruff/rules/manual-dict-comprehension/"><code>manual-dict-comprehension</code></a> (<code>PERF403</code>)</li>
<li><a href="https://docs.astral.sh/ruff/rules/print-empty-string/"><code>print-empty-string</code></a> (<code>FURB105</code>)</li>
<li><a href="https://docs.astral.sh/ruff/rules/readlines-in-for/"><code>readlines-in-for</code></a> (<code>FURB129</code>)</li>
<li><a href="https://docs.astral.sh/ruff/rules/if-expr-min-max/"><code>if-expr-min-max</code></a> (<code>FURB136</code>)</li>
<li><a href="https://docs.astral.sh/ruff/rules/bit-count/"><code>bit-count</code></a> (<code>FURB161</code>)</li>
<li><a href="https://docs.astral.sh/ruff/rules/redundant-log-base/"><code>redundant-log-base</code></a> (<code>FURB163</code>)</li>
<li><a href="https://docs.astral.sh/ruff/rules/regex-flag-alias/"><code>regex-flag-alias</code></a> (<code>FURB167</code>)</li>
<li><a href="https://docs.astral.sh/ruff/rules/isinstance-type-none/"><code>isinstance-type-none</code></a> (<code>FURB168</code>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
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
<h3>Deprecations</h3>
<p>The following rules are now deprecated:</p>
<ul>
<li><a href="https://docs.astral.sh/ruff/rules/syntax-error/"><code>syntax-error</code></a> (<code>E999</code>): Syntax errors are now always shown</li>
</ul>
<h3>Remapped rules</h3>
<p>The following rules have been remapped to new rule codes:</p>
<ul>
<li><a href="https://docs.astral.sh/ruff/rules/blocking-http-call-in-async-function/"><code>blocking-http-call-in-async-function</code></a>: <code>ASYNC100</code> to <code>ASYNC210</code></li>
<li><a href="https://docs.astral.sh/ruff/rules/open-sleep-or-subprocess-in-async-function/"><code>open-sleep-or-subprocess-in-async-function</code></a>: <code>ASYNC101</code> split into <code>ASYNC220</code>, <code>ASYNC221</code>, <code>ASYNC230</code>, and <code>ASYNC251</code></li>
<li><a href="https://docs.astral.sh/ruff/rules/blocking-os-call-in-async-function/"><code>blocking-os-call-in-async-function</code></a>: <code>ASYNC102</code> has been merged into <code>ASYNC220</code> and <code>ASYNC221</code></li>
<li><a href="https://docs.astral.sh/ruff/rules/trio-timeout-without-await/"><code>trio-timeout-without-await</code></a>: <code>TRIO100</code> to <code>ASYNC100</code></li>
<li><a href="https://docs.astral.sh/ruff/rules/trio-sync-call/"><code>trio-sync-call</code></a>: <code>TRIO105</code> to <code>ASYNC105</code></li>
<li><a href="https://docs.astral.sh/ruff/rules/trio-async-function-with-timeout/"><code>trio-async-function-with-timeout</code></a>: <code>TRIO109</code> to <code>ASYNC109</code></li>
<li><a href="https://docs.astral.sh/ruff/rules/trio-unneeded-sleep/"><code>trio-unneeded-sleep</code></a>: <code>TRIO110</code> to <code>ASYNC110</code></li>
<li><a href="https://docs.astral.sh/ruff/rules/trio-zero-sleep-call/"><code>trio-zero-sleep-call</code></a>: <code>TRIO115</code> to <code>ASYNC115</code></li>
<li><a href="https://docs.astral.sh/ruff/rules/repeated-isinstance-calls/"><code>repeated-isinstance-calls</code></a>: <code>PLR1701</code> to <code>SIM101</code></li>
</ul>
<h3>Stabilization</h3>
<p>The following rules have been stabilized and are no longer in preview:</p>
<ul>
<li><a href="https://docs.astral.sh/ruff/rules/mutable-fromkeys-value/"><code>mutable-fromkeys-value</code></a> (<code>RUF024</code>)</li>
<li><a href="https://docs.astral.sh/ruff/rules/default-factory-kwarg/"><code>default-factory-kwarg</code></a> (<code>RUF026</code>)</li>
<li><a href="https://docs.astral.sh/ruff/rules/django-extra/"><code>django-extra</code></a> (<code>S610</code>)</li>
<li><a href="https://docs.astral.sh/ruff/rules/manual-dict-comprehension/"><code>manual-dict-comprehension</code></a> (<code>PERF403</code>)</li>
<li><a href="https://docs.astral.sh/ruff/rules/print-empty-string/"><code>print-empty-string</code></a> (<code>FURB105</code>)</li>
<li><a href="https://docs.astral.sh/ruff/rules/readlines-in-for/"><code>readlines-in-for</code></a> (<code>FURB129</code>)</li>
<li><a href="https://docs.astral.sh/ruff/rules/if-expr-min-max/"><code>if-expr-min-max</code></a> (<code>FURB136</code>)</li>
<li><a href="https://docs.astral.sh/ruff/rules/bit-count/"><code>bit-count</code></a> (<code>FURB161</code>)</li>
<li><a href="https://docs.astral.sh/ruff/rules/redundant-log-base/"><code>redundant-log-base</code></a> (<code>FURB163</code>)</li>
<li><a href="https://docs.astral.sh/ruff/rules/regex-flag-alias/"><code>regex-flag-alias</code></a> (<code>FURB167</code>)</li>
<li><a href="https://docs.astral.sh/ruff/rules/isinstance-type-none/"><code>isinstance-type-none</code></a> (<code>FURB168</code>)</li>
<li><a href="https://docs.astral.sh/ruff/rules/type-none-comparison/"><code>type-none-comparison</code></a> (<code>FURB169</code>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/244b923f615c2c162278fc0e06051853614760f3"><code>244b923</code></a> Add necessary permissions for cargo-dist Docker build (<a href="https://redirect.github.com/astral-sh/ruff/issues/12072">#12072</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/a8b48fce7e32b35538072ccd55dac64e158d1e34"><code>a8b48fc</code></a> Release v0.5.0 (<a href="https://redirect.github.com/astral-sh/ruff/issues/12068">#12068</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/04c8597b8ab1a459d77058b6899571095092bc2d"><code>04c8597</code></a> [<code>flake8-simplify</code>] Stabilize detection of Yoda conditions for &quot;constant&quot; col...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4029a25ebd88a26424f45b20aba20c8e56a54d62"><code>4029a25</code></a> [Ruff v0.5] Stabilise 15 pylint rules (<a href="https://redirect.github.com/astral-sh/ruff/issues/12051">#12051</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/0917ce16f477f20b60d6d6f96462d4c83168f6f6"><code>0917ce1</code></a> Update documentation to mention <code>etcetera</code> crate instead of <code>dirs</code> for user c...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/22cebdf29b79c9bb39b341149b2764730de72d97"><code>22cebdf</code></a> Add server config to filter out syntax error diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/issues/12059">#12059</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/72b6c26101ca920137202d455b014f9e680712f7"><code>72b6c26</code></a> Simplify <code>LinterResult</code>, avoid cloning <code>ParseError</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11903">#11903</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/73851e73ab0629461fbec84ee35ea91948d0c474"><code>73851e7</code></a> Avoid displaying syntax error as log message (<a href="https://redirect.github.com/astral-sh/ruff/issues/11902">#11902</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e7b49694a795e3347ffc6f499245dfcbbb4b28ed"><code>e7b4969</code></a> Remove <code>E999</code> as a rule, disallow any disablement methods for syntax error (#...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c98d8a040fbcd3428f1b0189ebdc9fbb8183b215"><code>c98d8a0</code></a> [<code>pyflakes</code>] Stabilize detection of is comparisons to lists, etc. (<code>F632</code>) (#...</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.4.4...0.5.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.4.4&new-version=0.5.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-01 11:33:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-endorser-service/pull/110" class=".btn">#110</a>
            </td>
            <td>
                <b>
                    Bump pydantic-settings from 2.2.1 to 2.3.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pydantic-settings](https://github.com/pydantic/pydantic-settings) from 2.2.1 to 2.3.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pydantic/pydantic-settings/releases">pydantic-settings's releases</a>.</em></p>
<blockquote>
<h2>v2.3.4</h2>
<h2>What's Changed</h2>
<ul>
<li>add in-place reloading in docs by <a href="https://github.com/nrolin"><code>@​nrolin</code></a> in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/316">pydantic/pydantic-settings#316</a></li>
<li>Nested pydantic dataclasses and doc fixes. by <a href="https://github.com/kschwab"><code>@​kschwab</code></a> in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/317">pydantic/pydantic-settings#317</a></li>
<li>Remove leftover docstring causing warning on <code>pydantic</code> docs build by <a href="https://github.com/sydney-runkle"><code>@​sydney-runkle</code></a> in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/321">pydantic/pydantic-settings#321</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/nrolin"><code>@​nrolin</code></a> made their first contribution in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/316">pydantic/pydantic-settings#316</a></li>
<li><a href="https://github.com/sydney-runkle"><code>@​sydney-runkle</code></a> made their first contribution in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/321">pydantic/pydantic-settings#321</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pydantic/pydantic-settings/compare/v2.3.3...v2.3.4">https://github.com/pydantic/pydantic-settings/compare/v2.3.3...v2.3.4</a></p>
<h2>v2.3.3</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix an intriduced bug in parsing json field with discriminated union by <a href="https://github.com/hramezani"><code>@​hramezani</code></a> in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/312">pydantic/pydantic-settings#312</a></li>
<li>Add CliSettingsSource alias handling for AliasChoices and AliasPath. by <a href="https://github.com/kschwab"><code>@​kschwab</code></a> in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/313">pydantic/pydantic-settings#313</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pydantic/pydantic-settings/compare/v2.3.2...v2.3.3">https://github.com/pydantic/pydantic-settings/compare/v2.3.2...v2.3.3</a></p>
<h2>v2.3.2</h2>
<h2>What's Changed</h2>
<ul>
<li>Initialize CLI source on demand. by <a href="https://github.com/kschwab"><code>@​kschwab</code></a> in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/305">pydantic/pydantic-settings#305</a></li>
<li>Fix command line help from <code>argparse</code> formatting problem by <a href="https://github.com/scottstanie"><code>@​scottstanie</code></a> in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/307">pydantic/pydantic-settings#307</a></li>
<li>Fix issue with nested model uppercase field name in case insensitive mode by <a href="https://github.com/hramezani"><code>@​hramezani</code></a> in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/309">pydantic/pydantic-settings#309</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/scottstanie"><code>@​scottstanie</code></a> made their first contribution in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/307">pydantic/pydantic-settings#307</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pydantic/pydantic-settings/compare/v2.3.1...v2.3.2">https://github.com/pydantic/pydantic-settings/compare/v2.3.1...v2.3.2</a></p>
<h2>v2.3.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix a regression in parsing env value for nested dict by <a href="https://github.com/hramezani"><code>@​hramezani</code></a> in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/301">pydantic/pydantic-settings#301</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pydantic/pydantic-settings/compare/v2.3.0...v2.3.1">https://github.com/pydantic/pydantic-settings/compare/v2.3.0...v2.3.1</a></p>
<h2>v2.3.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Add environment parsing support for enums. by <a href="https://github.com/kschwab"><code>@​kschwab</code></a> in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/252">pydantic/pydantic-settings#252</a></li>
<li>Improve <code>explode_env_vars</code> for better dict handling by <a href="https://github.com/hramezani"><code>@​hramezani</code></a> in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/261">pydantic/pydantic-settings#261</a></li>
<li>add <code>PyprojectTomlConfigSettingsSource</code> by <a href="https://github.com/ITProKyle"><code>@​ITProKyle</code></a> in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/255">pydantic/pydantic-settings#255</a></li>
<li>Fix broken link in AliasChoices class by <a href="https://github.com/keenranger"><code>@​keenranger</code></a> in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/271">pydantic/pydantic-settings#271</a></li>
<li>Update Pydantic by <a href="https://github.com/hramezani"><code>@​hramezani</code></a> in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/273">pydantic/pydantic-settings#273</a></li>
<li>fix: superfluous deep env conflicts with non-dict model leaf by <a href="https://github.com/diefans"><code>@​diefans</code></a> in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/276">pydantic/pydantic-settings#276</a></li>
<li>fix: a second level of environment nesting expected a dict by <a href="https://github.com/diefans"><code>@​diefans</code></a> in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/281">pydantic/pydantic-settings#281</a></li>
<li>Fix an issue when inner types of a discriminated union with a callable discriminator were not correctly identified as complex. by <a href="https://github.com/jenskeiner"><code>@​jenskeiner</code></a> in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/285">pydantic/pydantic-settings#285</a></li>
<li>Fix a bug when we have case insentive field in nested model by <a href="https://github.com/hramezani"><code>@​hramezani</code></a> in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/294">pydantic/pydantic-settings#294</a></li>
<li>Add CLI Settings Source by <a href="https://github.com/kschwab"><code>@​kschwab</code></a> in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/214">pydantic/pydantic-settings#214</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pydantic/pydantic-settings/commit/fe1f9509da2a1951167666b92fa2083ff2ea35bf"><code>fe1f950</code></a> Prepare release 2.3.4 (<a href="https://redirect.github.com/pydantic/pydantic-settings/issues/322">#322</a>)</li>
<li><a href="https://github.com/pydantic/pydantic-settings/commit/674ebd9cbeb5b9535bcfc5cdabbbe69518b10c52"><code>674ebd9</code></a> Remove leftover docstring causing warning on <code>pydantic</code> docs build (<a href="https://redirect.github.com/pydantic/pydantic-settings/issues/321">#321</a>)</li>
<li><a href="https://github.com/pydantic/pydantic-settings/commit/7ede0ec18c5678dfa1212e6e8d6d7c6489ac7d78"><code>7ede0ec</code></a> Nested pydantic dataclasses and doc fixes. (<a href="https://redirect.github.com/pydantic/pydantic-settings/issues/317">#317</a>)</li>
<li><a href="https://github.com/pydantic/pydantic-settings/commit/c2d44a7723a00f75ba6790cc654aaa507a7ab123"><code>c2d44a7</code></a> add in-place reloading in docs (<a href="https://redirect.github.com/pydantic/pydantic-settings/issues/316">#316</a>)</li>
<li><a href="https://github.com/pydantic/pydantic-settings/commit/f1b82d834abfed0aa2c263d88bc017c0ea1530af"><code>f1b82d8</code></a> Prepare release 2.3.3 (<a href="https://redirect.github.com/pydantic/pydantic-settings/issues/314">#314</a>)</li>
<li><a href="https://github.com/pydantic/pydantic-settings/commit/bd294a4b1ed49357446a38765af302d14b94bcc6"><code>bd294a4</code></a> Add CliSettingsSource alias handling for AliasChoices and AliasPath. (<a href="https://redirect.github.com/pydantic/pydantic-settings/issues/313">#313</a>)</li>
<li><a href="https://github.com/pydantic/pydantic-settings/commit/abe7cc5e3268a9093def94917bc581c31ba74f20"><code>abe7cc5</code></a> Fix an intriduced bug in parsing json field with discriminated union (<a href="https://redirect.github.com/pydantic/pydantic-settings/issues/312">#312</a>)</li>
<li><a href="https://github.com/pydantic/pydantic-settings/commit/b5d4534cdcddb1bb99258d88a0e6d1f16e6788f4"><code>b5d4534</code></a> Prepare release 2.3.2 (<a href="https://redirect.github.com/pydantic/pydantic-settings/issues/310">#310</a>)</li>
<li><a href="https://github.com/pydantic/pydantic-settings/commit/b2e84c2729d73ee2f1ab7962398003d933c5227a"><code>b2e84c2</code></a> Fix issue with nested model uppercase field name in case insensitive mode (<a href="https://redirect.github.com/pydantic/pydantic-settings/issues/309">#309</a>)</li>
<li><a href="https://github.com/pydantic/pydantic-settings/commit/0a9faca91e9503afbcb8fdd652114f9f69ba13b0"><code>0a9faca</code></a> Fix command line help from <code>argparse</code> formatting problem (<a href="https://redirect.github.com/pydantic/pydantic-settings/issues/307">#307</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pydantic/pydantic-settings/compare/v2.2.1...v2.3.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pydantic-settings&package-manager=pip&previous-version=2.2.1&new-version=2.3.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-01 11:32:57 +0000 UTC
    </div>
</div>

