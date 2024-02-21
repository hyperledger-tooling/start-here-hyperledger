---
layout: default
title: aries-socketdock
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-socketdock
---

# aries-socketdock <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-socketdock){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-socketdock/pull/17" class=".btn">#17</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump the all-actions group with 6 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps the all-actions group with 6 updates:

| Package | From | To |
| --- | --- | --- |
| [actions/checkout](https://github.com/actions/checkout) | `3` | `4` |
| [actions/cache](https://github.com/actions/cache) | `3` | `4` |
| [docker/setup-buildx-action](https://github.com/docker/setup-buildx-action) | `2` | `3` |
| [docker/login-action](https://github.com/docker/login-action) | `2` | `3` |
| [docker/metadata-action](https://github.com/docker/metadata-action) | `4` | `5` |
| [docker/build-push-action](https://github.com/docker/build-push-action) | `3` | `5` |

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
<li>Bump <code>@​actions/core</code> from 1.10.0 to 1.10.1 in <a href="https://redirect.github.com/docker/login-action/pull/598">docker/login-action#598</a></li>
<li>Bump <code>@​aws-sdk/client-ecr</code> and <code>@​aws-sdk/client-ecr-public</code> to 3.410.0 in <a href="https://redirect.github.com/docker/login-action/pull/555">docker/login-action#555</a> <a href="https://redirect.github.com/docker/login-action/pull/560">docker/login-action#560</a> <a href="https://redirect.github.com/docker/login-action/pull/582">docker/login-action#582</a> <a href="https://redirect.github.com/docker/login-action/pull/599">docker/login-action#599</a></li>
<li>Bump semver from 6.3.0 to 6.3.1 in <a href="https://redirect.github.com/docker/login-action/pull/556">docker/login-action#556</a></li>
<li>Bump https-proxy-agent to 7.0.2 <a href="https://redirect.github.com/docker/login-action/pull/561">docker/login-action#561</a> <a href="https://redirect.github.com/docker/login-action/pull/588">docker/login-action#588</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/login-action/compare/v2.2.0...v3.0.0">https://github.com/docker/login-action/compare/v2.2.0...v3.0.0</a></p>
<h2>v2.2.0</h2>
<ul>
<li>Switch to actions-toolkit implementation by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/login-action/pull/409">docker/login-action#409</a> <a href="https://redirect.github.com/docker/login-action/pull/470">docker/login-action#470</a> <a href="https://redirect.github.com/docker/login-action/pull/476">docker/login-action#476</a></li>
<li>Bump <code>@​aws-sdk/client-ecr</code> and <code>@​aws-sdk/client-ecr-public</code> to 3.347.1 in <a href="https://redirect.github.com/docker/login-action/pull/524">docker/login-action#524</a> <a href="https://redirect.github.com/docker/login-action/pull/364">docker/login-action#364</a> <a href="https://redirect.github.com/docker/login-action/pull/363">docker/login-action#363</a></li>
<li>Bump minimatch from 3.0.4 to 3.1.2 in <a href="https://redirect.github.com/docker/login-action/pull/354">docker/login-action#354</a></li>
<li>Bump json5 from 2.2.0 to 2.2.3 in <a href="https://redirect.github.com/docker/login-action/pull/378">docker/login-action#378</a></li>
<li>Bump http-proxy-agent from 5.0.0 to 7.0.0 in <a href="https://redirect.github.com/docker/login-action/pull/509">docker/login-action#509</a></li>
<li>Bump https-proxy-agent from 5.0.1 to 7.0.0 in <a href="https://redirect.github.com/docker/login-action/pull/508">docker/login-action#508</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/login-action/compare/v2.1.0...v2.2.0">https://github.com/docker/login-action/compare/v2.1.0...v2.2.0</a></p>
<h2>v2.1.0</h2>
<ul>
<li>Ensure AWS temp credentials are redacted in workflow logs by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://redirect.github.com/docker/login-action/issues/275">#275</a>)</li>
<li>Bump <code>@​actions/core</code> from 1.6.0 to 1.10.0 (<a href="https://redirect.github.com/docker/login-action/issues/252">#252</a> <a href="https://redirect.github.com/docker/login-action/issues/292">#292</a>)</li>
<li>Bump <code>@​aws-sdk/client-ecr</code> from 3.53.0 to 3.186.0 (<a href="https://redirect.github.com/docker/login-action/issues/298">#298</a>)</li>
<li>Bump <code>@​aws-sdk/client-ecr-public</code> from 3.53.0 to 3.186.0 (<a href="https://redirect.github.com/docker/login-action/issues/299">#299</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/login-action/compare/v2.0.0...v2.1.0">https://github.com/docker/login-action/compare/v2.0.0...v2.1.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/docker/login-action/commit/343f7c4344506bcbf9b4de18042ae17996df046d"><code>343f7c4</code></a> Merge pull request <a href="https://redirect.github.com/docker/login-action/issues/599">#599</a> from docker/dependabot/npm_and_yarn/aws-sdk-dependenc...</li>
<li><a href="https://github.com/docker/login-action/commit/aad0f974f21dc644b324e9fa84c4e364f62acbe6"><code>aad0f97</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/login-action/commit/2e0cd391447ec1a654ce199502a5d596fad131a2"><code>2e0cd39</code></a> build(deps): bump the aws-sdk-dependencies group with 2 updates</li>
<li><a href="https://github.com/docker/login-action/commit/203bc9c4eff55a7fac1552bc4811dc0ea4814f2e"><code>203bc9c</code></a> Merge pull request <a href="https://redirect.github.com/docker/login-action/issues/588">#588</a> from docker/dependabot/npm_and_yarn/proxy-agent-depen...</li>
<li><a href="https://github.com/docker/login-action/commit/2199648fc889a2592472959743a8e7d4423bcb29"><code>2199648</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/login-action/commit/b489376173c4ff2c6e783dcb597ba8eff69245fe"><code>b489376</code></a> build(deps): bump the proxy-agent-dependencies group with 1 update</li>
<li><a href="https://github.com/docker/login-action/commit/7c309e74e68d0a0055fd02607b10b3d96510544c"><code>7c309e7</code></a> Merge pull request <a href="https://redirect.github.com/docker/login-action/issues/598">#598</a> from docker/dependabot/npm_and_yarn/actions/core-1.10.1</li>
<li><a href="https://github.com/docker/login-action/commit/0ccf222961de35820c1704a0293ca7483b07d065"><code>0ccf222</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/login-action/commit/56d703e106032867ad04c1e54d781c209f451e26"><code>56d703e</code></a> Merge pull request <a href="https://redirect.github.com/docker/login-action/issues/597">#597</a> from docker/dependabot/github_actions/aws-actions/con...</li>
<li><a href="https://github.com/docker/login-action/commit/24d3b3519e6e369d4d0a307a02881c2f81318560"><code>24d3b35</code></a> build(deps): bump <code>@​actions/core</code> from 1.10.0 to 1.10.1</li>
<li>Additional commits viewable in <a href="https://github.com/docker/login-action/compare/v2...v3">compare view</a></li>
</ul>
</details>
<br />

Updates `docker/metadata-action` from 4 to 5
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/metadata-action/releases">docker/metadata-action's releases</a>.</em></p>
<blockquote>
<h2>v5.0.0</h2>
<ul>
<li>Node 20 as default runtime (requires <a href="https://github.com/actions/runner/releases/tag/v2.308.0">Actions Runner v2.308.0</a> or later) by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/metadata-action/pull/328">docker/metadata-action#328</a></li>
<li>Bump <code>@​actions/core</code> from 1.10.0 to 1.10.1 in <a href="https://redirect.github.com/docker/metadata-action/pull/333">docker/metadata-action#333</a></li>
<li>Bump csv-parse from 5.4.0 to 5.5.0 in <a href="https://redirect.github.com/docker/metadata-action/pull/320">docker/metadata-action#320</a></li>
<li>Bump semver from 7.5.1 to 7.5.2 in <a href="https://redirect.github.com/docker/metadata-action/pull/304">docker/metadata-action#304</a></li>
<li>Bump handlebars from 4.7.7 to 4.7.8 in <a href="https://redirect.github.com/docker/metadata-action/pull/315">docker/metadata-action#315</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/metadata-action/compare/v4.6.0...v5.0.0">https://github.com/docker/metadata-action/compare/v4.6.0...v5.0.0</a></p>
<h2>v4.6.0</h2>
<ul>
<li>Dedup and sort labels by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/metadata-action/pull/301">docker/metadata-action#301</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.3.0 to 0.5.0 in <a href="https://redirect.github.com/docker/metadata-action/pull/302">docker/metadata-action#302</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/metadata-action/compare/v4.5.0...v4.6.0">https://github.com/docker/metadata-action/compare/v4.5.0...v4.6.0</a></p>
<h2>v4.5.0</h2>
<ul>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.1.0 to 0.3.0 in <a href="https://redirect.github.com/docker/metadata-action/pull/296">docker/metadata-action#296</a></li>
<li>Bump csv-parse from 5.3.8 to 5.4.0 in <a href="https://redirect.github.com/docker/metadata-action/pull/294">docker/metadata-action#294</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/metadata-action/compare/v4.4.0...v4.5.0">https://github.com/docker/metadata-action/compare/v4.4.0...v4.5.0</a></p>
<h2>v4.4.0</h2>
<ul>
<li>Add <code>context</code> input to define the metadata provider by <a href="https://github.com/neilime"><code>@​neilime</code></a> in <a href="https://redirect.github.com/docker/metadata-action/pull/248">docker/metadata-action#248</a></li>
<li>Switch to actions-toolkit implementation by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/metadata-action/pull/266">docker/metadata-action#266</a> <a href="https://redirect.github.com/docker/metadata-action/pull/273">docker/metadata-action#273</a> <a href="https://redirect.github.com/docker/metadata-action/pull/284">docker/metadata-action#284</a></li>
<li>Bump csv-parse from 5.3.3 to 5.3.8 in <a href="https://redirect.github.com/docker/metadata-action/pull/271">docker/metadata-action#271</a> <a href="https://redirect.github.com/docker/metadata-action/pull/286">docker/metadata-action#286</a></li>
<li>Bump moment-timezone from 0.5.40 to 0.5.43 in <a href="https://redirect.github.com/docker/metadata-action/pull/268">docker/metadata-action#268</a> <a href="https://redirect.github.com/docker/metadata-action/pull/278">docker/metadata-action#278</a> <a href="https://redirect.github.com/docker/metadata-action/pull/281">docker/metadata-action#281</a></li>
<li>Bump semver from 7.4.0 to 7.5.0 in <a href="https://redirect.github.com/docker/metadata-action/pull/285">docker/metadata-action#285</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/metadata-action/compare/v4.3.0...v4.4.0">https://github.com/docker/metadata-action/compare/v4.3.0...v4.4.0</a></p>
<h2>v4.3.0</h2>
<ul>
<li>Provide outputs as env vars by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://redirect.github.com/docker/metadata-action/issues/257">#257</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/metadata-action/compare/v4.2.0...v4.3.0">https://github.com/docker/metadata-action/compare/v4.2.0...v4.3.0</a></p>
<h2>v4.2.0</h2>
<ul>
<li>Add <code>tz</code> attribute to handlebar date function by <a href="https://github.com/chroju"><code>@​chroju</code></a> (<a href="https://redirect.github.com/docker/metadata-action/issues/251">#251</a>)</li>
<li>Bump minimatch from 3.0.4 to 3.1.2 (<a href="https://redirect.github.com/docker/metadata-action/issues/242">#242</a>)</li>
<li>Bump csv-parse from 5.3.1 to 5.3.3 (<a href="https://redirect.github.com/docker/metadata-action/issues/245">#245</a>)</li>
<li>Bump json5 from 2.2.0 to 2.2.3 (<a href="https://redirect.github.com/docker/metadata-action/issues/252">#252</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/metadata-action/compare/v4.1.1...v4.2.0">https://github.com/docker/metadata-action/compare/v4.1.1...v4.2.0</a></p>
<h2>v4.1.1</h2>
<ul>
<li>Revert changes to set associated head sha on pull request event by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://redirect.github.com/docker/metadata-action/issues/239">#239</a>)
<ul>
<li>User can still set associated head sha on PR by setting the env var <code>DOCKER_METADATA_PR_HEAD_SHA=true</code></li>
</ul>
</li>
<li>Bump csv-parse from 5.3.0 to 5.3.1 (<a href="https://redirect.github.com/docker/metadata-action/issues/237">#237</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/metadata-action/compare/v4.1.0...v4.1.1">https://github.com/docker/metadata-action/compare/v4.1.0...v4.1.1</a></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Upgrade guide</summary>
<p><em>Sourced from <a href="https://github.com/docker/metadata-action/blob/master/UPGRADE.md">docker/metadata-action's upgrade guide</a>.</em></p>
<blockquote>
<h1>Upgrade notes</h1>
<h2>v2 to v3</h2>
<ul>
<li>Repository has been moved to docker org. Replace <code>crazy-max/ghaction-docker-meta@v2</code>
with <code>docker/metadata-action@v5</code></li>
<li>The default bake target has been changed: <code>ghaction-docker-meta</code> &gt; <code>docker-metadata-action</code></li>
</ul>
<h2>v1 to v2</h2>
<ul>
<li><a href="https://github.com/docker/metadata-action/blob/master/#inputs">inputs</a>
<ul>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-sha"><code>tag-sha</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-edge--tag-edge-branch"><code>tag-edge</code> / <code>tag-edge-branch</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-semver"><code>tag-semver</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-match--tag-match-group"><code>tag-match</code> / <code>tag-match-group</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-latest"><code>tag-latest</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-schedule"><code>tag-schedule</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-custom--tag-custom-only"><code>tag-custom</code> / <code>tag-custom-only</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#label-custom"><code>label-custom</code></a></li>
</ul>
</li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#basic-workflow">Basic workflow</a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#semver-workflow">Semver workflow</a></li>
</ul>
<h3>inputs</h3>
<table>
<thead>
<tr>
<th>New</th>
<th>Unchanged</th>
<th>Removed</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>tags</code></td>
<td><code>images</code></td>
<td><code>tag-sha</code></td>
</tr>
<tr>
<td><code>flavor</code></td>
<td><code>sep-tags</code></td>
<td><code>tag-edge</code></td>
</tr>
<tr>
<td><code>labels</code></td>
<td><code>sep-labels</code></td>
<td><code>tag-edge-branch</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-semver</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-match</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-match-group</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-latest</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-schedule</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-custom</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-custom-only</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>label-custom</code></td>
</tr>
</tbody>
</table>
<h4><code>tag-sha</code></h4>
<pre lang="yaml"><code>tags: |
  type=sha
</code></pre>
<h4><code>tag-edge</code> / <code>tag-edge-branch</code></h4>
<pre lang="yaml"><code>tags: |
  # default branch
&lt;/tr&gt;&lt;/table&gt; 
</code></pre>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/docker/metadata-action/commit/8e5442c4ef9f78752691e2d8f8d19755c6f78e81"><code>8e5442c</code></a> Merge pull request <a href="https://redirect.github.com/docker/metadata-action/issues/382">#382</a> from crazy-max/dont-set-cwd-prefix</li>
<li><a href="https://github.com/docker/metadata-action/commit/eda41b71bf54521bf493851a7dab9da9624655ac"><code>eda41b7</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/metadata-action/commit/388c08f740dca49f310f648ea63c30046d49a255"><code>388c08f</code></a> don't set cwd:// prefix for local bake files</li>
<li><a href="https://github.com/docker/metadata-action/commit/dbef88086f6cef02e264edb7dbf63250c17cef6c"><code>dbef880</code></a> Merge pull request <a href="https://redirect.github.com/docker/metadata-action/issues/374">#374</a> from docker/dependabot/npm_and_yarn/moment-timezone-0...</li>
<li><a href="https://github.com/docker/metadata-action/commit/b73e7a71ace0f6ec603f2c5052d8304f33e5dbff"><code>b73e7a7</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/metadata-action/commit/b9fba690eb63fbb6eee7f71bd710b75d4f0128c8"><code>b9fba69</code></a> chore(deps): Bump moment-timezone from 0.5.43 to 0.5.44</li>
<li><a href="https://github.com/docker/metadata-action/commit/ac82374ba6046fefd36df45f67cec12fa6ebeb75"><code>ac82374</code></a> Merge pull request <a href="https://redirect.github.com/docker/metadata-action/issues/373">#373</a> from docker/dependabot/npm_and_yarn/moment-2.30.1</li>
<li><a href="https://github.com/docker/metadata-action/commit/c92519a44ee7b643d904a587e47563f49f24b387"><code>c92519a</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/metadata-action/commit/3b4179d34de6b2ba21a306f387c50672dbbe8612"><code>3b4179d</code></a> chore(deps): Bump moment from 2.29.4 to 2.30.1</li>
<li><a href="https://github.com/docker/metadata-action/commit/0784993ef80dda711a73b98a352e2b73c7feaf32"><code>0784993</code></a> Merge pull request <a href="https://redirect.github.com/docker/metadata-action/issues/371">#371</a> from docker/dependabot/npm_and_yarn/docker/actions-to...</li>
<li>Additional commits viewable in <a href="https://github.com/docker/metadata-action/compare/v4...v5">compare view</a></li>
</ul>
</details>
<br />

Updates `docker/build-push-action` from 3 to 5
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/build-push-action/releases">docker/build-push-action's releases</a>.</em></p>
<blockquote>
<h2>v5.0.0</h2>
<ul>
<li>Node 20 as default runtime (requires <a href="https://github.com/actions/runner/releases/tag/v2.308.0">Actions Runner v2.308.0</a> or later) by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/954">docker/build-push-action#954</a></li>
<li>Bump <code>@​actions/core</code> from 1.10.0 to 1.10.1 in <a href="https://redirect.github.com/docker/build-push-action/pull/959">docker/build-push-action#959</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v4.2.1...v5.0.0">https://github.com/docker/build-push-action/compare/v4.2.1...v5.0.0</a></p>
<h2>v4.2.1</h2>
<blockquote>
<p><strong>Note</strong></p>
<p>Buildx v0.10 enables support for a minimal <a href="https://slsa.dev/provenance/">SLSA Provenance</a> attestation, which requires support for <a href="https://github.com/opencontainers/image-spec">OCI-compliant</a> multi-platform images. This may introduce issues with registry and runtime support (e.g. <a href="https://redirect.github.com/docker/buildx/issues/1533">Google Cloud Run and AWS Lambda</a>). You can optionally disable the default provenance attestation functionality using <code>provenance: false</code>.</p>
</blockquote>
<ul>
<li>warn if docker config can't be parsed by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/957">docker/build-push-action#957</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v4.2.0...v4.2.1">https://github.com/docker/build-push-action/compare/v4.2.0...v4.2.1</a></p>
<h2>v4.2.0</h2>
<blockquote>
<p><strong>Note</strong></p>
<p>Buildx v0.10 enables support for a minimal <a href="https://slsa.dev/provenance/">SLSA Provenance</a> attestation, which requires support for <a href="https://github.com/opencontainers/image-spec">OCI-compliant</a> multi-platform images. This may introduce issues with registry and runtime support (e.g. <a href="https://redirect.github.com/docker/buildx/issues/1533">Google Cloud Run and AWS Lambda</a>). You can optionally disable the default provenance attestation functionality using <code>provenance: false</code>.</p>
</blockquote>
<ul>
<li>display proxy configuration  by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/872">docker/build-push-action#872</a></li>
<li>chore(deps): Bump <code>@​docker/actions-toolkit</code> from 0.6.0 to 0.8.0 in <a href="https://redirect.github.com/docker/build-push-action/pull/930">docker/build-push-action#930</a></li>
<li>chore(deps): Bump word-wrap from 1.2.3 to 1.2.5 in <a href="https://redirect.github.com/docker/build-push-action/pull/925">docker/build-push-action#925</a></li>
<li>chore(deps): Bump semver from 6.3.0 to 6.3.1 in <a href="https://redirect.github.com/docker/build-push-action/pull/902">docker/build-push-action#902</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v4.1.1...v4.2.0">https://github.com/docker/build-push-action/compare/v4.1.1...v4.2.0</a></p>
<h2>v4.1.1</h2>
<blockquote>
<p><strong>Note</strong></p>
<p>Buildx v0.10 enables support for a minimal <a href="https://slsa.dev/provenance/">SLSA Provenance</a> attestation, which requires support for <a href="https://github.com/opencontainers/image-spec">OCI-compliant</a> multi-platform images. This may introduce issues with registry and runtime support (e.g. <a href="https://redirect.github.com/docker/buildx/issues/1533">Google Cloud Run and AWS Lambda</a>). You can optionally disable the default provenance attestation functionality using <code>provenance: false</code>.</p>
</blockquote>
<ul>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.3.0 to 0.5.0 by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/880">docker/build-push-action#880</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v4.1.0...v4.1.1">https://github.com/docker/build-push-action/compare/v4.1.0...v4.1.1</a></p>
<h2>v4.1.0</h2>
<blockquote>
<p><strong>Note</strong></p>
<p>Buildx v0.10 enables support for a minimal <a href="https://slsa.dev/provenance/">SLSA Provenance</a> attestation, which requires support for <a href="https://github.com/opencontainers/image-spec">OCI-compliant</a> multi-platform images. This may introduce issues with registry and runtime support (e.g. <a href="https://redirect.github.com/docker/buildx/issues/1533">Google Cloud Run and AWS Lambda</a>). You can optionally disable the default provenance attestation functionality using <code>provenance: false</code>.</p>
</blockquote>
<ul>
<li>Switch to actions-toolkit implementation by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/811">docker/build-push-action#811</a>  <a href="https://redirect.github.com/docker/build-push-action/pull/838">docker/build-push-action#838</a> <a href="https://redirect.github.com/docker/build-push-action/pull/855">docker/build-push-action#855</a> <a href="https://redirect.github.com/docker/build-push-action/pull/860">docker/build-push-action#860</a> <a href="https://redirect.github.com/docker/build-push-action/pull/875">docker/build-push-action#875</a></li>
<li>e2e: quay.io by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/799">docker/build-push-action#799</a> <a href="https://redirect.github.com/docker/build-push-action/pull/805">docker/build-push-action#805</a></li>
<li>e2e: local harbor and nexus by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/800">docker/build-push-action#800</a></li>
<li>e2e: add artifactory container registry to test against by <a href="https://github.com/jedevc"><code>@​jedevc</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/804">docker/build-push-action#804</a></li>
<li>e2e: add distribution tests by <a href="https://github.com/jedevc"><code>@​jedevc</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/814">docker/build-push-action#814</a> <a href="https://redirect.github.com/docker/build-push-action/pull/815">docker/build-push-action#815</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v4.0.0...v4.1.0">https://github.com/docker/build-push-action/compare/v4.0.0...v4.1.0</a></p>
<h2>v4.0.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/docker/build-push-action/commit/4a13e500e55cf31b7a5d59a38ab2040ab0f42f56"><code>4a13e50</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1006">#1006</a> from docker/dependabot/npm_and_yarn/docker/actions-t...</li>
<li><a href="https://github.com/docker/build-push-action/commit/74166686865cdc289a02f214871fb53447b73447"><code>7416668</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/build-push-action/commit/b4f76a5dc6a67282180eddc6d460f23bc97bfcbc"><code>b4f76a5</code></a> chore(deps): Bump <code>@​docker/actions-toolkit</code> from 0.13.0 to 0.14.0</li>
<li><a href="https://github.com/docker/build-push-action/commit/b7feb766fae338d85274c87a9d0f24c09690dbe2"><code>b7feb76</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1005">#1005</a> from crazy-max/ci-inspect</li>
<li><a href="https://github.com/docker/build-push-action/commit/fae8018297c67066fff64a6e9c319c86f89b8982"><code>fae8018</code></a> ci: inspect sbom and provenance</li>
<li><a href="https://github.com/docker/build-push-action/commit/b625868b13c3feb675cabbf9bfeb52ae94166606"><code>b625868</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1004">#1004</a> from crazy-max/ci-update-buildx</li>
<li><a href="https://github.com/docker/build-push-action/commit/5193ef1da6ea0d66de97d22817c258b203ade96a"><code>5193ef1</code></a> ci: update buildx to latest</li>
<li><a href="https://github.com/docker/build-push-action/commit/d3afd779e409ac26db5374fb27fe4aae9f6adb42"><code>d3afd77</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/991">#991</a> from docker/dependabot/npm_and_yarn/babel/traverse-7....</li>
<li><a href="https://github.com/docker/build-push-action/commit/7a786bb2b9408f7f997564f677248fabd4b886d5"><code>7a786bb</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/992">#992</a> from crazy-max/annotations</li>
<li><a href="https://github.com/docker/build-push-action/commit/c66ae3adcfbf698ecd851c6bb782654a0c6ffcae"><code>c66ae3a</code></a> chore: update generated content</li>
<li>Additional commits viewable in <a href="https://github.com/docker/build-push-action/compare/v3...v5">compare view</a></li>
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
        Created At 2024-02-14 18:18:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-socketdock/pull/16" class=".btn">#16</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump the all-actions group with 6 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps the all-actions group with 6 updates:

| Package | From | To |
| --- | --- | --- |
| [actions/checkout](https://github.com/actions/checkout) | `3` | `4` |
| [actions/cache](https://github.com/actions/cache) | `3` | `4` |
| [docker/setup-buildx-action](https://github.com/docker/setup-buildx-action) | `2` | `3` |
| [docker/login-action](https://github.com/docker/login-action) | `2` | `3` |
| [docker/metadata-action](https://github.com/docker/metadata-action) | `4` | `5` |
| [docker/build-push-action](https://github.com/docker/build-push-action) | `3` | `5` |

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
<li>Bump <code>@​actions/core</code> from 1.10.0 to 1.10.1 in <a href="https://redirect.github.com/docker/login-action/pull/598">docker/login-action#598</a></li>
<li>Bump <code>@​aws-sdk/client-ecr</code> and <code>@​aws-sdk/client-ecr-public</code> to 3.410.0 in <a href="https://redirect.github.com/docker/login-action/pull/555">docker/login-action#555</a> <a href="https://redirect.github.com/docker/login-action/pull/560">docker/login-action#560</a> <a href="https://redirect.github.com/docker/login-action/pull/582">docker/login-action#582</a> <a href="https://redirect.github.com/docker/login-action/pull/599">docker/login-action#599</a></li>
<li>Bump semver from 6.3.0 to 6.3.1 in <a href="https://redirect.github.com/docker/login-action/pull/556">docker/login-action#556</a></li>
<li>Bump https-proxy-agent to 7.0.2 <a href="https://redirect.github.com/docker/login-action/pull/561">docker/login-action#561</a> <a href="https://redirect.github.com/docker/login-action/pull/588">docker/login-action#588</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/login-action/compare/v2.2.0...v3.0.0">https://github.com/docker/login-action/compare/v2.2.0...v3.0.0</a></p>
<h2>v2.2.0</h2>
<ul>
<li>Switch to actions-toolkit implementation by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/login-action/pull/409">docker/login-action#409</a> <a href="https://redirect.github.com/docker/login-action/pull/470">docker/login-action#470</a> <a href="https://redirect.github.com/docker/login-action/pull/476">docker/login-action#476</a></li>
<li>Bump <code>@​aws-sdk/client-ecr</code> and <code>@​aws-sdk/client-ecr-public</code> to 3.347.1 in <a href="https://redirect.github.com/docker/login-action/pull/524">docker/login-action#524</a> <a href="https://redirect.github.com/docker/login-action/pull/364">docker/login-action#364</a> <a href="https://redirect.github.com/docker/login-action/pull/363">docker/login-action#363</a></li>
<li>Bump minimatch from 3.0.4 to 3.1.2 in <a href="https://redirect.github.com/docker/login-action/pull/354">docker/login-action#354</a></li>
<li>Bump json5 from 2.2.0 to 2.2.3 in <a href="https://redirect.github.com/docker/login-action/pull/378">docker/login-action#378</a></li>
<li>Bump http-proxy-agent from 5.0.0 to 7.0.0 in <a href="https://redirect.github.com/docker/login-action/pull/509">docker/login-action#509</a></li>
<li>Bump https-proxy-agent from 5.0.1 to 7.0.0 in <a href="https://redirect.github.com/docker/login-action/pull/508">docker/login-action#508</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/login-action/compare/v2.1.0...v2.2.0">https://github.com/docker/login-action/compare/v2.1.0...v2.2.0</a></p>
<h2>v2.1.0</h2>
<ul>
<li>Ensure AWS temp credentials are redacted in workflow logs by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://redirect.github.com/docker/login-action/issues/275">#275</a>)</li>
<li>Bump <code>@​actions/core</code> from 1.6.0 to 1.10.0 (<a href="https://redirect.github.com/docker/login-action/issues/252">#252</a> <a href="https://redirect.github.com/docker/login-action/issues/292">#292</a>)</li>
<li>Bump <code>@​aws-sdk/client-ecr</code> from 3.53.0 to 3.186.0 (<a href="https://redirect.github.com/docker/login-action/issues/298">#298</a>)</li>
<li>Bump <code>@​aws-sdk/client-ecr-public</code> from 3.53.0 to 3.186.0 (<a href="https://redirect.github.com/docker/login-action/issues/299">#299</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/login-action/compare/v2.0.0...v2.1.0">https://github.com/docker/login-action/compare/v2.0.0...v2.1.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/docker/login-action/commit/343f7c4344506bcbf9b4de18042ae17996df046d"><code>343f7c4</code></a> Merge pull request <a href="https://redirect.github.com/docker/login-action/issues/599">#599</a> from docker/dependabot/npm_and_yarn/aws-sdk-dependenc...</li>
<li><a href="https://github.com/docker/login-action/commit/aad0f974f21dc644b324e9fa84c4e364f62acbe6"><code>aad0f97</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/login-action/commit/2e0cd391447ec1a654ce199502a5d596fad131a2"><code>2e0cd39</code></a> build(deps): bump the aws-sdk-dependencies group with 2 updates</li>
<li><a href="https://github.com/docker/login-action/commit/203bc9c4eff55a7fac1552bc4811dc0ea4814f2e"><code>203bc9c</code></a> Merge pull request <a href="https://redirect.github.com/docker/login-action/issues/588">#588</a> from docker/dependabot/npm_and_yarn/proxy-agent-depen...</li>
<li><a href="https://github.com/docker/login-action/commit/2199648fc889a2592472959743a8e7d4423bcb29"><code>2199648</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/login-action/commit/b489376173c4ff2c6e783dcb597ba8eff69245fe"><code>b489376</code></a> build(deps): bump the proxy-agent-dependencies group with 1 update</li>
<li><a href="https://github.com/docker/login-action/commit/7c309e74e68d0a0055fd02607b10b3d96510544c"><code>7c309e7</code></a> Merge pull request <a href="https://redirect.github.com/docker/login-action/issues/598">#598</a> from docker/dependabot/npm_and_yarn/actions/core-1.10.1</li>
<li><a href="https://github.com/docker/login-action/commit/0ccf222961de35820c1704a0293ca7483b07d065"><code>0ccf222</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/login-action/commit/56d703e106032867ad04c1e54d781c209f451e26"><code>56d703e</code></a> Merge pull request <a href="https://redirect.github.com/docker/login-action/issues/597">#597</a> from docker/dependabot/github_actions/aws-actions/con...</li>
<li><a href="https://github.com/docker/login-action/commit/24d3b3519e6e369d4d0a307a02881c2f81318560"><code>24d3b35</code></a> build(deps): bump <code>@​actions/core</code> from 1.10.0 to 1.10.1</li>
<li>Additional commits viewable in <a href="https://github.com/docker/login-action/compare/v2...v3">compare view</a></li>
</ul>
</details>
<br />

Updates `docker/metadata-action` from 4 to 5
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/metadata-action/releases">docker/metadata-action's releases</a>.</em></p>
<blockquote>
<h2>v5.0.0</h2>
<ul>
<li>Node 20 as default runtime (requires <a href="https://github.com/actions/runner/releases/tag/v2.308.0">Actions Runner v2.308.0</a> or later) by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/metadata-action/pull/328">docker/metadata-action#328</a></li>
<li>Bump <code>@​actions/core</code> from 1.10.0 to 1.10.1 in <a href="https://redirect.github.com/docker/metadata-action/pull/333">docker/metadata-action#333</a></li>
<li>Bump csv-parse from 5.4.0 to 5.5.0 in <a href="https://redirect.github.com/docker/metadata-action/pull/320">docker/metadata-action#320</a></li>
<li>Bump semver from 7.5.1 to 7.5.2 in <a href="https://redirect.github.com/docker/metadata-action/pull/304">docker/metadata-action#304</a></li>
<li>Bump handlebars from 4.7.7 to 4.7.8 in <a href="https://redirect.github.com/docker/metadata-action/pull/315">docker/metadata-action#315</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/metadata-action/compare/v4.6.0...v5.0.0">https://github.com/docker/metadata-action/compare/v4.6.0...v5.0.0</a></p>
<h2>v4.6.0</h2>
<ul>
<li>Dedup and sort labels by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/metadata-action/pull/301">docker/metadata-action#301</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.3.0 to 0.5.0 in <a href="https://redirect.github.com/docker/metadata-action/pull/302">docker/metadata-action#302</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/metadata-action/compare/v4.5.0...v4.6.0">https://github.com/docker/metadata-action/compare/v4.5.0...v4.6.0</a></p>
<h2>v4.5.0</h2>
<ul>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.1.0 to 0.3.0 in <a href="https://redirect.github.com/docker/metadata-action/pull/296">docker/metadata-action#296</a></li>
<li>Bump csv-parse from 5.3.8 to 5.4.0 in <a href="https://redirect.github.com/docker/metadata-action/pull/294">docker/metadata-action#294</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/metadata-action/compare/v4.4.0...v4.5.0">https://github.com/docker/metadata-action/compare/v4.4.0...v4.5.0</a></p>
<h2>v4.4.0</h2>
<ul>
<li>Add <code>context</code> input to define the metadata provider by <a href="https://github.com/neilime"><code>@​neilime</code></a> in <a href="https://redirect.github.com/docker/metadata-action/pull/248">docker/metadata-action#248</a></li>
<li>Switch to actions-toolkit implementation by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/metadata-action/pull/266">docker/metadata-action#266</a> <a href="https://redirect.github.com/docker/metadata-action/pull/273">docker/metadata-action#273</a> <a href="https://redirect.github.com/docker/metadata-action/pull/284">docker/metadata-action#284</a></li>
<li>Bump csv-parse from 5.3.3 to 5.3.8 in <a href="https://redirect.github.com/docker/metadata-action/pull/271">docker/metadata-action#271</a> <a href="https://redirect.github.com/docker/metadata-action/pull/286">docker/metadata-action#286</a></li>
<li>Bump moment-timezone from 0.5.40 to 0.5.43 in <a href="https://redirect.github.com/docker/metadata-action/pull/268">docker/metadata-action#268</a> <a href="https://redirect.github.com/docker/metadata-action/pull/278">docker/metadata-action#278</a> <a href="https://redirect.github.com/docker/metadata-action/pull/281">docker/metadata-action#281</a></li>
<li>Bump semver from 7.4.0 to 7.5.0 in <a href="https://redirect.github.com/docker/metadata-action/pull/285">docker/metadata-action#285</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/metadata-action/compare/v4.3.0...v4.4.0">https://github.com/docker/metadata-action/compare/v4.3.0...v4.4.0</a></p>
<h2>v4.3.0</h2>
<ul>
<li>Provide outputs as env vars by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://redirect.github.com/docker/metadata-action/issues/257">#257</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/metadata-action/compare/v4.2.0...v4.3.0">https://github.com/docker/metadata-action/compare/v4.2.0...v4.3.0</a></p>
<h2>v4.2.0</h2>
<ul>
<li>Add <code>tz</code> attribute to handlebar date function by <a href="https://github.com/chroju"><code>@​chroju</code></a> (<a href="https://redirect.github.com/docker/metadata-action/issues/251">#251</a>)</li>
<li>Bump minimatch from 3.0.4 to 3.1.2 (<a href="https://redirect.github.com/docker/metadata-action/issues/242">#242</a>)</li>
<li>Bump csv-parse from 5.3.1 to 5.3.3 (<a href="https://redirect.github.com/docker/metadata-action/issues/245">#245</a>)</li>
<li>Bump json5 from 2.2.0 to 2.2.3 (<a href="https://redirect.github.com/docker/metadata-action/issues/252">#252</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/metadata-action/compare/v4.1.1...v4.2.0">https://github.com/docker/metadata-action/compare/v4.1.1...v4.2.0</a></p>
<h2>v4.1.1</h2>
<ul>
<li>Revert changes to set associated head sha on pull request event by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://redirect.github.com/docker/metadata-action/issues/239">#239</a>)
<ul>
<li>User can still set associated head sha on PR by setting the env var <code>DOCKER_METADATA_PR_HEAD_SHA=true</code></li>
</ul>
</li>
<li>Bump csv-parse from 5.3.0 to 5.3.1 (<a href="https://redirect.github.com/docker/metadata-action/issues/237">#237</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/metadata-action/compare/v4.1.0...v4.1.1">https://github.com/docker/metadata-action/compare/v4.1.0...v4.1.1</a></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Upgrade guide</summary>
<p><em>Sourced from <a href="https://github.com/docker/metadata-action/blob/master/UPGRADE.md">docker/metadata-action's upgrade guide</a>.</em></p>
<blockquote>
<h1>Upgrade notes</h1>
<h2>v2 to v3</h2>
<ul>
<li>Repository has been moved to docker org. Replace <code>crazy-max/ghaction-docker-meta@v2</code>
with <code>docker/metadata-action@v5</code></li>
<li>The default bake target has been changed: <code>ghaction-docker-meta</code> &gt; <code>docker-metadata-action</code></li>
</ul>
<h2>v1 to v2</h2>
<ul>
<li><a href="https://github.com/docker/metadata-action/blob/master/#inputs">inputs</a>
<ul>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-sha"><code>tag-sha</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-edge--tag-edge-branch"><code>tag-edge</code> / <code>tag-edge-branch</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-semver"><code>tag-semver</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-match--tag-match-group"><code>tag-match</code> / <code>tag-match-group</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-latest"><code>tag-latest</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-schedule"><code>tag-schedule</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#tag-custom--tag-custom-only"><code>tag-custom</code> / <code>tag-custom-only</code></a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#label-custom"><code>label-custom</code></a></li>
</ul>
</li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#basic-workflow">Basic workflow</a></li>
<li><a href="https://github.com/docker/metadata-action/blob/master/#semver-workflow">Semver workflow</a></li>
</ul>
<h3>inputs</h3>
<table>
<thead>
<tr>
<th>New</th>
<th>Unchanged</th>
<th>Removed</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>tags</code></td>
<td><code>images</code></td>
<td><code>tag-sha</code></td>
</tr>
<tr>
<td><code>flavor</code></td>
<td><code>sep-tags</code></td>
<td><code>tag-edge</code></td>
</tr>
<tr>
<td><code>labels</code></td>
<td><code>sep-labels</code></td>
<td><code>tag-edge-branch</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-semver</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-match</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-match-group</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-latest</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-schedule</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-custom</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>tag-custom-only</code></td>
</tr>
<tr>
<td></td>
<td></td>
<td><code>label-custom</code></td>
</tr>
</tbody>
</table>
<h4><code>tag-sha</code></h4>
<pre lang="yaml"><code>tags: |
  type=sha
</code></pre>
<h4><code>tag-edge</code> / <code>tag-edge-branch</code></h4>
<pre lang="yaml"><code>tags: |
  # default branch
&lt;/tr&gt;&lt;/table&gt; 
</code></pre>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/docker/metadata-action/commit/8e5442c4ef9f78752691e2d8f8d19755c6f78e81"><code>8e5442c</code></a> Merge pull request <a href="https://redirect.github.com/docker/metadata-action/issues/382">#382</a> from crazy-max/dont-set-cwd-prefix</li>
<li><a href="https://github.com/docker/metadata-action/commit/eda41b71bf54521bf493851a7dab9da9624655ac"><code>eda41b7</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/metadata-action/commit/388c08f740dca49f310f648ea63c30046d49a255"><code>388c08f</code></a> don't set cwd:// prefix for local bake files</li>
<li><a href="https://github.com/docker/metadata-action/commit/dbef88086f6cef02e264edb7dbf63250c17cef6c"><code>dbef880</code></a> Merge pull request <a href="https://redirect.github.com/docker/metadata-action/issues/374">#374</a> from docker/dependabot/npm_and_yarn/moment-timezone-0...</li>
<li><a href="https://github.com/docker/metadata-action/commit/b73e7a71ace0f6ec603f2c5052d8304f33e5dbff"><code>b73e7a7</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/metadata-action/commit/b9fba690eb63fbb6eee7f71bd710b75d4f0128c8"><code>b9fba69</code></a> chore(deps): Bump moment-timezone from 0.5.43 to 0.5.44</li>
<li><a href="https://github.com/docker/metadata-action/commit/ac82374ba6046fefd36df45f67cec12fa6ebeb75"><code>ac82374</code></a> Merge pull request <a href="https://redirect.github.com/docker/metadata-action/issues/373">#373</a> from docker/dependabot/npm_and_yarn/moment-2.30.1</li>
<li><a href="https://github.com/docker/metadata-action/commit/c92519a44ee7b643d904a587e47563f49f24b387"><code>c92519a</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/metadata-action/commit/3b4179d34de6b2ba21a306f387c50672dbbe8612"><code>3b4179d</code></a> chore(deps): Bump moment from 2.29.4 to 2.30.1</li>
<li><a href="https://github.com/docker/metadata-action/commit/0784993ef80dda711a73b98a352e2b73c7feaf32"><code>0784993</code></a> Merge pull request <a href="https://redirect.github.com/docker/metadata-action/issues/371">#371</a> from docker/dependabot/npm_and_yarn/docker/actions-to...</li>
<li>Additional commits viewable in <a href="https://github.com/docker/metadata-action/compare/v4...v5">compare view</a></li>
</ul>
</details>
<br />

Updates `docker/build-push-action` from 3 to 5
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/build-push-action/releases">docker/build-push-action's releases</a>.</em></p>
<blockquote>
<h2>v5.0.0</h2>
<ul>
<li>Node 20 as default runtime (requires <a href="https://github.com/actions/runner/releases/tag/v2.308.0">Actions Runner v2.308.0</a> or later) by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/954">docker/build-push-action#954</a></li>
<li>Bump <code>@​actions/core</code> from 1.10.0 to 1.10.1 in <a href="https://redirect.github.com/docker/build-push-action/pull/959">docker/build-push-action#959</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v4.2.1...v5.0.0">https://github.com/docker/build-push-action/compare/v4.2.1...v5.0.0</a></p>
<h2>v4.2.1</h2>
<blockquote>
<p><strong>Note</strong></p>
<p>Buildx v0.10 enables support for a minimal <a href="https://slsa.dev/provenance/">SLSA Provenance</a> attestation, which requires support for <a href="https://github.com/opencontainers/image-spec">OCI-compliant</a> multi-platform images. This may introduce issues with registry and runtime support (e.g. <a href="https://redirect.github.com/docker/buildx/issues/1533">Google Cloud Run and AWS Lambda</a>). You can optionally disable the default provenance attestation functionality using <code>provenance: false</code>.</p>
</blockquote>
<ul>
<li>warn if docker config can't be parsed by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/957">docker/build-push-action#957</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v4.2.0...v4.2.1">https://github.com/docker/build-push-action/compare/v4.2.0...v4.2.1</a></p>
<h2>v4.2.0</h2>
<blockquote>
<p><strong>Note</strong></p>
<p>Buildx v0.10 enables support for a minimal <a href="https://slsa.dev/provenance/">SLSA Provenance</a> attestation, which requires support for <a href="https://github.com/opencontainers/image-spec">OCI-compliant</a> multi-platform images. This may introduce issues with registry and runtime support (e.g. <a href="https://redirect.github.com/docker/buildx/issues/1533">Google Cloud Run and AWS Lambda</a>). You can optionally disable the default provenance attestation functionality using <code>provenance: false</code>.</p>
</blockquote>
<ul>
<li>display proxy configuration  by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/872">docker/build-push-action#872</a></li>
<li>chore(deps): Bump <code>@​docker/actions-toolkit</code> from 0.6.0 to 0.8.0 in <a href="https://redirect.github.com/docker/build-push-action/pull/930">docker/build-push-action#930</a></li>
<li>chore(deps): Bump word-wrap from 1.2.3 to 1.2.5 in <a href="https://redirect.github.com/docker/build-push-action/pull/925">docker/build-push-action#925</a></li>
<li>chore(deps): Bump semver from 6.3.0 to 6.3.1 in <a href="https://redirect.github.com/docker/build-push-action/pull/902">docker/build-push-action#902</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v4.1.1...v4.2.0">https://github.com/docker/build-push-action/compare/v4.1.1...v4.2.0</a></p>
<h2>v4.1.1</h2>
<blockquote>
<p><strong>Note</strong></p>
<p>Buildx v0.10 enables support for a minimal <a href="https://slsa.dev/provenance/">SLSA Provenance</a> attestation, which requires support for <a href="https://github.com/opencontainers/image-spec">OCI-compliant</a> multi-platform images. This may introduce issues with registry and runtime support (e.g. <a href="https://redirect.github.com/docker/buildx/issues/1533">Google Cloud Run and AWS Lambda</a>). You can optionally disable the default provenance attestation functionality using <code>provenance: false</code>.</p>
</blockquote>
<ul>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.3.0 to 0.5.0 by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/880">docker/build-push-action#880</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v4.1.0...v4.1.1">https://github.com/docker/build-push-action/compare/v4.1.0...v4.1.1</a></p>
<h2>v4.1.0</h2>
<blockquote>
<p><strong>Note</strong></p>
<p>Buildx v0.10 enables support for a minimal <a href="https://slsa.dev/provenance/">SLSA Provenance</a> attestation, which requires support for <a href="https://github.com/opencontainers/image-spec">OCI-compliant</a> multi-platform images. This may introduce issues with registry and runtime support (e.g. <a href="https://redirect.github.com/docker/buildx/issues/1533">Google Cloud Run and AWS Lambda</a>). You can optionally disable the default provenance attestation functionality using <code>provenance: false</code>.</p>
</blockquote>
<ul>
<li>Switch to actions-toolkit implementation by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/811">docker/build-push-action#811</a>  <a href="https://redirect.github.com/docker/build-push-action/pull/838">docker/build-push-action#838</a> <a href="https://redirect.github.com/docker/build-push-action/pull/855">docker/build-push-action#855</a> <a href="https://redirect.github.com/docker/build-push-action/pull/860">docker/build-push-action#860</a> <a href="https://redirect.github.com/docker/build-push-action/pull/875">docker/build-push-action#875</a></li>
<li>e2e: quay.io by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/799">docker/build-push-action#799</a> <a href="https://redirect.github.com/docker/build-push-action/pull/805">docker/build-push-action#805</a></li>
<li>e2e: local harbor and nexus by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/800">docker/build-push-action#800</a></li>
<li>e2e: add artifactory container registry to test against by <a href="https://github.com/jedevc"><code>@​jedevc</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/804">docker/build-push-action#804</a></li>
<li>e2e: add distribution tests by <a href="https://github.com/jedevc"><code>@​jedevc</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/814">docker/build-push-action#814</a> <a href="https://redirect.github.com/docker/build-push-action/pull/815">docker/build-push-action#815</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v4.0.0...v4.1.0">https://github.com/docker/build-push-action/compare/v4.0.0...v4.1.0</a></p>
<h2>v4.0.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/docker/build-push-action/commit/4a13e500e55cf31b7a5d59a38ab2040ab0f42f56"><code>4a13e50</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1006">#1006</a> from docker/dependabot/npm_and_yarn/docker/actions-t...</li>
<li><a href="https://github.com/docker/build-push-action/commit/74166686865cdc289a02f214871fb53447b73447"><code>7416668</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/build-push-action/commit/b4f76a5dc6a67282180eddc6d460f23bc97bfcbc"><code>b4f76a5</code></a> chore(deps): Bump <code>@​docker/actions-toolkit</code> from 0.13.0 to 0.14.0</li>
<li><a href="https://github.com/docker/build-push-action/commit/b7feb766fae338d85274c87a9d0f24c09690dbe2"><code>b7feb76</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1005">#1005</a> from crazy-max/ci-inspect</li>
<li><a href="https://github.com/docker/build-push-action/commit/fae8018297c67066fff64a6e9c319c86f89b8982"><code>fae8018</code></a> ci: inspect sbom and provenance</li>
<li><a href="https://github.com/docker/build-push-action/commit/b625868b13c3feb675cabbf9bfeb52ae94166606"><code>b625868</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1004">#1004</a> from crazy-max/ci-update-buildx</li>
<li><a href="https://github.com/docker/build-push-action/commit/5193ef1da6ea0d66de97d22817c258b203ade96a"><code>5193ef1</code></a> ci: update buildx to latest</li>
<li><a href="https://github.com/docker/build-push-action/commit/d3afd779e409ac26db5374fb27fe4aae9f6adb42"><code>d3afd77</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/991">#991</a> from docker/dependabot/npm_and_yarn/babel/traverse-7....</li>
<li><a href="https://github.com/docker/build-push-action/commit/7a786bb2b9408f7f997564f677248fabd4b886d5"><code>7a786bb</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/992">#992</a> from crazy-max/annotations</li>
<li><a href="https://github.com/docker/build-push-action/commit/c66ae3adcfbf698ecd851c6bb782654a0c6ffcae"><code>c66ae3a</code></a> chore: update generated content</li>
<li>Additional commits viewable in <a href="https://github.com/docker/build-push-action/compare/v3...v5">compare view</a></li>
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
        Created At 2024-02-14 18:17:32 +0000 UTC
    </div>
</div>

