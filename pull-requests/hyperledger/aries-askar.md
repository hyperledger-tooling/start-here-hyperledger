---
layout: default
title: aries-askar
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-askar
---

# aries-askar <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-askar){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/265" class=".btn">#265</a>
            </td>
            <td>
                <b>
                    build(deps-dev): update pytest requirement from ~=8.2.1 to ~=8.2.2 in /wrappers/python
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Updates the requirements on [pytest](https://github.com/pytest-dev/pytest) to permit the latest version.
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
        Created At 2024-06-05 22:45:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/264" class=".btn">#264</a>
            </td>
            <td>
                <b>
                    Replace serde_cbor with ciborium
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The crate `serde_cbor` is unmaintained and has not received any updates in the last 3 years. The author of serde_cbor proposes [ciborium](https://crates.io/crates/ciborium) as an alternative.
This PR replaces the dependency on `serde_cbor` with `ciborium`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-04 13:13:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/263" class=".btn">#263</a>
            </td>
            <td>
                <b>
                    build(deps): bump async-lock from 3.2.0 to 3.4.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [async-lock](https://github.com/smol-rs/async-lock) from 3.2.0 to 3.4.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/smol-rs/async-lock/releases">async-lock's releases</a>.</em></p>
<blockquote>
<h2>v3.4.0</h2>
<ul>
<li>Port to <code>event-listener</code> v5.0.0. (<a href="https://redirect.github.com/smol-rs/async-lock/issues/74">#74</a>)</li>
</ul>
<h2>v3.3.0</h2>
<ul>
<li>Add a <code>forget()</code> method for semaphore guards. (<a href="https://redirect.github.com/smol-rs/async-lock/issues/73">#73</a>)</li>
<li>Increase MSRV to v1.60. (<a href="https://redirect.github.com/smol-rs/async-lock/issues/75">#75</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/smol-rs/async-lock/blob/master/CHANGELOG.md">async-lock's changelog</a>.</em></p>
<blockquote>
<h1>Version 3.4.0</h1>
<ul>
<li>Port to <code>event-listener</code> v5.0.0. (<a href="https://redirect.github.com/smol-rs/async-lock/issues/74">#74</a>)</li>
</ul>
<h1>Version 3.3.0</h1>
<ul>
<li>Add a <code>forget()</code> method for semaphore guards. (<a href="https://redirect.github.com/smol-rs/async-lock/issues/73">#73</a>)</li>
<li>Increase MSRV to v1.60. (<a href="https://redirect.github.com/smol-rs/async-lock/issues/75">#75</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/smol-rs/async-lock/commit/cc249b2d31590a6e97616a351032747f3e19bc87"><code>cc249b2</code></a> v3.4.0</li>
<li><a href="https://github.com/smol-rs/async-lock/commit/12b54020c3ce85d5eebe3e073c3d0d264d64311d"><code>12b5402</code></a> m: Remove unused portable-atomic feature</li>
<li><a href="https://github.com/smol-rs/async-lock/commit/2c96fbfcd0d02be3d8c3955736fe8e35da8fd28a"><code>2c96fbf</code></a> tests: Instrument with loom</li>
<li><a href="https://github.com/smol-rs/async-lock/commit/542831132f2c707aae1c380edd43452053433814"><code>5428311</code></a> Replace async-channel with flume</li>
<li><a href="https://github.com/smol-rs/async-lock/commit/df82e5bb5e25f1215d2cfc290d6d7021e4516ef6"><code>df82e5b</code></a> chore: Silence clippy</li>
<li><a href="https://github.com/smol-rs/async-lock/commit/aeb9d8ff8e5ad6e33f87e5cbeb226faeb4452715"><code>aeb9d8f</code></a> Remove redundant import</li>
<li><a href="https://github.com/smol-rs/async-lock/commit/ff4c96fe4dc72f4233e17e016c36051b2f6e0aa5"><code>ff4c96f</code></a> m: Port to event-listener v5.0.0</li>
<li><a href="https://github.com/smol-rs/async-lock/commit/47dd439e5a822f92b8cec20dda72e48332d7e7bd"><code>47dd439</code></a> v3.3.0</li>
<li><a href="https://github.com/smol-rs/async-lock/commit/6581d8b655feb67c45f18ecd8801061533fa236f"><code>6581d8b</code></a> Use cfg(target_family = &quot;wasm&quot;) in Cargo.toml</li>
<li><a href="https://github.com/smol-rs/async-lock/commit/0493551beb7f8cac037750010115bdce5f59c51e"><code>0493551</code></a> Migrate to Rust 2021</li>
<li>Additional commits viewable in <a href="https://github.com/smol-rs/async-lock/compare/v3.2.0...v3.4.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=async-lock&package-manager=cargo&previous-version=3.2.0&new-version=3.4.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-03 11:57:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/262" class=".btn">#262</a>
            </td>
            <td>
                <b>
                    Add python requirements file and update dependabot workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently setup.py just indicates one dependency: `cached_property`.

It makes sense if the dependencies were parsed from a requirements.txt file (less effort than migrating to pyproject.toml format). Allows for easier management if any extras need to be added, and also means we can add pip dependency management to the dependabot workflow (namely to catch if there's an update to `cached_property`.

A requirements.dev.txt file is also added to track dev / test dependencies. I would add indy as a test requirement, since it's used in `indy_test.py`, but I can't find out which `indy` packages it's referring to ... it doesn't work with `pip install indy` or `python3-indy`. So for now I've just specified `pytest` and `pytest-asyncio`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-03 11:47:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/261" class=".btn">#261</a>
            </td>
            <td>
                <b>
                    fix: Incorrect SQLite expire check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In SQLite comparison of expiry date is done using query
```sql
(expiry IS NULL OR expiry > DATETIME('now'))
```
but SQLite considers text strings for date and time comparisons by character order, not by their actual date/time value., so the check is not working correctly and askar returns the items stored even after expired.

The fix is easy, `expiry` should be first converted to DATETIME, in above query something like:
```sql
(expiry IS NULL OR DATETIME(expiry) > DATETIME('now'))
```

Fixes issue #260 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-30 14:18:15 +0000 UTC
    </div>
</div>

