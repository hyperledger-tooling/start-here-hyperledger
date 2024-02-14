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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2784" class=".btn">#2784</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump the all-actions group with 10 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps the all-actions group with 10 updates:

| Package | From | To |
| --- | --- | --- |
| [actions/checkout](https://github.com/actions/checkout) | `2` | `4` |
| [actions/setup-python](https://github.com/actions/setup-python) | `4` | `5` |
| [psf/black](https://github.com/psf/black) | `24.1.1` | `24.2.0` |
| [github/codeql-action](https://github.com/github/codeql-action) | `2` | `3` |
| [pypa/gh-action-pip-audit](https://github.com/pypa/gh-action-pip-audit) | `1.0.0` | `1.0.8` |
| [actions/cache](https://github.com/actions/cache) | `3` | `4` |
| [docker/setup-buildx-action](https://github.com/docker/setup-buildx-action) | `2` | `3` |
| [docker/login-action](https://github.com/docker/login-action) | `2` | `3` |
| [docker/metadata-action](https://github.com/docker/metadata-action) | `4` | `5` |
| [docker/build-push-action](https://github.com/docker/build-push-action) | `3` | `5` |

Updates `actions/checkout` from 2 to 4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/checkout/releases">actions/checkout's releases</a>.</em></p>
<blockquote>
<h2>v4.0.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Update default runtime to node20 by <a href="https://github.com/takost"><code>@​takost</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1436">actions/checkout#1436</a></li>
<li>Support fetching without the --progress option by <a href="https://github.com/simonbaird"><code>@​simonbaird</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1067">actions/checkout#1067</a></li>
<li>Release 4.0.0 by <a href="https://github.com/takost"><code>@​takost</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1447">actions/checkout#1447</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/takost"><code>@​takost</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1436">actions/checkout#1436</a></li>
<li><a href="https://github.com/simonbaird"><code>@​simonbaird</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1067">actions/checkout#1067</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/checkout/compare/v3...v4.0.0">https://github.com/actions/checkout/compare/v3...v4.0.0</a></p>
<h2>v3.6.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Mark test scripts with Bash'isms to be run via Bash by <a href="https://github.com/dscho"><code>@​dscho</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1377">actions/checkout#1377</a></li>
<li>Add option to fetch tags even if fetch-depth &gt; 0 by <a href="https://github.com/RobertWieczoreck"><code>@​RobertWieczoreck</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/579">actions/checkout#579</a></li>
<li>Release 3.6.0 by <a href="https://github.com/luketomlinson"><code>@​luketomlinson</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1437">actions/checkout#1437</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/RobertWieczoreck"><code>@​RobertWieczoreck</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/579">actions/checkout#579</a></li>
<li><a href="https://github.com/luketomlinson"><code>@​luketomlinson</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1437">actions/checkout#1437</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/checkout/compare/v3.5.3...v3.6.0">https://github.com/actions/checkout/compare/v3.5.3...v3.6.0</a></p>
<h2>v3.5.3</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix: Checkout Issue in self hosted runner due to faulty submodule check-ins by <a href="https://github.com/megamanics"><code>@​megamanics</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1196">actions/checkout#1196</a></li>
<li>Fix typos found by codespell by <a href="https://github.com/DimitriPapadopoulos"><code>@​DimitriPapadopoulos</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1287">actions/checkout#1287</a></li>
<li>Add support for sparse checkouts by <a href="https://github.com/dscho"><code>@​dscho</code></a> and <a href="https://github.com/dfdez"><code>@​dfdez</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1369">actions/checkout#1369</a></li>
<li>Release v3.5.3 by <a href="https://github.com/TingluoHuang"><code>@​TingluoHuang</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1376">actions/checkout#1376</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/megamanics"><code>@​megamanics</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1196">actions/checkout#1196</a></li>
<li><a href="https://github.com/DimitriPapadopoulos"><code>@​DimitriPapadopoulos</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1287">actions/checkout#1287</a></li>
<li><a href="https://github.com/dfdez"><code>@​dfdez</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1369">actions/checkout#1369</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/checkout/compare/v3...v3.5.3">https://github.com/actions/checkout/compare/v3...v3.5.3</a></p>
<h2>v3.5.2</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix: Use correct API url / endpoint in GHES by <a href="https://github.com/fhammerl"><code>@​fhammerl</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1289">actions/checkout#1289</a> based on <a href="https://redirect.github.com/actions/checkout/issues/1286">#1286</a> by <a href="https://github.com/1newsr"><code>@​1newsr</code></a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/checkout/compare/v3.5.1...v3.5.2">https://github.com/actions/checkout/compare/v3.5.1...v3.5.2</a></p>
<h2>v3.5.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Improve checkout performance on Windows runners by upgrading <code>@​actions/github</code> dependency by <a href="https://github.com/BrettDong"><code>@​BrettDong</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1246">actions/checkout#1246</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/BrettDong"><code>@​BrettDong</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1246">actions/checkout#1246</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/actions/checkout/blob/main/CHANGELOG.md">actions/checkout's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<h2>v4.1.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1396">Add support for partial checkout filters</a></li>
</ul>
<h2>v4.0.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1067">Support fetching without the --progress option</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1436">Update to node20</a></li>
</ul>
<h2>v3.6.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1377">Fix: Mark test scripts with Bash'isms to be run via Bash</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/579">Add option to fetch tags even if fetch-depth &gt; 0</a></li>
</ul>
<h2>v3.5.3</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1196">Fix: Checkout fail in self-hosted runners when faulty submodule are checked-in</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1287">Fix typos found by codespell</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1369">Add support for sparse checkouts</a></li>
</ul>
<h2>v3.5.2</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1289">Fix api endpoint for GHES</a></li>
</ul>
<h2>v3.5.1</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1246">Fix slow checkout on Windows</a></li>
</ul>
<h2>v3.5.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1237">Add new public key for known_hosts</a></li>
</ul>
<h2>v3.4.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1209">Upgrade codeql actions to v2</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1210">Upgrade dependencies</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1225">Upgrade <code>@​actions/io</code></a></li>
</ul>
<h2>v3.3.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1045">Implement branch list using callbacks from exec function</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1050">Add in explicit reference to private checkout options</a></li>
<li>[Fix comment typos (that got added in <a href="https://redirect.github.com/actions/checkout/issues/770">#770</a>)](<a href="https://redirect.github.com/actions/checkout/pull/1057">actions/checkout#1057</a>)</li>
</ul>
<h2>v3.2.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/942">Add GitHub Action to perform release</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/967">Fix status badge</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1002">Replace datadog/squid with ubuntu/squid Docker image</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/964">Wrap pipeline commands for submoduleForeach in quotes</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1029">Update <code>@​actions/io</code> to 1.1.2</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1039">Upgrading version to 3.2.0</a></li>
</ul>
<h2>v3.1.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/939">Use <code>@​actions/core</code> <code>saveState</code> and <code>getState</code></a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/922">Add <code>github-server-url</code> input</a></li>
</ul>
<h2>v3.0.2</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/checkout/commit/b4ffde65f46336ab88eb53be808477a3936bae11"><code>b4ffde6</code></a> Link to release page from what's new section (<a href="https://redirect.github.com/actions/checkout/issues/1514">#1514</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/8530928916aaef40f59e6f221989ccb31f5759e7"><code>8530928</code></a> Correct link to GitHub Docs (<a href="https://redirect.github.com/actions/checkout/issues/1511">#1511</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/7cdaf2fbc075e6f3b9ca94cfd6cec5adc8a75622"><code>7cdaf2f</code></a> Update CODEOWNERS to Launch team (<a href="https://redirect.github.com/actions/checkout/issues/1510">#1510</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/8ade135a41bc03ea155e62e844d188df1ea18608"><code>8ade135</code></a> Prepare 4.1.0 release (<a href="https://redirect.github.com/actions/checkout/issues/1496">#1496</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/c533a0a4cfc4962971818edcfac47a2899e69799"><code>c533a0a</code></a> Add support for partial checkout filters (<a href="https://redirect.github.com/actions/checkout/issues/1396">#1396</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/72f2cec99f417b1a1c5e2e88945068983b7965f9"><code>72f2cec</code></a> Update README.md for V4 (<a href="https://redirect.github.com/actions/checkout/issues/1452">#1452</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/3df4ab11eba7bda6032a0b82a6bb43b11571feac"><code>3df4ab1</code></a> Release 4.0.0 (<a href="https://redirect.github.com/actions/checkout/issues/1447">#1447</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/8b5e8b768746b50394015010d25e690bfab9dfbc"><code>8b5e8b7</code></a> Support fetching without the --progress option (<a href="https://redirect.github.com/actions/checkout/issues/1067">#1067</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/97a652b80035363df47baee5031ec8670b8878ac"><code>97a652b</code></a> Update default runtime to node20 (<a href="https://redirect.github.com/actions/checkout/issues/1436">#1436</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/f43a0e5ff2bd294095638e18286ca9a3d1956744"><code>f43a0e5</code></a> Release 3.6.0 (<a href="https://redirect.github.com/actions/checkout/issues/1437">#1437</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/actions/checkout/compare/v2...v4">compare view</a></li>
</ul>
</details>
<br />

Updates `actions/setup-python` from 4 to 5
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/setup-python/releases">actions/setup-python's releases</a>.</em></p>
<blockquote>
<h2>v5.0.0</h2>
<h2>What's Changed</h2>
<p>In scope of this release, we update node version runtime from node16 to node20 (<a href="https://redirect.github.com/actions/setup-python/pull/772">actions/setup-python#772</a>). Besides, we update dependencies to the latest versions.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/setup-python/compare/v4.8.0...v5.0.0">https://github.com/actions/setup-python/compare/v4.8.0...v5.0.0</a></p>
<h2>v4.8.0</h2>
<h2>What's Changed</h2>
<p>In scope of this release we added support for GraalPy (<a href="https://redirect.github.com/actions/setup-python/pull/694">actions/setup-python#694</a>). You can use this snippet to set up GraalPy:</p>
<pre lang="yaml"><code>steps:
- uses: actions/checkout@v4
- uses: actions/setup-python@v4 
  with:
    python-version: 'graalpy-22.3' 
- run: python my_script.py
</code></pre>
<p>Besides, the release contains such changes as:</p>
<ul>
<li>Trim python version when reading from file by <a href="https://github.com/FerranPares"><code>@​FerranPares</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/628">actions/setup-python#628</a></li>
<li>Use non-deprecated versions in examples by <a href="https://github.com/jeffwidman"><code>@​jeffwidman</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/724">actions/setup-python#724</a></li>
<li>Change deprecation comment to past tense by <a href="https://github.com/jeffwidman"><code>@​jeffwidman</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/723">actions/setup-python#723</a></li>
<li>Bump <code>@​babel/traverse</code> from 7.9.0 to 7.23.2 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/743">actions/setup-python#743</a></li>
<li>advanced-usage.md: Encourage the use actions/checkout@v4 by <a href="https://github.com/cclauss"><code>@​cclauss</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/729">actions/setup-python#729</a></li>
<li>Examples now use checkout@v4 by <a href="https://github.com/simonw"><code>@​simonw</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/738">actions/setup-python#738</a></li>
<li>Update actions/checkout to v4 by <a href="https://github.com/dmitry-shibanov"><code>@​dmitry-shibanov</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/761">actions/setup-python#761</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/FerranPares"><code>@​FerranPares</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-python/pull/628">actions/setup-python#628</a></li>
<li><a href="https://github.com/timfel"><code>@​timfel</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-python/pull/694">actions/setup-python#694</a></li>
<li><a href="https://github.com/jeffwidman"><code>@​jeffwidman</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-python/pull/724">actions/setup-python#724</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/setup-python/compare/v4...v4.8.0">https://github.com/actions/setup-python/compare/v4...v4.8.0</a></p>
<h2>v4.7.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Bump word-wrap from 1.2.3 to 1.2.4 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/702">actions/setup-python#702</a></li>
<li>Add range validation for toml files by <a href="https://github.com/dmitry-shibanov"><code>@​dmitry-shibanov</code></a> in <a href="https://redirect.github.com/actions/setup-python/pull/726">actions/setup-python#726</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/setup-python/compare/v4...v4.7.1">https://github.com/actions/setup-python/compare/v4...v4.7.1</a></p>
<h2>v4.7.0</h2>
<p>In scope of this release, the support for reading python version from pyproject.toml was added (<a href="https://redirect.github.com/actions/setup-python/pull/669">actions/setup-python#669</a>).</p>
<pre lang="yaml"><code>      - name: Setup Python
        uses: actions/setup-python@v4
&lt;/tr&gt;&lt;/table&gt; 
</code></pre>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/setup-python/commit/0a5c61591373683505ea898e09a3ea4f39ef2b9c"><code>0a5c615</code></a> Update action to node20 (<a href="https://redirect.github.com/actions/setup-python/issues/772">#772</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/0ae58361cdfd39e2950bed97a1e26aa20c3d8955"><code>0ae5836</code></a> Add example of GraalPy to docs (<a href="https://redirect.github.com/actions/setup-python/issues/773">#773</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/b64ffcaf5b410884ad320a9cfac8866006a109aa"><code>b64ffca</code></a> update actions/checkout to v4 (<a href="https://redirect.github.com/actions/setup-python/issues/761">#761</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/8d2896179abf658742de432b3f203d2c2d86a587"><code>8d28961</code></a> Examples now use checkout@v4 (<a href="https://redirect.github.com/actions/setup-python/issues/738">#738</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/7bc6abb01e0555719edc2dbca70a2fde309e5e56"><code>7bc6abb</code></a> advanced-usage.md: Encourage the use actions/checkout@v4 (<a href="https://redirect.github.com/actions/setup-python/issues/729">#729</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/e8111cec9d3dc15220d8a3b638f08419f57b906a"><code>e8111ce</code></a> Bump <code>@​babel/traverse</code> from 7.9.0 to 7.23.2 (<a href="https://redirect.github.com/actions/setup-python/issues/743">#743</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/a00ea43da65e7c04d2bdae58b3afecd77057eb9e"><code>a00ea43</code></a> add fix for graalpy ci (<a href="https://redirect.github.com/actions/setup-python/issues/741">#741</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/8635b1ccc5934e73ed3510980fd2e7790b85839b"><code>8635b1c</code></a> Change deprecation comment to past tense (<a href="https://redirect.github.com/actions/setup-python/issues/723">#723</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/f6cc428f535856f9c23558d01765a42a4d6cf758"><code>f6cc428</code></a> Use non-deprecated versions in examples (<a href="https://redirect.github.com/actions/setup-python/issues/724">#724</a>)</li>
<li><a href="https://github.com/actions/setup-python/commit/5f2af211d616f86005883b44826180b21abb4060"><code>5f2af21</code></a> Add GraalPy support (<a href="https://redirect.github.com/actions/setup-python/issues/694">#694</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/actions/setup-python/compare/v4...v5">compare view</a></li>
</ul>
</details>
<br />

Updates `psf/black` from 24.1.1 to 24.2.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/black/releases">psf/black's releases</a>.</em></p>
<blockquote>
<h2>24.2.0</h2>
<h3>Stable style</h3>
<ul>
<li>Fixed a bug where comments where mistakenly removed along with redundant parentheses
(<a href="https://redirect.github.com/psf/black/issues/4218">#4218</a>)</li>
</ul>
<h3>Preview style</h3>
<ul>
<li>Move the <code>hug_parens_with_braces_and_square_brackets</code> feature to the unstable style
due to an outstanding crash and proposed formatting tweaks (<a href="https://redirect.github.com/psf/black/issues/4198">#4198</a>)</li>
<li>Fixed a bug where base expressions caused inconsistent formatting of ** in tenary
expression (<a href="https://redirect.github.com/psf/black/issues/4154">#4154</a>)</li>
<li>Checking for newline before adding one on docstring that is almost at the line limit
(<a href="https://redirect.github.com/psf/black/issues/4185">#4185</a>)</li>
<li>Remove redundant parentheses in <code>case</code> statement <code>if</code> guards (<a href="https://redirect.github.com/psf/black/issues/4214">#4214</a>).</li>
</ul>
<h3>Configuration</h3>
<ul>
<li>Fix issue where <em>Black</em> would ignore input files in the presence of symlinks (<a href="https://redirect.github.com/psf/black/issues/4222">#4222</a>)</li>
<li><em>Black</em> now ignores <code>pyproject.toml</code> that is missing a <code>tool.black</code> section when
discovering project root and configuration. Since <em>Black</em> continues to use version
control as an indicator of project root, this is expected to primarily change behavior
for users in a monorepo setup (desirably). If you wish to preserve previous behavior,
simply add an empty <code>[tool.black]</code> to the previously discovered <code>pyproject.toml</code>
(<a href="https://redirect.github.com/psf/black/issues/4204">#4204</a>)</li>
</ul>
<h3>Output</h3>
<ul>
<li>Black will swallow any <code>SyntaxWarning</code>s or <code>DeprecationWarning</code>s produced by the <code>ast</code>
module when performing equivalence checks (<a href="https://redirect.github.com/psf/black/issues/4189">#4189</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Add a JSONSchema and provide a validate-pyproject entry-point (<a href="https://redirect.github.com/psf/black/issues/4181">#4181</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/black/blob/main/CHANGES.md">psf/black's changelog</a>.</em></p>
<blockquote>
<h2>24.2.0</h2>
<h3>Stable style</h3>
<ul>
<li>Fixed a bug where comments where mistakenly removed along with redundant parentheses
(<a href="https://redirect.github.com/psf/black/issues/4218">#4218</a>)</li>
</ul>
<h3>Preview style</h3>
<ul>
<li>Move the <code>hug_parens_with_braces_and_square_brackets</code> feature to the unstable style
due to an outstanding crash and proposed formatting tweaks (<a href="https://redirect.github.com/psf/black/issues/4198">#4198</a>)</li>
<li>Fixed a bug where base expressions caused inconsistent formatting of ** in tenary
expression (<a href="https://redirect.github.com/psf/black/issues/4154">#4154</a>)</li>
<li>Checking for newline before adding one on docstring that is almost at the line limit
(<a href="https://redirect.github.com/psf/black/issues/4185">#4185</a>)</li>
<li>Remove redundant parentheses in <code>case</code> statement <code>if</code> guards (<a href="https://redirect.github.com/psf/black/issues/4214">#4214</a>).</li>
</ul>
<h3>Configuration</h3>
<ul>
<li>Fix issue where <em>Black</em> would ignore input files in the presence of symlinks (<a href="https://redirect.github.com/psf/black/issues/4222">#4222</a>)</li>
<li><em>Black</em> now ignores <code>pyproject.toml</code> that is missing a <code>tool.black</code> section when
discovering project root and configuration. Since <em>Black</em> continues to use version
control as an indicator of project root, this is expected to primarily change behavior
for users in a monorepo setup (desirably). If you wish to preserve previous behavior,
simply add an empty <code>[tool.black]</code> to the previously discovered <code>pyproject.toml</code>
(<a href="https://redirect.github.com/psf/black/issues/4204">#4204</a>)</li>
</ul>
<h3>Output</h3>
<ul>
<li>Black will swallow any <code>SyntaxWarning</code>s or <code>DeprecationWarning</code>s produced by the <code>ast</code>
module when performing equivalence checks (<a href="https://redirect.github.com/psf/black/issues/4189">#4189</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Add a JSONSchema and provide a validate-pyproject entry-point (<a href="https://redirect.github.com/psf/black/issues/4181">#4181</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/black/commit/6fdf8a4af28071ed1d079c01122b34c5d587207a"><code>6fdf8a4</code></a> Prepare release 24.2.0 (<a href="https://redirect.github.com/psf/black/issues/4226">#4226</a>)</li>
<li><a href="https://github.com/psf/black/commit/8af439407c051d55f3221cc93795d20bd9af49c9"><code>8af4394</code></a> fix: Don't remove comments along with parens (<a href="https://redirect.github.com/psf/black/issues/4218">#4218</a>)</li>
<li><a href="https://github.com/psf/black/commit/35e97769190d8c8fe94d9ea2d70d7d88b22a2642"><code>35e9776</code></a> Bump pre-commit/action from 3.0.0 to 3.0.1 (<a href="https://redirect.github.com/psf/black/issues/4225">#4225</a>)</li>
<li><a href="https://github.com/psf/black/commit/23dfc5b2c3b0694a8c27e58e28439591976aaf94"><code>23dfc5b</code></a> Fix ignoring input files for symlink reasons (<a href="https://redirect.github.com/psf/black/issues/4222">#4222</a>)</li>
<li><a href="https://github.com/psf/black/commit/a20100395cf6179a81289452efad1d8e72b19682"><code>a201003</code></a> Simplify check for symlinks that resolve outside root (<a href="https://redirect.github.com/psf/black/issues/4221">#4221</a>)</li>
<li><a href="https://github.com/psf/black/commit/dab37a6a1117d690d683121edc4d7c8fb8dd75a7"><code>dab37a6</code></a> Remove redundant parentheses in <code>case</code> statement <code>if</code> guards (<a href="https://redirect.github.com/psf/black/issues/4214">#4214</a>)</li>
<li><a href="https://github.com/psf/black/commit/32230e6f5c4bc6bb5c469451e15f3f54d9884b51"><code>32230e6</code></a> fix: bug where the doublestar operation had inconsistent formatting. (<a href="https://redirect.github.com/psf/black/issues/4154">#4154</a>)</li>
<li><a href="https://github.com/psf/black/commit/7edb50f5a0afc56bb648dc14640ced144366b43a"><code>7edb50f</code></a> fix: additional newline added to docstring when the previous line length is l...</li>
<li><a href="https://github.com/psf/black/commit/3e80de3447dee272e9977ab58b1560a669b7b848"><code>3e80de3</code></a> Bump furo from 2023.9.10 to 2024.1.29 in /docs (<a href="https://redirect.github.com/psf/black/issues/4211">#4211</a>)</li>
<li><a href="https://github.com/psf/black/commit/a08b480a2f39fb4fc7b210d8b450e33d3879f77d"><code>a08b480</code></a> Bump pypa/cibuildwheel from 2.16.4 to 2.16.5 (<a href="https://redirect.github.com/psf/black/issues/4212">#4212</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/psf/black/compare/24.1.1...24.2.0">compare view</a></li>
</ul>
</details>
<br />

Updates `github/codeql-action` from 2 to 3
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/github/codeql-action/releases">github/codeql-action's releases</a>.</em></p>
<blockquote>
<h2>CodeQL Bundle v2.16.2</h2>
<p>Bundles CodeQL CLI v2.16.2</p>
<ul>
<li>(<a href="https://github.com/github/codeql-cli-binaries/blob/HEAD/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql-cli-binaries/releases/tag/v2.16.2">release</a>)</li>
</ul>
<p>Includes the following CodeQL language packs from <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2"><code>github/codeql@codeql-cli/v2.16.2</code></a>:</p>
<ul>
<li><code>codeql/cpp-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/cpp/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/cpp/ql/src">source</a>)</li>
<li><code>codeql/cpp-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/cpp/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/cpp/ql/lib">source</a>)</li>
<li><code>codeql/csharp-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/csharp/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/csharp/ql/src">source</a>)</li>
<li><code>codeql/csharp-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/csharp/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/csharp/ql/lib">source</a>)</li>
<li><code>codeql/go-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/go/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/go/ql/src">source</a>)</li>
<li><code>codeql/go-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/go/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/go/ql/lib">source</a>)</li>
<li><code>codeql/java-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/java/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/java/ql/src">source</a>)</li>
<li><code>codeql/java-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/java/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/java/ql/lib">source</a>)</li>
<li><code>codeql/javascript-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/javascript/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/javascript/ql/src">source</a>)</li>
<li><code>codeql/javascript-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/javascript/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/javascript/ql/lib">source</a>)</li>
<li><code>codeql/python-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/python/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/python/ql/src">source</a>)</li>
<li><code>codeql/python-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/python/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/python/ql/lib">source</a>)</li>
<li><code>codeql/ruby-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/ruby/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/ruby/ql/src">source</a>)</li>
<li><code>codeql/ruby-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/ruby/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/ruby/ql/lib">source</a>)</li>
<li><code>codeql/swift-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/swift/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/swift/ql/src">source</a>)</li>
<li><code>codeql/swift-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/swift/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.2/swift/ql/lib">source</a>)</li>
</ul>
<h2>CodeQL Bundle v2.16.1</h2>
<p>Bundles CodeQL CLI v2.16.1</p>
<ul>
<li>(<a href="https://github.com/github/codeql-cli-binaries/blob/HEAD/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql-cli-binaries/releases/tag/v2.16.1">release</a>)</li>
</ul>
<p>Includes the following CodeQL language packs from <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1"><code>github/codeql@codeql-cli/v2.16.1</code></a>:</p>
<ul>
<li><code>codeql/cpp-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/cpp/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/cpp/ql/src">source</a>)</li>
<li><code>codeql/cpp-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/cpp/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/cpp/ql/lib">source</a>)</li>
<li><code>codeql/csharp-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/csharp/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/csharp/ql/src">source</a>)</li>
<li><code>codeql/csharp-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/csharp/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/csharp/ql/lib">source</a>)</li>
<li><code>codeql/go-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/go/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/go/ql/src">source</a>)</li>
<li><code>codeql/go-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/go/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/go/ql/lib">source</a>)</li>
<li><code>codeql/java-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/java/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/java/ql/src">source</a>)</li>
<li><code>codeql/java-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/java/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/java/ql/lib">source</a>)</li>
<li><code>codeql/javascript-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/javascript/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/javascript/ql/src">source</a>)</li>
<li><code>codeql/javascript-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/javascript/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/javascript/ql/lib">source</a>)</li>
<li><code>codeql/python-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/python/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/python/ql/src">source</a>)</li>
<li><code>codeql/python-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/python/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/python/ql/lib">source</a>)</li>
<li><code>codeql/ruby-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/ruby/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/ruby/ql/src">source</a>)</li>
<li><code>codeql/ruby-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/ruby/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/ruby/ql/lib">source</a>)</li>
<li><code>codeql/swift-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/swift/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/swift/ql/src">source</a>)</li>
<li><code>codeql/swift-all</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/swift/ql/lib/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.1/swift/ql/lib">source</a>)</li>
</ul>
<h2>CodeQL Bundle v2.16.0</h2>
<p>Bundles CodeQL CLI v2.16.0</p>
<ul>
<li>(<a href="https://github.com/github/codeql-cli-binaries/blob/HEAD/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql-cli-binaries/releases/tag/v2.16.0">release</a>)</li>
</ul>
<p>Includes the following CodeQL language packs from <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.0"><code>github/codeql@codeql-cli/v2.16.0</code></a>:</p>
<ul>
<li><code>codeql/cpp-queries</code> (<a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.0/cpp/ql/src/CHANGELOG.md">changelog</a>, <a href="https://github.com/github/codeql/tree/codeql-cli/v2.16.0/cpp/ql/src">source</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/github/codeql-action/blob/main/CHANGELOG.md">github/codeql-action's changelog</a>.</em></p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/github/codeql-action/commit/1d4866b058d22bfd3886703c302daa1d9db6dba1"><code>1d4866b</code></a> Only run custom <code>checkout_path</code> tests against a single CodeQL version</li>
<li><a href="https://github.com/github/codeql-action/commit/da89f3f4cfef781592a672ecabc7f79e2b0ff723"><code>da89f3f</code></a> Update checked-in dependencies</li>
<li><a href="https://github.com/github/codeql-action/commit/921adb69c6a2e54da4d90880be21877927783420"><code>921adb6</code></a> Update changelog and version after v3.24.0</li>
<li><a href="https://github.com/github/codeql-action/commit/e8893c57a1f3a2b659b6b55564fdfdbbd2982911"><code>e8893c5</code></a> Merge pull request <a href="https://redirect.github.com/github/codeql-action/issues/2113">#2113</a> from github/update-v3.24.0-2db032717</li>
<li><a href="https://github.com/github/codeql-action/commit/78d6c8e84d016cf4acb354a3303db8635054030f"><code>78d6c8e</code></a> Update changelog for v3.24.0</li>
<li><a href="https://github.com/github/codeql-action/commit/2db03271718eb704357b7bbf29ef6876a898f966"><code>2db0327</code></a> Merge pull request <a href="https://redirect.github.com/github/codeql-action/issues/2112">#2112</a> from github/henrymercer/status-report-handle-disk-fa...</li>
<li><a href="https://github.com/github/codeql-action/commit/f9dea84e297d93b380c8e1fbee3b726ae2f9a0d1"><code>f9dea84</code></a> Status report: Handle failures determining disk usage</li>
<li>See full diff in <a href="https://github.com/github/codeql-action/compare/v2...v3">compare view</a></li>
</ul>
</details>
<br />

Updates `pypa/gh-action-pip-audit` from 1.0.0 to 1.0.8
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pypa/gh-action-pip-audit/releases">pypa/gh-action-pip-audit's releases</a>.</em></p>
<blockquote>
<h2>v1.0.8</h2>
<h2>What's Changed</h2>
<ul>
<li>Remove pin on requests (fixes <a href="https://redirect.github.com/pypa/gh-action-pip-audit/issues/41">#41</a>) by <a href="https://github.com/Alexerson"><code>@​Alexerson</code></a> in <a href="https://redirect.github.com/pypa/gh-action-pip-audit/pull/42">pypa/gh-action-pip-audit#42</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/Alexerson"><code>@​Alexerson</code></a> made their first contribution in <a href="https://redirect.github.com/pypa/gh-action-pip-audit/pull/42">pypa/gh-action-pip-audit#42</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pypa/gh-action-pip-audit/compare/v1.0.7...v1.0.8">https://github.com/pypa/gh-action-pip-audit/compare/v1.0.7...v1.0.8</a></p>
<h2>v1.0.7</h2>
<h2>What's Changed</h2>
<ul>
<li>action: replace <code>internal-be-careful-debug</code> by <a href="https://github.com/tnytown"><code>@​tnytown</code></a> in <a href="https://redirect.github.com/pypa/gh-action-pip-audit/pull/36">pypa/gh-action-pip-audit#36</a></li>
<li>New issue templates by <a href="https://github.com/tnytown"><code>@​tnytown</code></a> in <a href="https://redirect.github.com/pypa/gh-action-pip-audit/pull/37">pypa/gh-action-pip-audit#37</a></li>
<li>requirements: constrain requests below 2.30 by <a href="https://github.com/woodruffw"><code>@​woodruffw</code></a> in <a href="https://redirect.github.com/pypa/gh-action-pip-audit/pull/39">pypa/gh-action-pip-audit#39</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pypa/gh-action-pip-audit/compare/v1.0.6...v1.0.7">https://github.com/pypa/gh-action-pip-audit/compare/v1.0.6...v1.0.7</a></p>
<h2>Release 1.0.6</h2>
<h2>What's Changed</h2>
<ul>
<li>Check that output file exists before opening by <a href="https://github.com/tnytown"><code>@​tnytown</code></a> in <a href="https://redirect.github.com/pypa/gh-action-pip-audit/pull/33">pypa/gh-action-pip-audit#33</a></li>
<li>README: prep 1.0.6 by <a href="https://github.com/woodruffw"><code>@​woodruffw</code></a> in <a href="https://redirect.github.com/pypa/gh-action-pip-audit/pull/34">pypa/gh-action-pip-audit#34</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/tnytown"><code>@​tnytown</code></a> made their first contribution in <a href="https://redirect.github.com/pypa/gh-action-pip-audit/pull/33">pypa/gh-action-pip-audit#33</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pypa/gh-action-pip-audit/compare/v1.0.5...v1.0.6">https://github.com/pypa/gh-action-pip-audit/compare/v1.0.5...v1.0.6</a></p>
<h2>Release 1.0.5</h2>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pypa/gh-action-pip-audit/compare/v1.0.4...v1.0.5">https://github.com/pypa/gh-action-pip-audit/compare/v1.0.4...v1.0.5</a></p>
<h2>Release 1.0.4</h2>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pypa/gh-action-pip-audit/compare/v1.0.3...v1.0.4">https://github.com/pypa/gh-action-pip-audit/compare/v1.0.3...v1.0.4</a></p>
<h2>Release 1.0.3</h2>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pypa/gh-action-pip-audit/compare/v1.0.2...v1.0.3">https://github.com/pypa/gh-action-pip-audit/compare/v1.0.2...v1.0.3</a></p>
<h2>Release 1.0.2</h2>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pypa/gh-action-pip-audit/compare/v1.0.1...v1.0.2">https://github.com/pypa/gh-action-pip-audit/compare/v1.0.1...v1.0.2</a></p>
<h2>Release 1.0.1</h2>
<h2>What's Changed</h2>
<ul>
<li>action, templates: switch to a template by <a href="https://github.com/woodruffw"><code>@​woodruffw</code></a> in <a href="https://redirect.github.com/pypa/gh-action-pip-audit/pull/24">pypa/gh-action-pip-audit#24</a></li>
<li>action.py: Remove unused line by <a href="https://github.com/di"><code>@​di</code></a> in <a href="https://redirect.github.com/pypa/gh-action-pip-audit/pull/25">pypa/gh-action-pip-audit#25</a></li>
<li>README: update slugs from trailofbits to pypa by <a href="https://github.com/woodruffw"><code>@​woodruffw</code></a> in <a href="https://redirect.github.com/pypa/gh-action-pip-audit/pull/26">pypa/gh-action-pip-audit#26</a></li>
<li>requirements: pip-audit 2.4.4 by <a href="https://github.com/woodruffw"><code>@​woodruffw</code></a> in <a href="https://redirect.github.com/pypa/gh-action-pip-audit/pull/27">pypa/gh-action-pip-audit#27</a></li>
<li>Add FAQ entry for pipenv support by <a href="https://github.com/ameily"><code>@​ameily</code></a> in <a href="https://redirect.github.com/pypa/gh-action-pip-audit/pull/28">pypa/gh-action-pip-audit#28</a></li>
<li>action: remove deprecated use of set-output by <a href="https://github.com/woodruffw"><code>@​woodruffw</code></a> in <a href="https://redirect.github.com/pypa/gh-action-pip-audit/pull/29">pypa/gh-action-pip-audit#29</a></li>
</ul>
<h2>New Contributors</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pypa/gh-action-pip-audit/commit/d499194be74aeb3bc7dbed3a224a87e1831132c7"><code>d499194</code></a> README: prep 1.0.8</li>
<li><a href="https://github.com/pypa/gh-action-pip-audit/commit/cf52d21d8328924292f7d35b638030c3ed537851"><code>cf52d21</code></a> Remove pin on requests (fixes <a href="https://redirect.github.com/pypa/gh-action-pip-audit/issues/41">#41</a>) (<a href="https://redirect.github.com/pypa/gh-action-pip-audit/issues/42">#42</a>)</li>
<li><a href="https://github.com/pypa/gh-action-pip-audit/commit/3ac8fed01c7b32ab70210f182e557d4cb8c45fec"><code>3ac8fed</code></a> README: prep 1.0.7 (<a href="https://redirect.github.com/pypa/gh-action-pip-audit/issues/40">#40</a>)</li>
<li><a href="https://github.com/pypa/gh-action-pip-audit/commit/f7e969538ff23ab335e58d66dbb213fd632e1136"><code>f7e9695</code></a> requirements: constrain requests below 2.30 (<a href="https://redirect.github.com/pypa/gh-action-pip-audit/issues/39">#39</a>)</li>
<li><a href="https://github.com/pypa/gh-action-pip-audit/commit/28aa5e1be685d616b82938ed1fc82c8c12573d25"><code>28aa5e1</code></a> New issue templates (<a href="https://redirect.github.com/pypa/gh-action-pip-audit/issues/37">#37</a>)</li>
<li><a href="https://github.com/pypa/gh-action-pip-audit/commit/1abec09c8d05907edafb747242288fb537fa0629"><code>1abec09</code></a> action: replace <code>internal-be-careful-debug</code> (<a href="https://redirect.github.com/pypa/gh-action-pip-audit/issues/36">#36</a>)</li>
<li><a href="https://github.com/pypa/gh-action-pip-audit/commit/75edeacda5c87f955b25c88b8582b10b9cd1ebc5"><code>75edeac</code></a> README: prep 1.0.6 (<a href="https://redirect.github.com/pypa/gh-action-pip-audit/issues/34">#34</a>)</li>
<li><a href="https://github.com/pypa/gh-action-pip-audit/commit/666b1b8831280710b2ed6b0105307a43302eadfb"><code>666b1b8</code></a> Check that output file exists before opening (<a href="https://redirect.github.com/pypa/gh-action-pip-audit/issues/33">#33</a>)</li>
<li><a href="https://github.com/pypa/gh-action-pip-audit/commit/9075e938de7d8a1c24076730a0c7644cf934826c"><code>9075e93</code></a> README: prep 1.0.5</li>
<li><a href="https://github.com/pypa/gh-action-pip-audit/commit/0007f08635e5ff23e4aec049a3e9b6e597e9822e"><code>0007f08</code></a> requirements: pip-audit &gt;= 2.4.13</li>
<li>Additional commits viewable in <a href="https://github.com/pypa/gh-action-pip-audit/compare/v1.0.0...v1.0.8">compare view</a></li>
</ul>
</details>
<br />

Updates `actions/cache` from 3 to 4
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
<h3>3.0.0</h3>
<ul>
<li>Updated minimum runner version support from node 12 -&gt; node 16</li>
</ul>
<h3>3.0.1</h3>
<ul>
<li>Added support for caching from GHES 3.5.</li>
<li>Fixed download issue for files &gt; 2GB during restore.</li>
</ul>
<h3>3.0.2</h3>
<ul>
<li>Added support for dynamic cache size cap on GHES.</li>
</ul>
<h3>3.0.3</h3>
<ul>
<li>Fixed avoiding empty cache save when no files are available for caching. (<a href="https://redirect.github.com/actions/cache/issues/624">issue</a>)</li>
</ul>
<h3>3.0.4</h3>
<ul>
<li>Fixed tar creation error while trying to create tar with path as <code>~/</code> home folder on <code>ubuntu-latest</code>. (<a href="https://redirect.github.com/actions/cache/issues/689">issue</a>)</li>
</ul>
<h3>3.0.5</h3>
<ul>
<li>Removed error handling by consuming actions/cache 3.0 toolkit, Now cache server error handling will be done by toolkit. (<a href="https://redirect.github.com/actions/cache/pull/834">PR</a>)</li>
</ul>
<h3>3.0.6</h3>
<ul>
<li>Fixed <a href="https://redirect.github.com/actions/cache/issues/809">#809</a> - zstd -d: no such file or directory error</li>
<li>Fixed <a href="https://redirect.github.com/actions/cache/issues/833">#833</a> - cache doesn't work with github workspace directory</li>
</ul>
<h3>3.0.7</h3>
<ul>
<li>Fixed <a href="https://redirect.github.com/actions/cache/issues/810">#810</a> - download stuck issue. A new timeout is introduced in the download process to abort the download if it gets stuck and doesn't finish within an hour.</li>
</ul>
<h3>3.0.8</h3>
<ul>
<li>Fix zstd not working for windows on gnu tar in issues <a href="https://redirect.github.com/actions/cache/issues/888">#888</a> and <a href="https://redirect.github.com/actions/cache/issues/891">#891</a>.</li>
<li>Allowing users to provide a custom timeout as input for aborting download of a cache segment using an environment variable <code>SEGMENT_DOWNLOAD_TIMEOUT_MINS</code>. Default is 60 minutes.</li>
</ul>
<h3>3.0.9</h3>
<ul>
<li>Enhanced the warning message for cache unavailablity in case of GHES.</li>
</ul>
<h3>3.0.10</h3>
<ul>
<li>Fix a bug with sorting inputs.</li>
<li>Update definition for restore-keys in README.md</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/cache/commit/13aacd865c20de90d75de3b17ebe84f7a17d57d2"><code>13aacd8</code></a> Merge pull request <a href="https://redirect.github.com/actions/cache/issues/1242">#1242</a> from to-s/main</li>
<li><a href="https://github.com/actions/cache/commit/53b35c543921fe2e8b288765ff817de9de8d906f"><code>53b35c5</code></a> Merge branch 'main' into main</li>
<li><a href="https://github.com/actions/cache/commit/65b8989fab3bb394817bdb845a453dff480c2b51"><code>65b8989</code></a> Merge pull request <a href="https://redirect.github.com/actions/cache/issues/1284">#1284</a> from takost/update-to-node-20</li>
<li><a href="https://github.com/actions/cache/commit/d0be34d54485f31ca2ccbe66e6ea3d96544a807b"><code>d0be34d</code></a> Fix dist</li>
<li><a href="https://github.com/actions/cache/commit/66cf064d47313d2cccf392d01bd10925da2bd072"><code>66cf064</code></a> Merge branch 'main' into update-to-node-20</li>
<li><a href="https://github.com/actions/cache/commit/1326563738ddb735c5f2ce85cba8c79f33b728cd"><code>1326563</code></a> Merge branch 'main' into main</li>
<li><a href="https://github.com/actions/cache/commit/e71876755e268d6cc25a5d3e3c46ae447e35290a"><code>e718767</code></a> Fix format</li>
<li><a href="https://github.com/actions/cache/commit/01229828ffa049a8dee4db27bcb23ed33f2b451f"><code>0122982</code></a> Apply workaround for earlyExit</li>
<li><a href="https://github.com/actions/cache/commit/3185ecfd6135856ca6d904ae032cff4f39b8b365"><code>3185ecf</code></a> Update &quot;only-&quot; actions to node20</li>
<li><a href="https://github.com/actions/cache/commit/25618a0a675e8447e5ffc8ed9b7ddb2aaf927f65"><code>25618a0</code></a> Bump version</li>
<li>Additional commits viewable in <a href="https://github.com/actions/cache/compare/v3...v4">compare view</a></li>
</ul>
</details>
<br />

Updates `docker/setup-buildx-action` from 2 to 3
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/setup-buildx-action/releases">docker/setup-buildx-action's releases</a>.</em></p>
<blockquote>
<h2>v3.0.0</h2>
<ul>
<li>Node 20 as default runtime (requires <a href="https://github.com/actions/runner/releases/tag/v2.308.0">Actions Runner v2.308.0</a> or later) by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/264">docker/setup-buildx-action#264</a></li>
<li>Bump <code>@​actions/core</code> from 1.10.0 to 1.10.1 in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/267">docker/setup-buildx-action#267</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/setup-buildx-action/compare/v2.10.0...v3.0.0">https://github.com/docker/setup-buildx-action/compare/v2.10.0...v3.0.0</a></p>
<h2>v2.10.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.7.1 to 0.10.0 by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/258">docker/setup-buildx-action#258</a></li>
<li>Bump word-wrap from 1.2.3 to 1.2.5 in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/253">docker/setup-buildx-action#253</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/setup-buildx-action/compare/v2.9.1...v2.10.0">https://github.com/docker/setup-buildx-action/compare/v2.9.1...v2.10.0</a></p>
<h2>v2.9.1</h2>
<ul>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.7.0 to 0.7.1 in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/248">docker/setup-buildx-action#248</a>
<ul>
<li>Fixes an issue where building Buildx does not match the local platform (<a href="https://redirect.github.com/docker/actions-toolkit/pull/135">docker/actions-toolkit#135</a>)</li>
</ul>
</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/setup-buildx-action/compare/v2.9.0...v2.9.1">https://github.com/docker/setup-buildx-action/compare/v2.9.0...v2.9.1</a></p>
<h2>v2.9.0</h2>
<ul>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.6.0 to 0.7.0 in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/246">docker/setup-buildx-action#246</a>
<ul>
<li>Adds support to cache Buildx binary to hosted tool cache and GHA cache backend</li>
</ul>
</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/setup-buildx-action/compare/v2.8.0...v2.9.0">https://github.com/docker/setup-buildx-action/compare/v2.8.0...v2.9.0</a></p>
<h2>v2.8.0</h2>
<ul>
<li>Only set specific flags for drivers supporting them by <a href="https://github.com/nicks"><code>@​nicks</code></a> in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/241">docker/setup-buildx-action#241</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.5.0 to 0.6.0 in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/242">docker/setup-buildx-action#242</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/setup-buildx-action/compare/v2.7.0...v2.8.0">https://github.com/docker/setup-buildx-action/compare/v2.7.0...v2.8.0</a></p>
<h2>v2.7.0</h2>
<ul>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.3.0 to 0.5.0 in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/237">docker/setup-buildx-action#237</a> <a href="https://redirect.github.com/docker/setup-buildx-action/pull/238">docker/setup-buildx-action#238</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/setup-buildx-action/compare/v2.6.0...v2.7.0">https://github.com/docker/setup-buildx-action/compare/v2.6.0...v2.7.0</a></p>
<h2>v2.6.0</h2>
<ul>
<li>Set node name for k8s driver when appending nodes by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/219">docker/setup-buildx-action#219</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.1.0-beta.18 to 0.3.0 in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/220">docker/setup-buildx-action#220</a> <a href="https://redirect.github.com/docker/setup-buildx-action/pull/229">docker/setup-buildx-action#229</a> <a href="https://redirect.github.com/docker/setup-buildx-action/pull/231">docker/setup-buildx-action#231</a> <a href="https://redirect.github.com/docker/setup-buildx-action/pull/236">docker/setup-buildx-action#236</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/setup-buildx-action/compare/v2.5.0...v2.6.0">https://github.com/docker/setup-buildx-action/compare/v2.5.0...v2.6.0</a></p>
<h2>v2.5.0</h2>
<ul>
<li><code>cleanup</code> input to remove builder and temp files by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/213">docker/setup-buildx-action#213</a></li>
<li>do not remove builder using the <code>docker</code> driver by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/218">docker/setup-buildx-action#218</a></li>
<li>fix current context as builder name for <code>docker</code> driver by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/209">docker/setup-buildx-action#209</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/setup-buildx-action/compare/v2.4.1...v2.5.0">https://github.com/docker/setup-buildx-action/compare/v2.4.1...v2.5.0</a></p>
<h2>v2.4.1</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/docker/setup-buildx-action/commit/f95db51fddba0c2d1ec667646a06c2ce06100226"><code>f95db51</code></a> Merge pull request <a href="https://redirect.github.com/docker/setup-buildx-action/issues/267">#267</a> from docker/dependabot/npm_and_yarn/actions/core-1.10.1</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/998a87c2c1933fe580ddf99d6f6f94a19c0f91b4"><code>998a87c</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/28bae5933655f85dce39ef1a90237c1942b8e2c6"><code>28bae59</code></a> build(deps): bump <code>@​actions/core</code> from 1.10.0 to 1.10.1</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/c2153417150d92671c82aea83a1583b776b52910"><code>c215341</code></a> Merge pull request <a href="https://redirect.github.com/docker/setup-buildx-action/issues/264">#264</a> from crazy-max/update-node20</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/02e9319239595dc97a5705a2df905d0b2ea023bf"><code>02e9319</code></a> chore: node 20 as default runtime</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/5c9160effc4a5e931046bcd3a44677eb8eaa7b00"><code>5c9160e</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/1283140f57ede4d0e30355ef4cb25390eaee8204"><code>1283140</code></a> chore: fix author in package.json</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/c6afe06e4a92d0bf5b6f524c3564e64647d0b97d"><code>c6afe06</code></a> vendor: bump <code>@​docker/actions-toolkit</code> from 0.10.0 to 0.12.0</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/f35e0d5a040dd319f1a502de9e27a7f748c79fc5"><code>f35e0d5</code></a> chore: update dev dependencies</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/baeb468fb29686888d706e7200d0e311a4fee4b2"><code>baeb468</code></a> dev: remove unneeded binaries</li>
<li>Additional commits viewable in <a href="https://github.com/docker/setup-buildx-action/compare/v2...v3">compare view</a></li>
</ul>
</details>
<br />

Updates `docker/login-action` from 2 to 3
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/login-action/releases">docker/login-action's releases</a>.</em></p>
<blockquote>
<h2>v3.0.0</h2>
<ul>
<li>Node 20 as default runtime (requires <a href="https://github.com/actions/runner/releases/tag/v2.308.0">Actions Runner v2.308.0</a> or later) by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/login-action/pull/593">docker/login-action#593</a></li>
<li>Bump <code>@​actions/core</code> from 1.10.0...

_Description has been truncated_
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 17:50:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2783" class=".btn">#2783</a>
            </td>
            <td>
                <b>
                    Add Dependabot configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Configure Dependabot to automatically maintain dependencies for GitHub Actions.
  - Check for updates once a week.
  - Group all updates into a single PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 17:00:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2782" class=".btn">#2782</a>
            </td>
            <td>
                <b>
                    Anoncreds revoke and publish-revocations endorsement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Opening for visibility. I'm still going to manually test more but the Integration tests are passing for endorsement and publishing revocations.

One area of confusion for me is what happens with the local wallet verse the ledger. Write now an endorsement transaction is created when the `update_revocation_list` is called with changes. Then the local wallet is updated. At the same time the endorsement manager receives the `114` event and notifies the anoncreds `RevocationListFinished` event handler. It checks if the wallet contains a record for the list via `rev_reg_def_id` and if it doesn't it creates the record. If it does then it assumes the record has been updated already and does nothing. 

I was trying some other stuff like deleting the record and creating a new one with a `wait` state but couldn't decide if this was necessary, or something we wanted to do.

I deleted the `/anoncreds/revoke` and `/anoncreds/publish-revocation` endpoints and instead just have the `/revocation/revoke` and `/revocation/publish-revocation`. I thought this was appropriate because the revocation endpoint are all loaded for anoncreds specifically and the rest of the anoncreds endpoints are to do with creating objects. I changed the params for requesting a transaction manually to use the body options and updated the integration tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-13 21:47:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2775" class=".btn">#2775</a>
            </td>
            <td>
                <b>
                    Implement B006 rule
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add rule `B006` to the linting config and implements it by creating empty objects in the functions when the parameter is None.

Didn't add any of the other `B` linting options.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-12 17:50:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2773" class=".btn">#2773</a>
            </td>
            <td>
                <b>
                    :arrow_up: Upgrade pytest to 8.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Upgrade pytest, now that the latest pytest-asyncio release supports pytest 8
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-12 11:21:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2771" class=".btn">#2771</a>
            </td>
            <td>
                <b>
                    Tweaks to MD files to enable aca-py.org publishing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-11 20:03:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2765" class=".btn">#2765</a>
            </td>
            <td>
                <b>
                    Reorganize the ACA-Py Documentation Files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR does a radical reorganization of the documents in the ACA-Py repository. The following is a summary of the changes:

- Most Markdown files in the root have been moved to the docs folder, and organized into folders that match those used on the [https://aca-py.org](https://aca-py.org) -- demo, gettingStarted, testing, deploying, etc.
- Expected files -- LICENSE, MAINTAINERS.md, README.md and the like were left in the root folder.
- The MD files in the `demo` folder were moved to `docs/demo' and a new README.md file added pointing to those.
- The previous Getting Started files were moved to the `docs/gettingStarted` folders.
- A pass was done to change all the links found (in a manual pass...) to be relative links and to the new location of the files.
- A pass was done to remove all of the MD lint warnings (other than spelling of ACA-Py/Aries/SSI terms).
- Some cleanup was done to external references -- changing references from greenlight ledger to BCovrin test, eliminating some references to old demos, adding references to the Traction Tutorial.
- New README.md files were needed -- such as in the root of the `docs` folder with pointers to guidance for maintaining both the ReadTheDocs documentation and the [https://aca-py.org](https://aca-py.org) documentation.
- I've not done anything with the ELK Stack MD documents -- will think about what to do with those later (if anything).

Not perfect, but I think it is close.

It is a lot of change. Would appreciate people browsing [my branch](https://github.com/swcurran/aries-cloudagent-python/tree/organize-docs) in the GitHub UI to scan for issues, and report them.  Important things to note are changes that need to be made before we merge this and more general updates that are overdue and needed.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-07 22:38:53 +0000 UTC
    </div>
</div>

