---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3117" class=".btn">#3117</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump pytest-asyncio from 0.23.7 to 0.23.8 in /demo/playground/examples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.23.7 to 0.23.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.8</h2>
<h1>0.23.8 (2024-07-17)</h1>
<ul>
<li>Fixes a bug that caused duplicate markers in async tests <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/813">#813</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4be86a5174f864f6098872fc9fdf0a557a1b50f8"><code>4be86a5</code></a> docs: Prepare release of v0.23.8.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/74b3a0a2057b6faaaf2dfc2d1de785abcf145bcb"><code>74b3a0a</code></a> Build(deps): Bump exceptiongroup in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b0009ca36ad66ec0bf40b2ad97edaa96fa39e510"><code>b0009ca</code></a> [build] Declare support for Python 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/c747c7db7837d7cb7fef029af92092e20759e217"><code>c747c7d</code></a> Build(deps): Bump coverage from 7.5.4 to 7.6.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/5c40a1cf8b6f47f47596fcf1117420585517c627"><code>5c40a1c</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b735e8a8ef3118109521c7b058596cf7decb03d0"><code>b735e8a</code></a> build: Remove development dependency on Docker.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/91171b41c2bd6714955cd3d72e07bd9091f909e2"><code>91171b4</code></a> ci: Test with CPython 3.13.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/d572138e097f493c07c84151649d191df5e09ee0"><code>d572138</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/a89e4d7a899d7587e1efa6cafe9e181b3e2a1d69"><code>a89e4d7</code></a> Build(deps): Bump certifi in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b646cc18a222c8043433c38a42c07245fe9735ce"><code>b646cc1</code></a> [fix] Fixed a bug that causes markers to be duplicated for async test functions.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.23.7...v0.23.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.23.7&new-version=0.23.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:30:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3115" class=".btn">#3115</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump pytest from 8.2.2 to 8.3.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.2 to 8.3.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.3.1</h2>
<h1>pytest 8.3.1 (2024-07-20)</h1>
<p>The 8.3.0 release failed to include the change notes and docs for the release. This patch release remedies this. There are no other changes.</p>
<h2>8.3.0</h2>
<h1>pytest 8.3.0 (2024-07-20)</h1>
<h2>New features</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12231">#12231</a>: Added [--xfail-tb]{.title-ref} flag, which turns on traceback output for XFAIL results.</p>
<ul>
<li>If the [--xfail-tb]{.title-ref} flag is not given, tracebacks for XFAIL results are NOT shown.</li>
<li>The style of traceback for XFAIL is set with [--tb]{.title-ref}, and can be [auto|long|short|line|native|no]{.title-ref}.</li>
<li>Note: Even if you have [--xfail-tb]{.title-ref} set, you won't see them if [--tb=no]{.title-ref}.</li>
</ul>
<p>Some history:</p>
<p>With pytest 8.0, [-rx]{.title-ref} or [-ra]{.title-ref} would not only turn on summary reports for xfail, but also report the tracebacks for xfail results. This caused issues with some projects that utilize xfail, but don't want to see all of the xfail tracebacks.</p>
<p>This change detaches xfail tracebacks from [-rx]{.title-ref}, and now we turn on xfail tracebacks with [--xfail-tb]{.title-ref}. With this, the default [-rx]{.title-ref}/ [-ra]{.title-ref} behavior is identical to pre-8.0 with respect to xfail tracebacks. While this is a behavior change, it brings default behavior back to pre-8.0.0 behavior, which ultimately was considered the better course of action.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12281">#12281</a>: Added support for keyword matching in marker expressions.</p>
<p>Now tests can be selected by marker keyword arguments.
Supported values are <code>int</code>{.interpreted-text role=&quot;class&quot;}, (unescaped) <code>str</code>{.interpreted-text role=&quot;class&quot;}, <code>bool</code>{.interpreted-text role=&quot;class&quot;} &amp; <code>None</code>{.interpreted-text role=&quot;data&quot;}.</p>
<p>See <code>marker examples &lt;marker_keyword_expression_example&gt;</code>{.interpreted-text role=&quot;ref&quot;} for more information.</p>
<p>-- by <code>lovetheguitar</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12567">#12567</a>: Added <code>--no-fold-skipped</code> command line option.</p>
<p>If this option is set, then skipped tests in short summary are no longer grouped
by reason but all tests are printed individually with their nodeid in the same
way as other statuses.</p>
<p>-- by <code>pbrezina</code>{.interpreted-text role=&quot;user&quot;}</p>
</li>
</ul>
<h2>Improvements in existing functionality</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12469">#12469</a>: The console output now uses the &quot;third-party plugins&quot; terminology,
replacing the previously established but confusing and outdated
reference to <code>setuptools &lt;setuptools:index&gt;</code>{.interpreted-text role=&quot;std:doc&quot;}
-- by <code>webknjaz</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12544">#12544</a>, <a href="https://redirect.github.com/pytest-dev/pytest/issues/12545">#12545</a>: Python virtual environment detection was improved by
checking for a <code>pyvenv.cfg</code>{.interpreted-text role=&quot;file&quot;} file, ensuring reliable detection on
various platforms -- by <code>zachsnickers</code>{.interpreted-text role=&quot;user&quot;}.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/de98446075cc07c768387cf64ba497dd75c205de"><code>de98446</code></a> Prepare release version 8.3.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bd0a0424037825bc23b9bf299115e92c53a67a9c"><code>bd0a042</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12636">#12636</a> from pytest-dev/update-release-notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/664325bc9fd90217f51fe7cc0e9fff2f29a41a15"><code>664325b</code></a> doc/changelog: update 8.3.0 notes</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/19d225d0ab0f586a9a1fc878dff871495c12bd06"><code>19d225d</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12635">#12635</a> from pytest-dev/release-8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bc3302850c52ec945eea1b2bbde7ec3b91fc3e44"><code>bc33028</code></a> Prepare release version 8.3.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/a7d5a8eba9addd119432fa71880b51052a89812f"><code>a7d5a8e</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12557">#12557</a> from x612skm/maintainence/11771-pypy-3.9-bump</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/ced7072bb4f7653ad2f1d0d33639d87e7bc5f358"><code>ced7072</code></a> Add a change note for PR <a href="https://redirect.github.com/pytest-dev/pytest/issues/11771">#11771</a></li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d42b76daadb88d993ee74753766e22711a27395f"><code>d42b76d</code></a> Adjust test_errors_in_xfail_skip_expressions for PyPy</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/9eee45a7479cf5fa23b79057708a994a3b8d0eee"><code>9eee45a</code></a> Bump PyPy runtime to v3.9 @ GHA</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d489247505a953885a156e61d4473497cbc167ea"><code>d489247</code></a> Fix caching of parameterized fixtures (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12600">#12600</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.2...8.3.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.2&new-version=8.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:14:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3114" class=".btn">#3114</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump ruff from 0.5.2 to 0.5.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.5.2 to 0.5.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>0.5.4</h2>
<h2>Release Notes</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>ruff</code>] Rename <code>RUF007</code> to <code>zip-instead-of-pairwise</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12399">#12399</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-builtins</code>] Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/pull/12415">#12415</a>)</li>
<li>[<code>flake8-comprehensions</code>] Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12422">#12422</a>)</li>
<li>[<code>pydocstyle</code>] Handle escaped docstrings within docstring (<code>D301</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12192">#12192</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Fix GitHub link to Neovim setup (<a href="https://redirect.github.com/astral-sh/ruff/pull/12410">#12410</a>)</li>
<li>Fix <code>output-format</code> default in settings reference (<a href="https://redirect.github.com/astral-sh/ruff/pull/12409">#12409</a>)</li>
</ul>
<h2>Install ruff 0.5.4</h2>
<h3>Install prebuilt binaries via shell script</h3>
<pre lang="sh"><code>curl --proto '=https' --tlsv1.2 -LsSf https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-installer.sh | sh
</code></pre>
<h3>Install prebuilt binaries via powershell script</h3>
<pre lang="sh"><code>powershell -c &quot;irm https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-installer.ps1 | iex&quot;
</code></pre>
<h2>Download ruff 0.5.4</h2>
<table>
<thead>
<tr>
<th>File</th>
<th>Platform</th>
<th>Checksum</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-apple-darwin.tar.gz">ruff-aarch64-apple-darwin.tar.gz</a></td>
<td>Apple Silicon macOS</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-apple-darwin.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-apple-darwin.tar.gz">ruff-x86_64-apple-darwin.tar.gz</a></td>
<td>Intel macOS</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-apple-darwin.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-pc-windows-msvc.zip">ruff-aarch64-pc-windows-msvc.zip</a></td>
<td>ARM64 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-pc-windows-msvc.zip">ruff-i686-pc-windows-msvc.zip</a></td>
<td>x86 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-pc-windows-msvc.zip">ruff-x86_64-pc-windows-msvc.zip</a></td>
<td>x64 Windows</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-pc-windows-msvc.zip.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-gnu.tar.gz">ruff-aarch64-unknown-linux-gnu.tar.gz</a></td>
<td>ARM64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-gnu.tar.gz">ruff-i686-unknown-linux-gnu.tar.gz</a></td>
<td>x86 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64-unknown-linux-gnu.tar.gz">ruff-powerpc64-unknown-linux-gnu.tar.gz</a></td>
<td>PPC64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64le-unknown-linux-gnu.tar.gz">ruff-powerpc64le-unknown-linux-gnu.tar.gz</a></td>
<td>PPC64LE Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-powerpc64le-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-s390x-unknown-linux-gnu.tar.gz">ruff-s390x-unknown-linux-gnu.tar.gz</a></td>
<td>S390x Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-s390x-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-unknown-linux-gnu.tar.gz">ruff-x86_64-unknown-linux-gnu.tar.gz</a></td>
<td>x64 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-x86_64-unknown-linux-gnu.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-armv7-unknown-linux-gnueabihf.tar.gz">ruff-armv7-unknown-linux-gnueabihf.tar.gz</a></td>
<td>ARMv7 Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-armv7-unknown-linux-gnueabihf.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-musl.tar.gz">ruff-aarch64-unknown-linux-musl.tar.gz</a></td>
<td>ARM64 MUSL Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-aarch64-unknown-linux-musl.tar.gz.sha256">checksum</a></td>
</tr>
<tr>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-musl.tar.gz">ruff-i686-unknown-linux-musl.tar.gz</a></td>
<td>x86 MUSL Linux</td>
<td><a href="https://github.com/astral-sh/ruff/releases/download/0.5.4/ruff-i686-unknown-linux-musl.tar.gz.sha256">checksum</a></td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.5.4</h2>
<h3>Rule changes</h3>
<ul>
<li>[<code>ruff</code>] Rename <code>RUF007</code> to <code>zip-instead-of-pairwise</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/12399">#12399</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-builtins</code>] Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/pull/12415">#12415</a>)</li>
<li>[<code>flake8-comprehensions</code>] Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/pull/12422">#12422</a>)</li>
<li>[<code>pydocstyle</code>] Handle escaped docstrings within docstring (<code>D301</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12192">#12192</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Fix GitHub link to Neovim setup (<a href="https://redirect.github.com/astral-sh/ruff/pull/12410">#12410</a>)</li>
<li>Fix <code>output-format</code> default in settings reference (<a href="https://redirect.github.com/astral-sh/ruff/pull/12409">#12409</a>)</li>
</ul>
<h2>0.5.3</h2>
<p><strong>Ruff 0.5.3 marks the stable release of the Ruff language server and introduces revamped
<a href="https://docs.astral.sh/ruff/editors">documentation</a>, including <a href="https://docs.astral.sh/ruff/editors/setup">setup guides for your editor of
choice</a> and <a href="https://docs.astral.sh/ruff/editors/settings">the language server
itself</a></strong>.</p>
<h3>Preview features</h3>
<ul>
<li>Formatter: Insert empty line between suite and alternative branch after function/class definition (<a href="https://redirect.github.com/astral-sh/ruff/pull/12294">#12294</a>)</li>
<li>[<code>pyupgrade</code>] Implement <code>unnecessary-default-type-args</code> (<code>UP043</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12371">#12371</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Detect enumerate iterations in <code>loop-iterator-mutation</code> (<code>B909</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12366">#12366</a>)</li>
<li>[<code>flake8-bugbear</code>] Remove <code>discard</code>, <code>remove</code>, and <code>pop</code> allowance for <code>loop-iterator-mutation</code> (<code>B909</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12365">#12365</a>)</li>
<li>[<code>pylint</code>] Allow <code>repeated-equality-comparison</code> for mixed operations (<code>PLR1714</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12369">#12369</a>)</li>
<li>[<code>pylint</code>] Ignore <code>self</code> and <code>cls</code> when counting arguments (<code>PLR0913</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12367">#12367</a>)</li>
<li>[<code>pylint</code>] Use UTF-8 as default encoding in <code>unspecified-encoding</code> fix (<code>PLW1514</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12370">#12370</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Build settings index in parallel for the native server (<a href="https://redirect.github.com/astral-sh/ruff/pull/12299">#12299</a>)</li>
<li>Use fallback settings when indexing the project (<a href="https://redirect.github.com/astral-sh/ruff/pull/12362">#12362</a>)</li>
<li>Consider <code>--preview</code> flag for <code>server</code> subcommand for the linter and formatter (<a href="https://redirect.github.com/astral-sh/ruff/pull/12208">#12208</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-comprehensions</code>] Allow additional arguments for <code>sum</code> and <code>max</code> comprehensions (<code>C419</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12364">#12364</a>)</li>
<li>[<code>pylint</code>] Avoid dropping extra boolean operations in <code>repeated-equality-comparison</code> (<code>PLR1714</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12368">#12368</a>)</li>
<li>[<code>pylint</code>] Consider expression before statement when determining binding kind (<code>PLR1704</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/12346">#12346</a>)</li>
</ul>
<h3>Documentation</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/53b84ab05460d006b10e035fd6a4ffb62d9b608a"><code>53b84ab</code></a> Cleanup redundant spaces from changelog (<a href="https://redirect.github.com/astral-sh/ruff/issues/12424">#12424</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/3664f85f4505b502a83af5abf01265582471d3f1"><code>3664f85</code></a> Bump version to v0.5.4 (<a href="https://redirect.github.com/astral-sh/ruff/issues/12423">#12423</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2c1926beeb145bcae42ff8d63a5f95e2eb9331d3"><code>2c1926b</code></a> Insert parentheses for multi-argument generators (<a href="https://redirect.github.com/astral-sh/ruff/issues/12422">#12422</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/4bcc96ae514127a1a1bece13f55d0409d98bbf68"><code>4bcc96a</code></a> Avoid shadowing diagnostics for <code>@override</code> methods (<a href="https://redirect.github.com/astral-sh/ruff/issues/12415">#12415</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c0a2b49bacfed394f4668cdf4ec3c97ee72db374"><code>c0a2b49</code></a> Fix the Github link error for Neovim in the setup for editors in the docs. (#...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/ca2224862882e73d40ebfe8fe3f99312b013a3e9"><code>ca22248</code></a> Update docs Settings output-format default (<a href="https://redirect.github.com/astral-sh/ruff/issues/12409">#12409</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d8cf8ac2ef26bb630b43b095f61662173b2bac2f"><code>d8cf8ac</code></a> [red-knot] Resolve symbols from <code>builtins.pyi</code> in the stdlib if they cannot b...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1c7b84059e5490b5c0a9f4658975559e5372a6ba"><code>1c7b840</code></a> [red-knot] fix incremental benchmark (<a href="https://redirect.github.com/astral-sh/ruff/issues/12400">#12400</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/f82bb675556097c5d99a62ad6b3b4c19023a96ae"><code>f82bb67</code></a> [red-knot] trace file when inferring types (<a href="https://redirect.github.com/astral-sh/ruff/issues/12401">#12401</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/5f96f69151568da8300fe6d3bf513ae4da3ee6ba"><code>5f96f69</code></a> [red-knot] Fix bug where module resolution would not be invalidated if an ent...</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/0.5.2...0.5.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.5.2&new-version=0.5.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:14:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3113" class=".btn">#3113</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump pytest-ruff from 0.4.0 to 0.4.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-ruff](https://github.com/businho/pytest-ruff) from 0.4.0 to 0.4.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/businho/pytest-ruff/releases">pytest-ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix pytest without cache <code>-pno:cacheprovider</code> by <a href="https://github.com/iurisilvio"><code>@​iurisilvio</code></a> in <a href="https://redirect.github.com/businho/pytest-ruff/pull/29">businho/pytest-ruff#29</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/businho/pytest-ruff/compare/v0.4.0...v0.4.1">https://github.com/businho/pytest-ruff/compare/v0.4.0...v0.4.1</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/businho/pytest-ruff/commit/0a0794e56f93f5f9358ad4972e9f4dd95c25104e"><code>0a0794e</code></a> Fix pytest without cache <code>-pno:cacheprovider</code> (<a href="https://redirect.github.com/businho/pytest-ruff/issues/29">#29</a>)</li>
<li>See full diff in <a href="https://github.com/businho/pytest-ruff/compare/v0.4.0...v0.4.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-ruff&package-manager=pip&previous-version=0.4.0&new-version=0.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-22 11:13:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3112" class=".btn">#3112</a>
            </td>
            <td>
                <b>
                    fix: multiuse invites with did peer 4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This corrects an issue where did:peer:4 connection records were failing to be resolved on inbound message, resulting in the multiuse invitation that created the connection being resolved instead.

Fixes #3111.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-21 19:51:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3110" class=".btn">#3110</a>
            </td>
            <td>
                <b>
                    DOC: Verifiable Credential Data Integrity (VC-DI) Credentials in Aries Cloud Agent Python (ACA-Py) #2947
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-19 12:47:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3109" class=".btn">#3109</a>
            </td>
            <td>
                <b>
                    Add descriptive error for issuance without RevRegRecord
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This just raises an exception with a descriptive message when revocable credential issuance is attempted but there is no RevRegRecord in the issuer wallet.

Can happen when there is issues with the tails server.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-18 22:09:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3107" class=".btn">#3107</a>
            </td>
            <td>
                <b>
                    Breaking: Fix publishing multiple rev reg defs with endorsement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes a bug/mistake when publishing revocations from multiple rev_reg_defs with endorsement. The endorsement process was occurring outside the manager and only considering the last rev_reg_def pre-endorsement result.

***Note:*** This would be considered a breaking change if a controller was reading and processing the response. It is now an array instead of an object. This should have been the response from the beginning as you can request a list, you should return a list. Could be a nested object instead if that's preferable.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-18 18:00:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3106" class=".btn">#3106</a>
            </td>
            <td>
                <b>
                    Fix the check for vc_di proof
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix the error that is getting raised in AATH.  (Double checked and the AATH tests will now pass.)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-17 18:15:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3105" class=".btn">#3105</a>
            </td>
            <td>
                <b>
                    Make single wallet config more explicit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This changes some naming and configuration to make the multitenant single wallet vs multi wallet settings and usage more clear. Askar wallets can use either the basic manager `MultitenantManager` which is used by default and creates a DB/wallet for each tenant. Or, it can use the `AskarProfileMultitenantManager` to create subwallets in a single DB/wallet. This has been renamed to `SingleWalletAskarMultitenantManager` for clarity, and the config changed to `multitenancy-config: '{"wallet_type": "single-wallet-askar"}'` from `multitenancy-config: '{"wallet_type": "askar-profile"}'`

Also fixed an issue with the upgrade check during startup that was using the base manager before initialization and creating subwallet db's on restart when in single wallet mode. I'm looking into this more because the `BaseMultitenantManager` is injected in many other places. Need to make sure they are also using the correct manager via the `MultitenantManagerProvider`.

Added some documentation in `Multitenancy.md`

***Note:*** the multitenant_provider plugin needs to be update because it inherits this class. Already done in my forked repo. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-17 17:32:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3103" class=".btn">#3103</a>
            </td>
            <td>
                <b>
                    Library update 15/07/24 / Fix unit test typing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes some type checking syntax in unit tests. I'm not really sure why these didn't get flagged before or why the command line doesn't seem to pick up these specific errors. They are easy to fix though so I just changed them.

Upgrades ruff, pytest-ruff, portalocer and mkdocs-material
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-15 16:24:54 +0000 UTC
    </div>
</div>

