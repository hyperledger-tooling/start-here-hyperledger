---
layout: default
title: bevel-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/bevel-samples
---

# bevel-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/bevel-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/46" class=".btn">#46</a>
            </td>
            <td>
                <b>
                    Bump postcss and react-scripts in /examples/supplychain-app/supplychain-frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [postcss](https://github.com/postcss/postcss) to 8.4.31 and updates ancestor dependency [react-scripts](https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts). These dependencies need to be updated together.

Updates `postcss` from 6.0.23 to 8.4.31
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/postcss/postcss/releases">postcss's releases</a>.</em></p>
<blockquote>
<h2>8.4.31</h2>
<ul>
<li>Fixed <code>\r</code> parsing to fix CVE-2023-44270.</li>
</ul>
<h2>8.4.30</h2>
<ul>
<li>Improved source map performance (by <a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
</ul>
<h2>8.4.29</h2>
<ul>
<li>Fixed <code>Node#source.offset</code> (by <a href="https://github.com/idoros"><code>@​idoros</code></a>).</li>
<li>Fixed docs (by <a href="https://github.com/coliff"><code>@​coliff</code></a>).</li>
</ul>
<h2>8.4.28</h2>
<ul>
<li>Fixed <code>Root.source.end</code> for better source map (by <a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed <code>Result.root</code> types when <code>process()</code> has no parser.</li>
</ul>
<h2>8.4.27</h2>
<ul>
<li>Fixed <code>Container</code> clone methods types.</li>
</ul>
<h2>8.4.26</h2>
<ul>
<li>Fixed clone methods types.</li>
</ul>
<h2>8.4.25</h2>
<ul>
<li>Improve stringify performance (by <a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed docs (by <a href="https://github.com/vikaskaliramna07"><code>@​vikaskaliramna07</code></a>).</li>
</ul>
<h2>8.4.24</h2>
<ul>
<li>Fixed <code>Plugin</code> types.</li>
</ul>
<h2>8.4.23</h2>
<ul>
<li>Fixed warnings in TypeDoc.</li>
</ul>
<h2>8.4.22</h2>
<ul>
<li>Fixed TypeScript support with <code>node16</code> (by <a href="https://github.com/remcohaszing"><code>@​remcohaszing</code></a>).</li>
</ul>
<h2>8.4.21</h2>
<ul>
<li>Fixed <code>Input#error</code> types (by <a href="https://github.com/hudochenkov"><code>@​hudochenkov</code></a>).</li>
</ul>
<h2>8.4.20</h2>
<ul>
<li>Fixed source map generation for childless at-rules like <code>@layer</code>.</li>
</ul>
<h2>8.4.19</h2>
<ul>
<li>Fixed whitespace preserving after AST transformations (by <a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
</ul>
<h2>8.4.18</h2>
<ul>
<li>Fixed an error on <code>absolute: true</code> with empty <code>sourceContent</code> (by <a href="https://github.com/KingSora"><code>@​KingSora</code></a>).</li>
</ul>
<h2>8.4.17</h2>
<ul>
<li>Fixed <code>Node.before()</code> unexpected behavior (by <a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Added TOC to docs (by <a href="https://github.com/muddv"><code>@​muddv</code></a>).</li>
</ul>
<h2>8.4.16</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/postcss/postcss/blob/main/CHANGELOG.md">postcss's changelog</a>.</em></p>
<blockquote>
<h2>8.4.31</h2>
<ul>
<li>Fixed <code>\r</code> parsing to fix CVE-2023-44270.</li>
</ul>
<h2>8.4.30</h2>
<ul>
<li>Improved source map performance (by Romain Menke).</li>
</ul>
<h2>8.4.29</h2>
<ul>
<li>Fixed <code>Node#source.offset</code> (by Ido Rosenthal).</li>
<li>Fixed docs (by Christian Oliff).</li>
</ul>
<h2>8.4.28</h2>
<ul>
<li>Fixed <code>Root.source.end</code> for better source map (by Romain Menke).</li>
<li>Fixed <code>Result.root</code> types when <code>process()</code> has no parser.</li>
</ul>
<h2>8.4.27</h2>
<ul>
<li>Fixed <code>Container</code> clone methods types.</li>
</ul>
<h2>8.4.26</h2>
<ul>
<li>Fixed clone methods types.</li>
</ul>
<h2>8.4.25</h2>
<ul>
<li>Improve stringify performance (by Romain Menke).</li>
<li>Fixed docs (by <a href="https://github.com/vikaskaliramna07"><code>@​vikaskaliramna07</code></a>).</li>
</ul>
<h2>8.4.24</h2>
<ul>
<li>Fixed <code>Plugin</code> types.</li>
</ul>
<h2>8.4.23</h2>
<ul>
<li>Fixed warnings in TypeDoc.</li>
</ul>
<h2>8.4.22</h2>
<ul>
<li>Fixed TypeScript support with <code>node16</code> (by Remco Haszing).</li>
</ul>
<h2>8.4.21</h2>
<ul>
<li>Fixed <code>Input#error</code> types (by Aleks Hudochenkov).</li>
</ul>
<h2>8.4.20</h2>
<ul>
<li>Fixed source map generation for childless at-rules like <code>@layer</code>.</li>
</ul>
<h2>8.4.19</h2>
<ul>
<li>Fixed whitespace preserving after AST transformations (by Romain Menke).</li>
</ul>
<h2>8.4.18</h2>
<ul>
<li>Fixed an error on <code>absolute: true</code> with empty <code>sourceContent</code> (by Rene Haas).</li>
</ul>
<h2>8.4.17</h2>
<ul>
<li>Fixed <code>Node.before()</code> unexpected behavior (by Romain Menke).</li>
<li>Added TOC to docs (by Mikhail Dedov).</li>
</ul>
<h2>8.4.16</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/postcss/postcss/commit/90208de8805dd762596c0028b8637ffbed23e371"><code>90208de</code></a> Release 8.4.31 version</li>
<li><a href="https://github.com/postcss/postcss/commit/58cc860b4c1707510c9cd1bc1fa30b423a9ad6c5"><code>58cc860</code></a> Fix carrier return parsing</li>
<li><a href="https://github.com/postcss/postcss/commit/4fff8e4cdc237619df1d73a444c0a8329701c1e2"><code>4fff8e4</code></a> Improve pnpm test output</li>
<li><a href="https://github.com/postcss/postcss/commit/cd43ed123274a92ebc13a1e8cccf1d65b8198f84"><code>cd43ed1</code></a> Update dependencies</li>
<li><a href="https://github.com/postcss/postcss/commit/caa916bdcbf66c51321574e2dde112ab13e8b306"><code>caa916b</code></a> Update dependencies</li>
<li><a href="https://github.com/postcss/postcss/commit/8972f76923e921a3c9655822382039b31b1c8e1a"><code>8972f76</code></a> Typo</li>
<li><a href="https://github.com/postcss/postcss/commit/11a5286f781d2a637f2c545c5e9cd661055acaab"><code>11a5286</code></a> Typo</li>
<li><a href="https://github.com/postcss/postcss/commit/45c55017776fc61f7815d1ea8e92d5291ca5d6c8"><code>45c5501</code></a> Release 8.4.30 version</li>
<li><a href="https://github.com/postcss/postcss/commit/bc3c341f589f9c15f1b56838a33d908374e537e0"><code>bc3c341</code></a> Update linter</li>
<li><a href="https://github.com/postcss/postcss/commit/b2be58a2eb788d12474ee1335f8ecdb9fa6225aa"><code>b2be58a</code></a> Merge pull request <a href="https://redirect.github.com/postcss/postcss/issues/1881">#1881</a> from romainmenke/improve-sourcemap-performance--phil...</li>
<li>Additional commits viewable in <a href="https://github.com/postcss/postcss/compare/6.0.23...8.4.31">compare view</a></li>
</ul>
</details>
<br />

Updates `react-scripts` from 2.1.8 to 5.0.1
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/facebook/create-react-app/blob/main/CHANGELOG-2.x.md">react-scripts's changelog</a>.</em></p>
<blockquote>
<h2>3.0.0 and Newer Versions</h2>
<p><strong>Please refer to <a href="https://github.com/facebook/create-react-app/blob/main/CHANGELOG.md">CHANGELOG.md</a> for the newer versions.</strong></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/facebook/create-react-app/commit/19fa58d527ae74f2b6baa0867463eea1d290f9a5"><code>19fa58d</code></a> Publish</li>
<li><a href="https://github.com/facebook/create-react-app/commit/9802941ff049a28da2682801bc182a29761b71f4"><code>9802941</code></a> fix: webpack noise printed only if error or warning (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/12245">#12245</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/2eef1d0a1db2e84cdcd6e7ca941c85a48cc7cc65"><code>2eef1d0</code></a> Update templates to use React 18 <code>createRoot</code> (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/12220">#12220</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/221e511730ca51c036c6954a9d2ee7659ff860f9"><code>221e511</code></a> Publish</li>
<li><a href="https://github.com/facebook/create-react-app/commit/5614c87bfbaae0ce52ac15aedd2cd0f91ffd420d"><code>5614c87</code></a> Add support for Tailwind (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11717">#11717</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/20edab4894b301f6b90dad0f90a2f82c52a7ac66"><code>20edab4</code></a> fix(webpackDevServer): disable overlay for warnings (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11413">#11413</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/3afbbc0ab922fb982bb275ccb3fe5beecdf5f889"><code>3afbbc0</code></a> Update all dependencies (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11624">#11624</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/f5467d5e77d51a3f23dd5fa70697dbab79832489"><code>f5467d5</code></a> feat(eslint-config-react-app): support ESLint 8.x (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11375">#11375</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/c7627ce96c4674f327081f101dd0e2771be4d045"><code>c7627ce</code></a> Update webpack and dev server (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11646">#11646</a>)</li>
<li><a href="https://github.com/facebook/create-react-app/commit/544befeb536a89b0ff95792df70bb037b17f55b9"><code>544befe</code></a> Update package.json (<a href="https://github.com/facebook/create-react-app/tree/HEAD/packages/react-scripts/issues/11597">#11597</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/facebook/create-react-app/commits/react-scripts@5.0.1/packages/react-scripts">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-04 02:19:46 +0000 UTC
    </div>
</div>

