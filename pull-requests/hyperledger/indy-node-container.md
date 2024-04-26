---
layout: default
title: indy-node-container
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-node-container
---

# indy-node-container <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-node-container){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node-container/pull/134" class=".btn">#134</a>
            </td>
            <td>
                <b>
                    Bump the all-actions group across 1 directory with 10 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps the all-actions group with 10 updates in the / directory:

| Package | From | To |
| --- | --- | --- |
| [actions/checkout](https://github.com/actions/checkout) | `3` | `4` |
| [docker/setup-buildx-action](https://github.com/docker/setup-buildx-action) | `2` | `3` |
| [actions/cache](https://github.com/actions/cache) | `3` | `4` |
| [docker/build-push-action](https://github.com/docker/build-push-action) | `3` | `5` |
| [actions/upload-artifact](https://github.com/actions/upload-artifact) | `3` | `4` |
| [actions/download-artifact](https://github.com/actions/download-artifact) | `3` | `4` |
| [actions/github-script](https://github.com/actions/github-script) | `3` | `7` |
| [docker/login-action](https://github.com/docker/login-action) | `1` | `3` |
| [docker/metadata-action](https://github.com/docker/metadata-action) | `4` | `5` |
| [github/codeql-action](https://github.com/github/codeql-action) | `2` | `3` |


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
<h2>v4.1.2</h2>
<ul>
<li>Fix: Disable sparse checkout whenever <code>sparse-checkout</code> option is not present <a href="https://github.com/dscho"><code>@​dscho</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1598">actions/checkout#1598</a></li>
</ul>
<h2>v4.1.1</h2>
<ul>
<li>Correct link to GitHub Docs by <a href="https://github.com/peterbe"><code>@​peterbe</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1511">actions/checkout#1511</a></li>
<li>Link to release page from what's new section by <a href="https://github.com/cory-miller"><code>@​cory-miller</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1514">actions/checkout#1514</a></li>
</ul>
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
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/checkout/commit/1d96c772d19495a3b5c517cd2bc0cb401ea0529f"><code>1d96c77</code></a> Add SSH user parameter (<a href="https://redirect.github.com/actions/checkout/issues/1685">#1685</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/cd7d8d697e10461458bc61a30d094dc601a8b017"><code>cd7d8d6</code></a> Check git version before attempting to disable <code>sparse-checkout</code> (<a href="https://redirect.github.com/actions/checkout/issues/1656">#1656</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/8410ad0602e1e429cee44a835ae9f77f654a6694"><code>8410ad0</code></a> Update <code>actions/checkout</code> version in <code>update-main-version.yml</code> (<a href="https://redirect.github.com/actions/checkout/issues/1650">#1650</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/9bb56186c3b09b4f86b1c65136769dd318469633"><code>9bb5618</code></a> Prep for release of  v4.1.2  (<a href="https://redirect.github.com/actions/checkout/issues/1649">#1649</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/8eb1f6a495037164bea451156472f35fdd6bafc0"><code>8eb1f6a</code></a> Bump <code>@​babel/traverse</code> from 7.20.5 to 7.24.0 (<a href="https://redirect.github.com/actions/checkout/issues/1642">#1642</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/556e4c3cb0b8b54b734286d5439adadcb0a8cb92"><code>556e4c3</code></a> Bump tough-cookie from 4.0.0 to 4.1.3 (<a href="https://redirect.github.com/actions/checkout/issues/1406">#1406</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/b32f140b0c872d58512e0a66172253c302617b90"><code>b32f140</code></a> Warn on attempts to publish <code>test-ubuntu-git</code> from non-main branch. (<a href="https://redirect.github.com/actions/checkout/issues/1623">#1623</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/2650dbd060003e3b5ae211e4358852f336b682a7"><code>2650dbd</code></a> Give <code>test-ubuntu-git</code> its own <code>README</code> (<a href="https://redirect.github.com/actions/checkout/issues/1620">#1620</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/aadec899646c8e0f34c52d9219c2faac36626b55"><code>aadec89</code></a> Explicitly disable sparse checkout unless asked for (<a href="https://redirect.github.com/actions/checkout/issues/1598">#1598</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/df0bcddf6d6823307c716b56a7ef9c3b25078874"><code>df0bcdd</code></a> Refine workflow for generating <code>test-ubuntu-git</code> (<a href="https://redirect.github.com/actions/checkout/issues/1617">#1617</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/actions/checkout/compare/v3...v4">compare view</a></li>
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
<ul>
<li>Get releases from actions toolkit by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://redirect.github.com/docker/setup-buildx-action/issues/200">#200</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/docker/setup-buildx-action/commit/d70bba72b1f3fd22344832f00baa16ece964efeb"><code>d70bba7</code></a> Merge pull request <a href="https://redirect.github.com/docker/setup-buildx-action/issues/307">#307</a> from crazy-max/bump-toolkit</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/7638634cb70c02d327dde3b558f22b0db32054a3"><code>7638634</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/c68420fe0b4de2444121eec8f08bc2500c8d9216"><code>c68420f</code></a> bump <code>@​docker/actions-toolkit</code> from 0.19.0 to 0.20.0</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/2b51285047da1547ffb1b2203d8be4c0af6b1f20"><code>2b51285</code></a> Merge pull request <a href="https://redirect.github.com/docker/setup-buildx-action/issues/306">#306</a> from docker/dependabot/npm_and_yarn/docker/actions-to...</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/0f00370563710ebfbdf4287b76a0a5d88864e7f9"><code>0f00370</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/11c9683db9ea73b2090280c1cfa7d725bd8a60fa"><code>11c9683</code></a> build(deps): bump <code>@​docker/actions-toolkit</code> from 0.18.0 to 0.19.0</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/56a16b8f2aa74bcbd3ab9ec13027cd3ac8e3f94f"><code>56a16b8</code></a> Merge pull request <a href="https://redirect.github.com/docker/setup-buildx-action/issues/303">#303</a> from crazy-max/fix-inputs</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/c23f46eb919af18b86ac6f0f4646a63a7a452b4d"><code>c23f46e</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/f876da6242168c5bb185ad517fb42f0b59fba456"><code>f876da6</code></a> rename and align config inputs</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/b7cf918227e7a90a94eea8534a6b0cc1965a0ccd"><code>b7cf918</code></a> Merge pull request <a href="https://redirect.github.com/docker/setup-buildx-action/issues/304">#304</a> from crazy-max/rm-docs-dir</li>
<li>Additional commits viewable in <a href="https://github.com/docker/setup-buildx-action/compare/v2...v3">compare view</a></li>
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
<li><a href="https://github.com/docker/build-push-action/commit/2cdde995de11925a030ce8070c3d77a52ffcf1c0"><code>2cdde99</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1080">#1080</a> from docker/dependabot/npm_and_yarn/docker/actions-t...</li>
<li><a href="https://github.com/docker/build-push-action/commit/008747aa03417139ec2995efe44e7f080b8323c3"><code>008747a</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/build-push-action/commit/15807531260fa0e39af66835230d13071751862e"><code>1580753</code></a> chore(deps): Bump <code>@​docker/actions-toolkit</code> from 0.18.0 to 0.19.0</li>
<li><a href="https://github.com/docker/build-push-action/commit/2a7db1d68aab1a514ba647f39bcde60888a1753f"><code>2a7db1d</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1075">#1075</a> from crazy-max/ci-multi-output</li>
<li><a href="https://github.com/docker/build-push-action/commit/35e7dd592106dcd929ef8706706f6d54678d1f67"><code>35e7dd5</code></a> ci: test multi output</li>
<li><a href="https://github.com/docker/build-push-action/commit/af5a7ed5ba88268d5278f7203fb52cd833f66d6e"><code>af5a7ed</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1074">#1074</a> from crazy-max/build-cmd-debug</li>
<li><a href="https://github.com/docker/build-push-action/commit/2a85189a6c719593171342d3d43d4034e8c81513"><code>2a85189</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/build-push-action/commit/6c2079483ed8cd675d71b5a395b81fa9a19eddc8"><code>6c20794</code></a> disable quotes detection for &quot;outputs&quot; input</li>
<li><a href="https://github.com/docker/build-push-action/commit/afdf0c0a6772ea0bc8c6af61d5dc2df8823c85de"><code>afdf0c0</code></a> chore: debug build cmd and args</li>
<li><a href="https://github.com/docker/build-push-action/commit/00ae31ab6ef216583e63647d8865f52da6b99a13"><code>00ae31a</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1070">#1070</a> from docker/dependabot/npm_and_yarn/docker/actions-t...</li>
<li>Additional commits viewable in <a href="https://github.com/docker/build-push-action/compare/v3...v5">compare view</a></li>
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
<li><a href="https://github.com/actions/upload-artifact/commit/65462800fd760344b1a7b4382951275a0abb4808"><code>6546280</code></a> updating package version</li>
<li><a href="https://github.com/actions/upload-artifact/commit/c004fb4bf6b1e87680ce1b219a3ad0b8e5dfb7ec"><code>c004fb4</code></a> Merge branch 'main' into eggyhead/use-artifact-v2.1.6</li>
<li><a href="https://github.com/actions/upload-artifact/commit/90aba496fcaa311fd7e784d55e568deabe0fa288"><code>90aba49</code></a> updating toolkit artifact dependency to 2.1.6</li>
<li><a href="https://github.com/actions/upload-artifact/commit/b06cde36fc32a3ee94080e87258567f73f921537"><code>b06cde3</code></a> Merge pull request <a href="https://redirect.github.com/actions/upload-artifact/issues/563">#563</a> from actions/eggyhead/release-4.3.2</li>
<li><a href="https://github.com/actions/upload-artifact/commit/1746f4ab65b179e0ea60a494b83293b640dd5bba"><code>1746f4a</code></a> Revert &quot;updating to release 4.3.2&quot;</li>
<li><a href="https://github.com/actions/upload-artifact/commit/31685d04a0d6557fe2be4174c3ea69ee4cbfa6bb"><code>31685d0</code></a> updating to release 4.3.2</li>
<li><a href="https://github.com/actions/upload-artifact/commit/18bf333cd2249fbbbdb605fd9d9ed57efd7adf34"><code>18bf333</code></a> Merge pull request <a href="https://redirect.github.com/actions/upload-artifact/issues/562">#562</a> from actions/eggyhead/update-artifact-v215</li>
<li><a href="https://github.com/actions/upload-artifact/commit/dac413befa086181ab17cf3db942667aede55e0d"><code>dac413b</code></a> update package lock version</li>
<li><a href="https://github.com/actions/upload-artifact/commit/bb3b4a3cdbef901e2e185ca492d513e798fd1b9f"><code>bb3b4a3</code></a> updating package version</li>
<li><a href="https://github.com/actions/upload-artifact/commit/3e3da837d2a1e030e44fe2bb5c4b9f63c25f33e3"><code>3e3da83</code></a> updating artifact and core dependencies</li>
<li>Additional commits viewable in <a href="https://github.com/actions/upload-artifact/compare/v3...v4">compare view</a></li>
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
<li><a href="https://github.com/actions/download-artifact/commit/9c19ed7fe5d278cd354c7dfd5d3b88589c7e2395"><code>9c19ed7</code></a> Merge branch 'main' into eggyhead/use-artifact-v2.1.6</li>
<li><a href="https://github.com/actions/download-artifact/commit/3d3ea8741ef44e86f7392b41e391bde3c36219bd"><code>3d3ea87</code></a> updating license</li>
<li><a href="https://github.com/actions/download-artifact/commit/89af5db8211998d3ca691103a86b0b9362a94286"><code>89af5db</code></a> updating artifact package v2.1.6</li>
<li><a href="https://github.com/actions/download-artifact/commit/b4aefff88e83a2676a730654e1ce3dce61880379"><code>b4aefff</code></a> Merge pull request <a href="https://redirect.github.com/actions/download-artifact/issues/323">#323</a> from actions/eggyhead/update-artifact-v215</li>
<li><a href="https://github.com/actions/download-artifact/commit/8caf195ad4b1dee92908e23f56eeb0696f1dd42d"><code>8caf195</code></a> package lock update</li>
<li><a href="https://github.com/actions/download-artifact/commit/d7a2ec411d177e8ca679ac5969b70be59c322700"><code>d7a2ec4</code></a> updating package version</li>
<li><a href="https://github.com/actions/download-artifact/commit/e56a1d48ef0f0a8ad8d864416ee03b4f1ab51164"><code>e56a1d4</code></a> updating core dependency</li>
<li><a href="https://github.com/actions/download-artifact/commit/1fcda58b3a5574619fcf6509778850ca2e4b8736"><code>1fcda58</code></a> updating core license</li>
<li><a href="https://github.com/actions/download-artifact/commit/325a10d8b7c55aa3c81692cd880369f752a98121"><code>325a10d</code></a> updating actions dependency to v2.1.5</li>
<li><a href="https://github.com/actions/download-artifact/commit/f8aaee4a210a18d68ebae4a0694be12377e38762"><code>f8aaee4</code></a> Merge pull request <a href="https://redirect.github.com/actions/download-artifact/issues/322">#322</a> from actions/robherley/deprecation-notice</li>
<li>Additional commits viewable in <a href="https://github.com/actions/download-artifact/compare/v3...v4">compare view</a></li>
</ul>
</details>
<br />

Updates `actions/github-script` from 3 to 7
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/github-script/releases">actions/github-script's releases</a>.</em></p>
<blockquote>
<h2>v7.0.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Add base-url option by <a href="https://github.com/robandpdx"><code>@​robandpdx</code></a> in <a href="https://redirect.github.com/actions/github-script/pull/429">actions/github-script#429</a></li>
<li>Expose async-function argument type by <a href="https://github.com/viktorlott"><code>@​viktorlott</code></a> in <a href="https://redirect.github.com/actions/github-script/pull/402">actions/github-script#402</a>, see for details <a href="https://github.com/actions/github-script#use-scripts-with-jsdoc-support">https://github.com/actions/github-script#use-scripts-with-jsdoc-support</a></li>
<li>Update dependencies and use Node 20 by <a href="https://github.com/joshmgross"><code>@​joshmgross</code></a> in <a href="https://redirect.github.com/actions/github-script/pull/425">actions/github-script#425</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/navarroaxel"><code>@​navarroaxel</code></a> made their first contribution in <a href="https://redirect.github.com/actions/github-script/pull/285">actions/github-script#285</a></li>
<li><a href="https://github.com/robandpdx"><code>@​robandpdx</code></a> made their first contribution in <a href="https://redirect.github.com/actions/github-script/pull/429">actions/github-script#429</a></li>
<li><a href="https://github.com/viktorlott"><code>@​viktorlott</code></a> made their first contribution in <a href="https://redirect.github.com/actions/github-script/pull/402">actions/github-script#402</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/github-script/compare/v6.4.1...v7.0.0">https://github.com/actions/github-script/compare/v6.4.1...v7.0.0</a></p>
<h2>v6.4.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Add <code>@​octokit/plugin-request-log</code>, to produce debug output for requests by <a href="https://github.com/mjpieters"><code>@​mjpieters</code></a> in <a href="https://redirect.github.com/actions/github-script/pull/358">actions/github-script#358</a></li>
<li>fix input handling by <a href="https://github.com/mjpieters"><code>@​mjpieters</code></a> in <a href="https://redirect.github.com/actions/github-script/pull/357">actions/github-script#357</a></li>
<li>Remove unused dependencies by <a href="https://github.com/mjpieters"><code>@​mjpieters</code></a> in <a href="https://redirect.github.com/actions/github-script/pull/356">actions/github-script#356</a></li>
<li>Default debug to current runner debug state by <a href="https://github.com/mjpieters"><code>@​mjpieters</code></a> in <a href="https://redirect.github.com/actions/github-script/pull/363">actions/github-script#363</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/mjpieters"><code>@​mjpieters</code></a> made their first contribution in <a href="https://redirect.github.com/actions/github-script/pull/358">actions/github-script#358</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/github-script/compare/v6.4.0...v6.4.1">https://github.com/actions/github-script/compare/v6.4.0...v6.4.1</a></p>
<h2>v6.4.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Bump json5 from 2.1.3 to 2.2.3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/actions/github-script/pull/319">actions/github-script#319</a></li>
<li>Bump minimatch from 3.0.4 to 3.1.2 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/actions/github-script/pull/320">actions/github-script#320</a></li>
<li>Add node-fetch by <a href="https://github.com/danmichaelo"><code>@​danmichaelo</code></a> in <a href="https://redirect.github.com/actions/github-script/pull/321">actions/github-script#321</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/jongwooo"><code>@​jongwooo</code></a> made their first contribution in <a href="https://redirect.github.com/actions/github-script/pull/313">actions/github-script#313</a></li>
<li><a href="https://github.com/austinvazquez"><code>@​austinvazquez</code></a> made their first contribution in <a href="https://redirect.github.com/actions/github-script/pull/306">actions/github-script#306</a></li>
<li><a href="https://github.com/danmichaelo"><code>@​danmichaelo</code></a> made their first contribution in <a href="https://redirect.github.com/actions/github-script/pull/321">actions/github-script#321</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/github-script/compare/v6.3.3...v6.4.0">https://github.com/actions/github-script/compare/v6.3.3...v6.4.0</a></p>
<h2>v6.3.3</h2>
<h2>What's Changed</h2>
<ul>
<li>Update <code>@actions/glob</code> to 0.3.0 by <a href="https://github.com/nineinchnick"><code>@​nineinchnick</code></a> in <a href="https://redirect.github.com/actions/github-script/pull/279">actions/github-script#279</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/nineinchnick"><code>@​nineinchnick</code></a> made their first contribution in <a href="https://redirect.github.com/actions/github-script/pull/279">actions/github-script#279</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/github-script/compare/v6.3.2...v6.3.3">https://github.com/actions/github-script/compare/v6.3.2...v6.3.3</a></p>
<h2>v6.3.2</h2>
<h2>What's Changed</h2>
<ul>
<li>Update <code>@​actions/core</code> to 1.10.0 by <a href="https://github.com/rentziass"><code>@​rentziass</code></a> in <a href="https://redirect.github.com/actions/github-script/pull/295">actions/github-script#295</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/github-script/commit/60a0d83039c74a4aee543508d2ffcb1c3799cdea"><code>60a0d83</code></a> Merge pull request <a href="https://redirect.github.com/actions/github-script/issues/440">#440</a> from actions/joshmgross/v7.0.1</li>
<li><a href="https://github.com/actions/github-script/commit/b7fb2001b410c9390cbe9e2c7d5cab7eefb7b29c"><code>b7fb200</code></a> Update version to 7.0.1</li>
<li><a href="https://github.com/actions/github-script/commit/12e22ed06b6cf302663f90a925045516e24c8bad"><code>12e22ed</code></a> Merge pull request <a href="https://redirect.github.com/actions/github-script/issues/439">#439</a> from actions/joshmgross/avoid-setting-base-url</li>
<li><a href="https://github.com/actions/github-script/commit/d319f8f5b55ea40916b869b2ca9ae2f059c60abf"><code>d319f8f</code></a> Avoid setting <code>baseUrl</code> to undefined when input is not provided</li>
<li><a href="https://github.com/actions/github-script/commit/e69ef5462fd455e02edcaf4dd7708eda96b9eda0"><code>e69ef54</code></a> Merge pull request <a href="https://redirect.github.com/actions/github-script/issues/425">#425</a> from actions/joshmgross/node-20</li>
<li><a href="https://github.com/actions/github-script/commit/ee0914b839b704083a749f8c77a73a9270674a32"><code>ee0914b</code></a> Update licenses</li>
<li><a href="https://github.com/actions/github-script/commit/d6fc56f33b017d55917d045da1a94efa2120f039"><code>d6fc56f</code></a> Use <code>@types/node</code> for Node 20</li>
<li><a href="https://github.com/actions/github-script/commit/384d6cf581452587d1e31f553c97ab165427124a"><code>384d6cf</code></a> Fix quotations in tests</li>
<li><a href="https://github.com/actions/github-script/commit/84724927e3e992f17768c17f57a47a85ea2a5160"><code>8472492</code></a> Only validate GraphQL <code>previews</code></li>
<li><a href="https://github.com/actions/github-script/commit/84903f51828821af5d03d3884c6ba699a2d44d6e"><code>84903f5</code></a> Remove <code>node-fetch</code> from type</li>
<li>Additional commits viewable in <a href="https://github.com/actions/github-script/compare/v3...v7">compare view</a></li>
</ul>
</details>
<br />

Updates `docker/login-action` from 1 to 3
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
<h2>v2.0.0</h2>
<ul>
<li>Node 16 as default runtime by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://redirect.github.com/docker/login-action/issues/161">#161</a>)
<ul>
<li>This requires a minimum <a href="https://github.com/actions/runner/releases/tag/v2.285.0">Actions Runner</a> version of v2.285.0, which is by default available in GHES 3.4 or later.</li>
</ul>
</li>
<li>chore: update dev dependencies and workflow by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://redirect.github.com/docker/login-action/issues/170">#170</a>)</li>
<li>Bump <code>@​actions/exec</code> from 1.1.0 to 1.1.1 (<a href="https://redirect.github.com/docker/login-action/issues/167">#167</a>)</li>
<li>Bump <code>@​actions/io</code> from 1.1.1 to 1.1.2 (<a href="https://redirect.github.com/docker/login-action/issues/168">#168</a>)</li>
<li>Bump minimist from 1.2.5 to 1.2.6 (<a href="https://redirect.github.com/docker/login-action/issues/176">#176</a>)</li>
<li>Bump https-proxy-agent from 5.0.0 to 5.0.1 (<a href="https://redirect.github.com/docker/login-action/issues/182">#182</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/login-action/compare/v1.14.1...v2.0.0">https://github.com/docker/login-action/compare/v1.14.1...v2.0.0</a></p>
<h2>v1.14.1</h2>
<ul>
<li>Revert to Node 12 as default runtime to fix issue for GHE users (<a href="https://redirect.github.com/docker/login-action/issues/160">#160</a>)</li>
</ul>
<h2>v1.14.0</h2>
<ul>
<li>Update to node 16 (<a href="https://redirect.github.com/docker/login-action/issues/158">#158</a>)</li>
<li>Bump <code>@​aws-sdk/client-ecr</code> from 3.45.0 to 3.53.0 (<a href="https://redirect.github.com/docker/login-action/issues/157">#157</a>)</li>
<li>Bump <code>@​aws-sdk/client-ecr-public</code> from 3.45.0 to 3.53.0 (<a href="https://redirect.githu...

_Description has been truncated_
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-23 13:27:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node-container/pull/133" class=".btn">#133</a>
            </td>
            <td>
                <b>
                    ubuntu 20 container with latest indy node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1.13.2 without rc for ubuntu 20
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-23 13:21:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node-container/pull/131" class=".btn">#131</a>
            </td>
            <td>
                <b>
                    fixing controller image build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                build controller image using apt indy 1.12.6  package instead of pip package
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-23 12:23:29 +0000 UTC
    </div>
</div>

