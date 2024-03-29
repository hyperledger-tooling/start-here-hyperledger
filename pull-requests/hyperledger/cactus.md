---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2263" class=".btn">#2263</a>
            </td>
            <td>
                <b>
                    fix(security): vulnerabilities found in keychain-vault-server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2058

Signed-off-by: aldousalvarez <aldousss.alvarez@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-11 12:50:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2262" class=".btn">#2262</a>
            </td>
            <td>
                <b>
                    build(deps): bump debug from 2.6.9 to 3.1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [debug](https://github.com/debug-js/debug) from 2.6.9 to 3.1.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/debug-js/debug/releases">debug's releases</a>.</em></p>
<blockquote>
<h2>3.1.0</h2>
<h3>Minor Changes</h3>
<ul>
<li>Ignore package-lock.json: e7e568a24736486721882282eb21beb31c741647</li>
<li>Remove <code>component.json</code>: 47747f329fe159e94262318b52b87a48f6c0acd4</li>
<li>Remove &quot;component&quot; from package.json: bdb7e0137f84dc8bcfc95daede7c694799d38dbf</li>
<li>Add <code>DEBUG_HIDE_DATE</code> env var: <a href="https://github-redirect.dependabot.com/debug-js/debug/issues/486">#486</a></li>
</ul>
<h3>Patches</h3>
<ul>
<li>Correct spelling mistake: daf1a7c8c0f62f5dbc8d48158d6748d0527cc551</li>
<li>Examples: fix colors printout: 7cd9e539ce571fc3314d34d9d1dac3124839dbac</li>
<li>Fix browser detection: fdfa0f5f6cc7e83fd60b6cf1e7b990cbf6388621</li>
<li>Remove ReDoS regexp in <code>%o</code> formatter: <a href="https://github-redirect.dependabot.com/debug-js/debug/issues/504">#504</a></li>
</ul>
<h3>Credits</h3>
<p>Huge thanks to <a href="https://github.com/amejiarosario"><code>@​amejiarosario</code></a> and <a href="https://github.com/zhuangya"><code>@​zhuangya</code></a> for their help!</p>
<h2>3.0.0</h2>
<p><a href="https://debug-browser-colors.now.sh/">Featuring pretty new colors!</a></p>
<!-- raw HTML omitted -->
<h3>Major Changes</h3>
<ul>
<li>Remove <code>DEBUG_FD</code>: <a href="https://github-redirect.dependabot.com/debug-js/debug/issues/406">#406</a></li>
<li>Make millisecond timer namespace specific and allow 'always enabled' output: <a href="https://github-redirect.dependabot.com/debug-js/debug/issues/408">#408</a></li>
<li>Use <code>Date#toISOString()</code> instead to <code>Date#toUTCString()</code> when output is not a TTY: <a href="https://github-redirect.dependabot.com/debug-js/debug/issues/418">#418</a></li>
<li><code>enabled()</code> updates existing debug instances: <a href="https://github-redirect.dependabot.com/debug-js/debug/issues/440">#440</a></li>
</ul>
<h3>Minor Changes</h3>
<ul>
<li>Add <code>destroy()</code> function: <a href="https://github-redirect.dependabot.com/debug-js/debug/issues/440">#440</a></li>
<li>Document <code>enabled</code> flag: <a href="https://github-redirect.dependabot.com/debug-js/debug/issues/465">#465</a></li>
<li>Support 256 colors: <a href="https://github-redirect.dependabot.com/debug-js/debug/issues/481">#481</a></li>
<li>Update &quot;browserify&quot; to v14.4.0: 826fd94639efeaa3c5701b50d335caead084a5d6</li>
<li>Separate Node.js and web browser examples: 87880f6ae1f48b12d9f3346bce564a66cba6b93e</li>
<li>Example: use %o formatter: 31f3343de76cb8687041387a1b811745c6e84473</li>
<li>More readme screenshots replaced: 25eb545324912dd2863658d0ba35426c0f617619</li>
<li>Add Namespace Colors section to readme: 8b5c438a222167bd0cc66db046bac073f01b3c01</li>
<li>Separate the Node and Browser tests in Travis: f178d861df18abacac6e9e4607c7306a1147bf3d</li>
</ul>
<h3>Patches</h3>
<ul>
<li>Readme: fix typo: <a href="https://github-redirect.dependabot.com/debug-js/debug/issues/473">#473</a></li>
<li>Component: update &quot;ms&quot; to v2.0.0: d2dd80aeaf1b037f0b3be21838c4594bbedc4a9c</li>
</ul>
<h3>Credits</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/debug-js/debug/blob/3.1.0/CHANGELOG.md">debug's changelog</a>.</em></p>
<blockquote>
<h1>3.1.0 / 2017-09-26</h1>
<ul>
<li>Add <code>DEBUG_HIDE_DATE</code> env var (<a href="https://github-redirect.dependabot.com/debug-js/debug/issues/486">#486</a>)</li>
<li>Remove ReDoS regexp in %o formatter (<a href="https://github-redirect.dependabot.com/debug-js/debug/issues/504">#504</a>)</li>
<li>Remove &quot;component&quot; from package.json</li>
<li>Remove <code>component.json</code></li>
<li>Ignore package-lock.json</li>
<li>Examples: fix colors printout</li>
<li>Fix: browser detection</li>
<li>Fix: spelling mistake (<a href="https://github-redirect.dependabot.com/debug-js/debug/issues/496">#496</a>, <a href="https://github.com/EdwardBetts"><code>@​EdwardBetts</code></a>)</li>
</ul>
<h1>3.0.1 / 2017-08-24</h1>
<ul>
<li>Fix: Disable colors in Edge and Internet Explorer (<a href="https://github-redirect.dependabot.com/debug-js/debug/issues/489">#489</a>)</li>
</ul>
<h1>3.0.0 / 2017-08-08</h1>
<ul>
<li>Breaking: Remove DEBUG_FD (<a href="https://github-redirect.dependabot.com/debug-js/debug/issues/406">#406</a>)</li>
<li>Breaking: Use <code>Date#toISOString()</code> instead to <code>Date#toUTCString()</code> when output is not a TTY (<a href="https://github-redirect.dependabot.com/debug-js/debug/issues/418">#418</a>)</li>
<li>Breaking: Make millisecond timer namespace specific and allow 'always enabled' output (<a href="https://github-redirect.dependabot.com/debug-js/debug/issues/408">#408</a>)</li>
<li>Addition: document <code>enabled</code> flag (<a href="https://github-redirect.dependabot.com/debug-js/debug/issues/465">#465</a>)</li>
<li>Addition: add 256 colors mode (<a href="https://github-redirect.dependabot.com/debug-js/debug/issues/481">#481</a>)</li>
<li>Addition: <code>enabled()</code> updates existing debug instances, add <code>destroy()</code> function (<a href="https://github-redirect.dependabot.com/debug-js/debug/issues/440">#440</a>)</li>
<li>Update: component: update &quot;ms&quot; to v2.0.0</li>
<li>Update: separate the Node and Browser tests in Travis-CI</li>
<li>Update: refactor Readme, fixed documentation, added &quot;Namespace Colors&quot; section, redid screenshots</li>
<li>Update: separate Node.js and web browser examples for organization</li>
<li>Update: update &quot;browserify&quot; to v14.4.0</li>
<li>Fix: fix Readme typo (<a href="https://github-redirect.dependabot.com/debug-js/debug/issues/473">#473</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/debug-js/debug/commit/f073e056f33efdd5b311381eb6bca2bc850745bf"><code>f073e05</code></a> Release 3.1.0</li>
<li><a href="https://github.com/debug-js/debug/commit/2c0df9baf7aefae2ea830e9d5eb2be64f0e71f18"><code>2c0df9b</code></a> rename <code>DEBUG_HIDE_TTY_DATE</code> to <code>DEBUG_HIDE_DATE</code></li>
<li><a href="https://github.com/debug-js/debug/commit/dcb37b2ca4ac0fdabe1f5c13299554464b5b6ae5"><code>dcb37b2</code></a> Merge branch '2.x'</li>
<li><a href="https://github.com/debug-js/debug/commit/56a3853b95990a22079d646601aa01e93eceb1c7"><code>56a3853</code></a> Add <code>DEBUG_HIDE_TTY_DATE</code> env var (<a href="https://github-redirect.dependabot.com/debug-js/debug/issues/486">#486</a>)</li>
<li><a href="https://github.com/debug-js/debug/commit/bdb7e0137f84dc8bcfc95daede7c694799d38dbf"><code>bdb7e01</code></a> remove &quot;component&quot; from package.json</li>
<li><a href="https://github.com/debug-js/debug/commit/c38a0166c266a679c8de012d4eaccec3f944e685"><code>c38a016</code></a> remove ReDoS regexp in %o formatter (<a href="https://github-redirect.dependabot.com/debug-js/debug/issues/504">#504</a>)</li>
<li><a href="https://github.com/debug-js/debug/commit/47747f329fe159e94262318b52b87a48f6c0acd4"><code>47747f3</code></a> remove <code>component.json</code></li>
<li><a href="https://github.com/debug-js/debug/commit/a0601e5e65ca80ce2f39b1243db332c64c124214"><code>a0601e5</code></a> fix</li>
<li><a href="https://github.com/debug-js/debug/commit/e7e568a24736486721882282eb21beb31c741647"><code>e7e568a</code></a> ignore package-lock.json</li>
<li><a href="https://github.com/debug-js/debug/commit/fdfa0f5f6cc7e83fd60b6cf1e7b990cbf6388621"><code>fdfa0f5</code></a> Fix browser detection</li>
<li>Additional commits viewable in <a href="https://github.com/debug-js/debug/compare/2.6.9...3.1.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=debug&package-manager=npm_and_yarn&previous-version=2.6.9&new-version=3.1.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cactus/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-11 11:00:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2261" class=".btn">#2261</a>
            </td>
            <td>
                <b>
                    build(deps): bump knex from 2.0.0 to 2.4.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [knex](https://github.com/knex/knex) from 2.0.0 to 2.4.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/knex/knex/releases">knex's releases</a>.</em></p>
<blockquote>
<h2>2.4.0</h2>
<h3>New features:</h3>
<ul>
<li>Support partial unique indexes <a href="https://github-redirect.dependabot.com/knex/knex/issues/5316">#5316</a></li>
<li>Make compiling SQL in error message optional <a href="https://github-redirect.dependabot.com/knex/knex/issues/5282">#5282</a></li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Insert array into json column <a href="https://github-redirect.dependabot.com/knex/knex/issues/5321">#5321</a></li>
<li>Fix unexpected max acquire-timeout <a href="https://github-redirect.dependabot.com/knex/knex/issues/5377">#5377</a></li>
<li>Fix: orWhereJson <a href="https://github-redirect.dependabot.com/knex/knex/issues/5361">#5361</a></li>
<li>MySQL: Add assertion for basic where clause not to be object or array <a href="https://github-redirect.dependabot.com/knex/knex/issues/1227">#1227</a></li>
<li>SQLite: Fix changing the default value of a boolean column in SQLite <a href="https://github-redirect.dependabot.com/knex/knex/issues/5319">#5319</a></li>
</ul>
<h3>Typings:</h3>
<ul>
<li>add missing type for 'expirationChecker' on PgConnectionConfig <a href="https://github-redirect.dependabot.com/knex/knex/issues/5334">#5334</a></li>
</ul>
<h2>2.3.0</h2>
<h3>New features:</h3>
<ul>
<li>PostgreSQL: Explicit jsonb support for custom pg clients <a href="https://github-redirect.dependabot.com/knex/knex/issues/5201">#5201</a></li>
<li>SQLite: Support returning with sqlite3 and better-sqlite3 <a href="https://github-redirect.dependabot.com/knex/knex/issues/5285">#5285</a></li>
<li>MSSQL: Implement mapBinding mssql dialect option <a href="https://github-redirect.dependabot.com/knex/knex/issues/5292">#5292</a></li>
</ul>
<h3>Typings:</h3>
<ul>
<li>Update types for TS 4.8 <a href="https://github-redirect.dependabot.com/knex/knex/issues/5279">#5279</a></li>
<li>Fix typo <a href="https://github-redirect.dependabot.com/knex/knex/issues/5267">#5267</a></li>
<li>Fix WhereJsonObject withCompositeTableType <a href="https://github-redirect.dependabot.com/knex/knex/issues/5306">#5306</a></li>
<li>Fix AnalyticFunction type <a href="https://github-redirect.dependabot.com/knex/knex/issues/5304">#5304</a></li>
<li>Infer specific column value type in aggregations <a href="https://github-redirect.dependabot.com/knex/knex/issues/5297">#5297</a></li>
</ul>
<h2>2.2.0</h2>
<h3>New features:</h3>
<ul>
<li>Inline primary key creation for postgres flavours <a href="https://github-redirect.dependabot.com/knex/knex/issues/5233">#5233</a></li>
<li>SQLite: Add warning for undefined connection file <a href="https://github-redirect.dependabot.com/knex/knex/issues/5223">#5223</a></li>
<li>MSSQL: Add JSON parameter support for connection <a href="https://github-redirect.dependabot.com/knex/knex/issues/5200">#5200</a></li>
</ul>
<h3>Bug fixes:</h3>
<ul>
<li>PostgreSQL: add primaryKey option for uuid <a href="https://github-redirect.dependabot.com/knex/knex/issues/5212">#5212</a></li>
</ul>
<h3>Typings:</h3>
<ul>
<li>Add promisable and better types <a href="https://github-redirect.dependabot.com/knex/knex/issues/5222">#5222</a></li>
<li>Update raw query bind parameter type <a href="https://github-redirect.dependabot.com/knex/knex/issues/5208">#5208</a></li>
</ul>
<h1>2.1.0 - 26 May, 2022</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/knex/knex/blob/master/CHANGELOG.md">knex's changelog</a>.</em></p>
<blockquote>
<h1>2.4.0 - 06 January, 2022</h1>
<h3>New features:</h3>
<ul>
<li>Support partial unique indexes <a href="https://github-redirect.dependabot.com/knex/knex/issues/5316">#5316</a></li>
<li>Make compiling SQL in error message optional <a href="https://github-redirect.dependabot.com/knex/knex/issues/5282">#5282</a></li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>Insert array into json column <a href="https://github-redirect.dependabot.com/knex/knex/issues/5321">#5321</a></li>
<li>Fix unexpected max acquire-timeout <a href="https://github-redirect.dependabot.com/knex/knex/issues/5377">#5377</a></li>
<li>Fix: orWhereJson <a href="https://github-redirect.dependabot.com/knex/knex/issues/5361">#5361</a></li>
<li>MySQL: Add assertion for basic where clause not to be object or array <a href="https://github-redirect.dependabot.com/knex/knex/issues/1227">#1227</a></li>
<li>SQLite: Fix changing the default value of a boolean column in SQLite <a href="https://github-redirect.dependabot.com/knex/knex/issues/5319">#5319</a></li>
</ul>
<h3>Typings:</h3>
<ul>
<li>add missing type for 'expirationChecker' on PgConnectionConfig <a href="https://github-redirect.dependabot.com/knex/knex/issues/5334">#5334</a></li>
</ul>
<h1>2.3.0 - 31 August, 2022</h1>
<h3>New features:</h3>
<ul>
<li>PostgreSQL: Explicit jsonb support for custom pg clients <a href="https://github-redirect.dependabot.com/knex/knex/issues/5201">#5201</a></li>
<li>SQLite: Support returning with sqlite3 and better-sqlite3 <a href="https://github-redirect.dependabot.com/knex/knex/issues/5285">#5285</a></li>
<li>MSSQL: Implement mapBinding mssql dialect option <a href="https://github-redirect.dependabot.com/knex/knex/issues/5292">#5292</a></li>
</ul>
<h3>Typings:</h3>
<ul>
<li>Update types for TS 4.8 <a href="https://github-redirect.dependabot.com/knex/knex/issues/5279">#5279</a></li>
<li>Fix typo <a href="https://github-redirect.dependabot.com/knex/knex/issues/5267">#5267</a></li>
<li>Fix WhereJsonObject withCompositeTableType <a href="https://github-redirect.dependabot.com/knex/knex/issues/5306">#5306</a></li>
<li>Fix AnalyticFunction type <a href="https://github-redirect.dependabot.com/knex/knex/issues/5304">#5304</a></li>
<li>Infer specific column value type in aggregations <a href="https://github-redirect.dependabot.com/knex/knex/issues/5297">#5297</a></li>
</ul>
<h1>2.2.0 - 19 July, 2022</h1>
<h3>New features:</h3>
<ul>
<li>Inline primary key creation for postgres flavours <a href="https://github-redirect.dependabot.com/knex/knex/issues/5233">#5233</a></li>
<li>SQLite: Add warning for undefined connection file <a href="https://github-redirect.dependabot.com/knex/knex/issues/5223">#5223</a></li>
<li>MSSQL: Add JSON parameter support for connection <a href="https://github-redirect.dependabot.com/knex/knex/issues/5200">#5200</a></li>
</ul>
<h3>Bug fixes:</h3>
<ul>
<li>PostgreSQL: add primaryKey option for uuid <a href="https://github-redirect.dependabot.com/knex/knex/issues/5212">#5212</a></li>
</ul>
<h3>Typings:</h3>
<ul>
<li>Add promisable and better types <a href="https://github-redirect.dependabot.com/knex/knex/issues/5222">#5222</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/knex/knex/commit/3475d8166863d6c9535527cd541d7c894e21ea84"><code>3475d81</code></a> Prepare to release 2.4.0</li>
<li><a href="https://github.com/knex/knex/commit/e97f92201a360f666e7df529fe5ff1cd1f7f9fcd"><code>e97f922</code></a> Bump tsd from 0.24.1 to 0.25.0 (<a href="https://github-redirect.dependabot.com/knex/knex/issues/5396">#5396</a>)</li>
<li><a href="https://github.com/knex/knex/commit/e145322da92749be7749f9ade5b5f5a66d6586a4"><code>e145322</code></a> 1227: add assertion for basic where clause values (<a href="https://github-redirect.dependabot.com/knex/knex/issues/5417">#5417</a>)</li>
<li><a href="https://github.com/knex/knex/commit/962bb0a635ed40a240021379521814b5bd36d438"><code>962bb0a</code></a> Bump sinon from 14.0.2 to 15.0.1 (<a href="https://github-redirect.dependabot.com/knex/knex/issues/5413">#5413</a>)</li>
<li><a href="https://github.com/knex/knex/commit/ab45314e70bc55a98de08d9c2bd7005bac146702"><code>ab45314</code></a> Add JSDoc (TS Flavour) to mjs stub file (<a href="https://github-redirect.dependabot.com/knex/knex/issues/5390">#5390</a>)</li>
<li><a href="https://github.com/knex/knex/commit/72bd1f7396b8472eb416a1eb8c8270737189b999"><code>72bd1f7</code></a> Fix: orWhereJson (<a href="https://github-redirect.dependabot.com/knex/knex/issues/5361">#5361</a>)</li>
<li><a href="https://github.com/knex/knex/commit/4fc939a17640fd1abf1a94d106b7836ae20c1d1e"><code>4fc939a</code></a> Fixes unexpected max acquire-timeout (<a href="https://github-redirect.dependabot.com/knex/knex/issues/5377">#5377</a>)</li>
<li><a href="https://github.com/knex/knex/commit/5c4837cd4f26d192527684a2d22ed2f0563060fe"><code>5c4837c</code></a> Fix lib/.gitignore path separator on Windows. (<a href="https://github-redirect.dependabot.com/knex/knex/issues/5325">#5325</a>)</li>
<li><a href="https://github.com/knex/knex/commit/7dbbd007014911b1f240fdf8cec8a191022eb6f7"><code>7dbbd00</code></a> Bump actions/setup-node from 3.4.1 to 3.5.1 (<a href="https://github-redirect.dependabot.com/knex/knex/issues/5356">#5356</a>)</li>
<li><a href="https://github.com/knex/knex/commit/d39051f4a56bbd4b2b48500f08198efddef5b94d"><code>d39051f</code></a> fix: add missing type for 'expirationChecker' on PgConnectionConfig (<a href="https://github-redirect.dependabot.com/knex/knex/issues/5334">#5334</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/knex/knex/compare/2.0.0...2.4.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=knex&package-manager=npm_and_yarn&previous-version=2.0.0&new-version=2.4.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cactus/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-11 04:31:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2260" class=".btn">#2260</a>
            </td>
            <td>
                <b>
                    build(deps): bump convict from 6.2.3 to 6.2.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [convict](https://github.com/mozilla/node-convict) from 6.2.3 to 6.2.4.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/mozilla/node-convict/blob/master/CHANGELOG.md">convict's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/mozilla/node-convict/compare/v6.2.3...v6.2.4">6.2.4</a> (2023-01-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>Fix imperfect prototype pollution fix (<a href="https://github-redirect.dependabot.com/mozilla/node-convict/issues/410">#410</a>) (<a href="https://github-redirect.dependabot.com/mozilla/node-convict/issues/411">#411</a>). Thanks to Captain-K-101</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/mozilla/node-convict/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=convict&package-manager=npm_and_yarn&previous-version=6.2.3&new-version=6.2.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cactus/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 22:22:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2259" class=".btn">#2259</a>
            </td>
            <td>
                <b>
                    feat(cactus-plugin-persistence-ethereum): add new persistence plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add a new plugin for storing ledger data into a database (or any other storage in the future).
- Add functional tests for plugin and data access layer operations.
- Increase gas limit on openethereum contract to solve occasional issues in automatic tests.
- Tests assume any postgres database, but for final deployment supabase is assumed.
- Data fed by this plugin can later by visualized by a GUI application or analyzed directly.

Depends on: https://github.com/hyperledger/cactus/pull/2254
Depends on: https://github.com/hyperledger/cactus/pull/2256

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 14:41:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2257" class=".btn">#2257</a>
            </td>
            <td>
                <b>
                    build(deps): bump jsonwebtoken from 8.5.1 to 9.0.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [jsonwebtoken](https://github.com/auth0/node-jsonwebtoken) from 8.5.1 to 9.0.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/auth0/node-jsonwebtoken/blob/master/CHANGELOG.md">jsonwebtoken's changelog</a>.</em></p>
<blockquote>
<h2>9.0.0 - 2022-12-21</h2>
<p><strong>Breaking changes: See <a href="https://github.com/auth0/node-jsonwebtoken/wiki/Migration-Notes:-v8-to-v9">Migration from v8 to v9</a></strong></p>
<h3>Breaking changes</h3>
<ul>
<li>Removed support for Node versions 11 and below.</li>
<li>The verify() function no longer accepts unsigned tokens by default. ([834503079514b72264fd13023a3b8d648afd6a16]<a href="https://github.com/auth0/node-jsonwebtoken/commit/834503079514b72264fd13023a3b8d648afd6a16">https://github.com/auth0/node-jsonwebtoken/commit/834503079514b72264fd13023a3b8d648afd6a16</a>)</li>
<li>RSA key size must be 2048 bits or greater. ([ecdf6cc6073ea13a7e71df5fad043550f08d0fa6]<a href="https://github.com/auth0/node-jsonwebtoken/commit/ecdf6cc6073ea13a7e71df5fad043550f08d0fa6">https://github.com/auth0/node-jsonwebtoken/commit/ecdf6cc6073ea13a7e71df5fad043550f08d0fa6</a>)</li>
<li>Key types must be valid for the signing / verification algorithm</li>
</ul>
<h3>Security fixes</h3>
<ul>
<li>security: fixes <code>Arbitrary File Write via verify function</code> - CVE-2022-23529</li>
<li>security: fixes <code>Insecure default algorithm in jwt.verify() could lead to signature validation bypass</code> - CVE-2022-23540</li>
<li>security: fixes <code>Insecure implementation of key retrieval function could lead to Forgeable Public/Private Tokens from RSA to HMAC</code> - CVE-2022-23541</li>
<li>security: fixes <code>Unrestricted key type could lead to legacy keys usage</code> - CVE-2022-23539</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/auth0/node-jsonwebtoken/commit/e1fa9dcc12054a8681db4e6373da1b30cf7016e3"><code>e1fa9dc</code></a> Merge pull request from GHSA-8cf7-32gw-wr33</li>
<li><a href="https://github.com/auth0/node-jsonwebtoken/commit/5eaedbf2b01676d952336e73b4d2efba847d2d1b"><code>5eaedbf</code></a> chore(ci): remove github test actions job (<a href="https://github-redirect.dependabot.com/auth0/node-jsonwebtoken/issues/861">#861</a>)</li>
<li><a href="https://github.com/auth0/node-jsonwebtoken/commit/cd4163eb1407aab0b3148f91b0b9c26276b96c6b"><code>cd4163e</code></a> chore(ci): configure Github Actions jobs for Tests &amp; Security Scanning (<a href="https://github-redirect.dependabot.com/auth0/node-jsonwebtoken/issues/856">#856</a>)</li>
<li><a href="https://github.com/auth0/node-jsonwebtoken/commit/ecdf6cc6073ea13a7e71df5fad043550f08d0fa6"><code>ecdf6cc</code></a> fix!: Prevent accidental use of insecure key sizes &amp; misconfiguration of secr...</li>
<li><a href="https://github.com/auth0/node-jsonwebtoken/commit/834503079514b72264fd13023a3b8d648afd6a16"><code>8345030</code></a> fix(sign&amp;verify)!: Remove default <code>none</code> support from <code>sign</code> and <code>verify</code> met...</li>
<li><a href="https://github.com/auth0/node-jsonwebtoken/commit/7e6a86b1c25e5fd05733c52c118848341aba1c4e"><code>7e6a86b</code></a> Upload OpsLevel YAML (<a href="https://github-redirect.dependabot.com/auth0/node-jsonwebtoken/issues/849">#849</a>)</li>
<li><a href="https://github.com/auth0/node-jsonwebtoken/commit/74d5719bd03993fcf71e3b176621f133eb6138c0"><code>74d5719</code></a> docs: update references vercel/ms references (<a href="https://github-redirect.dependabot.com/auth0/node-jsonwebtoken/issues/770">#770</a>)</li>
<li><a href="https://github.com/auth0/node-jsonwebtoken/commit/d71e383862fc735991fd2e759181480f066bf138"><code>d71e383</code></a> docs: document &quot;invalid token&quot; error</li>
<li><a href="https://github.com/auth0/node-jsonwebtoken/commit/37650031fd0bac1a5b0d682bbfcf8c1705917aa9"><code>3765003</code></a> docs: fix spelling in README.md: Peak -&gt; Peek (<a href="https://github-redirect.dependabot.com/auth0/node-jsonwebtoken/issues/754">#754</a>)</li>
<li><a href="https://github.com/auth0/node-jsonwebtoken/commit/a46097e962621ab2ba718d1da6025cdeba3597c8"><code>a46097e</code></a> docs: make decode impossible to discover before verify</li>
<li>Additional commits viewable in <a href="https://github.com/auth0/node-jsonwebtoken/compare/v8.5.1...v9.0.0">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~julien.wollscheid">julien.wollscheid</a>, a new releaser for jsonwebtoken since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jsonwebtoken&package-manager=npm_and_yarn&previous-version=8.5.1&new-version=9.0.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cactus/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 09:59:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2256" class=".btn">#2256</a>
            </td>
            <td>
                <b>
                    feat(connector-go-ethereum): add getBlock and getTransactionReceipt methods to connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - getBlock and getTransactionReceipt added in go-ethereum-socketio-connector
- Added nullish coalescing in monitor options

Closes: #2255
Signed-off-by: tomasz awramski <tomasz.awramski@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 16:07:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2254" class=".btn">#2254</a>
            </td>
            <td>
                <b>
                    feat(supabase-all-in-one): add docker image for test supabase instance
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add a new docker image `supabase-all-in-one` that will setup supabase instance for tests.
- Supabase is used as a backend for Cactus GUI.

Closes: #2253

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 15:27:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2252" class=".btn">#2252</a>
            </td>
            <td>
                <b>
                    feat(connector-iroha2): update to the new LTS image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Change iroha2 setup docker and helper classes to work with the new LTS image.
- Update Iroha SDK packages to the newest.
- Fix some tests that were failing after upgrade.
- Adjust SDK usage (new version doesn't create Torii client,
  arguments are provided with each method instead)

### WARNING
- Wait for pinned image versions before merging!

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 11:53:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2251" class=".btn">#2251</a>
            </td>
            <td>
                <b>
                    feat(besu-test-ledger): send funds to already created address
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Enable sending funds to an existing account.

New method created:
* sendEthToAccount

closes #2250

Signed-off-by: André Augusto <andre.augusto@tecnico.ulisboa.pt>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-08 20:07:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2249" class=".btn">#2249</a>
            </td>
            <td>
                <b>
                    feat(fabric-test-ledger): add support to enrolling users in different Orgs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Created new methods to avoid breaking changes in the API exported.

New methods created:
* capitalizedMspIdOfOrg
* enrollAdminV2
* enrollUserV2
* createCaClientV2

closes #2248

Signed-off-by: André Augusto <andre.augusto@tecnico.ulisboa.pt>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-08 19:51:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2247" class=".btn">#2247</a>
            </td>
            <td>
                <b>
                    build(deps): bump tokio from 1.19.2 to 1.20.3 in /packages/cactus-plugin-keychain-vault/src/cactus-keychain-vault-server/rust/gen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [tokio](https://github.com/tokio-rs/tokio) from 1.19.2 to 1.20.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tokio-rs/tokio/releases">tokio's releases</a>.</em></p>
<blockquote>
<h2>Tokio v1.20.2</h2>
<h1>1.20.2 (September 27, 2022)</h1>
<p>This release removes the dependency on the <code>once_cell</code> crate to restore the MSRV of the 1.20.x LTS release. (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5048">#5048</a>)</p>
<p><a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5048">#5048</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/5048">tokio-rs/tokio#5048</a></p>
<h2>Tokio v1.20.1</h2>
<h1>1.20.1 (July 25, 2022)</h1>
<h3>Fixed</h3>
<ul>
<li>chore: fix version detection in build script (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4860">#4860</a>)</li>
</ul>
<p><a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4860">#4860</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/4860">tokio-rs/tokio#4860</a></p>
<h2>Tokio v1.20.0</h2>
<h1>1.20.0 (July 12, 2022)</h1>
<h3>Added</h3>
<ul>
<li>tokio: add track_caller to public APIs (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4772">#4772</a>, <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4791">#4791</a>, <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4793">#4793</a>, <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4806">#4806</a>, <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4808">#4808</a>)</li>
<li>sync: Add <code>has_changed</code> method to <code>watch::Ref</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4758">#4758</a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>time: remove <code>src/time/driver/wheel/stack.rs</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4766">#4766</a>)</li>
<li>rt: clean up arguments passed to basic scheduler (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4767">#4767</a>)</li>
<li>net: be more specific about winapi features (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4764">#4764</a>)</li>
<li>tokio: use const initialized thread locals where possible (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4677">#4677</a>)</li>
<li>task: various small improvements to LocalKey (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4795">#4795</a>)</li>
</ul>
<h3>Fixed</h3>
<h3>Documented</h3>
<ul>
<li>fs: warn about performance pitfall (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4762">#4762</a>)</li>
<li>chore: fix spelling (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4769">#4769</a>)</li>
<li>sync: document spurious failures in oneshot (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4777">#4777</a>)</li>
<li>sync: add warning for watch in non-Send futures (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4741">#4741</a>)</li>
<li>chore: fix typo (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4798">#4798</a>)</li>
</ul>
<h3>Unstable</h3>
<ul>
<li>joinset: rename <code>join_one</code> to <code>join_next</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4755">#4755</a>)</li>
<li>rt: unhandled panic config for current thread rt (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4770">#4770</a>)</li>
</ul>
<p><a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4677">#4677</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/4677">tokio-rs/tokio#4677</a>
<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4741">#4741</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/4741">tokio-rs/tokio#4741</a>
<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4755">#4755</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/4755">tokio-rs/tokio#4755</a>
<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4758">#4758</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/4758">tokio-rs/tokio#4758</a>
<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4762">#4762</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/4762">tokio-rs/tokio#4762</a></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tokio-rs/tokio/commit/ba81945ffc2695b71f2bbcadbfb5e46ec55aaef3"><code>ba81945</code></a> chore: prepare Tokio 1.20.3 release</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/763bdc967e3e128d1e6e000238f1d257a81bf59a"><code>763bdc9</code></a> ci: run WASI tasks using latest Rust</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/9f98535877f8f706b436447952f40f153e2a52dc"><code>9f98535</code></a> Merge remote-tracking branch 'origin/tokio-1.18.x' into fix-named-pipes-1.20</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/9241c3eddf4a6a218681b088d71f7191513e2376"><code>9241c3e</code></a> chore: prepare Tokio v1.18.4 release</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/699573d550fabf4bfb45d82505d6709faaae9037"><code>699573d</code></a> net: fix named pipes server configuration builder</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/3d95a4626fc136b55e82e6bd480e14459a77a22c"><code>3d95a46</code></a> chore: prepare Tokio v1.20.2 (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5055">#5055</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/2063d6692e1a2f12522299d2e6f16dd482ebbb05"><code>2063d66</code></a> Merge 'tokio-1.18.3' into 'tokio-1.20.x' (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5054">#5054</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/5c76d070e28bd9153ec72f13d0ebe24935b9dea0"><code>5c76d07</code></a> chore: prepare Tokio v1.18.3 (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5051">#5051</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/05e661490b87a3d60a8342535bdc9d213048519c"><code>05e6614</code></a> chore: don't use <code>once_cell</code> for 1.18.x LTS release (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5048">#5048</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/c0746b6a300f558410e719e27d2d4855f5407262"><code>c0746b6</code></a> chore: prepare Tokio v1.20.1 (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4861">#4861</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/tokio-rs/tokio/compare/tokio-1.19.2...tokio-1.20.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tokio&package-manager=cargo&previous-version=1.19.2&new-version=1.20.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cactus/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 21:49:02 +0000 UTC
    </div>
</div>

