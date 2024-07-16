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
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/749" class=".btn">#749</a>
            </td>
            <td>
                <b>
                    Bump pytest-ruff from 0.3.2 to 0.4.0 in /rpc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-ruff](https://github.com/businho/pytest-ruff) from 0.3.2 to 0.4.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/businho/pytest-ruff/releases">pytest-ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Replace <code>--show-source</code> with <code>--output-format</code> by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/24">businho/pytest-ruff#24</a></li>
<li>Handle ruff config error by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/25">businho/pytest-ruff#25</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.0">https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/businho/pytest-ruff/commit/759cacd7cae8decaec4ff8b7c9aa4e447ba5a9c5"><code>759cacd</code></a> Handle ruff config error (<a href="https://redirect.github.com/businho/pytest-ruff/issues/25">#25</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/fd4c1e9ff2097f0b822d62978432e88adb4ffab5"><code>fd4c1e9</code></a> Replace <code>--show-source</code> with <code>--output-format</code> (<a href="https://redirect.github.com/businho/pytest-ruff/issues/24">#24</a>)</li>
<li>See full diff in <a href="https://github.com/businho/pytest-ruff/compare/v0.3.2...v0.4.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-ruff&package-manager=pip&previous-version=0.3.2&new-version=0.4.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-15 11:14:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/748" class=".btn">#748</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.5.1 to 0.5.2 in /plugin_globals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.5.1 to 0.5.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>0.5.2</h2>
<h2>Release Notes</h2>
<h3>Preview features</h3>
<ul>
<li>Use <code>space</code> separator before parenthesized expressions in comprehensions with leading comments (<a href="https://redirect.github.com/astral-sh/ruff/pull/12282">#12282</a>)</li>
<li>[<code>flake8-async</code>] Update <code>ASYNC100</code> to include <code>anyio</code> and <code>asyncio</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12221">#12221</a>)</li>
<li>[<code>flake8-async</code>] Update <code>ASYNC109</code> to include <code>anyio</code> and <code>asyncio</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12236">#12236</a>)</li>
<li>[<code>flake8-async</code>] Update <code>ASYNC110</code> to include <code>anyio</code> and <code>asyncio</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12261">#12261</a>)</li>
<li>[<code>flake8-async</code>] Update <code>ASYNC115</code> to include <code>anyio</code> and <code>asyncio</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12262">#12262</a>)</li>
<li>[<code>flake8-async</code>] Update <code>ASYNC116</code> to include <code>anyio</code> and <code>asyncio</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12266">#12266</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-return</code>] Exempt properties from explicit return rule (<code>RET501</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12243">#12243</a>)</li>
<li>[<code>numpy</code>] Add <code>np.NAN</code>-to-<code>np.nan</code> diagnostic (<a href="https://redirect.github.com/astral-sh/ruff/pull/12292">#12292</a>)</li>
<li>[<code>refurb</code>] Make <code>list-reverse-copy</code> an unsafe fix (<a href="https://redirect.github.com/astral-sh/ruff/pull/12303">#12303</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Consider <code>include</code> and <code>extend-include</code> settings in native server (<a href="https://redirect.github.com/astral-sh/ruff/pull/12252">#12252</a>)</li>
<li>Include nested configurations in settings reloading (<a href="https://redirect.github.com/astral-sh/ruff/pull/12253">#12253</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Omit code frames for fixes with empty ranges (<a href="https://redirect.github.com/astral-sh/ruff/pull/12304">#12304</a>)</li>
<li>Warn about formatter incompatibility for <code>D203</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12238">#12238</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Make cache-write failures non-fatal on Windows (<a href="https://redirect.github.com/astral-sh/ruff/pull/12302">#12302</a>)</li>
<li>Treat <code>not</code> operations as boolean tests (<a href="https://redirect.github.com/astral-sh/ruff/pull/12301">#12301</a>)</li>
<li>[<code>flake8-bandit</code>] Avoid <code>S310</code> violations for HTTP-safe f-strings (<a href="https://redirect.github.com/astral-sh/ruff/pull/12305">#12305</a>)</li>
<li>[<code>flake8-bandit</code>] Support explicit string concatenations in S310 HTTP detection (<a href="https://redirect.github.com/astral-sh/ruff/pull/12315">#12315</a>)</li>
<li>[<code>flake8-bandit</code>] fix S113 false positive for httpx without <code>timeout</code> argument (<a href="https://redirect.github.com/astral-sh/ruff/pull/12213">#12213</a>)</li>
<li>[<code>pycodestyle</code>] Remove &quot;non-obvious&quot; allowance for E721 (<a href="https://redirect.github.com/astral-sh/ruff/pull/12300">#12300</a>)</li>
<li>[<code>pyflakes</code>] Consider <code>with</code> blocks as single-item branches for redefinition analysis (<a href="https://redirect.github.com/astral-sh/ruff/pull/12311">#12311</a>)</li>
<li>[<code>refurb</code>] Restrict forwarding for <code>newline</code> argument in <code>open()</code> calls to Python versions &gt;= 3.10 (<a href="https://redirect.github.com/astral-sh/ruff/pull/12244">#12244</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Update help and documentation to reflect <code>--output-format full</code> default (<a href="https://redirect.github.com/astral-sh/ruff/pull/12248">#12248</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Use more threads when discovering Python files (<a href="https://redirect.github.com/astral-sh/ruff/pull/12258">#12258</a>)</li>
</ul>
<h2>Install ruff 0.5.2</h2>
<h3>Install prebuilt binaries via shell script</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.5.2</h2>
<h3>Preview features</h3>
<ul>
<li>Use <code>space</code> separator before parenthesized expressions in comprehensions with leading comments (<a href="https://redirect.github.com/astral-sh/ruff/pull/12282">#12282</a>)</li>
<li>[<code>flake8-async</code>] Update <code>ASYNC100</code> to include <code>anyio</code> and <code>asyncio</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12221">#12221</a>)</li>
<li>[<code>flake8-async</code>] Update <code>ASYNC109</code> to include <code>anyio</code> and <code>asyncio</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12236">#12236</a>)</li>
<li>[<code>flake8-async</code>] Update <code>ASYNC110</code> to include <code>anyio</code> and <code>asyncio</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12261">#12261</a>)</li>
<li>[<code>flake8-async</code>] Update <code>ASYNC115</code> to include <code>anyio</code> and <code>asyncio</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12262">#12262</a>)</li>
<li>[<code>flake8-async</code>] Update <code>ASYNC116</code> to include <code>anyio</code> and <code>asyncio</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12266">#12266</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-return</code>] Exempt properties from explicit return rule (<code>RET501</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12243">#12243</a>)</li>
<li>[<code>numpy</code>] Add <code>np.NAN</code>-to-<code>np.nan</code> diagnostic (<a href="https://redirect.github.com/astral-sh/ruff/pull/12292">#12292</a>)</li>
<li>[<code>refurb</code>] Make <code>list-reverse-copy</code> an unsafe fix (<a href="https://redirect.github.com/astral-sh/ruff/pull/12303">#12303</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Consider <code>include</code> and <code>extend-include</code> settings in native server (<a href="https://redirect.github.com/astral-sh/ruff/pull/12252">#12252</a>)</li>
<li>Include nested configurations in settings reloading (<a href="https://redirect.github.com/astral-sh/ruff/pull/12253">#12253</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Omit code frames for fixes with empty ranges (<a href="https://redirect.github.com/astral-sh/ruff/pull/12304">#12304</a>)</li>
<li>Warn about formatter incompatibility for <code>D203</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12238">#12238</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Make cache-write failures non-fatal on Windows (<a href="https://redirect.github.com/astral-sh/ruff/pull/12302">#12302</a>)</li>
<li>Treat <code>not</code> operations as boolean tests (<a href="https://redirect.github.com/astral-sh/ruff/pull/12301">#12301</a>)</li>
<li>[<code>flake8-bandit</code>] Avoid <code>S310</code> violations for HTTP-safe f-strings (<a href="https://redirect.github.com/astral-sh/ruff/pull/12305">#12305</a>)</li>
<li>[<code>flake8-bandit</code>] Support explicit string concatenations in S310 HTTP detection (<a href="https://redirect.github.com/astral-sh/ruff/pull/12315">#12315</a>)</li>
<li>[<code>flake8-bandit</code>] fix S113 false positive for httpx without <code>timeout</code> argument (<a href="https://redirect.github.com/astral-sh/ruff/pull/12213">#12213</a>)</li>
<li>[<code>pycodestyle</code>] Remove &quot;non-obvious&quot; allowance for E721 (<a href="https://redirect.github.com/astral-sh/ruff/pull/12300">#12300</a>)</li>
<li>[<code>pyflakes</code>] Consider <code>with</code> blocks as single-item branches for redefinition analysis (<a href="https://redirect.github.com/astral-sh/ruff/pull/12311">#12311</a>)</li>
<li>[<code>refurb</code>] Restrict forwarding for <code>newline</code> argument in <code>open()</code> calls to Python versions &gt;= 3.10 (<a href="https://redirect.github.com/astral-sh/ruff/pull/12244">#12244</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Update help and documentation to reflect <code>--output-format full</code> default (<a href="https://redirect.github.com/astral-sh/ruff/pull/12248">#12248</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Use more threads when discovering Python files (<a href="https://redirect.github.com/astral-sh/ruff/pull/12258">#12258</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/dc8db1afb08704ad6a788c497068b01edf8b460d"><code>dc8db1a</code></a> Make some amendments to the v0.5.2 changelog (<a href="https://redirect.github.com/astral-sh/ruff/issues/12319">#12319</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/18c364d5df7701cb3a09bc4a41df8954f37b2a5d"><code>18c364d</code></a> [<code>flake8-bandit</code>] Support explicit string concatenations in S310 HTTP detecti...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/7a7c601d5ed294a3c868b5e83f757105e0a189b8"><code>7a7c601</code></a> Bump version to v0.5.2 (<a href="https://redirect.github.com/astral-sh/ruff/issues/12316">#12316</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/3bfbbbc78c24d9fed4b25e7f6ede7f68b35fb8fd"><code>3bfbbbc</code></a> Avoid allocation when validating HTTP and HTTPS prefixes (<a href="https://redirect.github.com/astral-sh/ruff/issues/12313">#12313</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1a3ee45b236d93632289544ed54001d048064fbf"><code>1a3ee45</code></a> [<code>flake8-bandit</code>] Avoid <code>S310</code> violations for HTTP-safe f-strings (<a href="https://redirect.github.com/astral-sh/ruff/issues/12305">#12305</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/65848869d58aeeb12e1c77c4fc73ad0b4b941368"><code>6584886</code></a> [<code>refurb</code>] Make <code>list-reverse-copy</code> an unsafe fix (<a href="https://redirect.github.com/astral-sh/ruff/issues/12303">#12303</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/456d6a2fb201c697b18aa3d4a48f82c132548c19"><code>456d6a2</code></a> Consider <code>with</code> blocks as single-item branches (<a href="https://redirect.github.com/astral-sh/ruff/issues/12311">#12311</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/940df67823dc5237f95d36a94ef3a74dc4bd36fb"><code>940df67</code></a> Omit code frames for fixes with empty ranges (<a href="https://redirect.github.com/astral-sh/ruff/issues/12304">#12304</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e58713e2ac87a1203969dde29bf4f5509099acbd"><code>e58713e</code></a> Make cache-write failures non-fatal (<a href="https://redirect.github.com/astral-sh/ruff/issues/12302">#12302</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/aa5c53b38b23a55780b5ccd00c8cea6e527b0ada"><code>aa5c53b</code></a> Remove 'non-obvious' allowance for E721 (<a href="https://redirect.github.com/astral-sh/ruff/issues/12300">#12300</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/0.5.1...0.5.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.5.1&new-version=0.5.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-15 11:12:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/747" class=".btn">#747</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.5.1 to 0.5.2 in /kafka_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.5.1 to 0.5.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>0.5.2</h2>
<h2>Release Notes</h2>
<h3>Preview features</h3>
<ul>
<li>Use <code>space</code> separator before parenthesized expressions in comprehensions with leading comments (<a href="https://redirect.github.com/astral-sh/ruff/pull/12282">#12282</a>)</li>
<li>[<code>flake8-async</code>] Update <code>ASYNC100</code> to include <code>anyio</code> and <code>asyncio</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12221">#12221</a>)</li>
<li>[<code>flake8-async</code>] Update <code>ASYNC109</code> to include <code>anyio</code> and <code>asyncio</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12236">#12236</a>)</li>
<li>[<code>flake8-async</code>] Update <code>ASYNC110</code> to include <code>anyio</code> and <code>asyncio</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12261">#12261</a>)</li>
<li>[<code>flake8-async</code>] Update <code>ASYNC115</code> to include <code>anyio</code> and <code>asyncio</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12262">#12262</a>)</li>
<li>[<code>flake8-async</code>] Update <code>ASYNC116</code> to include <code>anyio</code> and <code>asyncio</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12266">#12266</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-return</code>] Exempt properties from explicit return rule (<code>RET501</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12243">#12243</a>)</li>
<li>[<code>numpy</code>] Add <code>np.NAN</code>-to-<code>np.nan</code> diagnostic (<a href="https://redirect.github.com/astral-sh/ruff/pull/12292">#12292</a>)</li>
<li>[<code>refurb</code>] Make <code>list-reverse-copy</code> an unsafe fix (<a href="https://redirect.github.com/astral-sh/ruff/pull/12303">#12303</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Consider <code>include</code> and <code>extend-include</code> settings in native server (<a href="https://redirect.github.com/astral-sh/ruff/pull/12252">#12252</a>)</li>
<li>Include nested configurations in settings reloading (<a href="https://redirect.github.com/astral-sh/ruff/pull/12253">#12253</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Omit code frames for fixes with empty ranges (<a href="https://redirect.github.com/astral-sh/ruff/pull/12304">#12304</a>)</li>
<li>Warn about formatter incompatibility for <code>D203</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12238">#12238</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Make cache-write failures non-fatal on Windows (<a href="https://redirect.github.com/astral-sh/ruff/pull/12302">#12302</a>)</li>
<li>Treat <code>not</code> operations as boolean tests (<a href="https://redirect.github.com/astral-sh/ruff/pull/12301">#12301</a>)</li>
<li>[<code>flake8-bandit</code>] Avoid <code>S310</code> violations for HTTP-safe f-strings (<a href="https://redirect.github.com/astral-sh/ruff/pull/12305">#12305</a>)</li>
<li>[<code>flake8-bandit</code>] Support explicit string concatenations in S310 HTTP detection (<a href="https://redirect.github.com/astral-sh/ruff/pull/12315">#12315</a>)</li>
<li>[<code>flake8-bandit</code>] fix S113 false positive for httpx without <code>timeout</code> argument (<a href="https://redirect.github.com/astral-sh/ruff/pull/12213">#12213</a>)</li>
<li>[<code>pycodestyle</code>] Remove &quot;non-obvious&quot; allowance for E721 (<a href="https://redirect.github.com/astral-sh/ruff/pull/12300">#12300</a>)</li>
<li>[<code>pyflakes</code>] Consider <code>with</code> blocks as single-item branches for redefinition analysis (<a href="https://redirect.github.com/astral-sh/ruff/pull/12311">#12311</a>)</li>
<li>[<code>refurb</code>] Restrict forwarding for <code>newline</code> argument in <code>open()</code> calls to Python versions &gt;= 3.10 (<a href="https://redirect.github.com/astral-sh/ruff/pull/12244">#12244</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Update help and documentation to reflect <code>--output-format full</code> default (<a href="https://redirect.github.com/astral-sh/ruff/pull/12248">#12248</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Use more threads when discovering Python files (<a href="https://redirect.github.com/astral-sh/ruff/pull/12258">#12258</a>)</li>
</ul>
<h2>Install ruff 0.5.2</h2>
<h3>Install prebuilt binaries via shell script</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.5.2</h2>
<h3>Preview features</h3>
<ul>
<li>Use <code>space</code> separator before parenthesized expressions in comprehensions with leading comments (<a href="https://redirect.github.com/astral-sh/ruff/pull/12282">#12282</a>)</li>
<li>[<code>flake8-async</code>] Update <code>ASYNC100</code> to include <code>anyio</code> and <code>asyncio</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12221">#12221</a>)</li>
<li>[<code>flake8-async</code>] Update <code>ASYNC109</code> to include <code>anyio</code> and <code>asyncio</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12236">#12236</a>)</li>
<li>[<code>flake8-async</code>] Update <code>ASYNC110</code> to include <code>anyio</code> and <code>asyncio</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12261">#12261</a>)</li>
<li>[<code>flake8-async</code>] Update <code>ASYNC115</code> to include <code>anyio</code> and <code>asyncio</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12262">#12262</a>)</li>
<li>[<code>flake8-async</code>] Update <code>ASYNC116</code> to include <code>anyio</code> and <code>asyncio</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12266">#12266</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-return</code>] Exempt properties from explicit return rule (<code>RET501</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12243">#12243</a>)</li>
<li>[<code>numpy</code>] Add <code>np.NAN</code>-to-<code>np.nan</code> diagnostic (<a href="https://redirect.github.com/astral-sh/ruff/pull/12292">#12292</a>)</li>
<li>[<code>refurb</code>] Make <code>list-reverse-copy</code> an unsafe fix (<a href="https://redirect.github.com/astral-sh/ruff/pull/12303">#12303</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Consider <code>include</code> and <code>extend-include</code> settings in native server (<a href="https://redirect.github.com/astral-sh/ruff/pull/12252">#12252</a>)</li>
<li>Include nested configurations in settings reloading (<a href="https://redirect.github.com/astral-sh/ruff/pull/12253">#12253</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Omit code frames for fixes with empty ranges (<a href="https://redirect.github.com/astral-sh/ruff/pull/12304">#12304</a>)</li>
<li>Warn about formatter incompatibility for <code>D203</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12238">#12238</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Make cache-write failures non-fatal on Windows (<a href="https://redirect.github.com/astral-sh/ruff/pull/12302">#12302</a>)</li>
<li>Treat <code>not</code> operations as boolean tests (<a href="https://redirect.github.com/astral-sh/ruff/pull/12301">#12301</a>)</li>
<li>[<code>flake8-bandit</code>] Avoid <code>S310</code> violations for HTTP-safe f-strings (<a href="https://redirect.github.com/astral-sh/ruff/pull/12305">#12305</a>)</li>
<li>[<code>flake8-bandit</code>] Support explicit string concatenations in S310 HTTP detection (<a href="https://redirect.github.com/astral-sh/ruff/pull/12315">#12315</a>)</li>
<li>[<code>flake8-bandit</code>] fix S113 false positive for httpx without <code>timeout</code> argument (<a href="https://redirect.github.com/astral-sh/ruff/pull/12213">#12213</a>)</li>
<li>[<code>pycodestyle</code>] Remove &quot;non-obvious&quot; allowance for E721 (<a href="https://redirect.github.com/astral-sh/ruff/pull/12300">#12300</a>)</li>
<li>[<code>pyflakes</code>] Consider <code>with</code> blocks as single-item branches for redefinition analysis (<a href="https://redirect.github.com/astral-sh/ruff/pull/12311">#12311</a>)</li>
<li>[<code>refurb</code>] Restrict forwarding for <code>newline</code> argument in <code>open()</code> calls to Python versions &gt;= 3.10 (<a href="https://redirect.github.com/astral-sh/ruff/pull/12244">#12244</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Update help and documentation to reflect <code>--output-format full</code> default (<a href="https://redirect.github.com/astral-sh/ruff/pull/12248">#12248</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Use more threads when discovering Python files (<a href="https://redirect.github.com/astral-sh/ruff/pull/12258">#12258</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/dc8db1afb08704ad6a788c497068b01edf8b460d"><code>dc8db1a</code></a> Make some amendments to the v0.5.2 changelog (<a href="https://redirect.github.com/astral-sh/ruff/issues/12319">#12319</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/18c364d5df7701cb3a09bc4a41df8954f37b2a5d"><code>18c364d</code></a> [<code>flake8-bandit</code>] Support explicit string concatenations in S310 HTTP detecti...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/7a7c601d5ed294a3c868b5e83f757105e0a189b8"><code>7a7c601</code></a> Bump version to v0.5.2 (<a href="https://redirect.github.com/astral-sh/ruff/issues/12316">#12316</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/3bfbbbc78c24d9fed4b25e7f6ede7f68b35fb8fd"><code>3bfbbbc</code></a> Avoid allocation when validating HTTP and HTTPS prefixes (<a href="https://redirect.github.com/astral-sh/ruff/issues/12313">#12313</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1a3ee45b236d93632289544ed54001d048064fbf"><code>1a3ee45</code></a> [<code>flake8-bandit</code>] Avoid <code>S310</code> violations for HTTP-safe f-strings (<a href="https://redirect.github.com/astral-sh/ruff/issues/12305">#12305</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/65848869d58aeeb12e1c77c4fc73ad0b4b941368"><code>6584886</code></a> [<code>refurb</code>] Make <code>list-reverse-copy</code> an unsafe fix (<a href="https://redirect.github.com/astral-sh/ruff/issues/12303">#12303</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/456d6a2fb201c697b18aa3d4a48f82c132548c19"><code>456d6a2</code></a> Consider <code>with</code> blocks as single-item branches (<a href="https://redirect.github.com/astral-sh/ruff/issues/12311">#12311</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/940df67823dc5237f95d36a94ef3a74dc4bd36fb"><code>940df67</code></a> Omit code frames for fixes with empty ranges (<a href="https://redirect.github.com/astral-sh/ruff/issues/12304">#12304</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/e58713e2ac87a1203969dde29bf4f5509099acbd"><code>e58713e</code></a> Make cache-write failures non-fatal (<a href="https://redirect.github.com/astral-sh/ruff/issues/12302">#12302</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/aa5c53b38b23a55780b5ccd00c8cea6e527b0ada"><code>aa5c53b</code></a> Remove 'non-obvious' allowance for E721 (<a href="https://redirect.github.com/astral-sh/ruff/issues/12300">#12300</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/0.5.1...0.5.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.5.1&new-version=0.5.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-15 11:07:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/745" class=".btn">#745</a>
            </td>
            <td>
                <b>
                    Bump zipp from 3.18.2 to 3.19.1 in /connection_update in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /connection_update with 1 update: [zipp](https://github.com/jaraco/zipp).

Updates `zipp` from 3.18.2 to 3.19.1
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
</blockquote>
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
<li>Additional commits viewable in <a href="https://github.com/jaraco/zipp/compare/v3.18.2...v3.19.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=zipp&package-manager=pip&previous-version=3.18.2&new-version=3.19.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-09 19:29:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/744" class=".btn">#744</a>
            </td>
            <td>
                <b>
                    Bump zipp from 3.18.2 to 3.19.1 in /kafka_events in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /kafka_events with 1 update: [zipp](https://github.com/jaraco/zipp).

Updates `zipp` from 3.18.2 to 3.19.1
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
</blockquote>
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
<li>Additional commits viewable in <a href="https://github.com/jaraco/zipp/compare/v3.18.2...v3.19.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=zipp&package-manager=pip&previous-version=3.18.2&new-version=3.19.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-09 19:29:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/743" class=".btn">#743</a>
            </td>
            <td>
                <b>
                    Bump zipp from 3.18.2 to 3.19.1 in /basicmessage_storage in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /basicmessage_storage with 1 update: [zipp](https://github.com/jaraco/zipp).

Updates `zipp` from 3.18.2 to 3.19.1
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
</blockquote>
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
<li>Additional commits viewable in <a href="https://github.com/jaraco/zipp/compare/v3.18.2...v3.19.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=zipp&package-manager=pip&previous-version=3.18.2&new-version=3.19.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-09 19:28:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/742" class=".btn">#742</a>
            </td>
            <td>
                <b>
                    Bump zipp from 3.18.2 to 3.19.1 in /rpc in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /rpc with 1 update: [zipp](https://github.com/jaraco/zipp).

Updates `zipp` from 3.18.2 to 3.19.1
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
</blockquote>
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
<li>Additional commits viewable in <a href="https://github.com/jaraco/zipp/compare/v3.18.2...v3.19.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=zipp&package-manager=pip&previous-version=3.18.2&new-version=3.19.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-09 19:28:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/741" class=".btn">#741</a>
            </td>
            <td>
                <b>
                    Bump zipp from 3.18.2 to 3.19.1 in /multitenant_provider in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /multitenant_provider with 1 update: [zipp](https://github.com/jaraco/zipp).

Updates `zipp` from 3.18.2 to 3.19.1
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
</blockquote>
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
<li>Additional commits viewable in <a href="https://github.com/jaraco/zipp/compare/v3.18.2...v3.19.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=zipp&package-manager=pip&previous-version=3.18.2&new-version=3.19.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-09 19:28:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/739" class=".btn">#739</a>
            </td>
            <td>
                <b>
                    Bump zipp from 3.18.2 to 3.19.1 in /redis_events in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /redis_events with 1 update: [zipp](https://github.com/jaraco/zipp).

Updates `zipp` from 3.18.2 to 3.19.1
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
</blockquote>
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
<li>Additional commits viewable in <a href="https://github.com/jaraco/zipp/compare/v3.18.2...v3.19.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=zipp&package-manager=pip&previous-version=3.18.2&new-version=3.19.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-09 19:27:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/738" class=".btn">#738</a>
            </td>
            <td>
                <b>
                    Bump zipp from 3.18.2 to 3.19.1 in /redis_events/integration in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /redis_events/integration with 1 update: [zipp](https://github.com/jaraco/zipp).

Updates `zipp` from 3.18.2 to 3.19.1
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
</blockquote>
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
<li>Additional commits viewable in <a href="https://github.com/jaraco/zipp/compare/v3.18.2...v3.19.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=zipp&package-manager=pip&previous-version=3.18.2&new-version=3.19.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-09 19:27:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/737" class=".btn">#737</a>
            </td>
            <td>
                <b>
                    Bump zipp from 3.18.2 to 3.19.1 in /firebase_push_notifications in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /firebase_push_notifications with 1 update: [zipp](https://github.com/jaraco/zipp).

Updates `zipp` from 3.18.2 to 3.19.1
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
</blockquote>
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
<li>Additional commits viewable in <a href="https://github.com/jaraco/zipp/compare/v3.18.2...v3.19.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=zipp&package-manager=pip&previous-version=3.18.2&new-version=3.19.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-09 19:27:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/736" class=".btn">#736</a>
            </td>
            <td>
                <b>
                    Bump zipp from 3.18.2 to 3.19.1 in /plugin_globals in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /plugin_globals with 1 update: [zipp](https://github.com/jaraco/zipp).

Updates `zipp` from 3.18.2 to 3.19.1
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
</blockquote>
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
<li>Additional commits viewable in <a href="https://github.com/jaraco/zipp/compare/v3.18.2...v3.19.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=zipp&package-manager=pip&previous-version=3.18.2&new-version=3.19.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-09 19:26:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/735" class=".btn">#735</a>
            </td>
            <td>
                <b>
                    Bump zipp from 3.18.2 to 3.19.1 in /connection_update/integration in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group in /connection_update/integration with 1 update: [zipp](https://github.com/jaraco/zipp).

Updates `zipp` from 3.18.2 to 3.19.1
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
</blockquote>
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
<li>Additional commits viewable in <a href="https://github.com/jaraco/zipp/compare/v3.18.2...v3.19.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=zipp&package-manager=pip&previous-version=3.18.2&new-version=3.19.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-09 19:26:34 +0000 UTC
    </div>
</div>

