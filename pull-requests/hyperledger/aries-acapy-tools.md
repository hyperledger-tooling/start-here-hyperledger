---
layout: default
title: aries-acapy-tools
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-tools
---

# aries-acapy-tools <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-tools){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-tools/pull/51" class=".btn">#51</a>
            </td>
            <td>
                <b>
                    build(deps-dev): Bump the pip group with 2 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group with 2 updates: [certifi](https://github.com/certifi/python-certifi) and [setuptools](https://github.com/pypa/setuptools).

Updates `certifi` from 2023.7.22 to 2024.7.4
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/bd8153872e9c6fc98f4023df9c2deaffea2fa463"><code>bd81538</code></a> 2024.07.04 (<a href="https://redirect.github.com/certifi/python-certifi/issues/295">#295</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/06a2cbf21f345563dde6c28b60e29d57e9b210b3"><code>06a2cbf</code></a> Bump peter-evans/create-pull-request from 6.0.5 to 6.1.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/294">#294</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/13bba02b72bac97c432c277158bc04b4d2a6bc23"><code>13bba02</code></a> Bump actions/checkout from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/293">#293</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e8abcd0e62b334c164b95d49fcabdc9ecbca0554"><code>e8abcd0</code></a> Bump pypa/gh-action-pypi-publish from 1.8.14 to 1.9.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/292">#292</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/124f4adf171e15cd9a91a8b6e0325ecc97be8fe1"><code>124f4ad</code></a> 2024.06.02 (<a href="https://redirect.github.com/certifi/python-certifi/issues/291">#291</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c2196ce5d6ee675b27755a19948480a7823e2c6a"><code>c2196ce</code></a> --- (<a href="https://redirect.github.com/certifi/python-certifi/issues/290">#290</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/fefdeec7588ff1c05214b85a552afcad5fdb51b2"><code>fefdeec</code></a> Bump actions/checkout from 4.1.4 to 4.1.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/289">#289</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/3c5fb1560b826a7f83f1f9750173ff766492c9cf"><code>3c5fb15</code></a> Bump actions/download-artifact from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/286">#286</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/4a9569a3eb58db8548536fc16c5c5c7af946a5b1"><code>4a9569a</code></a> Bump actions/checkout from 4.1.2 to 4.1.4 (<a href="https://redirect.github.com/certifi/python-certifi/issues/287">#287</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/1fc808626a895a916b1e4c2b63abae6c5eafdbe3"><code>1fc8086</code></a> Bump peter-evans/create-pull-request from 6.0.4 to 6.0.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/288">#288</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/certifi/python-certifi/compare/2023.07.22...2024.07.04">compare view</a></li>
</ul>
</details>
<br />

Updates `setuptools` from 67.4.0 to 70.0.0
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pypa/setuptools/blob/main/NEWS.rst">setuptools's changelog</a>.</em></p>
<blockquote>
<h1>v70.0.0</h1>
<h2>Features</h2>
<ul>
<li>Emit a warning when <code>[tools.setuptools]</code> is present in <code>pyproject.toml</code> and will be ignored. -- by :user:<code>SnoopJ</code> (<a href="https://redirect.github.com/pypa/setuptools/issues/4150">#4150</a>)</li>
<li>Improved <code>AttributeError</code> error message if <code>pkg_resources.EntryPoint.require</code> is called without extras or distribution
Gracefully &quot;do nothing&quot; when trying to activate a <code>pkg_resources.Distribution</code> with a <code>None</code> location, rather than raising a <code>TypeError</code>
-- by :user:<code>Avasam</code> (<a href="https://redirect.github.com/pypa/setuptools/issues/4262">#4262</a>)</li>
<li>Typed the dynamically defined variables from <code>pkg_resources</code> -- by :user:<code>Avasam</code> (<a href="https://redirect.github.com/pypa/setuptools/issues/4267">#4267</a>)</li>
<li>Modernized and refactored VCS handling in package_index. (<a href="https://redirect.github.com/pypa/setuptools/issues/4332">#4332</a>)</li>
</ul>
<h2>Bugfixes</h2>
<ul>
<li>In install command, use super to call the superclass methods. Avoids race conditions when monkeypatching from _distutils_system_mod occurs late. (<a href="https://redirect.github.com/pypa/setuptools/issues/4136">#4136</a>)</li>
<li>Fix finder template for lenient editable installs of implicit nested namespaces
constructed by using <code>package_dir</code> to reorganise directory structure. (<a href="https://redirect.github.com/pypa/setuptools/issues/4278">#4278</a>)</li>
<li>Fix an error with <code>UnicodeDecodeError</code> handling in <code>pkg_resources</code> when trying to read files in UTF-8 with a fallback -- by :user:<code>Avasam</code> (<a href="https://redirect.github.com/pypa/setuptools/issues/4348">#4348</a>)</li>
</ul>
<h2>Improved Documentation</h2>
<ul>
<li>Uses RST substitution to put badges in 1 line. (<a href="https://redirect.github.com/pypa/setuptools/issues/4312">#4312</a>)</li>
</ul>
<h2>Deprecations and Removals</h2>
<ul>
<li>
<p>Further adoption of UTF-8 in <code>setuptools</code>.
This change regards mostly files produced and consumed during the build process
(e.g. metadata files, script wrappers, automatically updated config files, etc..)
Although precautions were taken to minimize disruptions, some edge cases might
be subject to backwards incompatibility.</p>
<p>Support for <code>&quot;locale&quot;</code> encoding is now <strong>deprecated</strong>. (<a href="https://redirect.github.com/pypa/setuptools/issues/4309">#4309</a>)</p>
</li>
<li>
<p>Remove <code>setuptools.convert_path</code> after long deprecation period.
This function was never defined by <code>setuptools</code> itself, but rather a
side-effect of an import for internal usage. (<a href="https://redirect.github.com/pypa/setuptools/issues/4322">#4322</a>)</p>
</li>
<li>
<p>Remove fallback for customisations of <code>distutils</code>' <code>build.sub_command</code> after long
deprecated period.
Users are advised to import <code>build</code> directly from <code>setuptools.command.build</code>. (<a href="https://redirect.github.com/pypa/setuptools/issues/4322">#4322</a>)</p>
</li>
<li>
<p>Removed <code>typing_extensions</code> from vendored dependencies -- by :user:<code>Avasam</code> (<a href="https://redirect.github.com/pypa/setuptools/issues/4324">#4324</a>)</p>
</li>
<li>
<p>Remove deprecated <code>setuptools.dep_util</code>.
The provided alternative is <code>setuptools.modified</code>. (<a href="https://redirect.github.com/pypa/setuptools/issues/4360">#4360</a>)</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pypa/setuptools/commit/5cbf12a9b63fd37985a4525617b46576b8ac3a7b"><code>5cbf12a</code></a> Workaround for release error in v70</li>
<li><a href="https://github.com/pypa/setuptools/commit/9c1bcc3417bd12668123f7e731e241d9e57bfc57"><code>9c1bcc3</code></a> Bump version: 69.5.1 → 70.0.0</li>
<li><a href="https://github.com/pypa/setuptools/commit/4dc0c31644b458ac43ce6148f6a9dc729a7e78b5"><code>4dc0c31</code></a> Remove deprecated <code>setuptools.dep_util</code> (<a href="https://redirect.github.com/pypa/setuptools/issues/4360">#4360</a>)</li>
<li><a href="https://github.com/pypa/setuptools/commit/6c1ef5748dbd70c8c5423e12680345766ee101d9"><code>6c1ef57</code></a> Remove xfail now that test passes. Ref <a href="https://redirect.github.com/pypa/setuptools/issues/4371">#4371</a>.</li>
<li><a href="https://github.com/pypa/setuptools/commit/d14fa0162c95450898c11534caf26a0f03553176"><code>d14fa01</code></a> Add all site-packages dirs when creating simulated environment for test_edita...</li>
<li><a href="https://github.com/pypa/setuptools/commit/6b7f7a18afc90007544092c446dc0cd856d86b17"><code>6b7f7a1</code></a> Prevent <code>bin</code> folders to be taken as extern packages when vendoring (<a href="https://redirect.github.com/pypa/setuptools/issues/4370">#4370</a>)</li>
<li><a href="https://github.com/pypa/setuptools/commit/69141f69f8bf38da34cbea552d6fdaa9c8619c53"><code>69141f6</code></a> Add doctest for vendorised bin folder</li>
<li><a href="https://github.com/pypa/setuptools/commit/2a53cc1200ec4b14e08e84be3c042f8983dfb7d7"><code>2a53cc1</code></a> Prevent 'bin' folders to be taken as extern packages</li>
<li><a href="https://github.com/pypa/setuptools/commit/720862807dea012f3a0e7061880691025f736f11"><code>7208628</code></a> Replace call to deprecated <code>validate_pyproject</code> command (<a href="https://redirect.github.com/pypa/setuptools/issues/4363">#4363</a>)</li>
<li><a href="https://github.com/pypa/setuptools/commit/96d681aa405460f724c62c00ca125ae722ad810a"><code>96d681a</code></a> Remove call to deprecated validate_pyproject command</li>
<li>Additional commits viewable in <a href="https://github.com/pypa/setuptools/compare/v67.4.0...v70.0.0">compare view</a></li>
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
- `@dependabot ignore <dependency name> major version` will close this group update PR and stop Dependabot creating any more for the specific dependency's major version (unless you unignore this specific dependency's major version or upgrade to it yourself)
- `@dependabot ignore <dependency name> minor version` will close this group update PR and stop Dependabot creating any more for the specific dependency's minor version (unless you unignore this specific dependency's minor version or upgrade to it yourself)
- `@dependabot ignore <dependency name>` will close this group update PR and stop Dependabot creating any more for the specific dependency (unless you unignore this specific dependency or upgrade to it yourself)
- `@dependabot unignore <dependency name>` will remove all of the ignore conditions of the specified dependency
- `@dependabot unignore <dependency name> <ignore condition>` will remove the ignore condition of the specified dependency and ignore conditions
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-tools/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-15 17:57:04 +0000 UTC
    </div>
</div>

