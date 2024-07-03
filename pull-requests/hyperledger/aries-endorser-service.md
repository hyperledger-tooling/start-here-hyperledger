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

