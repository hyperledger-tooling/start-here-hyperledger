---
layout: default
title: aries-acapy-controllers
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-controllers
---

# aries-acapy-controllers <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-controllers){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-controllers/pull/100" class=".btn">#100</a>
            </td>
            <td>
                <b>
                    Bump undici and @angular-devkit/build-angular in /AliceFaberAcmeDemo/controllers/alice-controller
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [undici](https://github.com/nodejs/undici) to 6.6.2 and updates ancestor dependency [@angular-devkit/build-angular](https://github.com/angular/angular-cli). These dependencies need to be updated together.

Updates `undici` from 5.27.2 to 6.6.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nodejs/undici/releases">undici's releases</a>.</em></p>
<blockquote>
<h2>v6.6.2</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: webidl.brandcheck non strict should throw by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2683">nodejs/undici#2683</a></li>
<li>fix: expose EventSource for nodejs by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2645">nodejs/undici#2645</a></li>
<li>test: more information from debug tests by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2695">nodejs/undici#2695</a></li>
<li>Fix broken test on linux by <a href="https://github.com/mcollina"><code>@​mcollina</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2699">nodejs/undici#2699</a></li>
<li>fix: fix the linux patch by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2703">nodejs/undici#2703</a></li>
<li>test(wpt): mark timed out tests as 'failed' by <a href="https://github.com/rossilor95"><code>@​rossilor95</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2644">nodejs/undici#2644</a></li>
<li>build(deps-dev): bump borp from 0.5.0 to 0.9.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2702">nodejs/undici#2702</a></li>
<li>perf: use insertion sort algorithm by <a href="https://github.com/tsctx"><code>@​tsctx</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2706">nodejs/undici#2706</a></li>
<li>fix: run node tests on merge by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2707">nodejs/undici#2707</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/rossilor95"><code>@​rossilor95</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/2644">nodejs/undici#2644</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v6.6.1...v6.6.2">https://github.com/nodejs/undici/compare/v6.6.1...v6.6.2</a></p>
<h2>v6.6.1</h2>
<h2>⚠️ Security Release ⚠️</h2>
<p>Fixes:</p>
<ul>
<li><a href="https://github.com/nodejs/undici/security/advisories/GHSA-9f24-jqhm-jfcw">CVE-2024-24750, Backpressure request ignored in fetch()</a></li>
<li><a href="https://github.com/nodejs/undici/security/advisories/GHSA-3787-6prv-h9w3">CVE-2024-24758 Proxy-Authorization header not cleared on cross-origin redirect in fetch</a></li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>fix: flaky debug test by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2687">nodejs/undici#2687</a></li>
<li>build(deps): bump github/codeql-action from 3.22.12 to 3.23.2 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2688">nodejs/undici#2688</a></li>
<li>build(deps): bump actions/dependency-review-action from 3.1.0 to 4.0.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2689">nodejs/undici#2689</a></li>
<li>fix: ci pipeline warnings by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2685">nodejs/undici#2685</a></li>
<li>perf: optimize Iterator by <a href="https://github.com/tsctx"><code>@​tsctx</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2692">nodejs/undici#2692</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v6.6.0...v6.6.1">https://github.com/nodejs/undici/compare/v6.6.0...v6.6.1</a></p>
<h2>v6.6.0</h2>
<h2>What's Changed</h2>
<ul>
<li>add webSocket example by <a href="https://github.com/mertcanaltin"><code>@​mertcanaltin</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2626">nodejs/undici#2626</a></li>
<li>chore: remove atomic-sleep as dev dependency by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2648">nodejs/undici#2648</a></li>
<li>chore: remove semver as dev dependency by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2646">nodejs/undici#2646</a></li>
<li>chore: remove table as dev dependency by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2649">nodejs/undici#2649</a></li>
<li>chore: remove delay as dev dependency by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2647">nodejs/undici#2647</a></li>
<li>chore: reduce noise in test-logs test/issue-2349.js by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2655">nodejs/undici#2655</a></li>
<li>chore: fix faketimer warning in test/request-timeout.js by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2656">nodejs/undici#2656</a></li>
<li>chore: reduce noise in test logs test/client-node-max-header-size.js by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2654">nodejs/undici#2654</a></li>
<li>refactor: use fromInnerResponse by <a href="https://github.com/tsctx"><code>@​tsctx</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2635">nodejs/undici#2635</a></li>
<li>fix: support deflate raw responses by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2650">nodejs/undici#2650</a></li>
<li>Support building for externally shared js builtins by <a href="https://github.com/mochaaP"><code>@​mochaaP</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2643">nodejs/undici#2643</a></li>
<li>fix: typo clampAndCoarsenConnectionTimingInfo by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2653">nodejs/undici#2653</a></li>
<li>chore: use 'node:'-prefix for requiring node core modules by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2662">nodejs/undici#2662</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nodejs/undici/commit/e48df9620edf1428bd457f481d47fa2c77f75322"><code>e48df96</code></a> fix: run node tests on merge (<a href="https://redirect.github.com/nodejs/undici/issues/2707">#2707</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/2b3c9b72c84155f8b4ad72a95f5c3a24d2d6045a"><code>2b3c9b7</code></a> perf: use insertion sort algorithm (<a href="https://redirect.github.com/nodejs/undici/issues/2706">#2706</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/f1873208c02bcef7af64f08a194a2c065d7a0710"><code>f187320</code></a> Bumped v6.6.2</li>
<li><a href="https://github.com/nodejs/undici/commit/8e1407824ccd55ed5348eb6fd13616975f4f3a25"><code>8e14078</code></a> build(deps-dev): bump borp from 0.5.0 to 0.9.1 (<a href="https://redirect.github.com/nodejs/undici/issues/2702">#2702</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/fa28c054ee765f8533d36a2960912b86cc890ee7"><code>fa28c05</code></a> test(wpt): mark timed out tests as 'failed' (<a href="https://redirect.github.com/nodejs/undici/issues/2644">#2644</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/d5ad4664732f928bd88a90a2f13c382f094fb5f9"><code>d5ad466</code></a> fix: fix the linux patch (<a href="https://redirect.github.com/nodejs/undici/issues/2703">#2703</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/cf4d90dff47dd9d1be9241fe9a324f6b7f671dda"><code>cf4d90d</code></a> Fix broken test on linux (<a href="https://redirect.github.com/nodejs/undici/issues/2699">#2699</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/a0812d8aed8752f76cdbd11f14693abd43689fa6"><code>a0812d8</code></a> test: more resilient debug tests (<a href="https://redirect.github.com/nodejs/undici/issues/2695">#2695</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/415a54081deeb5b4a081897f60454f6bd107c6b0"><code>415a540</code></a> fix: expose eventsource for nodejs (<a href="https://redirect.github.com/nodejs/undici/issues/2645">#2645</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/2cc38adb0fffbab8c917790c638206596083fd74"><code>2cc38ad</code></a> fix: webidl.brandcheck non strict should throw (<a href="https://redirect.github.com/nodejs/undici/issues/2683">#2683</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/nodejs/undici/compare/v5.27.2...v6.6.2">compare view</a></li>
</ul>
</details>
<br />

Updates `@angular-devkit/build-angular` from 17.0.0 to 17.2.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/angular/angular-cli/releases"><code>@​angular-devkit/build-angular</code>'s releases</a>.</em></p>
<blockquote>
<h2>v17.2.0</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>17.2.0 (2024-02-14)</h1>
<h3><code>@​schematics/angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/03e1aa7904acfe9d12eaf3717d1b136159893a76"><img src="https://img.shields.io/badge/03e1aa790-feat-blue" alt="feat - 03e1aa790" /></a></td>
<td>add support to <code>bun</code> package manager</td>
</tr>
</tbody>
</table>
<h3><code>@​angular/cli</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/b3e206741c5b59b8563b7c60a1f66c49802549e7"><img src="https://img.shields.io/badge/b3e206741-feat-blue" alt="feat - b3e206741" /></a></td>
<td>add support to <code>bun</code> package manager</td>
</tr>
</tbody>
</table>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/7f57123fd40b345d7880cb9e2eccd4757c0fb6ee"><img src="https://img.shields.io/badge/7f57123fd-feat-blue" alt="feat - 7f57123fd" /></a></td>
<td>add define build option to application builder</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/f4f535653a34c2a7c37c51c98680b6b1766c6d0d"><img src="https://img.shields.io/badge/f4f535653-feat-blue" alt="feat - f4f535653" /></a></td>
<td>add JSON build logs when using the application builder</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/b59f663e5715e009b05bf560637c1bca3b112784"><img src="https://img.shields.io/badge/b59f663e5-feat-blue" alt="feat - b59f663e5" /></a></td>
<td>allow control of Vite-based development server prebundling</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/8f47f1e965b25f3d976eda701ae2e7b7e8cccfa3"><img src="https://img.shields.io/badge/8f47f1e96-feat-blue" alt="feat - 8f47f1e96" /></a></td>
<td>provide default and abbreviated build target support for dev-server and extract-i18n</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/7a12074dc940f1aa8f5347071324fa0d2fd1300b"><img src="https://img.shields.io/badge/7a12074dc-feat-blue" alt="feat - 7a12074dc" /></a></td>
<td>provide option to allow automatically cleaning the terminal screen during rebuilds</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/7c522aa8742cd936bb0dfd30773d88f3ef92d488"><img src="https://img.shields.io/badge/7c522aa87-feat-blue" alt="feat - 7c522aa87" /></a></td>
<td>support using custom postcss configuration with application builder</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/476a68daa9746d29d3f74f68307d982d1d66f94c"><img src="https://img.shields.io/badge/476a68daa-fix-green" alt="fix - 476a68daa" /></a></td>
<td>add output location in build stats</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/5e6f1a9f4362e9b12db64c7c2e609a346b17963d"><img src="https://img.shields.io/badge/5e6f1a9f4-fix-green" alt="fix - 5e6f1a9f4" /></a></td>
<td>avoid preloading server chunks</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/41ea985f9317b11cfa6627a2d3f6b34ff4dbc134"><img src="https://img.shields.io/badge/41ea985f9-fix-green" alt="fix - 41ea985f9" /></a></td>
<td>display server bundles in build stats</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/d493609d30e1f148a7efb72bd64227521a326fbb"><img src="https://img.shields.io/badge/d493609d3-fix-green" alt="fix - d493609d3" /></a></td>
<td>downgrade copy-webpack-plugin to workaround Node.js support issue</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/8d5af1d5c78ce9aa996f6ba138b99d0bb5005d46"><img src="https://img.shields.io/badge/8d5af1d5c-fix-green" alt="fix - 8d5af1d5c" /></a></td>
<td>ensure correct <code>.html</code> served with Vite dev-server</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/944cbcdb1af62855febc931fce92debf28a3b2a5"><img src="https://img.shields.io/badge/944cbcdb1-fix-green" alt="fix - 944cbcdb1" /></a></td>
<td>limit the number of lazy chunks visible in the stats table</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/905e13633071b1db25621ae9f2762a48fe010df1"><img src="https://img.shields.io/badge/905e13633-fix-green" alt="fix - 905e13633" /></a></td>
<td>support string as plugin option in custom postcss plugin config</td>
</tr>
</tbody>
</table>
<h3><code>@​angular-devkit/schematics</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/da1c38c486b07d5a1b2933f23f83c6231b512e0f"><img src="https://img.shields.io/badge/da1c38c48-fix-green" alt="fix - da1c38c48" /></a></td>
<td>add <code>bun</code> to known package managers</td>
</tr>
</tbody>
</table>
<h3><code>@​angular/create</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/600498f2cd3e3251e7e6e3dd3505c5e943b2986a"><img src="https://img.shields.io/badge/600498f2c-feat-blue" alt="feat - 600498f2c" /></a></td>
<td>add support to <code>bun</code> package manager</td>
</tr>
</tbody>
</table>
<h2>v17.2.0-rc.0</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>17.2.0-rc.0 (2024-02-08)</h1>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/7f57123fd40b345d7880cb9e2eccd4757c0fb6ee"><img src="https://img.shields.io/badge/7f57123fd-feat-blue" alt="feat - 7f57123fd" /></a></td>
<td>add define build option to application builder</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/b59f663e5715e009b05bf560637c1bca3b112784"><img src="https://img.shields.io/badge/b59f663e5-feat-blue" alt="feat - b59f663e5" /></a></td>
<td>allow control of Vite-based development server prebundling</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/7a12074dc940f1aa8f5347071324fa0d2fd1300b"><img src="https://img.shields.io/badge/7a12074dc-feat-blue" alt="feat - 7a12074dc" /></a></td>
<td>provide option to allow automatically cleaning the terminal screen during rebuilds</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/2a25e06eaeba1e30ca6ddd76e7bd46b66c2112db"><img src="https://img.shields.io/badge/2a25e06ea-fix-green" alt="fix - 2a25e06ea" /></a></td>
<td>allow <code>./</code> baseHref when using vite based server</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/5e6f1a9f4362e9b12db64c7c2e609a346b17963d"><img src="https://img.shields.io/badge/5e6f1a9f4-fix-green" alt="fix - 5e6f1a9f4" /></a></td>
<td>avoid preloading server chunks</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/8d5af1d5c78ce9aa996f6ba138b99d0bb5005d46"><img src="https://img.shields.io/badge/8d5af1d5c-fix-green" alt="fix - 8d5af1d5c" /></a></td>
<td>ensure correct <code>.html</code> served with Vite dev-server</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/1aeeb7da099ff90126b0844eb6c8ed21d174e617"><img src="https://img.shields.io/badge/1aeeb7da0-fix-green" alt="fix - 1aeeb7da0" /></a></td>
<td>ensure WebWorker main entry is used in output code</td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/angular/angular-cli/blob/main/CHANGELOG.md"><code>@​angular-devkit/build-angular</code>'s changelog</a>.</em></p>
<blockquote>
<h1>17.2.0 (2024-02-14)</h1>
<h3><code>@​angular/cli</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/b3e206741c5b59b8563b7c60a1f66c49802549e7">b3e206741</a></td>
<td>feat</td>
<td>add support to <code>bun</code> package manager</td>
</tr>
</tbody>
</table>
<h3><code>@​schematics/angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/03e1aa7904acfe9d12eaf3717d1b136159893a76">03e1aa790</a></td>
<td>feat</td>
<td>add support to <code>bun</code> package manager</td>
</tr>
</tbody>
</table>
<h3><code>@​angular-devkit/build-angular</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/7f57123fd40b345d7880cb9e2eccd4757c0fb6ee">7f57123fd</a></td>
<td>feat</td>
<td>add define build option to application builder</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/f4f535653a34c2a7c37c51c98680b6b1766c6d0d">f4f535653</a></td>
<td>feat</td>
<td>add JSON build logs when using the application builder</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/b59f663e5715e009b05bf560637c1bca3b112784">b59f663e5</a></td>
<td>feat</td>
<td>allow control of Vite-based development server prebundling</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/8f47f1e965b25f3d976eda701ae2e7b7e8cccfa3">8f47f1e96</a></td>
<td>feat</td>
<td>provide default and abbreviated build target support for dev-server and extract-i18n</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/7a12074dc940f1aa8f5347071324fa0d2fd1300b">7a12074dc</a></td>
<td>feat</td>
<td>provide option to allow automatically cleaning the terminal screen during rebuilds</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/7c522aa8742cd936bb0dfd30773d88f3ef92d488">7c522aa87</a></td>
<td>feat</td>
<td>support using custom postcss configuration with application builder</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/476a68daa9746d29d3f74f68307d982d1d66f94c">476a68daa</a></td>
<td>fix</td>
<td>add output location in build stats</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/5e6f1a9f4362e9b12db64c7c2e609a346b17963d">5e6f1a9f4</a></td>
<td>fix</td>
<td>avoid preloading server chunks</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/41ea985f9317b11cfa6627a2d3f6b34ff4dbc134">41ea985f9</a></td>
<td>fix</td>
<td>display server bundles in build stats</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/d493609d30e1f148a7efb72bd64227521a326fbb">d493609d3</a></td>
<td>fix</td>
<td>downgrade copy-webpack-plugin to workaround Node.js support issue</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/8d5af1d5c78ce9aa996f6ba138b99d0bb5005d46">8d5af1d5c</a></td>
<td>fix</td>
<td>ensure correct <code>.html</code> served with Vite dev-server</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/944cbcdb1af62855febc931fce92debf28a3b2a5">944cbcdb1</a></td>
<td>fix</td>
<td>limit the number of lazy chunks visible in the stats table</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/905e13633071b1db25621ae9f2762a48fe010df1">905e13633</a></td>
<td>fix</td>
<td>support string as plugin option in custom postcss plugin config</td>
</tr>
</tbody>
</table>
<h3><code>@​angular-devkit/schematics</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/da1c38c486b07d5a1b2933f23f83c6231b512e0f">da1c38c48</a></td>
<td>fix</td>
<td>add <code>bun</code> to known package managers</td>
</tr>
</tbody>
</table>
<h3><code>@​angular/create</code></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/600498f2cd3e3251e7e6e3dd3505c5e943b2986a">600498f2c</a></td>
<td>feat</td>
<td>add support to <code>bun</code> package manager</td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>17.1.4 (2024-02-14)</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/angular/angular-cli/commit/644010d2f41e1c2f2935866a0a8b2b80b5ee39d1"><code>644010d</code></a> release: cut the v17.2.0 release</li>
<li><a href="https://github.com/angular/angular-cli/commit/79b1edd9bf228a6e5d27f2e48b1d39d064963913"><code>79b1edd</code></a> build: update Angular peer deps packages to 17.2.0</li>
<li><a href="https://github.com/angular/angular-cli/commit/905e13633071b1db25621ae9f2762a48fe010df1"><code>905e136</code></a> fix(<code>@​angular-devkit/build-angular</code>): support string as plugin option in custom...</li>
<li><a href="https://github.com/angular/angular-cli/commit/d493609d30e1f148a7efb72bd64227521a326fbb"><code>d493609</code></a> fix(<code>@​angular-devkit/build-angular</code>): downgrade copy-webpack-plugin to workarou...</li>
<li><a href="https://github.com/angular/angular-cli/commit/8598bb51bfb107b318fc6ce6a9f4d3504effeb41"><code>8598bb5</code></a> fix(<code>@​angular-devkit/build-angular</code>): bypass Vite prebundling for absolute URL ...</li>
<li><a href="https://github.com/angular/angular-cli/commit/b07246a092e8941d0a37e0c452adf1431dd9ab33"><code>b07246a</code></a> fix(<code>@​angular/cli</code>): prevent BOM errors in <code>package.json</code> during <code>ng update</code></li>
<li><a href="https://github.com/angular/angular-cli/commit/da1c38c486b07d5a1b2933f23f83c6231b512e0f"><code>da1c38c</code></a> fix(<code>@​angular-devkit/schematics</code>): add <code>bun</code> to known package managers</li>
<li><a href="https://github.com/angular/angular-cli/commit/d50c4ccc4dfc1fc7b4ec0ece3cc47bcd81b5dd90"><code>d50c4cc</code></a> release: cut the v17.2.0-rc.0 release</li>
<li><a href="https://github.com/angular/angular-cli/commit/1b6b7942aae7148bbc12fcb2d792d0dac7fc1568"><code>1b6b794</code></a> docs: release notes for the v17.1.3 release</li>
<li><a href="https://github.com/angular/angular-cli/commit/1aeeb7da099ff90126b0844eb6c8ed21d174e617"><code>1aeeb7d</code></a> fix(<code>@​angular-devkit/build-angular</code>): ensure WebWorker main entry is used in ou...</li>
<li>Additional commits viewable in <a href="https://github.com/angular/angular-cli/compare/17.0.0...17.2.0">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-controllers/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-16 18:19:44 +0000 UTC
    </div>
</div>

