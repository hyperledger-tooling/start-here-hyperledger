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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3081" class=".btn">#3081</a>
            </td>
            <td>
                <b>
                    Add by_format to terse webhook for presentations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix for issue #3065

Note that this is for the 2.0 presentation protocol only, do we need to apply a similar fix for 1.0?

This adds the `by_format` attribute for all webhooks, not just for status `done`, however the demo requires this to work with terse webhooks (and no additional calls to the api endpoints)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-03 17:21:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3080" class=".btn">#3080</a>
            </td>
            <td>
                <b>
                    Switch from black to ruff
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Completely removes black from the project in favour of ruff for linting and formatting.

***Note*** there's a few things failing right now because they are linting issues. They are fixed in the Rule D437 PR.

Adjust the decontainer and the github actions workflow.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-03 02:14:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3077" class=".btn">#3077</a>
            </td>
            <td>
                <b>
                    fix: print provision messages when auto-provision is triggered
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It was recently discovered that if you set a static seed, and you have auto-provisioning enabled on the start command, there is no way to get the verkey for the created DID. The verkey is never printed out to the command line and I do not remember there being an API for retrieving the verkey (one of those, "See it once, copy it, or forever lose it" kinds of things).

After this point in the code, the only thing that "provision" enables are the print statements talking about the did/verkey being created as well as some basic profile information. It doesn't trigger any code that would make changes to the system, those lines precede the line I've added.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-02 15:39:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3076" class=".btn">#3076</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump requests from 2.32.2 to 2.32.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [requests](https://github.com/psf/requests) from 2.32.2 to 2.32.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/releases">requests's releases</a>.</em></p>
<blockquote>
<h2>v2.32.3</h2>
<h2>2.32.3 (2024-05-29)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Fixed bug breaking the ability to specify custom SSLContexts in sub-classes of
HTTPAdapter. (<a href="https://redirect.github.com/psf/requests/issues/6716">#6716</a>)</li>
<li>Fixed issue where Requests started failing to run on Python versions compiled
without the <code>ssl</code> module. (<a href="https://redirect.github.com/psf/requests/issues/6724">#6724</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/blob/main/HISTORY.md">requests's changelog</a>.</em></p>
<blockquote>
<h2>2.32.3 (2024-05-29)</h2>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Fixed bug breaking the ability to specify custom SSLContexts in sub-classes of
HTTPAdapter. (<a href="https://redirect.github.com/psf/requests/issues/6716">#6716</a>)</li>
<li>Fixed issue where Requests started failing to run on Python versions compiled
without the <code>ssl</code> module. (<a href="https://redirect.github.com/psf/requests/issues/6724">#6724</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/requests/commit/0e322af87745eff34caffe4df68456ebc20d9068"><code>0e322af</code></a> v2.32.3</li>
<li><a href="https://github.com/psf/requests/commit/e18879932287c2bf4bcee4ddf6ccb8a69b6fc656"><code>e188799</code></a> Don't create default SSLContext if ssl module isn't present (<a href="https://redirect.github.com/psf/requests/issues/6724">#6724</a>)</li>
<li><a href="https://github.com/psf/requests/commit/145b5399486b56e00250204f033441f3fdf2f3c9"><code>145b539</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6716">#6716</a> from sigmavirus24/bug/6715</li>
<li><a href="https://github.com/psf/requests/commit/b1d73ddb509a3a2d3e10744e85f9cdebdbde90f0"><code>b1d73dd</code></a> Don't use default SSLContext with custom poolmanager kwargs</li>
<li><a href="https://github.com/psf/requests/commit/6badbac6e0d6b5a53872f26401761ad37a9002b8"><code>6badbac</code></a> Update HISTORY.md</li>
<li><a href="https://github.com/psf/requests/commit/a62a2d35d918baa8e793f7aa4fb41527644dfca5"><code>a62a2d3</code></a> Allow for overriding of specific pool key params</li>
<li>See full diff in <a href="https://github.com/psf/requests/compare/v2.32.2...v2.32.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=requests&package-manager=pip&previous-version=2.32.2&new-version=2.32.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-01 12:02:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3075" class=".btn">#3075</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump uuid-utils from 0.8.0 to 0.9.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [uuid-utils](https://github.com/aminalaee/uuid-utils) from 0.8.0 to 0.9.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/aminalaee/uuid-utils/releases">uuid-utils's releases</a>.</em></p>
<blockquote>
<h2>Version 0.9.0</h2>
<h3>What's Changed</h3>
<ul>
<li>Upgrade <code>uuid</code> to <code>1.9.1</code> and <code>pyo3</code> to <code>0.22.0</code> in <a href="https://redirect.github.com/aminalaee/uuid-utils/pull/60">aminalaee/uuid-utils#60</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/aminalaee/uuid-utils/compare/0.8.0...0.9.0">https://github.com/aminalaee/uuid-utils/compare/0.8.0...0.9.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/aminalaee/uuid-utils/commit/a80fb4f838158c5c4b6e821c93977a74a29a05ab"><code>a80fb4f</code></a> Version 0.9.0 (<a href="https://redirect.github.com/aminalaee/uuid-utils/issues/61">#61</a>)</li>
<li><a href="https://github.com/aminalaee/uuid-utils/commit/21b455c36399baed29cf060a23b74c3140a676c4"><code>21b455c</code></a> Upgrade dependencies (<a href="https://redirect.github.com/aminalaee/uuid-utils/issues/60">#60</a>)</li>
<li>See full diff in <a href="https://github.com/aminalaee/uuid-utils/compare/0.8.0...0.9.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=uuid-utils&package-manager=pip&previous-version=0.8.0&new-version=0.9.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-01 12:02:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3074" class=".btn">#3074</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump mike from 2.0.0 to 2.1.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [mike](https://github.com/jimporter/mike) from 2.0.0 to 2.1.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/jimporter/mike/releases">mike's releases</a>.</em></p>
<blockquote>
<h2>v2.1.2</h2>
<h3>Bug fixes</h3>
<ul>
<li>Remove ambiguity of some Git commands so that file and branch names don't collide</li>
</ul>
<h2>v2.1.1</h2>
<h3>Bug fixes</h3>
<ul>
<li>Support using environment variables for <code>INHERIT</code> when injecting the <code>mike</code> plugin into <code>mkdocs.yml</code></li>
</ul>
<h2>v2.1.0</h2>
<h3>New features</h3>
<ul>
<li>When calling <code>set-default</code>, you can now pass <code>--allow-undefined</code> to set the default to a version that doesn't exist yet</li>
<li>Add global-level <code>-q</code> / <code>--quiet</code> option to suppress warning messages</li>
<li>Add support for handling <code>!relative</code> in <code>mkdocs.yml</code></li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>When loading an MkDocs config, mike now runs the <code>startup</code> and <code>shutdown</code> events</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/jimporter/mike/blob/master/CHANGES.md">mike's changelog</a>.</em></p>
<blockquote>
<h2>v2.1.2 (2024-06-23)</h2>
<h3>Bug fixes</h3>
<ul>
<li>Remove ambiguity of some Git commands so that file and branch names don't
collide</li>
</ul>
<hr />
<h2>v2.1.1 (2024-05-03)</h2>
<h3>Bug fixes</h3>
<ul>
<li>Support using environment variables for <code>INHERIT</code> when injecting the <code>mike</code>
plugin into <code>mkdocs.yml</code></li>
</ul>
<hr />
<h2>v2.1.0 (2024-05-01)</h2>
<h3>New features</h3>
<ul>
<li>When calling <code>set-default</code>, you can now pass <code>--allow-undefined</code> to set the
default to a version that doesn't exist yet</li>
<li>Add global-level <code>-q</code> / <code>--quiet</code> option to suppress warning messages</li>
<li>Add support for handling <code>!relative</code> in <code>mkdocs.yml</code></li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>When loading an MkDocs config, mike now runs the <code>startup</code> and <code>shutdown</code>
events</li>
</ul>
<hr />
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jimporter/mike/commit/62aaeafe60927b0653b319585cbe4a1a1eb1bc23"><code>62aaeaf</code></a> Update version to 2.1.2</li>
<li><a href="https://github.com/jimporter/mike/commit/3f7d756e26fca03660e6f08927c7cd911e933c78"><code>3f7d756</code></a> Use &quot;--&quot; to disambiguate Git arguments in a few more places; resolves <a href="https://redirect.github.com/jimporter/mike/issues/218">#218</a></li>
<li><a href="https://github.com/jimporter/mike/commit/5e6970d65beaf2c92fa1d22dbf524a931a393e8b"><code>5e6970d</code></a> Belatedly update copyright year</li>
<li><a href="https://github.com/jimporter/mike/commit/9291efbd6961d652c16c000dc1fe4f2f1e19f94c"><code>9291efb</code></a> Update version to 2.2.0.dev0</li>
<li><a href="https://github.com/jimporter/mike/commit/0bdfe24c20fb0774652230a7abe8466b98098da4"><code>0bdfe24</code></a> Update version to 2.1.1</li>
<li><a href="https://github.com/jimporter/mike/commit/3351d5feabff8ee107f4ad6d1f86055843c7dbf1"><code>3351d5f</code></a> Expand environment variables when injecting the mike plugin; resolves <a href="https://redirect.github.com/jimporter/mike/issues/217">#217</a></li>
<li><a href="https://github.com/jimporter/mike/commit/e4d83eda046b1dea0493f91fcacbf86634c93db5"><code>e4d83ed</code></a> Update version to 2.2.0.dev0</li>
<li><a href="https://github.com/jimporter/mike/commit/6e6cfbb9a3e78d2ab2a529b72b84e8918c101f6c"><code>6e6cfbb</code></a> Update version to 2.1.0</li>
<li><a href="https://github.com/jimporter/mike/commit/5773be928d1a6e99e61755df0d73a8b2ce16660f"><code>5773be9</code></a> Fix CI</li>
<li><a href="https://github.com/jimporter/mike/commit/7904925595827ccba3908775b2f9b5add3ae9030"><code>7904925</code></a> Further tests for deserializing Python objects during <code>inject_plugin</code></li>
<li>Additional commits viewable in <a href="https://github.com/jimporter/mike/compare/v2.0.0...v2.1.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mike&package-manager=pip&previous-version=2.0.0&new-version=2.1.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-01 12:01:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3073" class=".btn">#3073</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump ruff from 0.4.10 to 0.5.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.4.10 to 0.5.0.
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
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.4.10...0.5.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.4.10&new-version=0.5.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-01 12:01:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3072" class=".btn">#3072</a>
            </td>
            <td>
                <b>
                    Rule D417
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates function documentation to the appropriate level needed for rule D417 https://docs.astral.sh/ruff/rules/undocumented-param/. Helps developers understand and more quickly use functions if these are accurate.

Mostly used co-pilot to fill in wrong or missing arguments. Reviewed most of it and it looked like it was doing a good job.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-28 19:59:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3070" class=".btn">#3070</a>
            </td>
            <td>
                <b>
                    Re-enable ledger plugin when `--no-legder` is set
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @ff137 @jamshale [in response to this](https://github.com/hyperledger/aries-cloudagent-python/pull/2990#discussion_r1654980350)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-28 02:40:07 +0000 UTC
    </div>
</div>

