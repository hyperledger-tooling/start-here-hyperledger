---
layout: default
title: indy-shared-rs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-shared-rs
---

# indy-shared-rs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-shared-rs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-shared-rs/pull/46" class=".btn">#46</a>
            </td>
            <td>
                <b>
                    Bump the all-actions group with 5 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps the all-actions group with 5 updates:

| Package | From | To |
| --- | --- | --- |
| [actions/checkout](https://github.com/actions/checkout) | `3` | `4` |
| [actions/upload-artifact](https://github.com/actions/upload-artifact) | `3` | `4` |
| [a7ul/tar-action](https://github.com/a7ul/tar-action) | `1.1.2` | `1.1.3` |
| [actions/setup-python](https://github.com/actions/setup-python) | `4` | `5` |
| [actions/download-artifact](https://github.com/actions/download-artifact) | `3` | `4` |

Updates `actions/checkout` from 3 to 4
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
<li>See full diff in <a href="https://github.com/actions/checkout/compare/v3...v4">compare view</a></li>
</ul>
</details>
<br />

Updates `actions/upload-artifact` from 3 to 4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/upload-artifact/releases">actions/upload-artifact's releases</a>.</em></p>
<blockquote>
<h2>v4.0.0</h2>
<h2>What's Changed</h2>
<p>The release of upload-artifact@v4 and download-artifact@v4 are major changes to the backend architecture of Artifacts. They have numerous performance and behavioral improvements.</p>
<p>ℹ️ However, this is a major update that includes breaking changes. Artifacts created with versions v3 and below are not compatible with the v4 actions. Uploads and downloads <em>must</em> use the same major actions versions. There are also key differences from previous versions that may require updates to your workflows.</p>
<p>For more information, please see:</p>
<ol>
<li>The <a href="https://github.blog/changelog/2023-12-14-github-actions-artifacts-v4-is-now-generally-available/">changelog</a> post.</li>
<li>The <a href="https://github.com/actions/upload-artifact/blob/main/README.md">README</a>.</li>
<li>The <a href="https://github.com/actions/upload-artifact/blob/main/docs/MIGRATION.md">migration documentation</a>.</li>
<li>As well as the underlying npm package, <a href="https://github.com/actions/toolkit/tree/main/packages/artifact"><code>@​actions/artifact</code></a> documentation.</li>
</ol>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/vmjoseph"><code>@​vmjoseph</code></a> made their first contribution in <a href="https://redirect.github.com/actions/upload-artifact/pull/464">actions/upload-artifact#464</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/upload-artifact/compare/v3...v4.0.0">https://github.com/actions/upload-artifact/compare/v3...v4.0.0</a></p>
<h2>v3.1.3</h2>
<h2>What's Changed</h2>
<ul>
<li>chore(github): remove trailing whitespaces by <a href="https://github.com/ljmf00"><code>@​ljmf00</code></a> in <a href="https://redirect.github.com/actions/upload-artifact/pull/313">actions/upload-artifact#313</a></li>
<li>Bump <code>@​actions/artifact</code> version to v1.1.2 by <a href="https://github.com/bethanyj28"><code>@​bethanyj28</code></a> in <a href="https://redirect.github.com/actions/upload-artifact/pull/436">actions/upload-artifact#436</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/upload-artifact/compare/v3...v3.1.3">https://github.com/actions/upload-artifact/compare/v3...v3.1.3</a></p>
<h2>v3.1.2</h2>
<ul>
<li>Update all <code>@actions/*</code> NPM packages to their latest versions- <a href="https://redirect.github.com/actions/upload-artifact/issues/374">#374</a></li>
<li>Update all dev dependencies to their most recent versions - <a href="https://redirect.github.com/actions/upload-artifact/issues/375">#375</a></li>
</ul>
<h2>v3.1.1</h2>
<ul>
<li>Update actions/core package to latest version to remove <code>set-output</code> deprecation warning <a href="https://redirect.github.com/actions/upload-artifact/issues/351">#351</a></li>
</ul>
<h2>v3.1.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Bump <code>@​actions/artifact</code> to v1.1.0 (<a href="https://redirect.github.com/actions/upload-artifact/pull/327">actions/upload-artifact#327</a>)
<ul>
<li>Adds checksum headers on artifact upload (<a href="https://redirect.github.com/actions/toolkit/pull/1095">actions/toolkit#1095</a>) (<a href="https://redirect.github.com/actions/toolkit/pull/1063">actions/toolkit#1063</a>)</li>
</ul>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/upload-artifact/commit/5d5d22a31266ced268874388b861e4b58bb5c2f3"><code>5d5d22a</code></a> Merge pull request <a href="https://redirect.github.com/actions/upload-artifact/issues/515">#515</a> from actions/eggyhead/update-artifact-v2.1.1</li>
<li><a href="https://github.com/actions/upload-artifact/commit/f1e993d9663a03508e7fc0370c744c4b963f0044"><code>f1e993d</code></a> update artifact license</li>
<li><a href="https://github.com/actions/upload-artifact/commit/4881bfd3f27855c63733d8cfff17721cc0ad611f"><code>4881bfd</code></a> updating dist:</li>
<li><a href="https://github.com/actions/upload-artifact/commit/a30777e2653648a0a7bbd3efb5c96ef9131b96cc"><code>a30777e</code></a> <a href="https://github.com/eggyhead"><code>@​eggyhead</code></a></li>
<li><a href="https://github.com/actions/upload-artifact/commit/3a8048248f2f288c271830f8ecf2a1c5d8eb0e9a"><code>3a80482</code></a> Merge pull request <a href="https://redirect.github.com/actions/upload-artifact/issues/511">#511</a> from actions/robherley/migration-docs-typo</li>
<li><a href="https://github.com/actions/upload-artifact/commit/9d63e3f2f81d9dc4e13d83fc330408f8a94b79d1"><code>9d63e3f</code></a> Merge branch 'main' into robherley/migration-docs-typo</li>
<li><a href="https://github.com/actions/upload-artifact/commit/dfa1ab292d2fdd78d056187f11c568c16ab53de9"><code>dfa1ab2</code></a> fix typo with v3 artifact downloads in migration guide</li>
<li><a href="https://github.com/actions/upload-artifact/commit/d00351bf698398c17253d21cf8f90e57a344e14b"><code>d00351b</code></a> Merge pull request <a href="https://redirect.github.com/actions/upload-artifact/issues/509">#509</a> from markmssd/patch-1</li>
<li><a href="https://github.com/actions/upload-artifact/commit/707f5a7b71e0fb01c5df1e16e9679a3292606ef2"><code>707f5a7</code></a> Update limitation of <code>10</code> artifacts upload to <code>500</code></li>
<li><a href="https://github.com/actions/upload-artifact/commit/26f96dfa697d77e81fd5907df203aa23a56210a8"><code>26f96df</code></a> Merge pull request <a href="https://redirect.github.com/actions/upload-artifact/issues/505">#505</a> from actions/robherley/merge-artifacts</li>
<li>Additional commits viewable in <a href="https://github.com/actions/upload-artifact/compare/v3...v4">compare view</a></li>
</ul>
</details>
<br />

Updates `a7ul/tar-action` from 1.1.2 to 1.1.3
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/a7ul/tar-action/releases">a7ul/tar-action's releases</a>.</em></p>
<blockquote>
<h2>v1.1.3</h2>
<h2>What's Changed</h2>
<ul>
<li>Update <code>@​actions/core</code> to fix set-output warning by <a href="https://github.com/redian"><code>@​redian</code></a> in <a href="https://redirect.github.com/a7ul/tar-action/pull/20">a7ul/tar-action#20</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/a7ul/tar-action/compare/v1.1.2...v1.1.3">https://github.com/a7ul/tar-action/compare/v1.1.2...v1.1.3</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/a7ul/tar-action/commit/0349c8af1c0926712da20ad4b0ae96918e83cdd1"><code>0349c8a</code></a> Update <code>@​actions/core</code> to fix set-output warning (<a href="https://redirect.github.com/a7ul/tar-action/issues/20">#20</a>)</li>
<li>See full diff in <a href="https://github.com/a7ul/tar-action/compare/v1.1.2...v1.1.3">compare view</a></li>
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

Updates `actions/download-artifact` from 3 to 4
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/download-artifact/releases">actions/download-artifact's releases</a>.</em></p>
<blockquote>
<h2>v4.0.0</h2>
<h2>What's Changed</h2>
<p>The release of upload-artifact@v4 and download-artifact@v4 are major changes to the backend architecture of Artifacts. They have numerous performance and behavioral improvements.</p>
<p>ℹ️ However, this is a major update that includes breaking changes. Artifacts created with versions v3 and below are not compatible with the v4 actions. Uploads and downloads <em>must</em> use the same major actions versions. There are also key differences from previous versions that may require updates to your workflows.</p>
<p>For more information, please see:</p>
<ol>
<li>The <a href="https://github.blog/changelog/2023-12-14-github-actions-artifacts-v4-is-now-generally-available/">changelog</a> post.</li>
<li>The <a href="https://github.com/actions/download-artifact/blob/main/README.md">README</a>.</li>
<li>The <a href="https://github.com/actions/upload-artifact/blob/main/docs/MIGRATION.md">migration documentation</a>.</li>
<li>As well as the underlying npm package, <a href="https://github.com/actions/toolkit/tree/main/packages/artifact"><code>@​actions/artifact</code></a> documentation.</li>
</ol>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/bflad"><code>@​bflad</code></a> made their first contribution in <a href="https://redirect.github.com/actions/download-artifact/pull/194">actions/download-artifact#194</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/download-artifact/compare/v3...v4.0.0">https://github.com/actions/download-artifact/compare/v3...v4.0.0</a></p>
<h2>v3.0.2</h2>
<ul>
<li>Bump <code>@actions/artifact</code> to v1.1.1 - <a href="https://redirect.github.com/actions/download-artifact/pull/195">actions/download-artifact#195</a></li>
<li>Fixed a bug in Node16 where if an HTTP download finished too quickly (&lt;1ms, e.g. when it's mocked) we attempt to delete a temp file that has not been created yet <a href="hhttps://redirect.github.com/actions/toolkit/pull/1278">actions/toolkit#1278</a></li>
</ul>
<h2>v3.0.1</h2>
<ul>
<li><a href="https://redirect.github.com/actions/download-artifact/pull/178">Bump <code>@​actions/core</code> to 1.10.0</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/download-artifact/commit/eaceaf801fd36c7dee90939fad912460b18a1ffe"><code>eaceaf8</code></a> Merge pull request <a href="https://redirect.github.com/actions/download-artifact/issues/291">#291</a> from actions/eggyhead/update-artifact-v2.1.1</li>
<li><a href="https://github.com/actions/download-artifact/commit/81eafdc926c95ab3a46553696557fe28c599a41a"><code>81eafdc</code></a> update artifact license</li>
<li><a href="https://github.com/actions/download-artifact/commit/9ac5cad9e2799348da3b2da75c8fbfa73ab3011c"><code>9ac5cad</code></a> updating artifact dependency to version 2.1.1</li>
<li><a href="https://github.com/actions/download-artifact/commit/3ad8411bbdac537922aa8fb779989d55b1df4a4e"><code>3ad8411</code></a> Merge pull request <a href="https://redirect.github.com/actions/download-artifact/issues/287">#287</a> from actions/robherley/sync-migration-docs</li>
<li><a href="https://github.com/actions/download-artifact/commit/1de464352cdcac2b5838c0c1bb78bb3424a51953"><code>1de4643</code></a> Sync migration docs with upload-artifact</li>
<li><a href="https://github.com/actions/download-artifact/commit/bb3fa7fd35ab8113a980912eb9f59b846d14e3ff"><code>bb3fa7f</code></a> Merge pull request <a href="https://redirect.github.com/actions/download-artifact/issues/275">#275</a> from actions/robherley/better-log-msgs</li>
<li><a href="https://github.com/actions/download-artifact/commit/a244de5a621ac562efb2450e88968f4ad7c5a877"><code>a244de5</code></a> ncc</li>
<li><a href="https://github.com/actions/download-artifact/commit/355659bff273563439cd7fd7dfd81595a30e1f33"><code>355659b</code></a> clarify log messages when using pattern/merge-multiple params</li>
<li><a href="https://github.com/actions/download-artifact/commit/6b208ae046db98c579e8a3aa621ab581ff575935"><code>6b208ae</code></a> Merge pull request <a href="https://redirect.github.com/actions/download-artifact/issues/274">#274</a> from actions/vmjoseph/timeout-patch</li>
<li><a href="https://github.com/actions/download-artifact/commit/6c5b5806e1d833ffbeb6c412b38ba07d67086dc6"><code>6c5b580</code></a> only adding updated license</li>
<li>Additional commits viewable in <a href="https://github.com/actions/download-artifact/compare/v3...v4">compare view</a></li>
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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 18:06:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-shared-rs/pull/45" class=".btn">#45</a>
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
        Created At 2024-02-14 17:39:42 +0000 UTC
    </div>
</div>

