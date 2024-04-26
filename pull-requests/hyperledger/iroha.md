---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4515" class=".btn">#4515</a>
            </td>
            <td>
                <b>
                    [chore]: Bump serde_with from 3.7.0 to 3.8.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Chore</span><span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde_with](https://github.com/jonasbb/serde_with) from 3.7.0 to 3.8.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/jonasbb/serde_with/releases">serde_with's releases</a>.</em></p>
<blockquote>
<h2>serde_with v3.8.0</h2>
<h3>Added</h3>
<ul>
<li>Implement (De)Serialization for Pinned Smart Pointers by <a href="https://github.com/Astralchroma"><code>@​Astralchroma</code></a> (<a href="https://redirect.github.com/jonasbb/serde_with/issues/733">#733</a>)</li>
<li>Implement <code>JsonSchemaAs</code> for <code>PickFirst</code> by <a href="https://github.com/swlynch99"><code>@​swlynch99</code></a>  (<a href="https://redirect.github.com/jonasbb/serde_with/issues/721">#721</a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Bump <code>base64</code> dependency to v0.22 (<a href="https://redirect.github.com/jonasbb/serde_with/issues/724">#724</a>)</li>
<li>Update dev dependencies</li>
</ul>
<h3>Fixed</h3>
<ul>
<li><code>serde_conv</code> regressed and triggered <code>clippy::ptr_arg</code> and add test to prevent future problems. (<a href="https://redirect.github.com/jonasbb/serde_with/issues/731">#731</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jonasbb/serde_with/commit/7e66d6bba9d853be888c6e9c819e4388301f67dc"><code>7e66d6b</code></a> Bump version to v3.8.0 (<a href="https://redirect.github.com/jonasbb/serde_with/issues/734">#734</a>)</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/4a4fcb3fd4b82bff9e40820e8a44162cfbd08110"><code>4a4fcb3</code></a> Bump version to v3.8.0</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/167e865e407e8f79e56eb8539913521663a96ae5"><code>167e865</code></a> Implement (De)Serialization for Pinned Smart Pointers (<a href="https://redirect.github.com/jonasbb/serde_with/issues/733">#733</a>)</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/04de4ce6d8a26dc755cf31b9e1889d19852c4e51"><code>04de4ce</code></a> Add SerializeAs support for Pin&lt;&amp;'a T&gt; and Pin&lt;&amp;'a mut T&gt;</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/9c2dac75e64a4cbf4db5673ae5a4a7b9039b1d15"><code>9c2dac7</code></a> Implement (De)Serialization for Pinned Smart Pointers</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/9989d8e658c5395277699714a3729614b6853bca"><code>9989d8e</code></a> Add test that serde_conv will not trigger <code>clippy::ptr_arg</code> (<a href="https://redirect.github.com/jonasbb/serde_with/issues/731">#731</a>)</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/754c0819125f00f382f539bdd9fb9d71c7c80fb4"><code>754c081</code></a> Add test that serde_conv will not trigger <code>clippy::ptr_arg</code></li>
<li><a href="https://github.com/jonasbb/serde_with/commit/bb90db5334ce7832ea63d06728527294ee5de647"><code>bb90db5</code></a> Update the OneOrMany doctest to test serialization too <a href="https://redirect.github.com/jonasbb/serde_with/issues/728">#728</a> (<a href="https://redirect.github.com/jonasbb/serde_with/issues/730">#730</a>)</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/f12ece26c8c50e7de5b097ed22608b9c194db888"><code>f12ece2</code></a> Update the OneOrMany doctest to test serialization too <a href="https://redirect.github.com/jonasbb/serde_with/issues/728">#728</a></li>
<li><a href="https://github.com/jonasbb/serde_with/commit/57e4ee2fcb8e03681fde86f74942422285d11277"><code>57e4ee2</code></a> Bump dev deps (<a href="https://redirect.github.com/jonasbb/serde_with/issues/726">#726</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/jonasbb/serde_with/compare/v3.7.0...v3.8.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde_with&package-manager=cargo&previous-version=3.7.0&new-version=3.8.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-25 16:54:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4514" class=".btn">#4514</a>
            </td>
            <td>
                <b>
                    [chore]: Bump faker from 24.11.0 to 24.14.0 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Chore</span><span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [faker](https://github.com/joke2k/faker) from 24.11.0 to 24.14.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/releases">faker's releases</a>.</em></p>
<blockquote>
<h2>Release v24.14.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v24.14.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
<h2>Release v24.13.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v24.13.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
<h2>Release v24.12.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v24.12.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/blob/master/CHANGELOG.md">faker's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/joke2k/faker/compare/v24.13.0...v24.14.0">v24.14.0 - 2024-04-25</a></h3>
<ul>
<li>Add job provider for <code>cs_CZ</code>. Thanks <a href="https://github.com/george0st"><code>@​george0st</code></a>.</li>
</ul>
<h3><a href="https://github.com/joke2k/faker/compare/v24.12.0...v24.13.0">v24.13.0 - 2024-04-25</a></h3>
<ul>
<li>Add geo provider for <code>sk_SK</code>. Thanks <a href="https://github.com/george0st"><code>@​george0st</code></a>.</li>
<li>Clean up data in <code>sk_SK</code> job provider. Thanks <a href="https://github.com/george0st"><code>@​george0st</code></a>.</li>
</ul>
<h3><a href="https://github.com/joke2k/faker/compare/v24.11.0...v24.12.0">v24.12.0 - 2024-04-25</a></h3>
<ul>
<li>Remove offensive word from <code>pl_PL</code> lorem provider. Thanks <a href="https://github.com/Rey092"><code>@​Rey092</code></a>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/joke2k/faker/commit/412ec97720d711184c09f02da3e6bbbf4c3e715f"><code>412ec97</code></a> Bump version: 24.13.0 → 24.14.0</li>
<li><a href="https://github.com/joke2k/faker/commit/9faf59a48020cf11471efcb88bbce1ac1fc27577"><code>9faf59a</code></a> :pencil: Update CHANGELOG.md</li>
<li><a href="https://github.com/joke2k/faker/commit/86d44c74d2af4d962f7c56ad3c0fa119fe899a07"><code>86d44c7</code></a> :lipstick: Add missing blank lines in test_job.py</li>
<li><a href="https://github.com/joke2k/faker/commit/ab53f70aea0f97305537c50827d9c7808c00ee35"><code>ab53f70</code></a> Add job provider for <code>cs_CZ</code> (<a href="https://redirect.github.com/joke2k/faker/issues/2023">#2023</a>)</li>
<li><a href="https://github.com/joke2k/faker/commit/a2e73cf035ba6d7f4bbc540fadcbebb9bb1e7f2e"><code>a2e73cf</code></a> Bump version: 24.12.0 → 24.13.0</li>
<li><a href="https://github.com/joke2k/faker/commit/7d4668b9ebbed1d165baec5fd3f07e62c521846c"><code>7d4668b</code></a> :pencil: Update CHANGELOG.md</li>
<li><a href="https://github.com/joke2k/faker/commit/215236fdbe1d50398200950a7bd17ffa2b610fd7"><code>215236f</code></a> :lipstick: Format code</li>
<li><a href="https://github.com/joke2k/faker/commit/35e1c128155d0aed1c78adb4a7d0ac3f0eb0da53"><code>35e1c12</code></a> Clean up data in <code>sk_SK</code> job provider</li>
<li><a href="https://github.com/joke2k/faker/commit/0888c361f3de85e7185c8b1208ddd42e0b55315a"><code>0888c36</code></a> Add geo provider for <code>sk_SK</code> (<a href="https://redirect.github.com/joke2k/faker/issues/2024">#2024</a>)</li>
<li><a href="https://github.com/joke2k/faker/commit/3b54c9692c0488cc140bded6016f2ba115765c38"><code>3b54c96</code></a> Bump version: 24.11.0 → 24.12.0</li>
<li>Additional commits viewable in <a href="https://github.com/joke2k/faker/compare/v24.11.0...v24.14.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=faker&package-manager=pip&previous-version=24.11.0&new-version=24.14.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-25 16:53:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4513" class=".btn">#4513</a>
            </td>
            <td>
                <b>
                    [refactor] #3901: Add method to define parameter in executor `migrate` entrypoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

* Added method `add_parameter` which can be called from executor (in `migrate` entrypoint) to define new executor parameter
* Added test which demonstrates how executor can use it, as suggested [here](https://github.com/hyperledger/iroha/pull/4310#issuecomment-1964247631)
* Note that this PR was mostly implemented before discussion in #4352, so potentially this should be implemented differently. E.g. if it will be decided to store executor parameters in `Domain::metadata`, then there will be no need for `add_parameter` method since executor parameter will be defined using `SetKeyValue` ISI
* Note that I didn't removed `NewParameter` ISI since it is currently used to define chain-wide parameters (for wasm engine and sumeragi), and potentially chain-wide parameters should be defined/stored differently as discussed in https://github.com/hyperledger/iroha/issues/4352#issuecomment-2076735651

### Linked issue

Closes #3901
Related: #4352
Related: #4310

### Benefits

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-25 13:55:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4508" class=".btn">#4508</a>
            </td>
            <td>
                <b>
                    [chore]: Bump mypy from 1.8.0 to 1.10.0 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Chore</span><span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [mypy](https://github.com/python/mypy) from 1.8.0 to 1.10.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/python/mypy/blob/master/CHANGELOG.md">mypy's changelog</a>.</em></p>
<blockquote>
<h1>Mypy Release Notes</h1>
<h2>Next release</h2>
<h2>Mypy 1.10</h2>
<p>We’ve just uploaded mypy 1.10 to the Python Package Index (<a href="https://pypi.org/project/mypy/">PyPI</a>). Mypy is a static type checker for Python. This release includes new features, performance improvements and bug fixes. You can install it as follows:</p>
<pre><code>python3 -m pip install -U mypy
</code></pre>
<p>You can read the full documentation for this release on <a href="http://mypy.readthedocs.io">Read the Docs</a>.</p>
<h4>Support TypeIs (PEP 742)</h4>
<p>Mypy now supports <code>TypeIs</code> (<a href="https://peps.python.org/pep-0742/">PEP 742</a>), which allows
functions to narrow the type of a value, similar to <code>isinstance()</code>. Unlike <code>TypeGuard</code>,
<code>TypeIs</code> can narrow in both the <code>if</code> and <code>else</code> branches of an if statement:</p>
<pre lang="python"><code>from typing_extensions import TypeIs
<p>def is_str(s: object) -&gt; TypeIs[str]:
return isinstance(s, str)</p>
<p>def f(o: str | int) -&gt; None:
if is_str(o):
# Type of o is 'str'
...
else:
# Type of o is 'int'
...
</code></pre></p>
<p><code>TypeIs</code> will be added to the <code>typing</code> module in Python 3.13, but it
can be used on earlier Python versions by importing it from
<code>typing_extensions</code>.</p>
<p>This feature was contributed by Jelle Zijlstra (PR <a href="https://redirect.github.com/python/mypy/pull/16898">16898</a>).</p>
<h4>Support TypeVar Defaults (PEP 696)</h4>
<p><a href="https://peps.python.org/pep-0696/">PEP 696</a> adds support for type parameter defaults.
Example:</p>
<pre lang="python"><code>from typing import Generic
from typing_extensions import TypeVar
<p>&lt;/tr&gt;&lt;/table&gt;
</code></pre></p>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/python/mypy/commit/3faf0fc4798ec3ee6b1cd123965193dc0a753fb0"><code>3faf0fc</code></a> Remove +dev for version for release 1.10</li>
<li><a href="https://github.com/python/mypy/commit/a5998d20402515f0c0bf05c7fe1029e93aa9bfa8"><code>a5998d2</code></a> Update CHANGELOG.md (<a href="https://redirect.github.com/python/mypy/issues/17159">#17159</a>)</li>
<li><a href="https://github.com/python/mypy/commit/62ea5b01f0c0c99e7db93326cb8d219eecfb3cb6"><code>62ea5b0</code></a> Various updates to changelog for 1.10 (<a href="https://redirect.github.com/python/mypy/issues/17158">#17158</a>)</li>
<li><a href="https://github.com/python/mypy/commit/2f0864c4e55a74700d8ce2d97ab2d3ca2b288513"><code>2f0864c</code></a> Update CHANGELOG.md with draft for release 1.10 (<a href="https://redirect.github.com/python/mypy/issues/17150">#17150</a>)</li>
<li><a href="https://github.com/python/mypy/commit/e1443bbade91118794055449cc8b4b4f7fd08b7d"><code>e1443bb</code></a> fix: incorrect returned type of access descriptors on unions of types (<a href="https://redirect.github.com/python/mypy/issues/16604">#16604</a>)</li>
<li><a href="https://github.com/python/mypy/commit/5161ac2e5b73dc7597536eb4444219868317e5d9"><code>5161ac2</code></a> Sync typeshed (<a href="https://redirect.github.com/python/mypy/issues/17124">#17124</a>)</li>
<li><a href="https://github.com/python/mypy/commit/e2fc1f28935806ca04b18fab277217f583b51594"><code>e2fc1f2</code></a> Fix crash when expanding invalid Unpack in a <code>Callable</code> alias (<a href="https://redirect.github.com/python/mypy/issues/17028">#17028</a>)</li>
<li><a href="https://github.com/python/mypy/commit/3ff6e47c57a67e807e0b4579a816b4f66ab16824"><code>3ff6e47</code></a> Docs: docstrings in checker.py, ast_helpers.py (<a href="https://redirect.github.com/python/mypy/issues/16908">#16908</a>)</li>
<li><a href="https://github.com/python/mypy/commit/732d98ecb2a98e4eaea14aba1ed8ac9c1f5ccdb6"><code>732d98e</code></a> Fix string formatting for string enums (<a href="https://redirect.github.com/python/mypy/issues/16555">#16555</a>)</li>
<li><a href="https://github.com/python/mypy/commit/80190101f68b52e960c22572ed6cc814de078b9c"><code>8019010</code></a> Narrow individual items when matching a tuple to a sequence pattern (<a href="https://redirect.github.com/python/mypy/issues/16905">#16905</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/python/mypy/compare/v1.8.0...v1.10.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mypy&package-manager=pip&previous-version=1.8.0&new-version=1.10.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-24 17:04:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4507" class=".btn">#4507</a>
            </td>
            <td>
                <b>
                    [chore]: Bump black from 24.2.0 to 24.4.1 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Chore</span><span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [black](https://github.com/psf/black) from 24.2.0 to 24.4.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/black/releases">black's releases</a>.</em></p>
<blockquote>
<h2>24.4.1</h2>
<h3>Highlights</h3>
<ul>
<li>Add support for the new Python 3.12 f-string syntax introduced by PEP 701 (<a href="https://redirect.github.com/psf/black/issues/3822">#3822</a>)</li>
</ul>
<h3>Stable style</h3>
<ul>
<li>Fix crash involving indented dummy functions containing newlines (<a href="https://redirect.github.com/psf/black/issues/4318">#4318</a>)</li>
</ul>
<h3>Parser</h3>
<ul>
<li>Add support for type parameter defaults, a new syntactic feature added to Python 3.13
by PEP 696 (<a href="https://redirect.github.com/psf/black/issues/4327">#4327</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Github Action now works even when <code>git archive</code> is skipped (<a href="https://redirect.github.com/psf/black/issues/4313">#4313</a>)</li>
</ul>
<h2>24.4.0</h2>
<h3>Stable style</h3>
<ul>
<li>Fix unwanted crashes caused by AST equivalency check (<a href="https://redirect.github.com/psf/black/issues/4290">#4290</a>)</li>
</ul>
<h3>Preview style</h3>
<ul>
<li><code>if</code> guards in <code>case</code> blocks are now wrapped in parentheses when the line is too long.
(<a href="https://redirect.github.com/psf/black/issues/4269">#4269</a>)</li>
<li>Stop moving multiline strings to a new line unless inside brackets (<a href="https://redirect.github.com/psf/black/issues/4289">#4289</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Add a new option <code>use_pyproject</code> to the GitHub Action <code>psf/black</code>. This will read the
Black version from <code>pyproject.toml</code>. (<a href="https://redirect.github.com/psf/black/issues/4294">#4294</a>)</li>
</ul>
<h2>24.3.0</h2>
<h3>Highlights</h3>
<p>This release is a milestone: it fixes Black's first CVE security vulnerability. If you
run Black on untrusted input, or if you habitually put thousands of leading tab
characters in your docstrings, you are strongly encouraged to upgrade immediately to fix
<a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2024-21503">CVE-2024-21503</a>.</p>
<p>This release also fixes a bug in Black's AST safety check that allowed Black to make
incorrect changes to certain f-strings that are valid in Python 3.12 and higher.</p>
<h3>Stable style</h3>
<ul>
<li>Don't move comments along with delimiters, which could cause crashes (<a href="https://redirect.github.com/psf/black/issues/4248">#4248</a>)</li>
<li>Strengthen AST safety check to catch more unsafe changes to strings. Previous versions</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/black/blob/main/CHANGES.md">black's changelog</a>.</em></p>
<blockquote>
<h2>24.4.1</h2>
<h3>Highlights</h3>
<ul>
<li>Add support for the new Python 3.12 f-string syntax introduced by PEP 701 (<a href="https://redirect.github.com/psf/black/issues/3822">#3822</a>)</li>
</ul>
<h3>Stable style</h3>
<ul>
<li>Fix crash involving indented dummy functions containing newlines (<a href="https://redirect.github.com/psf/black/issues/4318">#4318</a>)</li>
</ul>
<h3>Parser</h3>
<ul>
<li>Add support for type parameter defaults, a new syntactic feature added to Python 3.13
by PEP 696 (<a href="https://redirect.github.com/psf/black/issues/4327">#4327</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Github Action now works even when <code>git archive</code> is skipped (<a href="https://redirect.github.com/psf/black/issues/4313">#4313</a>)</li>
</ul>
<h2>24.4.0</h2>
<h3>Stable style</h3>
<ul>
<li>Fix unwanted crashes caused by AST equivalency check (<a href="https://redirect.github.com/psf/black/issues/4290">#4290</a>)</li>
</ul>
<h3>Preview style</h3>
<ul>
<li><code>if</code> guards in <code>case</code> blocks are now wrapped in parentheses when the line is too long.
(<a href="https://redirect.github.com/psf/black/issues/4269">#4269</a>)</li>
<li>Stop moving multiline strings to a new line unless inside brackets (<a href="https://redirect.github.com/psf/black/issues/4289">#4289</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Add a new option <code>use_pyproject</code> to the GitHub Action <code>psf/black</code>. This will read the
Black version from <code>pyproject.toml</code>. (<a href="https://redirect.github.com/psf/black/issues/4294">#4294</a>)</li>
</ul>
<h2>24.3.0</h2>
<h3>Highlights</h3>
<p>This release is a milestone: it fixes Black's first CVE security vulnerability. If you
run Black on untrusted input, or if you habitually put thousands of leading tab
characters in your docstrings, you are strongly encouraged to upgrade immediately to fix
<a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2024-21503">CVE-2024-21503</a>.</p>
<p>This release also fixes a bug in Black's AST safety check that allowed Black to make
incorrect changes to certain f-strings that are valid in Python 3.12 and higher.</p>
<h3>Stable style</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/black/commit/e7fb048281a83733f0b162fc7fa85e48044ea9ec"><code>e7fb048</code></a> Prepare release 24.4.1 (<a href="https://redirect.github.com/psf/black/issues/4328">#4328</a>)</li>
<li><a href="https://github.com/psf/black/commit/3f0f8f1956646fd9f6fc47e133364c1352a478d1"><code>3f0f8f1</code></a> Support PEP 696 (<a href="https://redirect.github.com/psf/black/issues/4327">#4327</a>)</li>
<li><a href="https://github.com/psf/black/commit/2f88085da588d34286bc9a24e288de204f141243"><code>2f88085</code></a> Github Action: Directly install from repo if <code>export-subst</code> is skipped (<a href="https://redirect.github.com/psf/black/issues/4313">#4313</a>)</li>
<li><a href="https://github.com/psf/black/commit/12ce3db077780ab01cc5ad1f92d5c85fcca3f54c"><code>12ce3db</code></a> Move changelog entry to right section (<a href="https://redirect.github.com/psf/black/issues/4326">#4326</a>)</li>
<li><a href="https://github.com/psf/black/commit/1354be2525e4910b8a0d7c46242eae76963db5d2"><code>1354be2</code></a> Add support to style function definitions with newlines before function stubs...</li>
<li><a href="https://github.com/psf/black/commit/f4b644b82f64d5aa2b8959277c9eb9ebcb16affe"><code>f4b644b</code></a> Prevent wrapping of multiline fstrings in parens (<a href="https://redirect.github.com/psf/black/issues/4325">#4325</a>)</li>
<li><a href="https://github.com/psf/black/commit/551ede2825e4a92e9880b90ef517cce333a5cbfc"><code>551ede2</code></a> Add PEP 701 support (<a href="https://redirect.github.com/psf/black/issues/3822">#3822</a>)</li>
<li><a href="https://github.com/psf/black/commit/944b99aa91f0a5afadf48b3a90cacdb5c8e9f858"><code>944b99a</code></a> Bump sphinx from 7.2.6 to 7.3.7 in /docs (<a href="https://redirect.github.com/psf/black/issues/4322">#4322</a>)</li>
<li><a href="https://github.com/psf/black/commit/7134754ef45078b032039ad858bdaaef146233b2"><code>7134754</code></a> Remove node-specific logic from visit_default (<a href="https://redirect.github.com/psf/black/issues/4321">#4321</a>)</li>
<li><a href="https://github.com/psf/black/commit/76693814204bb64fbac48b5c7096ddbd9c978518"><code>7669381</code></a> Pin to old flake8-bugbear (<a href="https://redirect.github.com/psf/black/issues/4319">#4319</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/psf/black/compare/24.2.0...24.4.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=black&package-manager=pip&previous-version=24.2.0&new-version=24.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-24 17:03:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4506" class=".btn">#4506</a>
            </td>
            <td>
                <b>
                    [chore]: Bump zeroize from 1.7.0 to 1.8.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [zeroize](https://github.com/RustCrypto/utils) from 1.7.0 to 1.8.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/RustCrypto/utils/commit/9bbfb49e6541d710aea6f7a95c68c9f3d99140e2"><code>9bbfb49</code></a> zeroize 1.8.0 (<a href="https://redirect.github.com/RustCrypto/utils/issues/1065">#1065</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/c0eab7f7abfc244e9fcd482520542329da31f87c"><code>c0eab7f</code></a> cpufeatures: fix macOS build (<a href="https://redirect.github.com/RustCrypto/utils/issues/1066">#1066</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/6d383a554b76df2c6796d8d2982a6a8535342617"><code>6d383a5</code></a> zeroize: always enable AArch64 support (<a href="https://redirect.github.com/RustCrypto/utils/issues/1064">#1064</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/24decb93793936110ae564b6c8e475d91f4e4e44"><code>24decb9</code></a> zeroize: use <code>doc_auto_cfg</code> (<a href="https://redirect.github.com/RustCrypto/utils/issues/1063">#1063</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/cd3a147d62f5f2bf8d5bd10185a52c90f842395b"><code>cd3a147</code></a> build(deps): bump prettyplease from 0.2.16 to 0.2.19 (<a href="https://redirect.github.com/RustCrypto/utils/issues/1061">#1061</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/0105576943f77ae6cd8109cd351a29839150bf02"><code>0105576</code></a> update README to reflect true <code>cmov</code> MSRV (<a href="https://redirect.github.com/RustCrypto/utils/issues/965">#965</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/216d2b82f691487b80e8d94022a1aaf45b2f926f"><code>216d2b8</code></a> build(deps): bump hybrid-array from 0.2.0-rc.7 to 0.2.0-rc.8 (<a href="https://redirect.github.com/RustCrypto/utils/issues/1058">#1058</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/ce47b3c74f46217995192d092c4d2dd3bc954986"><code>ce47b3c</code></a> fiat-constify: filter out <code>let mut</code> declarations (<a href="https://redirect.github.com/RustCrypto/utils/issues/1057">#1057</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/4c583ffa7714ebdaea822ff581aa15b737d66231"><code>4c583ff</code></a> zeroize: add Zeroize impls for <code>__m512</code> types; MSRV 1.72 (<a href="https://redirect.github.com/RustCrypto/utils/issues/1052">#1052</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/9e1287a31bc99bcab669710dd185bfa909899e6d"><code>9e1287a</code></a> build(deps): bump hybrid-array from 0.2.0-rc.5 to 0.2.0-rc.7 (<a href="https://redirect.github.com/RustCrypto/utils/issues/1056">#1056</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/RustCrypto/utils/compare/zeroize-v1.7.0...zeroize-v1.8.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=zeroize&package-manager=cargo&previous-version=1.7.0&new-version=1.8.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-24 16:35:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4505" class=".btn">#4505</a>
            </td>
            <td>
                <b>
                    [chore]: format doc comments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Chore</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-24 08:20:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4504" class=".btn">#4504</a>
            </td>
            <td>
                <b>
                    [chore]: Refer to MAINTAINERS.md in `main` from `iroha1-main`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

To avoid maintaining two separate MAINTAINERS lists (with the same content), only refer to it from the `iroha1-main` branch.

### Benefits

No need to keep two files in sync.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-24 06:35:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4503" class=".btn">#4503</a>
            </td>
            <td>
                <b>
                    [fix] #4331: Revoke removed `PermissionToken`s on `Upgrade<Executor>`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

If some permission token was removed from schema during executor migration, then revoke that permission token from related roles and accounts.

### Linked issue

Closes #4331

### Benefits

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-23 18:49:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4498" class=".btn">#4498</a>
            </td>
            <td>
                <b>
                    Bump actions/cache from 3 to 4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/cache](https://github.com/actions/cache) from 3 to 4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/cache/releases">actions/cache's releases</a>.</em></p>
<blockquote>
<h2>v4.0.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Update action to node20 by <a href="https://github.com/takost"><code>@​takost</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1284">actions/cache#1284</a></li>
<li>feat: save-always flag by <a href="https://github.com/to-s"><code>@​to-s</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1242">actions/cache#1242</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/takost"><code>@​takost</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1284">actions/cache#1284</a></li>
<li><a href="https://github.com/to-s"><code>@​to-s</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1242">actions/cache#1242</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/cache/compare/v3...v4.0.0">https://github.com/actions/cache/compare/v3...v4.0.0</a></p>
<h2>v3.3.3</h2>
<h2>What's Changed</h2>
<ul>
<li>Cache v3.3.3 by <a href="https://github.com/robherley"><code>@​robherley</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1302">actions/cache#1302</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/robherley"><code>@​robherley</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1302">actions/cache#1302</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/cache/compare/v3...v3.3.3">https://github.com/actions/cache/compare/v3...v3.3.3</a></p>
<h2>v3.3.2</h2>
<h2>What's Changed</h2>
<ul>
<li>Fixed readme with new segment timeout values by <a href="https://github.com/kotewar"><code>@​kotewar</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1133">actions/cache#1133</a></li>
<li>Readme fixes by <a href="https://github.com/kotewar"><code>@​kotewar</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1134">actions/cache#1134</a></li>
<li>Updated description of the lookup-only input for main action by <a href="https://github.com/kotewar"><code>@​kotewar</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1130">actions/cache#1130</a></li>
<li>Change two new actions mention as quoted text by <a href="https://github.com/bishal-pdMSFT"><code>@​bishal-pdMSFT</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1131">actions/cache#1131</a></li>
<li>Update Cross-OS Caching tips by <a href="https://github.com/pdotl"><code>@​pdotl</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1122">actions/cache#1122</a></li>
<li>Bazel example (Take <a href="https://redirect.github.com/actions/cache/issues/2">#2</a>️⃣) by <a href="https://github.com/vorburger"><code>@​vorburger</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1132">actions/cache#1132</a></li>
<li>Remove actions to add new PRs and issues to a project board by <a href="https://github.com/jorendorff"><code>@​jorendorff</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1187">actions/cache#1187</a></li>
<li>Consume latest toolkit and fix dangling promise bug by <a href="https://github.com/chkimes"><code>@​chkimes</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1217">actions/cache#1217</a></li>
<li>Bump action version to 3.3.2 by <a href="https://github.com/bethanyj28"><code>@​bethanyj28</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1236">actions/cache#1236</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/vorburger"><code>@​vorburger</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1132">actions/cache#1132</a></li>
<li><a href="https://github.com/jorendorff"><code>@​jorendorff</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1187">actions/cache#1187</a></li>
<li><a href="https://github.com/chkimes"><code>@​chkimes</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1217">actions/cache#1217</a></li>
<li><a href="https://github.com/bethanyj28"><code>@​bethanyj28</code></a> made their first contribution in <a href="https://redirect.github.com/actions/cache/pull/1236">actions/cache#1236</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/cache/compare/v3...v3.3.2">https://github.com/actions/cache/compare/v3...v3.3.2</a></p>
<h2>v3.3.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Reduced download segment size to 128 MB and timeout to 10 minutes by <a href="https://github.com/kotewar"><code>@​kotewar</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1129">actions/cache#1129</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/cache/compare/v3...v3.3.1">https://github.com/actions/cache/compare/v3...v3.3.1</a></p>
<h2>v3.3.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Bug: Permission is missing in cache delete example by <a href="https://github.com/kotokaze"><code>@​kotokaze</code></a> in <a href="https://redirect.github.com/actions/cache/pull/1123">actions/cache#1123</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/actions/cache/blob/main/RELEASES.md">actions/cache's changelog</a>.</em></p>
<blockquote>
<h1>Releases</h1>
<h3>4.0.2</h3>
<ul>
<li>Fixed restore <code>fail-on-cache-miss</code> not working.</li>
</ul>
<h3>4.0.1</h3>
<ul>
<li>Updated <code>isGhes</code> check</li>
</ul>
<h3>4.0.0</h3>
<ul>
<li>Updated minimum runner version support from node 12 -&gt; node 20</li>
</ul>
<h3>3.3.3</h3>
<ul>
<li>Updates <code>@​actions/cache</code> to v3.2.3 to fix accidental mutated path arguments to <code>getCacheVersion</code> <a href="https://redirect.github.com/actions/toolkit/pull/1378">actions/toolkit#1378</a></li>
<li>Additional audit fixes of npm package(s)</li>
</ul>
<h3>3.3.2</h3>
<ul>
<li>Fixes bug with Azure SDK causing blob downloads to get stuck.</li>
</ul>
<h3>3.3.1</h3>
<ul>
<li>Reduced segment size to 128MB and segment timeout to 10 minutes to fail fast in case the cache download is stuck.</li>
</ul>
<h3>3.3.0</h3>
<ul>
<li>Added option to lookup cache without downloading it.</li>
</ul>
<h3>3.2.6</h3>
<ul>
<li>Fix zstd not being used after zstd version upgrade to 1.5.4 on hosted runners.</li>
</ul>
<h3>3.2.5</h3>
<ul>
<li>Added fix to prevent from setting MYSYS environment variable globally.</li>
</ul>
<h3>3.2.4</h3>
<ul>
<li>Added option to fail job on cache miss.</li>
</ul>
<h3>3.2.3</h3>
<ul>
<li>Support cross os caching on Windows as an opt-in feature.</li>
<li>Fix issue with symlink restoration on Windows for cross-os caches.</li>
</ul>
<h3>3.2.2</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/cache/commit/0c45773b623bea8c8e75f6c82b208c3cf94ea4f9"><code>0c45773</code></a> Merge pull request <a href="https://redirect.github.com/actions/cache/issues/1327">#1327</a> from cdce8p/fix-fail-on-cache-miss</li>
<li><a href="https://github.com/actions/cache/commit/8a55f839aa4b4578e47bdc8a52828637cbb9a454"><code>8a55f83</code></a> Add test case for process exit</li>
<li><a href="https://github.com/actions/cache/commit/3884cace147bdf9307fcc52a277f421af7b30798"><code>3884cac</code></a> Bump version</li>
<li><a href="https://github.com/actions/cache/commit/e29dad3e36390db18fc19fb666cb1302f4929002"><code>e29dad3</code></a> Fix fail-on-cache-miss not working</li>
<li><a href="https://github.com/actions/cache/commit/ab5e6d0c87105b4c9c2047343972218f562e4319"><code>ab5e6d0</code></a> Merge pull request <a href="https://redirect.github.com/actions/cache/issues/1341">#1341</a> from bethanyj28/main</li>
<li><a href="https://github.com/actions/cache/commit/89c7d86c71006451e399dfcc588eed8e392e0dcf"><code>89c7d86</code></a> licensed cache</li>
<li><a href="https://github.com/actions/cache/commit/d2c84da363007d814e47d50565ba3794c1a84c56"><code>d2c84da</code></a> update <code>@​actions/cache</code></li>
<li><a href="https://github.com/actions/cache/commit/37e7d4eb166540050942d75a6e40742cbfc92f65"><code>37e7d4e</code></a> Merge pull request <a href="https://redirect.github.com/actions/cache/issues/1340">#1340</a> from actions/bethanyj28/update-publish-flow</li>
<li><a href="https://github.com/actions/cache/commit/a18323f50430a57f9094db3ce508dc1e3a25d4a2"><code>a18323f</code></a> add release action</li>
<li><a href="https://github.com/actions/cache/commit/a2ed59d39b352305bdd2f628719a53b2cc4f9613"><code>a2ed59d</code></a> Merge pull request <a href="https://redirect.github.com/actions/cache/issues/1305">#1305</a> from actions/yacaovsnc/update_examples</li>
<li>Additional commits viewable in <a href="https://github.com/actions/cache/compare/v3...v4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/cache&package-manager=github_actions&previous-version=3&new-version=4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-22 17:02:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4497" class=".btn">#4497</a>
            </td>
            <td>
                <b>
                    Bump base64 from 0.21.7 to 0.22.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [base64](https://github.com/marshallpierce/rust-base64) from 0.21.7 to 0.22.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/marshallpierce/rust-base64/blob/master/RELEASE-NOTES.md">base64's changelog</a>.</em></p>
<blockquote>
<h1>0.22.0</h1>
<ul>
<li><code>DecodeSliceError::OutputSliceTooSmall</code> is now conservative rather than precise. That is, the error will only occur if the decoded output <em>cannot</em> fit, meaning that <code>Engine::decode_slice</code> can now be used with exactly-sized output slices. As part of this, <code>Engine::internal_decode</code> now returns <code>DecodeSliceError</code> instead of <code>DecodeError</code>, but that is not expected to affect any external callers.</li>
<li><code>DecodeError::InvalidLength</code> now refers specifically to the <em>number of valid symbols</em> being invalid (i.e. <code>len % 4 == 1</code>), rather than just the number of input bytes. This avoids confusing scenarios when based on interpretation you could make a case for either <code>InvalidLength</code> or <code>InvalidByte</code> being appropriate.</li>
<li>Decoding is somewhat faster (5-10%)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/5d70ba7576f9aafcbf02bd8acfcb9973411fb95f"><code>5d70ba7</code></a> Merge pull request <a href="https://redirect.github.com/marshallpierce/rust-base64/issues/269">#269</a> from marshallpierce/mp/decode-precisely</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/efb6c006c75ddbe60c084c2e3e0e084cd18b0122"><code>efb6c00</code></a> Release notes</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/2b91084a31ad11624acd81e06455ba0cbd21d4a8"><code>2b91084</code></a> Add some tests to boost coverage</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/9e9c7abe65fed78c35a1e94e11446d66ff118c25"><code>9e9c7ab</code></a> Engine::internal_decode now returns DecodeSliceError</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/a8a60f43c56597259558261353b5bf7e953eed36"><code>a8a60f4</code></a> Decode main loop improvements</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/a25be0667c63460827cfadd71d1630acb442bb09"><code>a25be06</code></a> Simplify leftover output writes</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/9979cc33bb964b4ee36898773a01f546d2c6487a"><code>9979cc3</code></a> Keep morsels as separate bytes</li>
<li><a href="https://github.com/marshallpierce/rust-base64/commit/37670c5ec224eec3af9778fb371c5529dfab52af"><code>37670c5</code></a> Bump dev toolchain version (<a href="https://redirect.github.com/marshallpierce/rust-base64/issues/268">#268</a>)</li>
<li>See full diff in <a href="https://github.com/marshallpierce/rust-base64/compare/v0.21.7...v0.22.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=base64&package-manager=cargo&previous-version=0.21.7&new-version=0.22.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-22 16:43:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4496" class=".btn">#4496</a>
            </td>
            <td>
                <b>
                    Bump thiserror from 1.0.58 to 1.0.59
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [thiserror](https://github.com/dtolnay/thiserror) from 1.0.58 to 1.0.59.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/thiserror/releases">thiserror's releases</a>.</em></p>
<blockquote>
<h2>1.0.59</h2>
<ul>
<li>Unblock testing of rustc <code>debug-fmt-detail</code> option (<a href="https://redirect.github.com/dtolnay/thiserror/issues/297">#297</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/thiserror/commit/e7ad85ee6b135c5748d37ed1e8edda950336af77"><code>e7ad85e</code></a> Release 1.0.59</li>
<li><a href="https://github.com/dtolnay/thiserror/commit/af477ecbe5ed355cc1d5da17dc1f2a1b03a696a4"><code>af477ec</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/thiserror/issues/297">#297</a> from dtolnay/traitident</li>
<li><a href="https://github.com/dtolnay/thiserror/commit/f3fbd990483f43153a631604373bb9dc7e071982"><code>f3fbd99</code></a> Implement ToTokens without reliance on {:?}</li>
<li><a href="https://github.com/dtolnay/thiserror/commit/508ece867dce8443efec9d3ff2ace0af659a4755"><code>508ece8</code></a> Revert &quot;Temporarily disable miri on doctests&quot;</li>
<li><a href="https://github.com/dtolnay/thiserror/commit/c8c804ce80c119f5f7a5c20413c2759a4de79246"><code>c8c804c</code></a> Explicitly install a Rust toolchain for cargo-outdated job</li>
<li><a href="https://github.com/dtolnay/thiserror/commit/6969595f5f279cf909ebac7e99b64d17d4c8b08d"><code>6969595</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/thiserror/issues/293">#293</a> from dtolnay/workspacewrapper</li>
<li><a href="https://github.com/dtolnay/thiserror/commit/488d52f111e48103c5bb76cde7e17aafb1dbdcde"><code>488d52f</code></a> Apply RUSTC_WORKSPACE_WRAPPER</li>
<li><a href="https://github.com/dtolnay/thiserror/commit/ba33438c888a04e962c2b9c3439a7312144d386b"><code>ba33438</code></a> Temporarily disable miri on doctests</li>
<li>See full diff in <a href="https://github.com/dtolnay/thiserror/compare/1.0.58...1.0.59">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=thiserror&package-manager=cargo&previous-version=1.0.58&new-version=1.0.59)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-22 16:42:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4495" class=".btn">#4495</a>
            </td>
            <td>
                <b>
                    Bump secp256k1 from 0.28.2 to 0.29.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [secp256k1](https://github.com/rust-bitcoin/rust-secp256k1) from 0.28.2 to 0.29.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/rust-bitcoin/rust-secp256k1/blob/master/CHANGELOG.md">secp256k1's changelog</a>.</em></p>
<blockquote>
<h1>0.29.0 - 2024-04-02</h1>
<ul>
<li>
<p>Deprecate <code>ThirtyTwoByteHash</code> <a href="https://redirect.github.com/rust-bitcoin/rust-secp256k1/pull/686">#686</a></p>
<p>This trait turned out to be problematic during upgrade because we support a ranged dependency for
<code>bitcoin_hashes</code>. Consider implementing <code>From&lt;T&gt; for Message</code> for your type iff your type is a 32
byte hash (ie, output from a hash algorithm that produces a 32 byte digest like sha256). When
using the impl, consider using <code>Message::from</code> instead of <code>hash.into()</code> because we will be
introducing generics in a future version and the compiler will not be able to work out the target
type.</p>
</li>
<li>
<p>Bump MSRV to Rust <code>v1.56.1</code> <a href="https://redirect.github.com/rust-bitcoin/rust-secp256k1/pull/693">#693</a></p>
</li>
<li>
<p>Upgrade <code>hashes</code> using range dependency <code>version = &quot;&gt;= 0.12, &lt;= 0.14&quot;</code> <a href="https://redirect.github.com/rust-bitcoin/rust-secp256k1/pull/690">#690</a></p>
</li>
<li>
<p>Depend on latest <code>secp256k1-sys</code> (vendors <code>secp256k1 v0.4.1</code>) <a href="https://redirect.github.com/rust-bitcoin/rust-secp256k1/pull/688">#688</a></p>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rust-bitcoin/rust-secp256k1/commit/6648126c69ce8056d053cbaa22246d12c76f3fc1"><code>6648126</code></a> Merge <a href="https://redirect.github.com/rust-bitcoin/rust-secp256k1/issues/256">rust-bitcoin/rust-secp256k1256</a>: Release tracking PR: <code>v0.29.0</code></li>
<li><a href="https://github.com/rust-bitcoin/rust-secp256k1/commit/5f9baaa7d5f6ff84dafb780a3ab90afcdb1dd5a9"><code>5f9baaa</code></a> Bump version to 0.29.0</li>
<li><a href="https://github.com/rust-bitcoin/rust-secp256k1/commit/1e814e76392391fa04edbe06b85117cbac6b0d0b"><code>1e814e7</code></a> Merge <a href="https://redirect.github.com/rust-bitcoin/rust-secp256k1/issues/256">rust-bitcoin/rust-secp256k1256</a>: Release tracking PR: `secp256k1-sys 0....</li>
<li><a href="https://github.com/rust-bitcoin/rust-secp256k1/commit/2bba8f9f5a7ea8af619a0df0afb4f36f3e00013a"><code>2bba8f9</code></a> secp256k1-sys: Vendor latest secp256k1</li>
<li><a href="https://github.com/rust-bitcoin/rust-secp256k1/commit/a05078f6e58e2b41997c0dbf7401266fab7d76f6"><code>a05078f</code></a> Merge <a href="https://redirect.github.com/rust-bitcoin/rust-secp256k1/issues/256">rust-bitcoin/rust-secp256k1256</a>: Deprecate <code>ThirtyTwoByteHash</code></li>
<li><a href="https://github.com/rust-bitcoin/rust-secp256k1/commit/9f28cf6ad01157da2dfb35639db7f624f958cc69"><code>9f28cf6</code></a> Deprecate ThirtyTwoByteHash</li>
<li><a href="https://github.com/rust-bitcoin/rust-secp256k1/commit/88c8c58d8d914279f8aa809413fd53f4929f7de4"><code>88c8c58</code></a> Fix import warnings</li>
<li><a href="https://github.com/rust-bitcoin/rust-secp256k1/commit/d279c13bebc5886bf82009d137954f74d017c5ad"><code>d279c13</code></a> Merge <a href="https://redirect.github.com/rust-bitcoin/rust-secp256k1/issues/256">rust-bitcoin/rust-secp256k1256</a>: Upgrade hashes dependency</li>
<li><a href="https://github.com/rust-bitcoin/rust-secp256k1/commit/645271dd7456017e3040a7f5eecae74da947d64c"><code>645271d</code></a> Upgrade hashes dependency</li>
<li><a href="https://github.com/rust-bitcoin/rust-secp256k1/commit/ac706178bff5f0c5f4a848c44164449420e8b56a"><code>ac70617</code></a> Merge <a href="https://redirect.github.com/rust-bitcoin/rust-secp256k1/issues/256">rust-bitcoin/rust-secp256k1256</a>: Bump MSRV to 1.56.1</li>
<li>Additional commits viewable in <a href="https://github.com/rust-bitcoin/rust-secp256k1/compare/secp256k1-0.28.2...secp256k1-0.29.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=secp256k1&package-manager=cargo&previous-version=0.28.2&new-version=0.29.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-22 16:42:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4494" class=".btn">#4494</a>
            </td>
            <td>
                <b>
                    Bump serial_test from 2.0.0 to 3.1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serial_test](https://github.com/palfrey/serial_test) from 2.0.0 to 3.1.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/palfrey/serial_test/releases">serial_test's releases</a>.</em></p>
<blockquote>
<h2>v3.1.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Replace <code>lazy_static</code> with <code>once_cell</code> by <a href="https://github.com/Expyron"><code>@​Expyron</code></a> in <a href="https://redirect.github.com/palfrey/serial_test/pull/106">palfrey/serial_test#106</a></li>
<li>Replace <code>dashmap</code> with <code>scc</code> by <a href="https://github.com/palfrey"><code>@​palfrey</code></a> in <a href="https://redirect.github.com/palfrey/serial_test/pull/109">palfrey/serial_test#109</a></li>
<li>Standard test attribute worked with <code>mod</code>, others didn't (e.g. <code>tokio::test</code>) by <a href="https://github.com/palfrey"><code>@​palfrey</code></a> in <a href="https://redirect.github.com/palfrey/serial_test/pull/110">palfrey/serial_test#110</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/Expyron"><code>@​Expyron</code></a> made their first contribution in <a href="https://redirect.github.com/palfrey/serial_test/pull/106">palfrey/serial_test#106</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/palfrey/serial_test/compare/v3.0.0...v3.1.0">https://github.com/palfrey/serial_test/compare/v3.0.0...v3.1.0</a></p>
<h2>v3.0.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Multi key support <a href="https://redirect.github.com/palfrey/serial_test/pull/102">palfrey/serial_test#102</a>
<ul>
<li>Attributes like <code>#[serial(one, two)]</code> are now supported (for all attributes)</li>
<li>This is a breaking change, as <code>file_serial</code> paths now need to be done separately <code>#[file_serial(key, path =&gt; &quot;/tmp/foo&quot;)]</code></li>
</ul>
</li>
<li>Attributes at a mod-level <a href="https://redirect.github.com/palfrey/serial_test/pull/104">palfrey/serial_test#104</a>
<ul>
<li>You can set any of the attributes on a <code>mod</code> and all <code>#[test]</code> fn's in that mod will have the attribute applied.</li>
</ul>
</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/palfrey/serial_test/compare/v2.0.0...v3.0.0">https://github.com/palfrey/serial_test/compare/v2.0.0...v3.0.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/palfrey/serial_test/commit/25fb94855526a61aa70dba9d09d1d3fd177601be"><code>25fb948</code></a> 3.1.0</li>
<li><a href="https://github.com/palfrey/serial_test/commit/4ccc6bd7dc9ce1f3cc08b65fe44c17e3971cf486"><code>4ccc6bd</code></a> Merge pull request <a href="https://redirect.github.com/palfrey/serial_test/issues/110">#110</a> from palfrey/serial-mod-non-core</li>
<li><a href="https://github.com/palfrey/serial_test/commit/fb32f74f21ca7c19d26cb395270245d534534b2b"><code>fb32f74</code></a> Standard test attribute worked with mod, others didn't</li>
<li><a href="https://github.com/palfrey/serial_test/commit/23894121ec734df7fa12c8f86d95270a8a045c82"><code>2389412</code></a> Merge pull request <a href="https://redirect.github.com/palfrey/serial_test/issues/109">#109</a> from palfrey/remove-dashmap</li>
<li><a href="https://github.com/palfrey/serial_test/commit/14aa91f5d472a1fd2472d637c0e5a53657be514d"><code>14aa91f</code></a> Add more details fslock names</li>
<li><a href="https://github.com/palfrey/serial_test/commit/946db45593c1e5b9368e3ccc7da1d1683fca2c1b"><code>946db45</code></a> Allow unused name for Locks</li>
<li><a href="https://github.com/palfrey/serial_test/commit/1a634fc29b2238fffbbf71e8db7771c172ad750f"><code>1a634fc</code></a> Fix formatting</li>
<li><a href="https://github.com/palfrey/serial_test/commit/2fdcb0c1640a05a5fc09171007052c762b01a88a"><code>2fdcb0c</code></a> Don't capture logs in test_test</li>
<li><a href="https://github.com/palfrey/serial_test/commit/dd2e107185a7d32ad8f64473298a34c157d147ea"><code>dd2e107</code></a> Replace dashmap with scc</li>
<li><a href="https://github.com/palfrey/serial_test/commit/b20dad699e7b50b8b33f1688f57faacb1eb3e9e1"><code>b20dad6</code></a> Merge pull request <a href="https://redirect.github.com/palfrey/serial_test/issues/107">#107</a> from palfrey/dependabot/cargo/mio-0.8.11</li>
<li>Additional commits viewable in <a href="https://github.com/palfrey/serial_test/compare/v2.0.0...v3.1.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serial_test&package-manager=cargo&previous-version=2.0.0&new-version=3.1.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-22 16:41:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4493" class=".btn">#4493</a>
            </td>
            <td>
                <b>
                    [fix]: fix broken regex in PR title action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

"[fix]" in PR title breaks the check due to a malformed regex pattern

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-22 14:40:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4492" class=".btn">#4492</a>
            </td>
            <td>
                <b>
                    [fix]: config test cases use the current configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Some tests in `config` are failing because of outdated fixtures.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-22 14:30:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4491" class=".btn">#4491</a>
            </td>
            <td>
                <b>
                    [fix] #4418: Trigger is callable by multiple users
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Replace `AccountId` with `FilterOpt<AccountId>` to allow execute trigger by any user with permission.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4418 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-22 14:10:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4490" class=".btn">#4490</a>
            </td>
            <td>
                <b>
                    [ci]: Configure dependabot to follow commit message format
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                [ci] Recognize `chore` in PR titles

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks 

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-22 11:10:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4489" class=".btn">#4489</a>
            </td>
            <td>
                <b>
                    [refactor] #4378: Transactional trigger set
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span>
            </td>
            <td>
                <!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

As for WSV, make trigger set make trigger set transactional.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here 
recently, so please walk us through the concepts. -->

### Issues

Closes #4378

### Benefits

For large amount of triggers and frequent trigger execution transactional model allow not to clone trigger set all the time saving time and space.

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks 

Might be not so efficient when there is small amount of triggers.

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-22 11:04:25 +0000 UTC
    </div>
</div>

