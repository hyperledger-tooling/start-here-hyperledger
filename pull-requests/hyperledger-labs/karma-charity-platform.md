---
layout: default
title: karma-charity-platform
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/karma-charity-platform
---

# karma-charity-platform <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/karma-charity-platform){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/52" class=".btn">#52</a>
            </td>
            <td>
                <b>
                    Explorer merge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-10 14:05:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/48" class=".btn">#48</a>
            </td>
            <td>
                <b>
                    Bump terser and @angular-devkit/build-angular in /platform/frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [terser](https://github.com/terser/terser) to 5.14.2 and updates ancestor dependency [@angular-devkit/build-angular](https://github.com/angular/angular-cli). These dependencies need to be updated together.

Updates `terser` from 5.11.0 to 5.14.2
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/terser/terser/blob/master/CHANGELOG.md">terser's changelog</a>.</em></p>
<blockquote>
<h2>v5.14.2</h2>
<ul>
<li>Security fix for RegExps that should not be evaluated (regexp DDOS)</li>
<li>Source maps improvements (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1211">#1211</a>)</li>
<li>Performance improvements in long property access evaluation (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1213">#1213</a>)</li>
</ul>
<h2>v5.14.1</h2>
<ul>
<li>keep_numbers option added to TypeScript defs (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1208">#1208</a>)</li>
<li>Fixed parsing of nested template strings (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1204">#1204</a>)</li>
</ul>
<h2>v5.14.0</h2>
<ul>
<li>Switched to <code>@​jridgewell/source-map</code> for sourcemap generation (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1190">#1190</a>, <a href="https://github-redirect.dependabot.com/terser/terser/issues/1181">#1181</a>)</li>
<li>Fixed source maps with non-terminated segments (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1106">#1106</a>)</li>
<li>Enabled typescript types to be imported from the package (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1194">#1194</a>)</li>
<li>Extra DOM props have been added (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1191">#1191</a>)</li>
<li>Delete the AST while generating code, as a means to save RAM</li>
</ul>
<h2>v5.13.1</h2>
<ul>
<li>Removed self-assignments (<code>varname=varname</code>) (closes <a href="https://github-redirect.dependabot.com/terser/terser/issues/1081">#1081</a>)</li>
<li>Separated inlining code (for inlining things into references, or removing IIFEs)</li>
<li>Allow multiple identifiers with the same name in <code>var</code> destructuring (eg <code>var { a, a } = x</code>) (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1176">#1176</a>)</li>
</ul>
<h2>v5.13.0</h2>
<ul>
<li>All calls to eval() were removed (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1171">#1171</a>, <a href="https://github-redirect.dependabot.com/terser/terser/issues/1184">#1184</a>)</li>
<li><code>source-map</code> was updated to 0.8.0-beta.0 (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1164">#1164</a>)</li>
<li>NavigatorUAData was added to domprops to avoid property mangling (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1166">#1166</a>)</li>
</ul>
<h2>v5.12.1</h2>
<ul>
<li>Fixed an issue with function definitions inside blocks (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1155">#1155</a>)</li>
<li>Fixed parens of <code>new</code> in some situations (closes <a href="https://github-redirect.dependabot.com/terser/terser/issues/1159">#1159</a>)</li>
</ul>
<h2>v5.12.0</h2>
<ul>
<li><code>TERSER_DEBUG_DIR</code> environment variable</li>
<li><a href="https://github.com/copyright"><code>@​copyright</code></a> comments are now preserved with the comments=&quot;some&quot; option (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1153">#1153</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/terser/terser/commit/c5cb19de2baafa1db60b1e8c387d9d995844f7ef"><code>c5cb19d</code></a> 5.14.2</li>
<li><a href="https://github.com/terser/terser/commit/a4da7349fdc92c05094f41d33d06d8cd4e90e76b"><code>a4da734</code></a> fix potential regexp DDOS</li>
<li><a href="https://github.com/terser/terser/commit/839b81b24d04f217e8c454990c8b1de7e5e68b6b"><code>839b81b</code></a> Add source mapping for closing <code>}</code> (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1211">#1211</a>)</li>
<li><a href="https://github.com/terser/terser/commit/645a092323fad50d2fc4c1c6b49ce1db0d9eeb4f"><code>645a092</code></a> Optimize property access evaluation (<a href="https://github-redirect.dependabot.com/terser/terser/issues/1213">#1213</a>)</li>
<li><a href="https://github.com/terser/terser/commit/6706fec4b4e0622874854e75e7855b8afca4f1cc"><code>6706fec</code></a> 5.14.1</li>
<li><a href="https://github.com/terser/terser/commit/4a56ef22b96ac3b565bd21066c365a360b9559f7"><code>4a56ef2</code></a> update changelog</li>
<li><a href="https://github.com/terser/terser/commit/c558e1216b9f7cff21cb58ead6fb2d9785a41262"><code>c558e12</code></a> Add keep_numbers option. Closes <a href="https://github-redirect.dependabot.com/terser/terser/issues/1208">#1208</a></li>
<li><a href="https://github.com/terser/terser/commit/f745ac75f1adbfc5dc4d1e4a8c365eb9463def01"><code>f745ac7</code></a> fix parsing of nested template strings. Closes <a href="https://github-redirect.dependabot.com/terser/terser/issues/1204">#1204</a></li>
<li><a href="https://github.com/terser/terser/commit/17077538002e529ea96a37ae567d5121296177bf"><code>1707753</code></a> 5.14.0</li>
<li><a href="https://github.com/terser/terser/commit/cb8283378037c6ca18c6c950e0e6f5ed9f856b64"><code>cb82833</code></a> update changelog</li>
<li>Additional commits viewable in <a href="https://github.com/terser/terser/compare/v5.11.0...v5.14.2">compare view</a></li>
</ul>
</details>
<br />

Updates `@angular-devkit/build-angular` from 13.3.8 to 13.3.9
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/angular/angular-cli/releases"><code>@​angular-devkit/build-angular</code>'s releases</a>.</em></p>
<blockquote>
<h2>v13.3.9</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>13.3.9 (2022-07-20)</h1>
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
<td><a href="https://github.com/angular/angular-cli/commit/0d62716ae3753bb463de6b176ae07520ebb24fc9"><img src="https://img.shields.io/badge/0d62716ae-fix-green" alt="fix - 0d62716ae" /></a></td>
<td>update terser to address CVE-2022-25858</td>
</tr>
</tbody>
</table>
<h2>Special Thanks</h2>
<p>Alan Agius and Charles Lyding</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/angular/angular-cli/blob/main/CHANGELOG.md"><code>@​angular-devkit/build-angular</code>'s changelog</a>.</em></p>
<blockquote>
<h1>13.3.9 (2022-07-20)</h1>
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
<td><a href="https://github.com/angular/angular-cli/commit/0d62716ae3753bb463de6b176ae07520ebb24fc9">0d62716ae</a></td>
<td>fix</td>
<td>update terser to address CVE-2022-25858</td>
</tr>
</tbody>
</table>
<h2>Special Thanks</h2>
<p>Alan Agius and Charles Lyding</p>
<!-- raw HTML omitted -->
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>14.0.6 (2022-07-13)</h1>
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
<td><a href="https://github.com/angular/angular-cli/commit/1785505290940dad2ef9a62d4725e0d1b4b486d4">178550529</a></td>
<td>fix</td>
<td>handle cases when completion is enabled and running in an older CLI workspace</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular-cli/commit/10f24498ec2938487ae80d6ecea584e20b01dcbe">10f24498e</a></td>
<td>fix</td>
<td>remove deprecation warning of <code>no</code> prefixed schema options</td>
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
<td><a href="https://github.com/angular/angular-cli/commit/dfa6d73c5c45d3c3276fb1fecfb6535362d180c5">dfa6d73c5</a></td>
<td>fix</td>
<td>remove browserslist configuration</td>
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
<td><a href="https://github.com/angular/angular-cli/commit/4d848c4e6f6944f32b9ecb2cf2db5c544b3894fe">4d848c4e6</a></td>
<td>fix</td>
<td>generate different content hashes for scripts which are changed during the optimization phase</td>
</tr>
</tbody>
</table>
<h3><code>@​angular-devkit/core</code></h3>
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
<td><a href="https://github.com/angular/angular-cli/commit/2500f34a401c2ffb03b1dfa41299d91ddebe787e">2500f34a4</a></td>
<td>fix</td>
<td>provide actionable warning when a workspace project has missing <code>root</code> property</td>
</tr>
</tbody>
</table>
<h2>Special Thanks</h2>
<p>Alan Agius and martinfrancois</p>
<!-- raw HTML omitted -->
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/angular/angular-cli/commit/d091bb0c7b76a73e1b7d4b5690c532c68452b1d6"><code>d091bb0</code></a> release: cut the v13.3.9 release</li>
<li><a href="https://github.com/angular/angular-cli/commit/0d62716ae3753bb463de6b176ae07520ebb24fc9"><code>0d62716</code></a> fix(<code>@​angular-devkit/build-angular</code>): update terser to address CVE-2022-25858</li>
<li><a href="https://github.com/angular/angular-cli/commit/0bb875ddae9b3aba3c2fedb70e0222bc333f435a"><code>0bb875d</code></a> build: mark external only bazel rules</li>
<li>See full diff in <a href="https://github.com/angular/angular-cli/compare/13.3.8...13.3.9">compare view</a></li>
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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-10 13:01:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/47" class=".btn">#47</a>
            </td>
            <td>
                <b>
                    Bump async and cache-manager in /platform/backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [async](https://github.com/caolan/async) and [cache-manager](https://github.com/node-cache-manager/node-cache-manager). These dependencies needed to be updated together.
Updates `async` from 3.2.0 to 3.2.3
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/caolan/async/blob/master/CHANGELOG.md">async's changelog</a>.</em></p>
<blockquote>
<h1>v3.2.3</h1>
<ul>
<li>Fix bugs in comment parsing in <code>autoInject</code>. (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1767">#1767</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1780">#1780</a>)</li>
</ul>
<h1>v3.2.2</h1>
<ul>
<li>Fix potential prototype pollution exploit</li>
</ul>
<h1>v3.2.1</h1>
<ul>
<li>Use <code>queueMicrotask</code> if available to the environment (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1761">#1761</a>)</li>
<li>Minor perf improvement in <code>priorityQueue</code> (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1727">#1727</a>)</li>
<li>More examples in documentation (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1726">#1726</a>)</li>
<li>Various doc fixes (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1708">#1708</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1712">#1712</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1717">#1717</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1740">#1740</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1739">#1739</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1749">#1749</a>, <a href="https://github-redirect.dependabot.com/caolan/async/issues/1756">#1756</a>)</li>
<li>Improved test coverage (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1754">#1754</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/caolan/async/commit/62943cac64876328780792319a37da7f7b3966dd"><code>62943ca</code></a> Version 3.2.3</li>
<li><a href="https://github.com/caolan/async/commit/d2c9d51ebc1a43385449eb1a5192067f9442ac94"><code>d2c9d51</code></a> Update built files</li>
<li><a href="https://github.com/caolan/async/commit/de8d4c425f5c1b59c3b1a3ef9bdb325e50fc3816"><code>de8d4c4</code></a> Update changelog for v3.2.3</li>
<li><a href="https://github.com/caolan/async/commit/b015d34178801b8c717034f737927165007b07b4"><code>b015d34</code></a> fix: address edge case in comment stripping (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1780">#1780</a>)</li>
<li><a href="https://github.com/caolan/async/commit/e27aaab6cb5278ce312a673852bc962afa1ae233"><code>e27aaab</code></a> chore: remove unused Travis CI config (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1781">#1781</a>)</li>
<li><a href="https://github.com/caolan/async/commit/a038c8fb26419b35e2524564f7852c899ddd2251"><code>a038c8f</code></a> ci: setup GitHub Actions (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1782">#1782</a>)</li>
<li><a href="https://github.com/caolan/async/commit/e74bd18406e6511ca3da9d67d971d9b50dd9d8e8"><code>e74bd18</code></a> Core: const, let, arrow-fn and unused variables (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1776">#1776</a>)</li>
<li><a href="https://github.com/caolan/async/commit/2ee673f5af40bdbbec4ce21d81147e946b75d55a"><code>2ee673f</code></a> Housekeeping (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1772">#1772</a>)</li>
<li><a href="https://github.com/caolan/async/commit/cdfb4917e6028c8f966276d6e792018c7fd2ae3c"><code>cdfb491</code></a> Fix an inefficient regex in autoInject (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1767">#1767</a>)</li>
<li><a href="https://github.com/caolan/async/commit/bb41f2a59aa41af0b906f0cb9a11ffa6332e56dd"><code>bb41f2a</code></a> be explicit (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1769">#1769</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/caolan/async/compare/v3.2.0...v3.2.3">compare view</a></li>
</ul>
</details>
<br />

Updates `cache-manager` from 3.6.0 to 3.6.3
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/node-cache-manager/node-cache-manager/blob/master/History.md">cache-manager's changelog</a>.</em></p>
<blockquote>
<ul>
<li>
<p>3.6.3 2022-05-20</p>
<ul>
<li>Remove import from the code in order to be able to bundle and minify the module (<a href="https://github-redirect.dependabot.com/node-cache-manager/node-cache-manager/issues/191">#191</a>) - <a href="https://github.com/ricardomozartlino"><code>@​ricardomozartlino</code></a></li>
</ul>
</li>
<li>
<p>3.6.2 2022-05-19</p>
<ul>
<li>Use lodash.cloneDeep npm instead of full lodash. (<a href="https://github-redirect.dependabot.com/node-cache-manager/node-cache-manager/issues/190">#190</a>). - <a href="https://github.com/ricardomozartlino"><code>@​ricardomozartlino</code></a></li>
</ul>
</li>
<li>
<p>3.6.1 2022-04-07</p>
<ul>
<li>Fix for potential prototype polution exploit in async &lt; 3.2.2 (<a href="https://github-redirect.dependabot.com/node-cache-manager/node-cache-manager/issues/186">#186</a>). - <a href="https://github.com/tmbobbins"><code>@​tmbobbins</code></a></li>
</ul>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/node-cache-manager/node-cache-manager/commit/96a814fad67d3ff1c87c05ce04a06a50bec36cff"><code>96a814f</code></a> 3.6.3</li>
<li><a href="https://github.com/node-cache-manager/node-cache-manager/commit/46c3798bb7aad6ac917399239f1e2ba199d0bcfe"><code>46c3798</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/node-cache-manager/node-cache-manager/issues/191">#191</a> from ricardomozartlino/master</li>
<li><a href="https://github.com/node-cache-manager/node-cache-manager/commit/f524f5a41c1ad069da66ad04a001c75369cdc6ec"><code>f524f5a</code></a> Changed variable name</li>
<li><a href="https://github.com/node-cache-manager/node-cache-manager/commit/1f3508100d1948a48897c3d27525fb5d68e63d9d"><code>1f35081</code></a> Remove import from the code in order to be able to minify the module</li>
<li><a href="https://github.com/node-cache-manager/node-cache-manager/commit/076018f10493a41b0d22c6115ff061787d6e7d4e"><code>076018f</code></a> Merge branch 'release/3.6.2' into develop</li>
<li><a href="https://github.com/node-cache-manager/node-cache-manager/commit/cdf360ea1b0d953d172adb9046e9103c9adc8757"><code>cdf360e</code></a> Merge branch 'release/3.6.2'</li>
<li><a href="https://github.com/node-cache-manager/node-cache-manager/commit/8b61f7cb351f5b4c6e12869b37e0dfafe064ab75"><code>8b61f7c</code></a> 3.6.2</li>
<li><a href="https://github.com/node-cache-manager/node-cache-manager/commit/146c31fd56442489dfdf5e9d4623efd65d5227f1"><code>146c31f</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/node-cache-manager/node-cache-manager/issues/190">#190</a> from ricardomozartlino/master</li>
<li><a href="https://github.com/node-cache-manager/node-cache-manager/commit/8b9755a8a3567986ab7620abcf5a219c5f61cce0"><code>8b9755a</code></a> Using lodash.clonedeep instead of lodash to decrease module size</li>
<li><a href="https://github.com/node-cache-manager/node-cache-manager/commit/d7829d3a28ce509f95d32fba09254606f173cdc3"><code>d7829d3</code></a> Merge branch 'release/3.6.1' into develop</li>
<li>Additional commits viewable in <a href="https://github.com/node-cache-manager/node-cache-manager/compare/3.6.0...3.6.3">compare view</a></li>
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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-10 13:01:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/46" class=".btn">#46</a>
            </td>
            <td>
                <b>
                    Bump passport from 0.5.2 to 0.6.0 in /platform/backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [passport](https://github.com/jaredhanson/passport) from 0.5.2 to 0.6.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/jaredhanson/passport/blob/master/CHANGELOG.md">passport's changelog</a>.</em></p>
<blockquote>
<h2>[0.6.0] - 2022-05-20</h2>
<h3>Added</h3>
<ul>
<li><code>authenticate()</code>, <code>req#login</code>, and <code>req#logout</code> accept a
<code>keepSessionInfo: true</code> option to keep session information after regenerating
the session.</li>
</ul>
<h3>Changed</h3>
<ul>
<li><code>req#login()</code> and <code>req#logout()</code> regenerate the the session and clear session
information by default.</li>
<li><code>req#logout()</code> is now an asynchronous function and requires a callback
function as the last argument.</li>
</ul>
<h3>Security</h3>
<ul>
<li>Improved robustness against session fixation attacks in cases where there is
physical access to the same system or the application is susceptible to
cross-site scripting (XSS).</li>
</ul>
<h2>[0.5.3] - 2022-05-16</h2>
<h3>Fixed</h3>
<ul>
<li><code>initialize()</code> middleware extends request with <code>login()</code>, <code>logIn()</code>,
<code>logout()</code>, <code>logOut()</code>, <code>isAuthenticated()</code>, and <code>isUnauthenticated()</code> functions
again, reverting change from 0.5.1.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jaredhanson/passport/commit/c33067bc5aa81a6dd827076d810bf788bb6acac7"><code>c33067b</code></a> 0.6.0</li>
<li><a href="https://github.com/jaredhanson/passport/commit/3052bb4717673b88a27981f6bc91a1f585889e5c"><code>3052bb4</code></a> Update changelog.</li>
<li><a href="https://github.com/jaredhanson/passport/commit/42630cbd1ffd44d146ff96f0a4be6f3c12f81d75"><code>42630cb</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/jaredhanson/passport/issues/900">#900</a> from jaredhanson/fix-fixation</li>
<li><a href="https://github.com/jaredhanson/passport/commit/8dd79fe5f3f414435c4e0561fc925fb7ab6c8efb"><code>8dd79fe</code></a> Use utils-merge rather than Object.assign for compatibility.</li>
<li><a href="https://github.com/jaredhanson/passport/commit/4f6bd5b254454d3f61c3236e8f1dd33472704fd3"><code>4f6bd5b</code></a> Change keepSessionData to keepSessionData.</li>
<li><a href="https://github.com/jaredhanson/passport/commit/46756e56db671a822490f3d6c103a33a6691047d"><code>46756e5</code></a> Silence verbose logging.</li>
<li><a href="https://github.com/jaredhanson/passport/commit/987b1918a2c5056531bbd325a2ff888a3595b2df"><code>987b191</code></a> Add tests.</li>
<li><a href="https://github.com/jaredhanson/passport/commit/f8a175f1145c4efdffa7e4c511a642f608e11c0f"><code>f8a175f</code></a> Add tests.</li>
<li><a href="https://github.com/jaredhanson/passport/commit/29a90d68dd5d4bc807bc658cfe49fba968b34d7d"><code>29a90d6</code></a> No need to guard callback existence.</li>
<li><a href="https://github.com/jaredhanson/passport/commit/bfba8a1ab44b658f745e33e3484b389f0751cdc0"><code>bfba8a1</code></a> Add tests.</li>
<li>Additional commits viewable in <a href="https://github.com/jaredhanson/passport/compare/v0.5.2...v0.6.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=passport&package-manager=npm_and_yarn&previous-version=0.5.2&new-version=0.6.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-10 13:00:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/45" class=".btn">#45</a>
            </td>
            <td>
                <b>
                    update explorer backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Alexander Zemtsov <a.zemtsov@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-10 12:48:56 +0000 UTC
    </div>
</div>

