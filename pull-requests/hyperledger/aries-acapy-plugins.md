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
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/595" class=".btn">#595</a>
            </td>
            <td>
                <b>
                    Bump redis from 5.0.4 to 5.0.5 in /redis_events/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [redis](https://github.com/redis/redis-py) from 5.0.4 to 5.0.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/redis/redis-py/releases">redis's releases</a>.</em></p>
<blockquote>
<h2>5.0.5</h2>
<h1>Changes</h1>
<h2>🐛 Bug Fixes</h2>
<ul>
<li>Fix parsing of INFO response (<a href="https://redirect.github.com/redis/redis-py/issues/3265">#3265</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/redis/redis-py/commit/6f55c0286ccc444204a23e8738117f43c182bf9b"><code>6f55c02</code></a> Bump version to 5.0.5 (<a href="https://redirect.github.com/redis/redis-py/issues/3267">#3267</a>)</li>
<li><a href="https://github.com/redis/redis-py/commit/26d2d13edcf3f29a381df4850c5926cb285d3584"><code>26d2d13</code></a> Fix parsing of INFO response (<a href="https://redirect.github.com/redis/redis-py/issues/3264">#3264</a>)</li>
<li>See full diff in <a href="https://github.com/redis/redis-py/compare/v5.0.4...v5.0.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=redis&package-manager=pip&previous-version=5.0.4&new-version=5.0.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-10 11:19:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/594" class=".btn">#594</a>
            </td>
            <td>
                <b>
                    Bump pytest from 8.2.0 to 8.2.2 in /redis_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.0 to 8.2.2.
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
<h2>8.2.1</h2>
<h1>pytest 8.2.1 (2024-05-19)</h1>
<h2>Improvements</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12334">#12334</a>: Support for Python 3.13 (beta1 at the time of writing).</li>
</ul>
<h2>Bug Fixes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12120">#12120</a>: Fix [PermissionError]{.title-ref} crashes arising from directories which are not selected on the command-line.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12191">#12191</a>: Keyboard interrupts and system exits are now properly handled during the test collection.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12300">#12300</a>: Fixed handling of 'Function not implemented' error under squashfuse_ll, which is a different way to say that the mountpoint is read-only.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12308">#12308</a>: Fix a regression in pytest 8.2.0 where the permissions of automatically-created <code>.pytest_cache</code> directories became <code>rwx------</code> instead of the expected <code>rwxr-xr-x</code>.</li>
</ul>
<h2>Trivial/Internal Changes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12333">#12333</a>: pytest releases are now attested using the recent <a href="https://github.blog/2024-05-02-introducing-artifact-attestations-now-in-public-beta/">Artifact Attestation</a> support from GitHub, allowing users to verify the provenance of pytest's sdist and wheel artifacts.</li>
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
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.0...8.2.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.0&new-version=8.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-10 11:19:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/593" class=".btn">#593</a>
            </td>
            <td>
                <b>
                    Bump redis from 5.0.4 to 5.0.5 in /redis_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [redis](https://github.com/redis/redis-py) from 5.0.4 to 5.0.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/redis/redis-py/releases">redis's releases</a>.</em></p>
<blockquote>
<h2>5.0.5</h2>
<h1>Changes</h1>
<h2>🐛 Bug Fixes</h2>
<ul>
<li>Fix parsing of INFO response (<a href="https://redirect.github.com/redis/redis-py/issues/3265">#3265</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/redis/redis-py/commit/6f55c0286ccc444204a23e8738117f43c182bf9b"><code>6f55c02</code></a> Bump version to 5.0.5 (<a href="https://redirect.github.com/redis/redis-py/issues/3267">#3267</a>)</li>
<li><a href="https://github.com/redis/redis-py/commit/26d2d13edcf3f29a381df4850c5926cb285d3584"><code>26d2d13</code></a> Fix parsing of INFO response (<a href="https://redirect.github.com/redis/redis-py/issues/3264">#3264</a>)</li>
<li>See full diff in <a href="https://github.com/redis/redis-py/compare/v5.0.4...v5.0.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=redis&package-manager=pip&previous-version=5.0.4&new-version=5.0.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-10 11:18:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/592" class=".btn">#592</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.4.5 to 0.4.8 in /redis_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.4.5 to 0.4.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.8</h2>
<h2>Changes</h2>
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
<h3>Server</h3>
<ul>
<li>Formatting a document with syntax problems no longer spams a visible error popup (<a href="https://redirect.github.com/astral-sh/ruff/pull/11745">#11745</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Add RDJson support for <code>--output-format</code> flag (<a href="https://redirect.github.com/astral-sh/ruff/pull/11682">#11682</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>pyupgrade</code>] Write empty string in lieu of panic when fixing <code>UP032</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11696">#11696</a>)</li>
<li>[<code>flake8-simplify</code>] Simplify double negatives in <code>SIM103</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11684">#11684</a>)</li>
<li>Ensure the expression generator adds a newline before <code>type</code> statements (<a href="https://redirect.github.com/astral-sh/ruff/pull/11720">#11720</a>)</li>
<li>Respect per-file ignores for blanket and redirected noqa rules (<a href="https://redirect.github.com/astral-sh/ruff/pull/11728">#11728</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/MichaelOultram-pexip"><code>@​MichaelOultram-pexip</code></a></li>
<li><a href="https://github.com/ajesipow"><code>@​ajesipow</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/github-actions"><code>@​github-actions</code></a></li>
<li><a href="https://github.com/mtsokol"><code>@​mtsokol</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
<li><a href="https://github.com/snowsignal"><code>@​snowsignal</code></a></li>
<li><a href="https://github.com/tobb10001"><code>@​tobb10001</code></a></li>
<li><a href="https://github.com/tusharsadhwani"><code>@​tusharsadhwani</code></a></li>
</ul>
<h2>v0.4.7</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
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
<h3>Server</h3>
<ul>
<li>Formatting a document with syntax problems no longer spams a visible error popup (<a href="https://redirect.github.com/astral-sh/ruff/pull/11745">#11745</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Add RDJson support for <code>--output-format</code> flag (<a href="https://redirect.github.com/astral-sh/ruff/pull/11682">#11682</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>pyupgrade</code>] Write empty string in lieu of panic when fixing <code>UP032</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11696">#11696</a>)</li>
<li>[<code>flake8-simplify</code>] Simplify double negatives in <code>SIM103</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11684">#11684</a>)</li>
<li>Ensure the expression generator adds a newline before <code>type</code> statements (<a href="https://redirect.github.com/astral-sh/ruff/pull/11720">#11720</a>)</li>
<li>Respect per-file ignores for blanket and redirected noqa rules (<a href="https://redirect.github.com/astral-sh/ruff/pull/11728">#11728</a>)</li>
</ul>
<h2>0.4.7</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-pyi</code>] Implement <code>PYI064</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11325">#11325</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI066</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11541">#11541</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI057</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11486">#11486</a>)</li>
<li>[<code>pyflakes</code>] Enable <code>F822</code> in <code>__init__.py</code> files by default (<a href="https://redirect.github.com/astral-sh/ruff/pull/11370">#11370</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix incorrect placement of trailing stub function comments (<a href="https://redirect.github.com/astral-sh/ruff/pull/11632">#11632</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Respect file exclusions in <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11590">#11590</a>)</li>
<li>Add support for documents not exist on disk (<a href="https://redirect.github.com/astral-sh/ruff/pull/11588">#11588</a>)</li>
<li>Add Vim and Kate setup guide for <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11615">#11615</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/a8cf7096ff1acbccf3af3aa37cd6e2170f1b1bc5"><code>a8cf709</code></a> Bump version to v0.4.8 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11755">#11755</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/895eb3ef485836a75225e2534b638b98eaf30977"><code>895eb3e</code></a> [red-knot] refactor CFG outside of symbol table (<a href="https://redirect.github.com/astral-sh/ruff/issues/11746">#11746</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2e0a9755e07cfe7ee30683b65bbc1d9b5aa8b141"><code>2e0a975</code></a> Disallow access to <code>Parsed</code> output, use the API instead (<a href="https://redirect.github.com/astral-sh/ruff/issues/11741">#11741</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/b021b5babec5d88804cd67e03a946e1da0e1c0be"><code>b021b5b</code></a> Use <code>Tokens</code> from parsed type annotation or parsed source (<a href="https://redirect.github.com/astral-sh/ruff/issues/11740">#11740</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/eed6d784dfab61d0f1b1ebd95a7de7b1c6371149"><code>eed6d78</code></a> Update type annotation parsing API to return <code>Parsed</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11739">#11739</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/8338db6c1247a22e0e42ab1b24acc45ae4837149"><code>8338db6</code></a> <code>ruff server</code>: Formatting a document with syntax problems no longer spams a v...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d056d09547c5fe7ff5e787ada19fc37a73d9b444"><code>d056d09</code></a> [red-knot] add if-statement support to FlowGraph (<a href="https://redirect.github.com/astral-sh/ruff/issues/11673">#11673</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1645be018d208271bbc82b9b965eaef0e727c32a"><code>1645be0</code></a> Update <code>NPY001</code> rule for NumPy 2.0 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11735">#11735</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2c865023acb0593a9c367c43c46893c83ded25ba"><code>2c86502</code></a> CI: add job to run tests under minimum supported rust version (msrv) (<a href="https://redirect.github.com/astral-sh/ruff/issues/11737">#11737</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2567e14b7a550074c37fc5695e85510b5120a37a"><code>2567e14</code></a> Lexer should consider BOM for the start offset (<a href="https://redirect.github.com/astral-sh/ruff/issues/11732">#11732</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.4.5...v0.4.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.4.5&new-version=0.4.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-10 11:18:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/591" class=".btn">#591</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.4.5 to 0.4.8 in /rpc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.4.5 to 0.4.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.8</h2>
<h2>Changes</h2>
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
<h3>Server</h3>
<ul>
<li>Formatting a document with syntax problems no longer spams a visible error popup (<a href="https://redirect.github.com/astral-sh/ruff/pull/11745">#11745</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Add RDJson support for <code>--output-format</code> flag (<a href="https://redirect.github.com/astral-sh/ruff/pull/11682">#11682</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>pyupgrade</code>] Write empty string in lieu of panic when fixing <code>UP032</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11696">#11696</a>)</li>
<li>[<code>flake8-simplify</code>] Simplify double negatives in <code>SIM103</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11684">#11684</a>)</li>
<li>Ensure the expression generator adds a newline before <code>type</code> statements (<a href="https://redirect.github.com/astral-sh/ruff/pull/11720">#11720</a>)</li>
<li>Respect per-file ignores for blanket and redirected noqa rules (<a href="https://redirect.github.com/astral-sh/ruff/pull/11728">#11728</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/MichaelOultram-pexip"><code>@​MichaelOultram-pexip</code></a></li>
<li><a href="https://github.com/ajesipow"><code>@​ajesipow</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/github-actions"><code>@​github-actions</code></a></li>
<li><a href="https://github.com/mtsokol"><code>@​mtsokol</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
<li><a href="https://github.com/snowsignal"><code>@​snowsignal</code></a></li>
<li><a href="https://github.com/tobb10001"><code>@​tobb10001</code></a></li>
<li><a href="https://github.com/tusharsadhwani"><code>@​tusharsadhwani</code></a></li>
</ul>
<h2>v0.4.7</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
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
<h3>Server</h3>
<ul>
<li>Formatting a document with syntax problems no longer spams a visible error popup (<a href="https://redirect.github.com/astral-sh/ruff/pull/11745">#11745</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Add RDJson support for <code>--output-format</code> flag (<a href="https://redirect.github.com/astral-sh/ruff/pull/11682">#11682</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>pyupgrade</code>] Write empty string in lieu of panic when fixing <code>UP032</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11696">#11696</a>)</li>
<li>[<code>flake8-simplify</code>] Simplify double negatives in <code>SIM103</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11684">#11684</a>)</li>
<li>Ensure the expression generator adds a newline before <code>type</code> statements (<a href="https://redirect.github.com/astral-sh/ruff/pull/11720">#11720</a>)</li>
<li>Respect per-file ignores for blanket and redirected noqa rules (<a href="https://redirect.github.com/astral-sh/ruff/pull/11728">#11728</a>)</li>
</ul>
<h2>0.4.7</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-pyi</code>] Implement <code>PYI064</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11325">#11325</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI066</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11541">#11541</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI057</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11486">#11486</a>)</li>
<li>[<code>pyflakes</code>] Enable <code>F822</code> in <code>__init__.py</code> files by default (<a href="https://redirect.github.com/astral-sh/ruff/pull/11370">#11370</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix incorrect placement of trailing stub function comments (<a href="https://redirect.github.com/astral-sh/ruff/pull/11632">#11632</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Respect file exclusions in <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11590">#11590</a>)</li>
<li>Add support for documents not exist on disk (<a href="https://redirect.github.com/astral-sh/ruff/pull/11588">#11588</a>)</li>
<li>Add Vim and Kate setup guide for <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11615">#11615</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/a8cf7096ff1acbccf3af3aa37cd6e2170f1b1bc5"><code>a8cf709</code></a> Bump version to v0.4.8 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11755">#11755</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/895eb3ef485836a75225e2534b638b98eaf30977"><code>895eb3e</code></a> [red-knot] refactor CFG outside of symbol table (<a href="https://redirect.github.com/astral-sh/ruff/issues/11746">#11746</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2e0a9755e07cfe7ee30683b65bbc1d9b5aa8b141"><code>2e0a975</code></a> Disallow access to <code>Parsed</code> output, use the API instead (<a href="https://redirect.github.com/astral-sh/ruff/issues/11741">#11741</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/b021b5babec5d88804cd67e03a946e1da0e1c0be"><code>b021b5b</code></a> Use <code>Tokens</code> from parsed type annotation or parsed source (<a href="https://redirect.github.com/astral-sh/ruff/issues/11740">#11740</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/eed6d784dfab61d0f1b1ebd95a7de7b1c6371149"><code>eed6d78</code></a> Update type annotation parsing API to return <code>Parsed</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11739">#11739</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/8338db6c1247a22e0e42ab1b24acc45ae4837149"><code>8338db6</code></a> <code>ruff server</code>: Formatting a document with syntax problems no longer spams a v...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d056d09547c5fe7ff5e787ada19fc37a73d9b444"><code>d056d09</code></a> [red-knot] add if-statement support to FlowGraph (<a href="https://redirect.github.com/astral-sh/ruff/issues/11673">#11673</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1645be018d208271bbc82b9b965eaef0e727c32a"><code>1645be0</code></a> Update <code>NPY001</code> rule for NumPy 2.0 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11735">#11735</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2c865023acb0593a9c367c43c46893c83ded25ba"><code>2c86502</code></a> CI: add job to run tests under minimum supported rust version (msrv) (<a href="https://redirect.github.com/astral-sh/ruff/issues/11737">#11737</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2567e14b7a550074c37fc5695e85510b5120a37a"><code>2567e14</code></a> Lexer should consider BOM for the start offset (<a href="https://redirect.github.com/astral-sh/ruff/issues/11732">#11732</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.4.5...v0.4.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.4.5&new-version=0.4.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-10 11:16:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/590" class=".btn">#590</a>
            </td>
            <td>
                <b>
                    Bump pytest from 8.2.0 to 8.2.2 in /connection_update/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.0 to 8.2.2.
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
<h2>8.2.1</h2>
<h1>pytest 8.2.1 (2024-05-19)</h1>
<h2>Improvements</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12334">#12334</a>: Support for Python 3.13 (beta1 at the time of writing).</li>
</ul>
<h2>Bug Fixes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12120">#12120</a>: Fix [PermissionError]{.title-ref} crashes arising from directories which are not selected on the command-line.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12191">#12191</a>: Keyboard interrupts and system exits are now properly handled during the test collection.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12300">#12300</a>: Fixed handling of 'Function not implemented' error under squashfuse_ll, which is a different way to say that the mountpoint is read-only.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12308">#12308</a>: Fix a regression in pytest 8.2.0 where the permissions of automatically-created <code>.pytest_cache</code> directories became <code>rwx------</code> instead of the expected <code>rwxr-xr-x</code>.</li>
</ul>
<h2>Trivial/Internal Changes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12333">#12333</a>: pytest releases are now attested using the recent <a href="https://github.blog/2024-05-02-introducing-artifact-attestations-now-in-public-beta/">Artifact Attestation</a> support from GitHub, allowing users to verify the provenance of pytest's sdist and wheel artifacts.</li>
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
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.0...8.2.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.0&new-version=8.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-10 11:15:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/589" class=".btn">#589</a>
            </td>
            <td>
                <b>
                    Bump ruff from 0.4.5 to 0.4.8 in /plugin_globals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.4.5 to 0.4.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.4.8</h2>
<h2>Changes</h2>
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
<h3>Server</h3>
<ul>
<li>Formatting a document with syntax problems no longer spams a visible error popup (<a href="https://redirect.github.com/astral-sh/ruff/pull/11745">#11745</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Add RDJson support for <code>--output-format</code> flag (<a href="https://redirect.github.com/astral-sh/ruff/pull/11682">#11682</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>pyupgrade</code>] Write empty string in lieu of panic when fixing <code>UP032</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11696">#11696</a>)</li>
<li>[<code>flake8-simplify</code>] Simplify double negatives in <code>SIM103</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11684">#11684</a>)</li>
<li>Ensure the expression generator adds a newline before <code>type</code> statements (<a href="https://redirect.github.com/astral-sh/ruff/pull/11720">#11720</a>)</li>
<li>Respect per-file ignores for blanket and redirected noqa rules (<a href="https://redirect.github.com/astral-sh/ruff/pull/11728">#11728</a>)</li>
</ul>
<h2>Contributors</h2>
<ul>
<li><a href="https://github.com/AlexWaygood"><code>@​AlexWaygood</code></a></li>
<li><a href="https://github.com/MichaReiser"><code>@​MichaReiser</code></a></li>
<li><a href="https://github.com/MichaelOultram-pexip"><code>@​MichaelOultram-pexip</code></a></li>
<li><a href="https://github.com/ajesipow"><code>@​ajesipow</code></a></li>
<li><a href="https://github.com/carljm"><code>@​carljm</code></a></li>
<li><a href="https://github.com/charliermarsh"><code>@​charliermarsh</code></a></li>
<li><a href="https://github.com/dhruvmanila"><code>@​dhruvmanila</code></a></li>
<li><a href="https://github.com/github-actions"><code>@​github-actions</code></a></li>
<li><a href="https://github.com/mtsokol"><code>@​mtsokol</code></a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a></li>
<li><a href="https://github.com/snowsignal"><code>@​snowsignal</code></a></li>
<li><a href="https://github.com/tobb10001"><code>@​tobb10001</code></a></li>
<li><a href="https://github.com/tusharsadhwani"><code>@​tusharsadhwani</code></a></li>
</ul>
<h2>v0.4.7</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
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
<h3>Server</h3>
<ul>
<li>Formatting a document with syntax problems no longer spams a visible error popup (<a href="https://redirect.github.com/astral-sh/ruff/pull/11745">#11745</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Add RDJson support for <code>--output-format</code> flag (<a href="https://redirect.github.com/astral-sh/ruff/pull/11682">#11682</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>pyupgrade</code>] Write empty string in lieu of panic when fixing <code>UP032</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11696">#11696</a>)</li>
<li>[<code>flake8-simplify</code>] Simplify double negatives in <code>SIM103</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11684">#11684</a>)</li>
<li>Ensure the expression generator adds a newline before <code>type</code> statements (<a href="https://redirect.github.com/astral-sh/ruff/pull/11720">#11720</a>)</li>
<li>Respect per-file ignores for blanket and redirected noqa rules (<a href="https://redirect.github.com/astral-sh/ruff/pull/11728">#11728</a>)</li>
</ul>
<h2>0.4.7</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-pyi</code>] Implement <code>PYI064</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11325">#11325</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI066</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11541">#11541</a>)</li>
<li>[<code>flake8-pyi</code>] Implement <code>PYI057</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11486">#11486</a>)</li>
<li>[<code>pyflakes</code>] Enable <code>F822</code> in <code>__init__.py</code> files by default (<a href="https://redirect.github.com/astral-sh/ruff/pull/11370">#11370</a>)</li>
</ul>
<h3>Formatter</h3>
<ul>
<li>Fix incorrect placement of trailing stub function comments (<a href="https://redirect.github.com/astral-sh/ruff/pull/11632">#11632</a>)</li>
</ul>
<h3>Server</h3>
<ul>
<li>Respect file exclusions in <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11590">#11590</a>)</li>
<li>Add support for documents not exist on disk (<a href="https://redirect.github.com/astral-sh/ruff/pull/11588">#11588</a>)</li>
<li>Add Vim and Kate setup guide for <code>ruff server</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/11615">#11615</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/a8cf7096ff1acbccf3af3aa37cd6e2170f1b1bc5"><code>a8cf709</code></a> Bump version to v0.4.8 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11755">#11755</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/895eb3ef485836a75225e2534b638b98eaf30977"><code>895eb3e</code></a> [red-knot] refactor CFG outside of symbol table (<a href="https://redirect.github.com/astral-sh/ruff/issues/11746">#11746</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2e0a9755e07cfe7ee30683b65bbc1d9b5aa8b141"><code>2e0a975</code></a> Disallow access to <code>Parsed</code> output, use the API instead (<a href="https://redirect.github.com/astral-sh/ruff/issues/11741">#11741</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/b021b5babec5d88804cd67e03a946e1da0e1c0be"><code>b021b5b</code></a> Use <code>Tokens</code> from parsed type annotation or parsed source (<a href="https://redirect.github.com/astral-sh/ruff/issues/11740">#11740</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/eed6d784dfab61d0f1b1ebd95a7de7b1c6371149"><code>eed6d78</code></a> Update type annotation parsing API to return <code>Parsed</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/11739">#11739</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/8338db6c1247a22e0e42ab1b24acc45ae4837149"><code>8338db6</code></a> <code>ruff server</code>: Formatting a document with syntax problems no longer spams a v...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/d056d09547c5fe7ff5e787ada19fc37a73d9b444"><code>d056d09</code></a> [red-knot] add if-statement support to FlowGraph (<a href="https://redirect.github.com/astral-sh/ruff/issues/11673">#11673</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/1645be018d208271bbc82b9b965eaef0e727c32a"><code>1645be0</code></a> Update <code>NPY001</code> rule for NumPy 2.0 (<a href="https://redirect.github.com/astral-sh/ruff/issues/11735">#11735</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2c865023acb0593a9c367c43c46893c83ded25ba"><code>2c86502</code></a> CI: add job to run tests under minimum supported rust version (msrv) (<a href="https://redirect.github.com/astral-sh/ruff/issues/11737">#11737</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/2567e14b7a550074c37fc5695e85510b5120a37a"><code>2567e14</code></a> Lexer should consider BOM for the start offset (<a href="https://redirect.github.com/astral-sh/ruff/issues/11732">#11732</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.4.5...v0.4.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.4.5&new-version=0.4.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-10 11:13:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/588" class=".btn">#588</a>
            </td>
            <td>
                <b>
                    Bump pytest from 8.2.0 to 8.2.2 in /plugin_globals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.0 to 8.2.2.
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
<h2>8.2.1</h2>
<h1>pytest 8.2.1 (2024-05-19)</h1>
<h2>Improvements</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12334">#12334</a>: Support for Python 3.13 (beta1 at the time of writing).</li>
</ul>
<h2>Bug Fixes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12120">#12120</a>: Fix [PermissionError]{.title-ref} crashes arising from directories which are not selected on the command-line.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12191">#12191</a>: Keyboard interrupts and system exits are now properly handled during the test collection.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12300">#12300</a>: Fixed handling of 'Function not implemented' error under squashfuse_ll, which is a different way to say that the mountpoint is read-only.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12308">#12308</a>: Fix a regression in pytest 8.2.0 where the permissions of automatically-created <code>.pytest_cache</code> directories became <code>rwx------</code> instead of the expected <code>rwxr-xr-x</code>.</li>
</ul>
<h2>Trivial/Internal Changes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12333">#12333</a>: pytest releases are now attested using the recent <a href="https://github.blog/2024-05-02-introducing-artifact-attestations-now-in-public-beta/">Artifact Attestation</a> support from GitHub, allowing users to verify the provenance of pytest's sdist and wheel artifacts.</li>
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
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.0...8.2.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.0&new-version=8.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-10 11:13:22 +0000 UTC
    </div>
</div>

