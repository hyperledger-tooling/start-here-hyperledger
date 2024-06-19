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
                PR <a href="https://github.com/hyperledger/aries-endorser-service/pull/108" class=".btn">#108</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.4.4 to 0.4.9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.4.4 to 0.4.9.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.9</h2>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>consider-dict-items</code> (<code>C0206</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11688">#11688</a>)</li>
<li>[<code>refurb</code>] Implement <code>repeated-global</code> (<code>FURB154</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11187">#11187</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pycodestyle</code>] Adapt fix for <code>E203</code> to work identical to <code>ruff format</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10999">#10999</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix formatter instability for lines only consisting of zero-width characters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11748">#11748</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/pull/11850">#11850</a>)</li>
<li>Use real file path when available in <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11800">#11800</a>)</li>
<li>Improve error message when a command is run on an unavailable document (<a href="https://redirect.github.com/astral-sh/ruff/pull/11823">#11823</a>)</li>
<li>Introduce the <code>ruff.printDebugInformation</code> command (<a href="https://redirect.github.com/astral-sh/ruff/pull/11831">#11831</a>)</li>
<li>Tracing system now respects log level and trace level, with options to log to a file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11747">#11747</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Handle non-printable characters in diff view (<a href="https://redirect.github.com/astral-sh/ruff/pull/11687">#11687</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>refurb</code>] Avoid suggesting starmap when arguments are used outside call (<code>FURB140</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11830">#11830</a>)</li>
<li>[<code>flake8-bugbear</code>] Avoid panic in <code>B909</code> when checking large loop blocks (<a href="https://redirect.github.com/astral-sh/ruff/pull/11772">#11772</a>)</li>
<li>[<code>refurb</code>] Fix misbehavior of <code>operator.itemgetter</code> when getter param is a tuple (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11774">#11774</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/Embers-of-the-Fire"><code>@​Embers-of-the-Fire</code></a></li>
<li><a href="https://github.com/LukasMasuch"><code>@​LukasMasuch</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/Peiffap"><code>@​Peiffap</code></a></li>
<li><a href="https://github.com/Philipp-Thiel"><code>@​Philipp-Thiel</code></a></li>
<li><a href="https://github.com/alex-700"><code>@​alex-700</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/max-muoto"><code>@​max-muoto</code></a></li>
<li><a href="https://github.com/pilleye"><code>@​pilleye</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
<li><a href="https://github.com/snowsignal"><code>@​snowsignal</code></a></li>
<li><a href="https://github.com/starsep"><code>@​starsep</code></a></li>
<li><a href="https://github.com/yairp03"><code>@​yairp03</code></a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.4.9</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pylint</code>] Implement <code>consider-dict-items</code> (<code>C0206</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11688">#11688</a>)</li>
<li>[<code>refurb</code>] Implement <code>repeated-global</code> (<code>FURB154</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11187">#11187</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pycodestyle</code>] Adapt fix for <code>E203</code> to work identical to <code>ruff format</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10999">#10999</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix formatter instability for lines only consisting of zero-width characters (<a href="https://redirect.github.com/astral-sh/ruff/pull/11748">#11748</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/pull/11850">#11850</a>)</li>
<li>Use real file path when available in <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11800">#11800</a>)</li>
<li>Improve error message when a command is run on an unavailable document (<a href="https://redirect.github.com/astral-sh/ruff/pull/11823">#11823</a>)</li>
<li>Introduce the <code>ruff.printDebugInformation</code> command (<a href="https://redirect.github.com/astral-sh/ruff/pull/11831">#11831</a>)</li>
<li>Tracing system now respects log level and trace level, with options to log to a file (<a href="https://redirect.github.com/astral-sh/ruff/pull/11747">#11747</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Handle non-printable characters in diff view (<a href="https://redirect.github.com/astral-sh/ruff/pull/11687">#11687</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>refurb</code>] Avoid suggesting starmap when arguments are used outside call (<code>FURB140</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11830">#11830</a>)</li>
<li>[<code>flake8-bugbear</code>] Avoid panic in <code>B909</code> when checking large loop blocks (<a href="https://redirect.github.com/astral-sh/ruff/pull/11772">#11772</a>)</li>
<li>[<code>refurb</code>] Fix misbehavior of <code>operator.itemgetter</code> when getter param is a tuple (<code>FURB118</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11774">#11774</a>)</li>
</ul>
<h2>0.4.8</h2>
<h3>Performance</h3>
<ul>
<li>Linter performance has been improved by around 10% on some microbenchmarks by refactoring the lexer and parser to maintain synchronicity between them (<a href="https://redirect.github.com/astral-sh/ruff/pull/11457">#11457</a>)</li>
</ul>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Implement <code>return-in-generator</code> (<code>B901</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11644">#11644</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI063</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11699">#11699</a>)</li>
<li>[<code>pygrep_hooks</code>] Check blanket ignores via file-level pragmas (<code>PGH004</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/11540">#11540</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pyupgrade</code>] Update <code>UP035</code> for Python 3.13 and the latest version of <code>typing_extensions</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11693">#11693</a>)</li>
<li>[<code>numpy</code>] Update <code>NPY001</code> rule for NumPy 2.0 (<a href="https://redirect.github.com/astral-sh/ruff/pull/11735">#11735</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/4f49e918a9154de16145d77217a4af2b8ce38297"><code>4f49e91</code></a> Bump version to v0.4.9 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11872">#11872</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d681a45b08e20a77a42ae74d5c0f91fd0482079c"><code>d681a45</code></a> Make <code>ruff_db</code> a required crate for <code>ruff_python_semantic</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11874">#11874</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/89bb07c251474399607de9d278cb70902c8a0106"><code>89bb07c</code></a> UPDATE latest supported versions to 3.13 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11870">#11870</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/fe462b30e7af2a089016e45c3faa7dc2ea2ea3ae"><code>fe462b3</code></a> Update Python compatibility to 3.13 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11861">#11861</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c5bc368e430a30cb1d58d130c3d8eb2a1fe34d0a"><code>c5bc368</code></a> [red-knot] Improve <code>Vfs</code> and <code>FileSystem</code> documentation (<a href="https://redirect.github.com/astral-sh/ruff/issues/11856">#11856</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/73370fe7982c789ae91a95fba3e45cc6a054849e"><code>73370fe</code></a> Use <code>starts_with('/')</code> instead of <code>is_absolute</code> to avoid platform specific AP...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/22b6488550b9cb268eafe5161269952aca0df73b"><code>22b6488</code></a> red-knot: Add directory support to <code>MemoryFileSystem</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11825">#11825</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d4dd96d1f4a78d75e598c9cdfb778c88c21742d7"><code>d4dd96d</code></a> red-knot: <code>source_text</code>, <code>line_index</code>, and <code>parsed_module</code> queries (<a href="https://redirect.github.com/astral-sh/ruff/issues/11822">#11822</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/efbf7b14b5060475f0a0bf7753ff8426e2e3b875"><code>efbf7b1</code></a> red-knot[salsa part 2]: Setup semantic DB and Jar (<a href="https://redirect.github.com/astral-sh/ruff/issues/11837">#11837</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/9dc226be9793592262ac9fc6d8fab195f33f36b2"><code>9dc226b</code></a> Add supported commands in server capabilities (<a href="https://redirect.github.com/astral-sh/ruff/issues/11850">#11850</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.4.4...v0.4.9">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.4.4&new-version=0.4.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-18 21:00:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-endorser-service/pull/107" class=".btn">#107</a>
            </td>
            <td>
                <b>
                    Bump pytest from 8.2.1 to 8.2.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.1 to 8.2.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.2.2</h2>
<h1>pytest 8.2.2 (2024-06-04)</h1>
<h2>Bug Fixes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12355">#12355</a>: Fix possible catastrophic performance slowdown on a certain parametrization pattern involving many higher-scoped parameters.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12367">#12367</a>: Fix a regression in pytest 8.2.0 where unittest class instances (a fresh one is created for each test) were not released promptly on test teardown but only on session teardown.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12381">#12381</a>: Fix possible &quot;Directory not empty&quot; crashes arising from concurent cache dir (<code>.pytest_cache</code>) creation. Regressed in pytest 8.2.0.</li>
</ul>
<h2>Improved Documentation</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12290">#12290</a>: Updated Sphinx theme to use Furo instead of Flask, enabling Dark mode theme.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12356">#12356</a>: Added a subsection to the documentation for debugging flaky tests to mention
lack of thread safety in pytest as a possible source of flakyness.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12363">#12363</a>: The documentation webpages now links to a canonical version to reduce outdated documentation in search engine results.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/329d3712146e69c471be3e30883d54bdde2f76cb"><code>329d371</code></a> Prepare release version 8.2.2</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/214d098fcce88940f5ce9353786b3cc8f0bd3938"><code>214d098</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12414">#12414</a> from bluetech/backport-12409</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/153a436bc40c9e89d90d62255ef5a89e9a762dca"><code>153a436</code></a> [8.2.x] fixtures: fix catastrophic performance problem in <code>reorder_items</code></li>
<li><a href="https://github.com/pytest-dev/pytest/commit/b41d5a52bbb808780ab310456d71e5ce509fd402"><code>b41d5a5</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12412">#12412</a> from pytest-dev/backport-12408-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/9bb73d734ff40f52d7bbebd708b5e3ab1ba20798"><code>9bb73d7</code></a> [8.2.x] cacheprovider: fix &quot;Directory not empty&quot; crash from cache directory c...</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/4569a01e3d20d64811d48b0b09539596520ea5a6"><code>4569a01</code></a> [8.2.x] doc: Update trainings/events (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12402">#12402</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/1d103e5cdc1cb08f332e61a5b20fb205fa5228e7"><code>1d103e5</code></a> [8.2.x] Clarify pytest_ignore_collect docs (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12386">#12386</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/240a252d34fff26efad5b3a92e62be4c9af94b70"><code>240a252</code></a> [8.2.x] Add html_baseurl to sphinx conf.py (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12372">#12372</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/a5ee3c41268199c2c0af59c33050326b1c4a342e"><code>a5ee3c4</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12370">#12370</a> from pytest-dev/backport-12368-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/f7358aec2884720b4de4594ffd0811b46316514c"><code>f7358ae</code></a> [8.2.x] unittest: fix class instances no longer released on test teardown sin...</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.1...8.2.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.1&new-version=8.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-18 21:00:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-endorser-service/pull/106" class=".btn">#106</a>
            </td>
            <td>
                <b>
                    Bump sqlmodel from 0.0.18 to 0.0.19
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [sqlmodel](https://github.com/tiangolo/sqlmodel) from 0.0.18 to 0.0.19.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tiangolo/sqlmodel/releases">sqlmodel's releases</a>.</em></p>
<blockquote>
<h2>0.0.19</h2>
<h3>Fixes</h3>
<ul>
<li>🐛 Fix pydantic <code>EmailStr</code> support and <code>max_length</code> in several String subclasses. PR <a href="https://redirect.github.com/tiangolo/sqlmodel/pull/966">#966</a> by <a href="https://github.com/estebanx64"><code>@​estebanx64</code></a>.</li>
<li>🐛 Fix set varchar limit when <code>max_length</code> is set on Pydantic models using Pydantic v2. PR <a href="https://redirect.github.com/tiangolo/sqlmodel/pull/963">#963</a> by <a href="https://github.com/estebanx64"><code>@​estebanx64</code></a>.</li>
</ul>
<h3>Refactors</h3>
<ul>
<li>♻️ Refactor generate select template to isolate templated code to the minimum. PR <a href="https://redirect.github.com/tiangolo/sqlmodel/pull/967">#967</a> by <a href="https://github.com/tiangolo"><code>@​tiangolo</code></a>.</li>
</ul>
<h3>Upgrades</h3>
<ul>
<li>⬆️ Update minimum SQLAlchemy version to 2.0.14 as that one includes <code>TryCast</code> used internally. PR <a href="https://redirect.github.com/tiangolo/sqlmodel/pull/964">#964</a> by <a href="https://github.com/tiangolo"><code>@​tiangolo</code></a>.</li>
</ul>
<h3>Docs</h3>
<ul>
<li>✏️ Fix broken link to <code>@dataclass_transform</code> (now PEP 681) in <code>docs/features.md</code>. PR <a href="https://redirect.github.com/tiangolo/sqlmodel/pull/753">#753</a> by <a href="https://github.com/soof-golan"><code>@​soof-golan</code></a>.</li>
</ul>
<h3>Internal</h3>
<ul>
<li>⬆️ Upgrade Ruff and Black. PR <a href="https://redirect.github.com/tiangolo/sqlmodel/pull/968">#968</a> by <a href="https://github.com/tiangolo"><code>@​tiangolo</code></a>.</li>
<li>⬆ Bump tiangolo/issue-manager from 0.4.1 to 0.5.0. PR <a href="https://redirect.github.com/tiangolo/sqlmodel/pull/922">#922</a> by <a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>.</li>
<li>📌 Pin typing-extensions in tests for compatiblity with Python 3.8, dirty-equals, Pydantic. PR <a href="https://redirect.github.com/tiangolo/sqlmodel/pull/965">#965</a> by <a href="https://github.com/tiangolo"><code>@​tiangolo</code></a>.</li>
<li>👷 Update GitHub Actions to download and upload artifacts. PR <a href="https://redirect.github.com/tiangolo/sqlmodel/pull/936">#936</a> by <a href="https://github.com/tiangolo"><code>@​tiangolo</code></a>.</li>
<li>👷 Tweak CI for test-redistribute, add needed env vars for slim. PR <a href="https://redirect.github.com/tiangolo/sqlmodel/pull/929">#929</a> by <a href="https://github.com/tiangolo"><code>@​tiangolo</code></a>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/tiangolo/sqlmodel/blob/main/docs/release-notes.md">sqlmodel's changelog</a>.</em></p>
<blockquote>
<h2>0.0.19</h2>
<h3>Fixes</h3>
<ul>
<li>🐛 Fix pydantic <code>EmailStr</code> support and <code>max_length</code> in several String subclasses. PR <a href="https://redirect.github.com/tiangolo/sqlmodel/pull/966">#966</a> by <a href="https://github.com/estebanx64"><code>@​estebanx64</code></a>.</li>
<li>🐛 Fix set varchar limit when <code>max_length</code> is set on Pydantic models using Pydantic v2. PR <a href="https://redirect.github.com/tiangolo/sqlmodel/pull/963">#963</a> by <a href="https://github.com/estebanx64"><code>@​estebanx64</code></a>.</li>
</ul>
<h3>Refactors</h3>
<ul>
<li>♻️ Refactor generate select template to isolate templated code to the minimum. PR <a href="https://redirect.github.com/tiangolo/sqlmodel/pull/967">#967</a> by <a href="https://github.com/tiangolo"><code>@​tiangolo</code></a>.</li>
</ul>
<h3>Upgrades</h3>
<ul>
<li>⬆️ Update minimum SQLAlchemy version to 2.0.14 as that one includes <code>TryCast</code> used internally. PR <a href="https://redirect.github.com/tiangolo/sqlmodel/pull/964">#964</a> by <a href="https://github.com/tiangolo"><code>@​tiangolo</code></a>.</li>
</ul>
<h3>Docs</h3>
<ul>
<li>✏️ Fix broken link to <code>@dataclass_transform</code> (now PEP 681) in <code>docs/features.md</code>. PR <a href="https://redirect.github.com/tiangolo/sqlmodel/pull/753">#753</a> by <a href="https://github.com/soof-golan"><code>@​soof-golan</code></a>.</li>
</ul>
<h3>Internal</h3>
<ul>
<li>⬆️ Upgrade Ruff and Black. PR <a href="https://redirect.github.com/tiangolo/sqlmodel/pull/968">#968</a> by <a href="https://github.com/tiangolo"><code>@​tiangolo</code></a>.</li>
<li>⬆ Bump tiangolo/issue-manager from 0.4.1 to 0.5.0. PR <a href="https://redirect.github.com/tiangolo/sqlmodel/pull/922">#922</a> by <a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>.</li>
<li>📌 Pin typing-extensions in tests for compatiblity with Python 3.8, dirty-equals, Pydantic. PR <a href="https://redirect.github.com/tiangolo/sqlmodel/pull/965">#965</a> by <a href="https://github.com/tiangolo"><code>@​tiangolo</code></a>.</li>
<li>👷 Update GitHub Actions to download and upload artifacts. PR <a href="https://redirect.github.com/tiangolo/sqlmodel/pull/936">#936</a> by <a href="https://github.com/tiangolo"><code>@​tiangolo</code></a>.</li>
<li>👷 Tweak CI for test-redistribute, add needed env vars for slim. PR <a href="https://redirect.github.com/tiangolo/sqlmodel/pull/929">#929</a> by <a href="https://github.com/tiangolo"><code>@​tiangolo</code></a>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tiangolo/sqlmodel/commit/4590963e884e7f112a2fd28a6c3396b6570dc58d"><code>4590963</code></a> 🔖 Release version 0.0.19</li>
<li><a href="https://github.com/tiangolo/sqlmodel/commit/883cbe3a8dc7da3ab44d57cbec7828cf93d876a7"><code>883cbe3</code></a> 📝 Update release notes</li>
<li><a href="https://github.com/tiangolo/sqlmodel/commit/b560e9deb8d5ecb9982802e479faf3bedcc7a4b5"><code>b560e9d</code></a> ⬆️ Upgrade Ruff and Black (<a href="https://redirect.github.com/tiangolo/sqlmodel/issues/968">#968</a>)</li>
<li><a href="https://github.com/tiangolo/sqlmodel/commit/e2f646dea506233e9f88e122e19bbd7feeb044ed"><code>e2f646d</code></a> 📝 Update release notes</li>
<li><a href="https://github.com/tiangolo/sqlmodel/commit/b93dd9512543366c078b131970aef1b3d68a9db5"><code>b93dd95</code></a> ⬆ Bump tiangolo/issue-manager from 0.4.1 to 0.5.0 (<a href="https://redirect.github.com/tiangolo/sqlmodel/issues/922">#922</a>)</li>
<li><a href="https://github.com/tiangolo/sqlmodel/commit/ceac7bc2e81f4751b1b4d1889e2be6057e25ea8f"><code>ceac7bc</code></a> 📝 Update release notes</li>
<li><a href="https://github.com/tiangolo/sqlmodel/commit/1d43bd8b1e26b14b541f77feda0f606916df9699"><code>1d43bd8</code></a> 🐛 Fix pydantic <code>EmailStr</code> support and <code>max_length</code> in several String subclass...</li>
<li><a href="https://github.com/tiangolo/sqlmodel/commit/9f3af8507ebeb045dbfb63656c0a277f4d65761a"><code>9f3af85</code></a> 📝 Update release notes</li>
<li><a href="https://github.com/tiangolo/sqlmodel/commit/d165e4b5ad20ea9ecc5f4791b5a78ffd2b3aaeda"><code>d165e4b</code></a> ♻️ Refactor generate select template to isolate templated code to the minimum...</li>
<li><a href="https://github.com/tiangolo/sqlmodel/commit/d5cba6e35842dcfcbbb1273ce9dc50a87252bb58"><code>d5cba6e</code></a> 📝 Update release notes</li>
<li>Additional commits viewable in <a href="https://github.com/tiangolo/sqlmodel/compare/0.0.18...0.0.19">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=sqlmodel&package-manager=pip&previous-version=0.0.18&new-version=0.0.19)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-18 20:59:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-endorser-service/pull/105" class=".btn">#105</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 2.2.1 to 2.2.2 in the pip group
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group with 1 update: [urllib3](https://github.com/urllib3/urllib3).

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


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=urllib3&package-manager=pip&previous-version=2.2.1&new-version=2.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-18 20:59:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-endorser-service/pull/104" class=".btn">#104</a>
            </td>
            <td>
                <b>
                    Bump pydantic-settings from 2.2.1 to 2.3.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pydantic-settings](https://github.com/pydantic/pydantic-settings) from 2.2.1 to 2.3.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pydantic/pydantic-settings/releases">pydantic-settings's releases</a>.</em></p>
<blockquote>
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
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/ITProKyle"><code>@​ITProKyle</code></a> made their first contribution in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/255">pydantic/pydantic-settings#255</a></li>
<li><a href="https://github.com/keenranger"><code>@​keenranger</code></a> made their first contribution in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/271">pydantic/pydantic-settings#271</a></li>
<li><a href="https://github.com/diefans"><code>@​diefans</code></a> made their first contribution in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/276">pydantic/pydantic-settings#276</a></li>
<li><a href="https://github.com/jenskeiner"><code>@​jenskeiner</code></a> made their first contribution in <a href="https://redirect.github.com/pydantic/pydantic-settings/pull/285">pydantic/pydantic-settings#285</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pydantic/pydantic-settings/compare/v2.2.1...v2.3.0">https://github.com/pydantic/pydantic-settings/compare/v2.2.1...v2.3.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pydantic/pydantic-settings/commit/f1b82d834abfed0aa2c263d88bc017c0ea1530af"><code>f1b82d8</code></a> Prepare release 2.3.3 (<a href="https://redirect.github.com/pydantic/pydantic-settings/issues/314">#314</a>)</li>
<li><a href="https://github.com/pydantic/pydantic-settings/commit/bd294a4b1ed49357446a38765af302d14b94bcc6"><code>bd294a4</code></a> Add CliSettingsSource alias handling for AliasChoices and AliasPath. (<a href="https://redirect.github.com/pydantic/pydantic-settings/issues/313">#313</a>)</li>
<li><a href="https://github.com/pydantic/pydantic-settings/commit/abe7cc5e3268a9093def94917bc581c31ba74f20"><code>abe7cc5</code></a> Fix an intriduced bug in parsing json field with discriminated union (<a href="https://redirect.github.com/pydantic/pydantic-settings/issues/312">#312</a>)</li>
<li><a href="https://github.com/pydantic/pydantic-settings/commit/b5d4534cdcddb1bb99258d88a0e6d1f16e6788f4"><code>b5d4534</code></a> Prepare release 2.3.2 (<a href="https://redirect.github.com/pydantic/pydantic-settings/issues/310">#310</a>)</li>
<li><a href="https://github.com/pydantic/pydantic-settings/commit/b2e84c2729d73ee2f1ab7962398003d933c5227a"><code>b2e84c2</code></a> Fix issue with nested model uppercase field name in case insensitive mode (<a href="https://redirect.github.com/pydantic/pydantic-settings/issues/309">#309</a>)</li>
<li><a href="https://github.com/pydantic/pydantic-settings/commit/0a9faca91e9503afbcb8fdd652114f9f69ba13b0"><code>0a9faca</code></a> Fix command line help from <code>argparse</code> formatting problem (<a href="https://redirect.github.com/pydantic/pydantic-settings/issues/307">#307</a>)</li>
<li><a href="https://github.com/pydantic/pydantic-settings/commit/813ac94d20fe40f4bb8158ebaaab592b29869dc9"><code>813ac94</code></a> Initialize CLI source on demand. (<a href="https://redirect.github.com/pydantic/pydantic-settings/issues/305">#305</a>)</li>
<li><a href="https://github.com/pydantic/pydantic-settings/commit/39d5e816e97f129dbd8f86c4d35e0b8b1171b720"><code>39d5e81</code></a> Prepare release 2.3.1 (<a href="https://redirect.github.com/pydantic/pydantic-settings/issues/302">#302</a>)</li>
<li><a href="https://github.com/pydantic/pydantic-settings/commit/ad07a575e3a3e35a0fc7a7714cc3609863699032"><code>ad07a57</code></a> Fix a regresion in parsing env value for nested dict (<a href="https://redirect.github.com/pydantic/pydantic-settings/issues/301">#301</a>)</li>
<li><a href="https://github.com/pydantic/pydantic-settings/commit/bcbfd17affa5a90663c9afc5a7dc67b281a728dc"><code>bcbfd17</code></a> Prepare release 2.3.0 (<a href="https://redirect.github.com/pydantic/pydantic-settings/issues/297">#297</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pydantic/pydantic-settings/compare/v2.2.1...v2.3.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pydantic-settings&package-manager=pip&previous-version=2.2.1&new-version=2.3.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-18 20:59:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-endorser-service/pull/103" class=".btn">#103</a>
            </td>
            <td>
                <b>
                    Bump python from 3.10-slim-bullseye to 3.12-slim-bullseye in /endorser
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps python from 3.10-slim-bullseye to 3.12-slim-bullseye.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=python&package-manager=docker&previous-version=3.10-slim-bullseye&new-version=3.12-slim-bullseye)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-18 20:58:49 +0000 UTC
    </div>
</div>

