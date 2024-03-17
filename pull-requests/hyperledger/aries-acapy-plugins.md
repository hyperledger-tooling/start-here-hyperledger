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
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/256" class=".btn">#256</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Update ruff requirement from ^0.1.2 to ^0.3.2 in /plugin_globals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Updates the requirements on [ruff](https://github.com/astral-sh/ruff) to permit the latest version.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.3.2</h2>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>Improve single-<code>with</code> item formatting for Python 3.8 or older (<a href="https://redirect.github.com/astral-sh/ruff/pull/10276">#10276</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pyupgrade</code>] Allow fixes for f-string rule regardless of line length (<code>UP032</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10263">#10263</a>)</li>
<li>[<code>pycodestyle</code>] Include actual conditions in E712 diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/pull/10254">#10254</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Fix trailing kwargs end of line comment after slash (<a href="https://redirect.github.com/astral-sh/ruff/pull/10297">#10297</a>)</li>
<li>Fix unstable <code>with</code> items formatting (<a href="https://redirect.github.com/astral-sh/ruff/pull/10274">#10274</a>)</li>
<li>Avoid repeating function calls in f-string conversions (<a href="https://redirect.github.com/astral-sh/ruff/pull/10265">#10265</a>)</li>
<li>Fix E203 false positive for slices in format strings (<a href="https://redirect.github.com/astral-sh/ruff/pull/10280">#10280</a>)</li>
<li>Fix incorrect <code>Parameter</code> range  for <code>*args</code> and <code>**kwargs</code>  (<a href="https://redirect.github.com/astral-sh/ruff/pull/10283">#10283</a>)</li>
<li>Treat <code>typing.Annotated</code> subscripts as type definitions (<a href="https://redirect.github.com/astral-sh/ruff/pull/10285">#10285</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/GtrMo"><code>@​GtrMo</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/sciyoshi"><code>@​sciyoshi</code></a></li>
<li><a href="https://github.com/tjkuson"><code>@​tjkuson</code></a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.3.2</h2>
<h3>Preview features</h3>
<ul>
<li>Improve single-<code>with</code> item formatting for Python 3.8 or older (<a href="https://redirect.github.com/astral-sh/ruff/pull/10276">#10276</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pyupgrade</code>] Allow fixes for f-string rule regardless of line length (<code>UP032</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10263">#10263</a>)</li>
<li>[<code>pycodestyle</code>] Include actual conditions in E712 diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/pull/10254">#10254</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Fix trailing kwargs end of line comment after slash (<a href="https://redirect.github.com/astral-sh/ruff/pull/10297">#10297</a>)</li>
<li>Fix unstable <code>with</code> items formatting (<a href="https://redirect.github.com/astral-sh/ruff/pull/10274">#10274</a>)</li>
<li>Avoid repeating function calls in f-string conversions (<a href="https://redirect.github.com/astral-sh/ruff/pull/10265">#10265</a>)</li>
<li>Fix E203 false positive for slices in format strings (<a href="https://redirect.github.com/astral-sh/ruff/pull/10280">#10280</a>)</li>
<li>Fix incorrect <code>Parameter</code> range  for <code>*args</code> and <code>**kwargs</code>  (<a href="https://redirect.github.com/astral-sh/ruff/pull/10283">#10283</a>)</li>
<li>Treat <code>typing.Annotated</code> subscripts as type definitions (<a href="https://redirect.github.com/astral-sh/ruff/pull/10285">#10285</a>)</li>
</ul>
<h2>0.3.1</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pycodestyle</code>] Fix E301 not triggering on decorated methods. (<a href="https://redirect.github.com/astral-sh/ruff/pull/10117">#10117</a>)</li>
<li>[<code>pycodestyle</code>] Respect <code>isort</code> settings in blank line rules (<code>E3*</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10096">#10096</a>)</li>
<li>[<code>pycodestyle</code>] Make blank lines in typing stub files optional (<code>E3*</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10098">#10098</a>)</li>
<li>[<code>pylint</code>] Implement <code>singledispatch-method</code> (<code>E1519</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10140">#10140</a>)</li>
<li>[<code>pylint</code>] Implement <code>useless-exception-statement</code> (<code>W0133</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10176">#10176</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-debugger</code>] Check for use of <code>debugpy</code> and <code>ptvsd</code> debug modules (<a href="https://redirect.github.com/astral-sh/ruff/issues/10177">#10177</a>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10194">#10194</a>)</li>
<li>[<code>pyupgrade</code>] Generate diagnostic for all valid f-string conversions regardless of line length (<code>UP032</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10238">#10238</a>)</li>
<li>[<code>pep8_naming</code>] Add fixes for <code>N804</code> and <code>N805</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10215">#10215</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Colorize the output of <code>ruff format --diff</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10110">#10110</a>)</li>
<li>Make <code>--config</code> and <code>--isolated</code> global flags (<a href="https://redirect.github.com/astral-sh/ruff/pull/10150">#10150</a>)</li>
<li>Correctly expand tildes and environment variables in paths passed to <code>--config</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10219">#10219</a>)</li>
</ul>
<h3>Configuration</h3>
<ul>
<li>Accept a PEP 440 version specifier for <code>required-version</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10216">#10216</a>)</li>
<li>Implement isort's <code>default-section</code> setting (<a href="https://redirect.github.com/astral-sh/ruff/pull/10149">#10149</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Remove trailing space from <code>CapWords</code> message (<a href="https://redirect.github.com/astral-sh/ruff/pull/10220">#10220</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/a892fc755d6d4342c2f5a768aa50a401d704ae2c"><code>a892fc7</code></a> Bump version to v0.3.2 (<a href="https://redirect.github.com/astral-sh/ruff/issues/10304">#10304</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/a067d87ccc9a8e0348b1a2421b7879514d4f26c0"><code>a067d87</code></a> Fix incorrect <code>Parameter</code> range  for <code>*args</code> and <code>**kwargs</code>  (<a href="https://redirect.github.com/astral-sh/ruff/issues/10283">#10283</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/b64f2ea40192436639f668f4a342fcb04b0e4071"><code>b64f2ea</code></a> Formatter: Improve single-with item formatting for Python 3.8 or older (<a href="https://redirect.github.com/astral-sh/ruff/issues/10276">#10276</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4bce80106545af8d1edd028c7085a9e9d703fc6b"><code>4bce801</code></a> Fix unstable with-items formatting (<a href="https://redirect.github.com/astral-sh/ruff/issues/10274">#10274</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/a56d42f1839cb9b44f0fc369c441f4d329ed868a"><code>a56d42f</code></a> Refactor with statement formatting to have explicit layouts (<a href="https://redirect.github.com/astral-sh/ruff/issues/10296">#10296</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1d97f2733554c6825c8b4d3e1936d864e0cf4871"><code>1d97f27</code></a> Start tracking quoting style in the AST (<a href="https://redirect.github.com/astral-sh/ruff/issues/10298">#10298</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/965adbed4b56a76d6cce02534e47c4d7a2a9cd32"><code>965adbe</code></a> Fix trailing kwargs end of line comment after slash (<a href="https://redirect.github.com/astral-sh/ruff/issues/10297">#10297</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c504d7ab11308a08d6d91af7d6f47fc3b2ba4165"><code>c504d7a</code></a> Track quoting style in the tokenizer (<a href="https://redirect.github.com/astral-sh/ruff/issues/10256">#10256</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/72c9f7e4c9928ad2714e8ca68c1defe2e778d4f3"><code>72c9f7e</code></a> Include actual conditions in E712 diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/issues/10254">#10254</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/57be3fce900488a9ce1a0187863599ddf1c0d3ed"><code>57be3fc</code></a> Treat <code>typing.Annotated</code> subscripts as type definitions (<a href="https://redirect.github.com/astral-sh/ruff/issues/10285">#10285</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.1.2...v0.3.2">compare view</a></li>
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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-11 04:33:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/255" class=".btn">#255</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Update pytest-asyncio requirement from ~0.14.0 to ~0.23.5 in /plugin_globals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Updates the requirements on [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) to permit the latest version.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.5.post1</h2>
<h1>0.23.5 (2024-02-09)</h1>
<ul>
<li>Declare compatibility with pytest 8 <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/737">#737</a></li>
<li>Fix typing errors with recent versions of mypy <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/769">#769</a></li>
<li>Prevent DeprecationWarning about internal use of <code>asyncio.get_event_loop()</code> from affecting test cases <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/757">#757</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b22d84e1f0d53920352be4c66d1b6c7f7a9ce005"><code>b22d84e</code></a> [docs] Fixes the example showing how to run all tests in a session-scoped loop.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/f1de446a37b426f5882b103d5c2fd2f3045b1f01"><code>f1de446</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b60649a648912a79ce6f3443ca7ac2c67fe9a5b7"><code>b60649a</code></a> Build(deps): Bump urllib3 from 2.2.0 to 2.2.1 in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4baec47b8514b405e97a14a1d6c42fa07af8fb0a"><code>4baec47</code></a> Build(deps): Bump typing-extensions in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d44e3ac013cb3b6736492d3f920fb8820f3c8bbf"><code>d44e3ac</code></a> Build(deps): Bump pytest from 8.0.0 to 8.0.2 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/cefa62e7d007b5aa0add7bd58a3e33f246daee71"><code>cefa62e</code></a> Build(deps): Bump coverage from 7.4.1 to 7.4.3 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/290886063f1da8ec1865cd2cdae721b0ebb89edf"><code>2908860</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/20bd7d87bec30ee49a2ec1adc8df8857fc0a69ac"><code>20bd7d8</code></a> Build(deps): Bump pypa/gh-action-pypi-publish from 1.8.11 to 1.8.12</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3aef60532f2a1c634af5f4539eabdd4fbfffcabc"><code>3aef605</code></a> [build] Update actions/upload-artifact and actions/download-artifact to v4.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4b1908d9ed26895c194a4bb8d4c61cef2dfc5067"><code>4b1908d</code></a> [fix] Prevent DeprecationWarning from bubbling to user code.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.14.0...v0.23.5.post1">compare view</a></li>
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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-11 04:33:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/254" class=".btn">#254</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump pytest-asyncio from 0.14.0 to 0.23.5.post1 in /kafka_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.14.0 to 0.23.5.post1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.5.post1</h2>
<h1>0.23.5 (2024-02-09)</h1>
<ul>
<li>Declare compatibility with pytest 8 <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/737">#737</a></li>
<li>Fix typing errors with recent versions of mypy <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/769">#769</a></li>
<li>Prevent DeprecationWarning about internal use of <code>asyncio.get_event_loop()</code> from affecting test cases <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/757">#757</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
<h2>pytest-asyncio 0.23.5</h2>
<h1>0.23.5 (2024-02-09)</h1>
<ul>
<li>Declare compatibility with pytest 8 <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/737">#737</a></li>
<li>Fix typing errors with recent versions of mypy <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/769">#769</a></li>
<li>Prevent DeprecationWarning about internal use of <code>asyncio.get_event_loop()</code> from affecting test cases <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/757">#757</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
<h2>pytest-asyncio 0.23.5a0</h2>
<h1>0.23.5 (UNRELEASED)</h1>
<ul>
<li>Declare compatibility with pytest 8 <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/737">#737</a></li>
<li>Fix typing errors with recent versions of mypy <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/769">#769</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
<h2>pytest-asyncio 0.23.4</h2>
<h1>0.23.4 (2024-01-28)</h1>
<ul>
<li>pytest-asyncio no longer imports additional, unrelated packages during test collection <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/729">#729</a></li>
<li>Addresses further issues that caused an internal pytest error during test collection</li>
<li>Declares incompatibility with pytest 8 <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/737">#737</a></li>
</ul>
<h2>pytest-asyncio 0.23.4a2</h2>
<h1>0.23.4 (UNRELEASED)</h1>
<ul>
<li>pytest-asyncio no longer imports additional, unrelated packages during test collection <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/729">#729</a></li>
<li>Addresses further issues that caused an internal pytest error during test collection</li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
<h2>pytest-asyncio 0.23.4a1</h2>
<h1>0.23.4 (UNRELEASED)</h1>
<ul>
<li>pytest-asyncio no longer imports additional, unrelated packages during test collection <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/729">#729</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
<h2>pytest-asyncio 0.23.4a0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b22d84e1f0d53920352be4c66d1b6c7f7a9ce005"><code>b22d84e</code></a> [docs] Fixes the example showing how to run all tests in a session-scoped loop.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/f1de446a37b426f5882b103d5c2fd2f3045b1f01"><code>f1de446</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b60649a648912a79ce6f3443ca7ac2c67fe9a5b7"><code>b60649a</code></a> Build(deps): Bump urllib3 from 2.2.0 to 2.2.1 in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4baec47b8514b405e97a14a1d6c42fa07af8fb0a"><code>4baec47</code></a> Build(deps): Bump typing-extensions in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d44e3ac013cb3b6736492d3f920fb8820f3c8bbf"><code>d44e3ac</code></a> Build(deps): Bump pytest from 8.0.0 to 8.0.2 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/cefa62e7d007b5aa0add7bd58a3e33f246daee71"><code>cefa62e</code></a> Build(deps): Bump coverage from 7.4.1 to 7.4.3 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/290886063f1da8ec1865cd2cdae721b0ebb89edf"><code>2908860</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/20bd7d87bec30ee49a2ec1adc8df8857fc0a69ac"><code>20bd7d8</code></a> Build(deps): Bump pypa/gh-action-pypi-publish from 1.8.11 to 1.8.12</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3aef60532f2a1c634af5f4539eabdd4fbfffcabc"><code>3aef605</code></a> [build] Update actions/upload-artifact and actions/download-artifact to v4.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4b1908d9ed26895c194a4bb8d4c61cef2dfc5067"><code>4b1908d</code></a> [fix] Prevent DeprecationWarning from bubbling to user code.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.14.0...v0.23.5.post1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.14.0&new-version=0.23.5.post1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-03-11 04:25:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/253" class=".btn">#253</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump pytest from 7.4.4 to 8.1.1 in /kafka_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 7.4.4 to 8.1.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.1.1</h2>
<h1>pytest 8.1.1 (2024-03-08)</h1>
<p>::: {.note}
::: {.title}
Note
:::</p>
<p>This release is not a usual bug fix release -- it contains features and improvements, being a follow up
to <code>8.1.0</code>, which has been yanked from PyPI.
:::</p>
<h2>Features</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11475">#11475</a>: Added the new <code>consider_namespace_packages</code>{.interpreted-text role=&quot;confval&quot;} configuration option, defaulting to <code>False</code>.</p>
<p>If set to <code>True</code>, pytest will attempt to identify modules that are part of <a href="https://packaging.python.org/en/latest/guides/packaging-namespace-packages">namespace packages</a> when importing modules.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11653">#11653</a>: Added the new <code>verbosity_test_cases</code>{.interpreted-text role=&quot;confval&quot;} configuration option for fine-grained control of test execution verbosity.
See <code>Fine-grained verbosity &lt;pytest.fine_grained_verbosity&gt;</code>{.interpreted-text role=&quot;ref&quot;} for more details.</p>
</li>
</ul>
<h2>Improvements</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/10865">#10865</a>: <code>pytest.warns</code>{.interpreted-text role=&quot;func&quot;} now validates that <code>warnings.warn</code>{.interpreted-text role=&quot;func&quot;} was called with a [str]{.title-ref} or a [Warning]{.title-ref}.
Currently in Python it is possible to use other types, however this causes an exception when <code>warnings.filterwarnings</code>{.interpreted-text role=&quot;func&quot;} is used to filter those warnings (see [CPython <a href="https://redirect.github.com/pytest-dev/pytest/issues/103577">#103577</a>](<a href="https://redirect.github.com/python/cpython/issues/103577">python/cpython#103577</a>) for a discussion).
While this can be considered a bug in CPython, we decided to put guards in pytest as the error message produced without this check in place is confusing.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11311">#11311</a>: When using <code>--override-ini</code> for paths in invocations without a configuration file defined, the current working directory is used
as the relative directory.</p>
<p>Previoulsy this would raise an <code>AssertionError</code>{.interpreted-text role=&quot;class&quot;}.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11475">#11475</a>: <code>--import-mode=importlib &lt;import-mode-importlib&gt;</code>{.interpreted-text role=&quot;ref&quot;} now tries to import modules using the standard import mechanism (but still without changing :py<code>sys.path</code>{.interpreted-text role=&quot;data&quot;}), falling back to importing modules directly only if that fails.</p>
<p>This means that installed packages will be imported under their canonical name if possible first, for example <code>app.core.models</code>, instead of having the module name always be derived from their path (for example <code>.env310.lib.site_packages.app.core.models</code>).</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11801">#11801</a>: Added the <code>iter_parents() &lt;_pytest.nodes.Node.iter_parents&gt;</code>{.interpreted-text role=&quot;func&quot;} helper method on nodes.
It is similar to <code>listchain &lt;_pytest.nodes.Node.listchain&gt;</code>{.interpreted-text role=&quot;func&quot;}, but goes from bottom to top, and returns an iterator, not a list.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11850">#11850</a>: Added support for <code>sys.last_exc</code>{.interpreted-text role=&quot;data&quot;} for post-mortem debugging on Python&gt;=3.12.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11962">#11962</a>: In case no other suitable candidates for configuration file are found, a <code>pyproject.toml</code> (even without a <code>[tool.pytest.ini_options]</code> table) will be considered as the configuration file and define the <code>rootdir</code>.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11978">#11978</a>: Add <code>--log-file-mode</code> option to the logging plugin, enabling appending to log-files. This option accepts either <code>&quot;w&quot;</code> or <code>&quot;a&quot;</code> and defaults to <code>&quot;w&quot;</code>.</p>
<p>Previously, the mode was hard-coded to be <code>&quot;w&quot;</code> which truncates the file before logging.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/81653ee385f4c62ee7e64502a7b7530096553115"><code>81653ee</code></a> Adjust changelog manually for 8.1.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/e60b4b9ed80f761e3a51868a01338911a567b093"><code>e60b4b9</code></a> Prepare release version 8.1.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/15fbe57c44fed6737f5c6dad99cf4437b6755a6c"><code>15fbe57</code></a> [8.1.x] Revert legacy path removals (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12093">#12093</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/86c3aab005a98de7e12ee5e37782837f5db70ac3"><code>86c3aab</code></a> [8.1.x] Do not import duplicated modules with --importmode=importlib (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12077">#12077</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/5b82b0cd20c3adcc21f34ae30c595c7355a87e23"><code>5b82b0c</code></a> [8.1.x] Yank version 8.1.0 (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12076">#12076</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/0a536810dc5f51dac99bdb90dde06704b5aa034e"><code>0a53681</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12054">#12054</a> from pytest-dev/release-8.1.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/b9a167f9bbbd6eda4f0360c5bf5b7f5af50f2bc4"><code>b9a167f</code></a> Prepare release version 8.1.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/00043f7f1047b29fdaeb18e169fe9d6146988cb8"><code>00043f7</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12038">#12038</a> from bluetech/fixtures-rm-arg2index</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/f4e10251a4a003495b5228cea421d4de5fa0ce89"><code>f4e1025</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12048">#12048</a> from bluetech/fixture-teardown-excgroup</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/43492f5707b38dab9b62dfb829bb41a13579629f"><code>43492f5</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12051">#12051</a> from jakkdl/test_debugging_pythonbreakpoint</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/7.4.4...8.1.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=7.4.4&new-version=8.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-03-11 04:24:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/252" class=".btn">#252</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump pytest-ruff from 0.1.1 to 0.3.1 in /kafka_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-ruff](https://github.com/businho/pytest-ruff) from 0.1.1 to 0.3.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/businho/pytest-ruff/releases">pytest-ruff's releases</a>.</em></p>
<blockquote>
<h2>Add support to pytest 8.1.x</h2>
<p>No release notes provided.</p>
<h2>Support old pytest versions</h2>
<p>No release notes provided.</p>
<h2>Fix previous messed up release</h2>
<p>It makes <code>--ruff</code> and <code>--ruff-format</code> work independently and make the plugin work again.</p>
<h2>Support ruff format and respect exclude config</h2>
<p>No release notes provided.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/businho/pytest-ruff/commit/9efc242a519f8c7648bc732a170079864b592521"><code>9efc242</code></a> fix: pytest 8.1 compat (<a href="https://redirect.github.com/businho/pytest-ruff/issues/16">#16</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/41ec4c4cc327aa3c5f86f466025dc53bee29304d"><code>41ec4c4</code></a> Silence some deprecation warnings for Python 3.14</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/ef9d0e0bc173dac03f1af954f9a9d3574203a64e"><code>ef9d0e0</code></a> Fail tests with warnings</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/37b8e736063f61ca4b5118ac499ee63fb3943b17"><code>37b8e73</code></a> Support old pytests (<a href="https://redirect.github.com/businho/pytest-ruff/issues/13">#13</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/463bb48aed573d28b63b00e81f317ffcf0c2cbf9"><code>463bb48</code></a> Fix cov (<a href="https://redirect.github.com/businho/pytest-ruff/issues/14">#14</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/8a6a5a32602cd4936029ddae1bda4ce899b8d98f"><code>8a6a5a3</code></a> Run tox with 3.12 and drop 3.7</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/1ef9b2244f6dc63be9fefeef909092e4cf50c9a1"><code>1ef9b22</code></a> Merge pull request <a href="https://redirect.github.com/businho/pytest-ruff/issues/10">#10</a> from cclauss/patch-1</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/951ece4fff3c07d9be59ab1dcb64bf7e7ad49130"><code>951ece4</code></a> Upgrade GitHub Actions and add Python 3.12</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/2098829cfb8f95c2885c6dec3e229ed3092e2c1e"><code>2098829</code></a> Merge pull request <a href="https://redirect.github.com/businho/pytest-ruff/issues/8">#8</a> from skellys/fix/fix_v0_2</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/3e0cfef09777aff7411aad2bf50f89b8b4a72a62"><code>3e0cfef</code></a> Fix tests</li>
<li>Additional commits viewable in <a href="https://github.com/businho/pytest-ruff/compare/v0.1.1...v0.3.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-ruff&package-manager=pip&previous-version=0.1.1&new-version=0.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-03-11 04:24:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/251" class=".btn">#251</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump ruff from 0.1.15 to 0.3.2 in /kafka_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.1.15 to 0.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.3.2</h2>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>Improve single-<code>with</code> item formatting for Python 3.8 or older (<a href="https://redirect.github.com/astral-sh/ruff/pull/10276">#10276</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pyupgrade</code>] Allow fixes for f-string rule regardless of line length (<code>UP032</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10263">#10263</a>)</li>
<li>[<code>pycodestyle</code>] Include actual conditions in E712 diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/pull/10254">#10254</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Fix trailing kwargs end of line comment after slash (<a href="https://redirect.github.com/astral-sh/ruff/pull/10297">#10297</a>)</li>
<li>Fix unstable <code>with</code> items formatting (<a href="https://redirect.github.com/astral-sh/ruff/pull/10274">#10274</a>)</li>
<li>Avoid repeating function calls in f-string conversions (<a href="https://redirect.github.com/astral-sh/ruff/pull/10265">#10265</a>)</li>
<li>Fix E203 false positive for slices in format strings (<a href="https://redirect.github.com/astral-sh/ruff/pull/10280">#10280</a>)</li>
<li>Fix incorrect <code>Parameter</code> range  for <code>*args</code> and <code>**kwargs</code>  (<a href="https://redirect.github.com/astral-sh/ruff/pull/10283">#10283</a>)</li>
<li>Treat <code>typing.Annotated</code> subscripts as type definitions (<a href="https://redirect.github.com/astral-sh/ruff/pull/10285">#10285</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/GtrMo"><code>@​GtrMo</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/sciyoshi"><code>@​sciyoshi</code></a></li>
<li><a href="https://github.com/tjkuson"><code>@​tjkuson</code></a></li>
</ul>
<h2>v0.3.1</h2>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pycodestyle</code>] Fix E301 not triggering on decorated methods. (<a href="https://redirect.github.com/astral-sh/ruff/pull/10117">#10117</a>)</li>
<li>[<code>pycodestyle</code>] Respect <code>isort</code> settings in blank line rules (<code>E3*</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10096">#10096</a>)</li>
<li>[<code>pycodestyle</code>] Make blank lines in typing stub files optional (<code>E3*</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10098">#10098</a>)</li>
<li>[<code>pylint</code>] Implement <code>singledispatch-method</code> (<code>E1519</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10140">#10140</a>)</li>
<li>[<code>pylint</code>] Implement <code>useless-exception-statement</code> (<code>W0133</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10176">#10176</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-debugger</code>] Check for use of <code>debugpy</code> and <code>ptvsd</code> debug modules (<a href="https://redirect.github.com/astral-sh/ruff/issues/10177">#10177</a>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10194">#10194</a>)</li>
<li>[<code>pyupgrade</code>] Generate diagnostic for all valid f-string conversions regardless of line length (<code>UP032</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10238">#10238</a>)</li>
<li>[<code>pep8_naming</code>] Add fixes for <code>N804</code> and <code>N805</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10215">#10215</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Colorize the output of <code>ruff format --diff</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10110">#10110</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.3.2</h2>
<h3>Preview features</h3>
<ul>
<li>Improve single-<code>with</code> item formatting for Python 3.8 or older (<a href="https://redirect.github.com/astral-sh/ruff/pull/10276">#10276</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pyupgrade</code>] Allow fixes for f-string rule regardless of line length (<code>UP032</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10263">#10263</a>)</li>
<li>[<code>pycodestyle</code>] Include actual conditions in E712 diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/pull/10254">#10254</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Fix trailing kwargs end of line comment after slash (<a href="https://redirect.github.com/astral-sh/ruff/pull/10297">#10297</a>)</li>
<li>Fix unstable <code>with</code> items formatting (<a href="https://redirect.github.com/astral-sh/ruff/pull/10274">#10274</a>)</li>
<li>Avoid repeating function calls in f-string conversions (<a href="https://redirect.github.com/astral-sh/ruff/pull/10265">#10265</a>)</li>
<li>Fix E203 false positive for slices in format strings (<a href="https://redirect.github.com/astral-sh/ruff/pull/10280">#10280</a>)</li>
<li>Fix incorrect <code>Parameter</code> range  for <code>*args</code> and <code>**kwargs</code>  (<a href="https://redirect.github.com/astral-sh/ruff/pull/10283">#10283</a>)</li>
<li>Treat <code>typing.Annotated</code> subscripts as type definitions (<a href="https://redirect.github.com/astral-sh/ruff/pull/10285">#10285</a>)</li>
</ul>
<h2>0.3.1</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pycodestyle</code>] Fix E301 not triggering on decorated methods. (<a href="https://redirect.github.com/astral-sh/ruff/pull/10117">#10117</a>)</li>
<li>[<code>pycodestyle</code>] Respect <code>isort</code> settings in blank line rules (<code>E3*</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10096">#10096</a>)</li>
<li>[<code>pycodestyle</code>] Make blank lines in typing stub files optional (<code>E3*</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10098">#10098</a>)</li>
<li>[<code>pylint</code>] Implement <code>singledispatch-method</code> (<code>E1519</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10140">#10140</a>)</li>
<li>[<code>pylint</code>] Implement <code>useless-exception-statement</code> (<code>W0133</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10176">#10176</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-debugger</code>] Check for use of <code>debugpy</code> and <code>ptvsd</code> debug modules (<a href="https://redirect.github.com/astral-sh/ruff/issues/10177">#10177</a>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10194">#10194</a>)</li>
<li>[<code>pyupgrade</code>] Generate diagnostic for all valid f-string conversions regardless of line length (<code>UP032</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10238">#10238</a>)</li>
<li>[<code>pep8_naming</code>] Add fixes for <code>N804</code> and <code>N805</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10215">#10215</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Colorize the output of <code>ruff format --diff</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10110">#10110</a>)</li>
<li>Make <code>--config</code> and <code>--isolated</code> global flags (<a href="https://redirect.github.com/astral-sh/ruff/pull/10150">#10150</a>)</li>
<li>Correctly expand tildes and environment variables in paths passed to <code>--config</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10219">#10219</a>)</li>
</ul>
<h3>Configuration</h3>
<ul>
<li>Accept a PEP 440 version specifier for <code>required-version</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10216">#10216</a>)</li>
<li>Implement isort's <code>default-section</code> setting (<a href="https://redirect.github.com/astral-sh/ruff/pull/10149">#10149</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Remove trailing space from <code>CapWords</code> message (<a href="https://redirect.github.com/astral-sh/ruff/pull/10220">#10220</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/a892fc755d6d4342c2f5a768aa50a401d704ae2c"><code>a892fc7</code></a> Bump version to v0.3.2 (<a href="https://redirect.github.com/astral-sh/ruff/issues/10304">#10304</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/a067d87ccc9a8e0348b1a2421b7879514d4f26c0"><code>a067d87</code></a> Fix incorrect <code>Parameter</code> range  for <code>*args</code> and <code>**kwargs</code>  (<a href="https://redirect.github.com/astral-sh/ruff/issues/10283">#10283</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/b64f2ea40192436639f668f4a342fcb04b0e4071"><code>b64f2ea</code></a> Formatter: Improve single-with item formatting for Python 3.8 or older (<a href="https://redirect.github.com/astral-sh/ruff/issues/10276">#10276</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4bce80106545af8d1edd028c7085a9e9d703fc6b"><code>4bce801</code></a> Fix unstable with-items formatting (<a href="https://redirect.github.com/astral-sh/ruff/issues/10274">#10274</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/a56d42f1839cb9b44f0fc369c441f4d329ed868a"><code>a56d42f</code></a> Refactor with statement formatting to have explicit layouts (<a href="https://redirect.github.com/astral-sh/ruff/issues/10296">#10296</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1d97f2733554c6825c8b4d3e1936d864e0cf4871"><code>1d97f27</code></a> Start tracking quoting style in the AST (<a href="https://redirect.github.com/astral-sh/ruff/issues/10298">#10298</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/965adbed4b56a76d6cce02534e47c4d7a2a9cd32"><code>965adbe</code></a> Fix trailing kwargs end of line comment after slash (<a href="https://redirect.github.com/astral-sh/ruff/issues/10297">#10297</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c504d7ab11308a08d6d91af7d6f47fc3b2ba4165"><code>c504d7a</code></a> Track quoting style in the tokenizer (<a href="https://redirect.github.com/astral-sh/ruff/issues/10256">#10256</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/72c9f7e4c9928ad2714e8ca68c1defe2e778d4f3"><code>72c9f7e</code></a> Include actual conditions in E712 diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/issues/10254">#10254</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/57be3fce900488a9ce1a0187863599ddf1c0d3ed"><code>57be3fc</code></a> Treat <code>typing.Annotated</code> subscripts as type definitions (<a href="https://redirect.github.com/astral-sh/ruff/issues/10285">#10285</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.1.15...v0.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.1.15&new-version=0.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-03-11 04:24:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/250" class=".btn">#250</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump ruff from 0.1.15 to 0.3.2 in /rpc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.1.15 to 0.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.3.2</h2>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>Improve single-<code>with</code> item formatting for Python 3.8 or older (<a href="https://redirect.github.com/astral-sh/ruff/pull/10276">#10276</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pyupgrade</code>] Allow fixes for f-string rule regardless of line length (<code>UP032</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10263">#10263</a>)</li>
<li>[<code>pycodestyle</code>] Include actual conditions in E712 diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/pull/10254">#10254</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Fix trailing kwargs end of line comment after slash (<a href="https://redirect.github.com/astral-sh/ruff/pull/10297">#10297</a>)</li>
<li>Fix unstable <code>with</code> items formatting (<a href="https://redirect.github.com/astral-sh/ruff/pull/10274">#10274</a>)</li>
<li>Avoid repeating function calls in f-string conversions (<a href="https://redirect.github.com/astral-sh/ruff/pull/10265">#10265</a>)</li>
<li>Fix E203 false positive for slices in format strings (<a href="https://redirect.github.com/astral-sh/ruff/pull/10280">#10280</a>)</li>
<li>Fix incorrect <code>Parameter</code> range  for <code>*args</code> and <code>**kwargs</code>  (<a href="https://redirect.github.com/astral-sh/ruff/pull/10283">#10283</a>)</li>
<li>Treat <code>typing.Annotated</code> subscripts as type definitions (<a href="https://redirect.github.com/astral-sh/ruff/pull/10285">#10285</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/GtrMo"><code>@​GtrMo</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/sciyoshi"><code>@​sciyoshi</code></a></li>
<li><a href="https://github.com/tjkuson"><code>@​tjkuson</code></a></li>
</ul>
<h2>v0.3.1</h2>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pycodestyle</code>] Fix E301 not triggering on decorated methods. (<a href="https://redirect.github.com/astral-sh/ruff/pull/10117">#10117</a>)</li>
<li>[<code>pycodestyle</code>] Respect <code>isort</code> settings in blank line rules (<code>E3*</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10096">#10096</a>)</li>
<li>[<code>pycodestyle</code>] Make blank lines in typing stub files optional (<code>E3*</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10098">#10098</a>)</li>
<li>[<code>pylint</code>] Implement <code>singledispatch-method</code> (<code>E1519</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10140">#10140</a>)</li>
<li>[<code>pylint</code>] Implement <code>useless-exception-statement</code> (<code>W0133</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10176">#10176</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-debugger</code>] Check for use of <code>debugpy</code> and <code>ptvsd</code> debug modules (<a href="https://redirect.github.com/astral-sh/ruff/issues/10177">#10177</a>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10194">#10194</a>)</li>
<li>[<code>pyupgrade</code>] Generate diagnostic for all valid f-string conversions regardless of line length (<code>UP032</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10238">#10238</a>)</li>
<li>[<code>pep8_naming</code>] Add fixes for <code>N804</code> and <code>N805</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10215">#10215</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Colorize the output of <code>ruff format --diff</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10110">#10110</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.3.2</h2>
<h3>Preview features</h3>
<ul>
<li>Improve single-<code>with</code> item formatting for Python 3.8 or older (<a href="https://redirect.github.com/astral-sh/ruff/pull/10276">#10276</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>pyupgrade</code>] Allow fixes for f-string rule regardless of line length (<code>UP032</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10263">#10263</a>)</li>
<li>[<code>pycodestyle</code>] Include actual conditions in E712 diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/pull/10254">#10254</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Fix trailing kwargs end of line comment after slash (<a href="https://redirect.github.com/astral-sh/ruff/pull/10297">#10297</a>)</li>
<li>Fix unstable <code>with</code> items formatting (<a href="https://redirect.github.com/astral-sh/ruff/pull/10274">#10274</a>)</li>
<li>Avoid repeating function calls in f-string conversions (<a href="https://redirect.github.com/astral-sh/ruff/pull/10265">#10265</a>)</li>
<li>Fix E203 false positive for slices in format strings (<a href="https://redirect.github.com/astral-sh/ruff/pull/10280">#10280</a>)</li>
<li>Fix incorrect <code>Parameter</code> range  for <code>*args</code> and <code>**kwargs</code>  (<a href="https://redirect.github.com/astral-sh/ruff/pull/10283">#10283</a>)</li>
<li>Treat <code>typing.Annotated</code> subscripts as type definitions (<a href="https://redirect.github.com/astral-sh/ruff/pull/10285">#10285</a>)</li>
</ul>
<h2>0.3.1</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>pycodestyle</code>] Fix E301 not triggering on decorated methods. (<a href="https://redirect.github.com/astral-sh/ruff/pull/10117">#10117</a>)</li>
<li>[<code>pycodestyle</code>] Respect <code>isort</code> settings in blank line rules (<code>E3*</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10096">#10096</a>)</li>
<li>[<code>pycodestyle</code>] Make blank lines in typing stub files optional (<code>E3*</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10098">#10098</a>)</li>
<li>[<code>pylint</code>] Implement <code>singledispatch-method</code> (<code>E1519</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10140">#10140</a>)</li>
<li>[<code>pylint</code>] Implement <code>useless-exception-statement</code> (<code>W0133</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10176">#10176</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-debugger</code>] Check for use of <code>debugpy</code> and <code>ptvsd</code> debug modules (<a href="https://redirect.github.com/astral-sh/ruff/issues/10177">#10177</a>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10194">#10194</a>)</li>
<li>[<code>pyupgrade</code>] Generate diagnostic for all valid f-string conversions regardless of line length (<code>UP032</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10238">#10238</a>)</li>
<li>[<code>pep8_naming</code>] Add fixes for <code>N804</code> and <code>N805</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10215">#10215</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Colorize the output of <code>ruff format --diff</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10110">#10110</a>)</li>
<li>Make <code>--config</code> and <code>--isolated</code> global flags (<a href="https://redirect.github.com/astral-sh/ruff/pull/10150">#10150</a>)</li>
<li>Correctly expand tildes and environment variables in paths passed to <code>--config</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10219">#10219</a>)</li>
</ul>
<h3>Configuration</h3>
<ul>
<li>Accept a PEP 440 version specifier for <code>required-version</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10216">#10216</a>)</li>
<li>Implement isort's <code>default-section</code> setting (<a href="https://redirect.github.com/astral-sh/ruff/pull/10149">#10149</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Remove trailing space from <code>CapWords</code> message (<a href="https://redirect.github.com/astral-sh/ruff/pull/10220">#10220</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/a892fc755d6d4342c2f5a768aa50a401d704ae2c"><code>a892fc7</code></a> Bump version to v0.3.2 (<a href="https://redirect.github.com/astral-sh/ruff/issues/10304">#10304</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/a067d87ccc9a8e0348b1a2421b7879514d4f26c0"><code>a067d87</code></a> Fix incorrect <code>Parameter</code> range  for <code>*args</code> and <code>**kwargs</code>  (<a href="https://redirect.github.com/astral-sh/ruff/issues/10283">#10283</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/b64f2ea40192436639f668f4a342fcb04b0e4071"><code>b64f2ea</code></a> Formatter: Improve single-with item formatting for Python 3.8 or older (<a href="https://redirect.github.com/astral-sh/ruff/issues/10276">#10276</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4bce80106545af8d1edd028c7085a9e9d703fc6b"><code>4bce801</code></a> Fix unstable with-items formatting (<a href="https://redirect.github.com/astral-sh/ruff/issues/10274">#10274</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/a56d42f1839cb9b44f0fc369c441f4d329ed868a"><code>a56d42f</code></a> Refactor with statement formatting to have explicit layouts (<a href="https://redirect.github.com/astral-sh/ruff/issues/10296">#10296</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1d97f2733554c6825c8b4d3e1936d864e0cf4871"><code>1d97f27</code></a> Start tracking quoting style in the AST (<a href="https://redirect.github.com/astral-sh/ruff/issues/10298">#10298</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/965adbed4b56a76d6cce02534e47c4d7a2a9cd32"><code>965adbe</code></a> Fix trailing kwargs end of line comment after slash (<a href="https://redirect.github.com/astral-sh/ruff/issues/10297">#10297</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c504d7ab11308a08d6d91af7d6f47fc3b2ba4165"><code>c504d7a</code></a> Track quoting style in the tokenizer (<a href="https://redirect.github.com/astral-sh/ruff/issues/10256">#10256</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/72c9f7e4c9928ad2714e8ca68c1defe2e778d4f3"><code>72c9f7e</code></a> Include actual conditions in E712 diagnostics (<a href="https://redirect.github.com/astral-sh/ruff/issues/10254">#10254</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/57be3fce900488a9ce1a0187863599ddf1c0d3ed"><code>57be3fc</code></a> Treat <code>typing.Annotated</code> subscripts as type definitions (<a href="https://redirect.github.com/astral-sh/ruff/issues/10285">#10285</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.1.15...v0.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.1.15&new-version=0.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-03-11 04:13:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/249" class=".btn">#249</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump pytest-ruff from 0.1.1 to 0.3.1 in /rpc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-ruff](https://github.com/businho/pytest-ruff) from 0.1.1 to 0.3.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/businho/pytest-ruff/releases">pytest-ruff's releases</a>.</em></p>
<blockquote>
<h2>Add support to pytest 8.1.x</h2>
<p>No release notes provided.</p>
<h2>Support old pytest versions</h2>
<p>No release notes provided.</p>
<h2>Fix previous messed up release</h2>
<p>It makes <code>--ruff</code> and <code>--ruff-format</code> work independently and make the plugin work again.</p>
<h2>Support ruff format and respect exclude config</h2>
<p>No release notes provided.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/businho/pytest-ruff/commit/9efc242a519f8c7648bc732a170079864b592521"><code>9efc242</code></a> fix: pytest 8.1 compat (<a href="https://redirect.github.com/businho/pytest-ruff/issues/16">#16</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/41ec4c4cc327aa3c5f86f466025dc53bee29304d"><code>41ec4c4</code></a> Silence some deprecation warnings for Python 3.14</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/ef9d0e0bc173dac03f1af954f9a9d3574203a64e"><code>ef9d0e0</code></a> Fail tests with warnings</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/37b8e736063f61ca4b5118ac499ee63fb3943b17"><code>37b8e73</code></a> Support old pytests (<a href="https://redirect.github.com/businho/pytest-ruff/issues/13">#13</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/463bb48aed573d28b63b00e81f317ffcf0c2cbf9"><code>463bb48</code></a> Fix cov (<a href="https://redirect.github.com/businho/pytest-ruff/issues/14">#14</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/8a6a5a32602cd4936029ddae1bda4ce899b8d98f"><code>8a6a5a3</code></a> Run tox with 3.12 and drop 3.7</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/1ef9b2244f6dc63be9fefeef909092e4cf50c9a1"><code>1ef9b22</code></a> Merge pull request <a href="https://redirect.github.com/businho/pytest-ruff/issues/10">#10</a> from cclauss/patch-1</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/951ece4fff3c07d9be59ab1dcb64bf7e7ad49130"><code>951ece4</code></a> Upgrade GitHub Actions and add Python 3.12</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/2098829cfb8f95c2885c6dec3e229ed3092e2c1e"><code>2098829</code></a> Merge pull request <a href="https://redirect.github.com/businho/pytest-ruff/issues/8">#8</a> from skellys/fix/fix_v0_2</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/3e0cfef09777aff7411aad2bf50f89b8b4a72a62"><code>3e0cfef</code></a> Fix tests</li>
<li>Additional commits viewable in <a href="https://github.com/businho/pytest-ruff/compare/v0.1.1...v0.3.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-ruff&package-manager=pip&previous-version=0.1.1&new-version=0.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-03-11 04:12:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/248" class=".btn">#248</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump pytest-asyncio from 0.14.0 to 0.23.5.post1 in /rpc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.14.0 to 0.23.5.post1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.5.post1</h2>
<h1>0.23.5 (2024-02-09)</h1>
<ul>
<li>Declare compatibility with pytest 8 <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/737">#737</a></li>
<li>Fix typing errors with recent versions of mypy <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/769">#769</a></li>
<li>Prevent DeprecationWarning about internal use of <code>asyncio.get_event_loop()</code> from affecting test cases <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/757">#757</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
<h2>pytest-asyncio 0.23.5</h2>
<h1>0.23.5 (2024-02-09)</h1>
<ul>
<li>Declare compatibility with pytest 8 <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/737">#737</a></li>
<li>Fix typing errors with recent versions of mypy <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/769">#769</a></li>
<li>Prevent DeprecationWarning about internal use of <code>asyncio.get_event_loop()</code> from affecting test cases <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/757">#757</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
<h2>pytest-asyncio 0.23.5a0</h2>
<h1>0.23.5 (UNRELEASED)</h1>
<ul>
<li>Declare compatibility with pytest 8 <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/737">#737</a></li>
<li>Fix typing errors with recent versions of mypy <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/769">#769</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
<h2>pytest-asyncio 0.23.4</h2>
<h1>0.23.4 (2024-01-28)</h1>
<ul>
<li>pytest-asyncio no longer imports additional, unrelated packages during test collection <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/729">#729</a></li>
<li>Addresses further issues that caused an internal pytest error during test collection</li>
<li>Declares incompatibility with pytest 8 <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/737">#737</a></li>
</ul>
<h2>pytest-asyncio 0.23.4a2</h2>
<h1>0.23.4 (UNRELEASED)</h1>
<ul>
<li>pytest-asyncio no longer imports additional, unrelated packages during test collection <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/729">#729</a></li>
<li>Addresses further issues that caused an internal pytest error during test collection</li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
<h2>pytest-asyncio 0.23.4a1</h2>
<h1>0.23.4 (UNRELEASED)</h1>
<ul>
<li>pytest-asyncio no longer imports additional, unrelated packages during test collection <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/729">#729</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
<h2>pytest-asyncio 0.23.4a0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b22d84e1f0d53920352be4c66d1b6c7f7a9ce005"><code>b22d84e</code></a> [docs] Fixes the example showing how to run all tests in a session-scoped loop.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/f1de446a37b426f5882b103d5c2fd2f3045b1f01"><code>f1de446</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b60649a648912a79ce6f3443ca7ac2c67fe9a5b7"><code>b60649a</code></a> Build(deps): Bump urllib3 from 2.2.0 to 2.2.1 in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4baec47b8514b405e97a14a1d6c42fa07af8fb0a"><code>4baec47</code></a> Build(deps): Bump typing-extensions in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d44e3ac013cb3b6736492d3f920fb8820f3c8bbf"><code>d44e3ac</code></a> Build(deps): Bump pytest from 8.0.0 to 8.0.2 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/cefa62e7d007b5aa0add7bd58a3e33f246daee71"><code>cefa62e</code></a> Build(deps): Bump coverage from 7.4.1 to 7.4.3 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/290886063f1da8ec1865cd2cdae721b0ebb89edf"><code>2908860</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/20bd7d87bec30ee49a2ec1adc8df8857fc0a69ac"><code>20bd7d8</code></a> Build(deps): Bump pypa/gh-action-pypi-publish from 1.8.11 to 1.8.12</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3aef60532f2a1c634af5f4539eabdd4fbfffcabc"><code>3aef605</code></a> [build] Update actions/upload-artifact and actions/download-artifact to v4.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4b1908d9ed26895c194a4bb8d4c61cef2dfc5067"><code>4b1908d</code></a> [fix] Prevent DeprecationWarning from bubbling to user code.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.14.0...v0.23.5.post1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.14.0&new-version=0.23.5.post1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-03-11 04:12:13 +0000 UTC
    </div>
</div>

