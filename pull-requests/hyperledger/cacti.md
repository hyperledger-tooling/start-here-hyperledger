---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2750" class=".btn">#2750</a>
            </td>
            <td>
                <b>
                    feat(cactus-plugin-ledger-connector-ethereum): add signing utils
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add methods for signing transactions to ethereum connector.
- Modify offline signing test to use this new method.
- Modify electricity trade sample to use new signing method.
- Add offline signature section to ethereum connector readme.

**Pull Request Requirements**
[ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-06 12:24:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2749" class=".btn">#2749</a>
            </td>
            <td>
                <b>
                    feat(cactus-plugin-persistence-ethereum): use openapi ethereum connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                 - Refactor persistence ethereum plugin to use openapi ethereum connector
    instead of ethereum-socketio.
- Upgrade web3js to 4.X in both persistence plugin and its tests.
- Update persistence plugin dependency list.
- Recompile base token contracts in persistence plugin to match format
    required by ethereum connector (full compilation output, not just ABI)
- Minor fix in ethereum connector to return empty transactions
    array instead of undefined.
- Fix minor runtime issues in geth-test-ledger

Depends on #2631

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-05 15:02:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2748" class=".btn">#2748</a>
            </td>
            <td>
                <b>
                    Satp
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Pull Request Requirements**
[ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-05 13:49:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2740" class=".btn">#2740</a>
            </td>
            <td>
                <b>
                    build(lint): fix linter - doesn't work after last prettier upgrade to v3.0.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I ran `yarn up eslint-plugin-prettier --exact` to produce the diff of
this commit. I also ran `yarn lint` to verify that the linter works.

[skip ci]

Fixes #2727

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>


**Pull Request Requirements**
[x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-04 22:16:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2738" class=".btn">#2738</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump postcss from 8.4.16 to 8.4.31 in /packages/cacti-ledger-browser
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [postcss](https://github.com/postcss/postcss) from 8.4.16 to 8.4.31.
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
</blockquote>
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
</blockquote>
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
<li>Additional commits viewable in <a href="https://github.com/postcss/postcss/compare/8.4.16...8.4.31">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=postcss&package-manager=npm_and_yarn&previous-version=8.4.16&new-version=8.4.31)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-04 05:41:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2735" class=".btn">#2735</a>
            </td>
            <td>
                <b>
                    feat(cactus-example-electricity-trade): use openapi ethereum connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Refactor electricity trade sample to use openapi ethereum connector instead of ethereum-socketio.
- Sample still uses offline signing from cmd-socketio-server
- Handle case in ethereum connector where receipt doesn't contain status.
- Add sawtooth test-ledger script to wait until docker is fully started before proceeding forward.
- Remove periodicExecuter from sample app (didn't work and not used

**Pull Request Requirements**
[ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 15:11:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2734" class=".btn">#2734</a>
            </td>
            <td>
                <b>
                    ci(dast-nuclei): fix Could not run nuclei: no valid templates were found
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2590

**Pull Request Requirements**
[ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 07:45:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2733" class=".btn">#2733</a>
            </td>
            <td>
                <b>
                    build(deps): bump debug from 4.1.1 to 4.3.1 in /packages/cactus-plugin-ledger-connector-tcs-huawei-socketio
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [debug](https://github.com/debug-js/debug) from 4.1.1 to 4.3.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/debug-js/debug/releases">debug's releases</a>.</em></p>
<blockquote>
<h2>4.3.1</h2>
<h1>Patch release 4.3.1</h1>
<ul>
<li>Fixes a ReDOS regression (<a href="https://redirect.github.com/debug-js/debug/issues/458">#458</a>) - see <a href="https://redirect.github.com/debug-js/debug/issues/797">#797</a> for details.</li>
</ul>
<h2>4.3.0</h2>
<h1>Minor release</h1>
<ul>
<li><strong>Deprecated <code>debugInstance.destroy()</code></strong>. Future major versions will not have this method; please remove it from your codebases as it currently does nothing.</li>
<li>Fixed quoted percent sign</li>
<li>Fixed memory leak within debug instances that are created dynamically</li>
</ul>
<h2>4.2.0</h2>
<h1>Minor Release</h1>
<ul>
<li>Replaced phantomJS with chrome backend for browser tests</li>
<li>Deprecated and later removed Changelog.md in lieu of releases page</li>
<li>Removed bower.json (<a href="https://redirect.github.com/debug-js/debug/issues/602">#602</a>)</li>
<li>Removed .eslintrc (since we've switched to XO)</li>
<li>Removed .coveralls.yml</li>
<li>Removed the build system that was in place for various alternate package managers</li>
<li>Removed the examples folder (<a href="https://redirect.github.com/debug-js/debug/issues/650">#650</a>)</li>
<li>Switched to <code>console.debug</code> <strong>in the browser only</strong> when it is available (<a href="https://redirect.github.com/debug-js/debug/issues/600">#600</a>)</li>
<li>Copied custom logger to namespace extension (<a href="https://redirect.github.com/debug-js/debug/issues/646">#646</a>)</li>
<li>Added issue and pull request templates</li>
<li>Added <code>&quot;engines&quot;</code> key to package.json</li>
<li>Added ability to control <code>selectColor</code> (<a href="https://redirect.github.com/debug-js/debug/issues/747">#747</a>)</li>
<li>Updated dependencies</li>
<li>Marked <code>supports-color</code> as an optional peer dependency</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/debug-js/debug/commit/0d3d66b0eb47c5d34e1a940e8a204446fdd832cd"><code>0d3d66b</code></a> 4.3.1</li>
<li><a href="https://github.com/debug-js/debug/commit/b6d12fdbc63b483e5c969da33ea6adc09946b5ac"><code>b6d12fd</code></a> fix regression</li>
<li><a href="https://github.com/debug-js/debug/commit/3f56313c1e4a0d59c1054fb9b10026b6903bfba7"><code>3f56313</code></a> 4.3.0</li>
<li><a href="https://github.com/debug-js/debug/commit/e2d3bc9e428bdd45adb8d6e7f8ab543bee54d9a6"><code>e2d3bc9</code></a> add deprecation notice for debug.destroy()</li>
<li><a href="https://github.com/debug-js/debug/commit/72e7f864bd75fc8353e4dd450de96d9104ba9f35"><code>72e7f86</code></a> fix memory leak within debug instance</li>
<li><a href="https://github.com/debug-js/debug/commit/27152cad248df54217a14c072e7be1cd16da5f6d"><code>27152ca</code></a> add test for enable/disable of existing instances</li>
<li><a href="https://github.com/debug-js/debug/commit/22e13fe07e21f32888201aa40833599fd10a4fbb"><code>22e13fe</code></a> fix quoted percent sign</li>
<li><a href="https://github.com/debug-js/debug/commit/80ef62a3af4df95250d77d64edfc3d0e1667e7e8"><code>80ef62a</code></a> 4.2.0</li>
<li><a href="https://github.com/debug-js/debug/commit/09914af00e4c1479db9aa160bc51cb8c7e063ca4"><code>09914af</code></a> Marks supports-color as an <em>optional</em> peer dependency</li>
<li><a href="https://github.com/debug-js/debug/commit/db306db99e7822d355724698990d335927563210"><code>db306db</code></a> Update and pin ms to 2.1.2</li>
<li>Additional commits viewable in <a href="https://github.com/debug-js/debug/compare/4.1.1...4.3.1">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~qix">qix</a>, a new releaser for debug since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=debug&package-manager=npm_and_yarn&previous-version=4.1.1&new-version=4.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-02 23:03:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2732" class=".btn">#2732</a>
            </td>
            <td>
                <b>
                    build(plugin-keychain-vault): fix gradle error Redeclaration: ResponseType
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary change:
---------------

1. The codegen script now runs the clean script prior to its own
execution automatically (so that we don't forget to run it).
If we don't run the clean script prior to the code generation, then
the code generation doesn't delete old files just dumps the new ones
next to the old ones which leads to problems after upgrading the generator:
A newer version of the generator usually ships with different templates
that have restructured their code files so we end up with duplicates
breaking the build (unless we do a clean prior to codegen).

As for the actual build issue that this task was about:
It was a cross-cutting concern because the root cause of it was that
we were not cleaning up properly prior to the codegen task but this
applied to all the 2 or so dozen kotlin projects that we generate.

So as part of the solution I've ran the clean script and ran codegen
again which now produces code that builds without issues.

Secondary changes:
-----------------

Modified the clean script in the root project the following ways:
1. It is now cleaning up generated kotlin OpenAPI code as well
(previously it was not doing this at all despite what the name of the
script might suggest...)
2. It excludes all the openapi-generator-ignore files from being deleted
which has the beneficial side-effect that they do not get re-generated
with their default contents which would be missing files that we want
to ignore in addition to them.
3. The clean script NO LONGER DELETES the
`src/main/typescript/generated/proto/protoc-gen-ts` sub-folder of the
cmd-api-server package because the contents of it were not being re-
generated by the `codegen` script for some reason. This is something
to be fixed properly in the future but for now I just had to cut my
losses and make it work.

This depends on the PR being merged above because they both touch on
the generated code but in different ways. If we merged this one first,
the other one would have its diff emptied out (stealing the show).

[skip ci]

Fixes #2730

Depends on https://github.com/hyperledger/cacti/pull/2729

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-02 21:56:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2731" class=".btn">#2731</a>
            </td>
            <td>
                <b>
                    build(deps): bump webpki from 0.22.1 to 0.22.2 in /weaver/common/protos-rs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [webpki](https://github.com/briansmith/webpki) from 0.22.1 to 0.22.2.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/briansmith/webpki/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpki&package-manager=cargo&previous-version=0.22.1&new-version=0.22.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-02 21:42:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2729" class=".btn">#2729</a>
            </td>
            <td>
                <b>
                    chore(release): forgot to run codegen before v2.0.0-alpha.2 publish
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Ran the `yarn codegen` command so that all the generated docs/code comments/etc
get updated with the correct version (which changed from alpha.1 to alpha.2)

[skip ci]

Fixes #2728

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-02 17:55:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2726" class=".btn">#2726</a>
            </td>
            <td>
                <b>
                    docs(all): integrated documentation using canonical MkDocs template
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Moved old `docs` folder containing source files for legacy Cactus documentation to `docs-cactus`.
- Created new `docs ` folder using the MkDocs template specified in https://github.com/tkuhrt/documentation-template as the base.
  * Created overview files with useful links, diagrams, and references, for new and existing users
  * Migrated older Cactus and Weaver documentation for getting hands-on with code and samples to the new website, available through separate tabs
  * Fixed formatting, image references and other URLs, and organization
  * Created several stub files with temporary links, to be filled and expanded upon in due course, drawing on content already present in the above legacy documents
- Added a GitHub action to automatically push the documentation build (generated using `mkdocs`) to the `gh-pages` branch, and then publish those the `hyperledger` organization's GitHub page for Cacti.
  * To get an idea of how this looks and feels, see https://vramakrishna.github.io/cacti/, where these docs are currently being served from.
- Updated Discord handles for maintainers in the `MAINTAINERS.md` file.
- Fixed formatting typos in old doc files.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-01 15:56:40 +0000 UTC
    </div>
</div>

