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
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/291" class=".btn">#291</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump pytest-asyncio from 0.14.0 to 0.23.6 in /basicmessage_storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.14.0 to 0.23.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.6</h2>
<h1>0.23.6 (2024-03-19)</h1>
<ul>
<li>Fix compatibility with pytest 8.2 <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/pull/800">#800</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/c34da04b82153ce052109bad31ccdbc0be7938e1"><code>c34da04</code></a> [docs] Mentioned pytest 8.2 compatibility fix in changelog.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/143f745d279afc070cf5cf6144fbf34d960fae72"><code>143f745</code></a> Fix compatibility with pytest 8.2 FixtureDef.unittest removal</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/13d4b79f7ff0d9d0ea70880b3276f85dea7f1f15"><code>13d4b79</code></a> Remove unused function <code>_removesuffix</code></li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/cdd2c4906835b6f627d681fbee5d487554884e5f"><code>cdd2c49</code></a> Use <code>FixtureRequest</code> instead of <code>SubRequest</code></li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/c3429fa4d72239be9b428342f0f1407e0840b9ec"><code>c3429fa</code></a> Build(deps): Bump packaging from 23.2 to 24.0 in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/5f2338dfc9f9b5ac2c27d3bef490fa3e2cd7c156"><code>5f2338d</code></a> Build(deps): Bump pypa/gh-action-pypi-publish from 1.8.12 to 1.8.14</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/726c6e0f3c185f10d8a842bcd1d781de32a3b2f5"><code>726c6e0</code></a> Build(deps): Bump coverage from 7.4.3 to 7.4.4 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/8bd8288709717165b352c7f2f207c8e4ef624a01"><code>8bd8288</code></a> Build(deps): Bump pytest from 8.0.2 to 8.1.1 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/ef3b3477070d6a270e1bb2c1d438c64dba42724c"><code>ef3b347</code></a> Build(deps): Bump packaging from 23.2 to 24.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b22d84e1f0d53920352be4c66d1b6c7f7a9ce005"><code>b22d84e</code></a> [docs] Fixes the example showing how to run all tests in a session-scoped loop.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.14.0...v0.23.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.14.0&new-version=0.23.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-03-20 04:15:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/290" class=".btn">#290</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump pytest-asyncio from 0.14.0 to 0.23.6 in /rpc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.14.0 to 0.23.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.6</h2>
<h1>0.23.6 (2024-03-19)</h1>
<ul>
<li>Fix compatibility with pytest 8.2 <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/pull/800">#800</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/c34da04b82153ce052109bad31ccdbc0be7938e1"><code>c34da04</code></a> [docs] Mentioned pytest 8.2 compatibility fix in changelog.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/143f745d279afc070cf5cf6144fbf34d960fae72"><code>143f745</code></a> Fix compatibility with pytest 8.2 FixtureDef.unittest removal</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/13d4b79f7ff0d9d0ea70880b3276f85dea7f1f15"><code>13d4b79</code></a> Remove unused function <code>_removesuffix</code></li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/cdd2c4906835b6f627d681fbee5d487554884e5f"><code>cdd2c49</code></a> Use <code>FixtureRequest</code> instead of <code>SubRequest</code></li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/c3429fa4d72239be9b428342f0f1407e0840b9ec"><code>c3429fa</code></a> Build(deps): Bump packaging from 23.2 to 24.0 in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/5f2338dfc9f9b5ac2c27d3bef490fa3e2cd7c156"><code>5f2338d</code></a> Build(deps): Bump pypa/gh-action-pypi-publish from 1.8.12 to 1.8.14</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/726c6e0f3c185f10d8a842bcd1d781de32a3b2f5"><code>726c6e0</code></a> Build(deps): Bump coverage from 7.4.3 to 7.4.4 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/8bd8288709717165b352c7f2f207c8e4ef624a01"><code>8bd8288</code></a> Build(deps): Bump pytest from 8.0.2 to 8.1.1 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/ef3b3477070d6a270e1bb2c1d438c64dba42724c"><code>ef3b347</code></a> Build(deps): Bump packaging from 23.2 to 24.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/b22d84e1f0d53920352be4c66d1b6c7f7a9ce005"><code>b22d84e</code></a> [docs] Fixes the example showing how to run all tests in a session-scoped loop.</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.14.0...v0.23.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.14.0&new-version=0.23.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-03-20 04:11:16 +0000 UTC
    </div>
</div>

