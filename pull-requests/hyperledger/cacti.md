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
                PR <a href="https://github.com/hyperledger/cacti/pull/2280" class=".btn">#2280</a>
            </td>
            <td>
                <b>
                    build(deps): bump jszip from 3.7.1 to 3.10.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [jszip](https://github.com/Stuk/jszip) from 3.7.1 to 3.10.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/Stuk/jszip/blob/main/CHANGES.md">jszip's changelog</a>.</em></p>
<blockquote>
<h3>v3.10.1 2022-08-02</h3>
<ul>
<li>Add sponsorship files.
<ul>
<li>If you appreciate the time spent maintaining JSZip then I would really appreciate <a href="https://github.com/sponsors/Stuk">your sponsorship</a>.</li>
</ul>
</li>
<li>Consolidate metadata types and expose OnUpdateCallback <a href="https://github-redirect.dependabot.com/Stuk/jszip/pull/851">#851</a> and <a href="https://github-redirect.dependabot.com/Stuk/jszip/pull/852">#852</a></li>
<li>use <code>const</code> instead <code>var</code> in example from README.markdown <a href="https://github-redirect.dependabot.com/Stuk/jszip/pull/828">#828</a></li>
<li>Switch manual download link to HTTPS <a href="https://github-redirect.dependabot.com/Stuk/jszip/pull/839">#839</a></li>
</ul>
<p>Internals:</p>
<ul>
<li>Replace jshint with eslint <a href="https://github-redirect.dependabot.com/Stuk/jszip/pull/842">#842</a></li>
<li>Add performance tests <a href="https://github-redirect.dependabot.com/Stuk/jszip/pull/834">#834</a></li>
</ul>
<h3>v3.10.0 2022-05-20</h3>
<ul>
<li>Change setimmediate dependency to more efficient one. Fixes <a href="https://github-redirect.dependabot.com/Stuk/jszip/issues/617">Stuk/jszip#617</a> (see <a href="https://github-redirect.dependabot.com/Stuk/jszip/pull/829">#829</a>)</li>
<li>Update types of <code>currentFile</code> metadata to include <code>null</code> (see <a href="https://github-redirect.dependabot.com/Stuk/jszip/pull/826">#826</a>)</li>
</ul>
<h3>v3.9.1 2022-04-06</h3>
<ul>
<li>Fix recursive definition of <code>InputFileFormat</code> introduced in 3.9.0.</li>
</ul>
<h3>v3.9.0 2022-04-04</h3>
<ul>
<li>Update types JSZip#loadAsync to accept a promise for data, and remove arguments from <code>new JSZip()</code> (see <a href="https://github-redirect.dependabot.com/Stuk/jszip/pull/752">#752</a>)</li>
<li>Update types for <code>compressionOptions</code> to JSZipFileOptions and JSZipGeneratorOptions (see <a href="https://github-redirect.dependabot.com/Stuk/jszip/pull/722">#722</a>)</li>
<li>Add types for <code>generateInternalStream</code> (see <a href="https://github-redirect.dependabot.com/Stuk/jszip/pull/774">#774</a>)</li>
</ul>
<h3>v3.8.0 2022-03-30</h3>
<ul>
<li>Santize filenames when files are loaded with <code>loadAsync</code>, to avoid <a href="https://snyk.io/research/zip-slip-vulnerability">&quot;zip slip&quot; attacks</a>. The original filename is available on each zip entry as <code>unsafeOriginalName</code>. See the <a href="https://stuk.github.io/jszip/documentation/api_jszip/load_async.html">documentation</a>. Many thanks to McCaulay Hudson for reporting.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/Stuk/jszip/commit/0f2f1e4d0509514417db83fe5b86bde90e0ffe8d"><code>0f2f1e4</code></a> 3.10.1</li>
<li><a href="https://github.com/Stuk/jszip/commit/cae55105f5e8bd37c270cdb76eab2cf40388dfd9"><code>cae5510</code></a> Updates for v3.10.1</li>
<li><a href="https://github.com/Stuk/jszip/commit/179c9a0340477985b82734f1b09560411adb5b94"><code>179c9a0</code></a> Update changelog for 3.10.1</li>
<li><a href="https://github.com/Stuk/jszip/commit/61e1df58dac54eec1e9733649638518b79896731"><code>61e1df5</code></a> Add Jekyll files to gitignore</li>
<li><a href="https://github.com/Stuk/jszip/commit/f299cce9b8d9e2be11db997919cf1777167902b7"><code>f299cce</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/Stuk/jszip/issues/852">#852</a> from Stuk/metadata-ts</li>
<li><a href="https://github.com/Stuk/jszip/commit/852887aa9483c552cd88e4eb8c298a475c0f9269"><code>852887a</code></a> Consolidate metadata types and expose OnUpdateCallback</li>
<li><a href="https://github.com/Stuk/jszip/commit/5be00dfd0cc86c948420901e911e2b0fb286f19a"><code>5be00df</code></a> Add sponsorship files</li>
<li><a href="https://github.com/Stuk/jszip/commit/dabe86445ce60705936ad15830c817ccb182e649"><code>dabe864</code></a> Update package-lock for benchmark</li>
<li><a href="https://github.com/Stuk/jszip/commit/cc554dae51d306fe0f188891f33e16cb6d81372d"><code>cc554da</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/Stuk/jszip/issues/841">#841</a> from stevennyman/patch-2</li>
<li><a href="https://github.com/Stuk/jszip/commit/caefbc082d4bed536207fe473819fc91041d4f65"><code>caefbc0</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/Stuk/jszip/issues/834">#834</a> from Stuk/benchmark</li>
<li>Additional commits viewable in <a href="https://github.com/Stuk/jszip/compare/v3.7.1...v3.10.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jszip&package-manager=npm_and_yarn&previous-version=3.7.1&new-version=3.10.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-02 18:08:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2278" class=".btn">#2278</a>
            </td>
            <td>
                <b>
                    Merge Weaver codebase to Cacti
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
        Created At 2023-02-01 03:01:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2277" class=".btn">#2277</a>
            </td>
            <td>
                <b>
                    feat(connector-chia): add plugin implementation #1634
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For #1634 

chia-test-ledger.ts
plugin-ledger-connector-chia.ts
open API


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-30 07:56:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2276" class=".btn">#2276</a>
            </td>
            <td>
                <b>
                    build(deps): bump debug from 4.1.1 to 4.3.1
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
<li>Fixes a ReDOS regression (<a href="https://github-redirect.dependabot.com/debug-js/debug/issues/458">#458</a>) - see <a href="https://github-redirect.dependabot.com/debug-js/debug/issues/797">#797</a> for details.</li>
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
<li>Removed bower.json (<a href="https://github-redirect.dependabot.com/debug-js/debug/issues/602">#602</a>)</li>
<li>Removed .eslintrc (since we've switched to XO)</li>
<li>Removed .coveralls.yml</li>
<li>Removed the build system that was in place for various alternate package managers</li>
<li>Removed the examples folder (<a href="https://github-redirect.dependabot.com/debug-js/debug/issues/650">#650</a>)</li>
<li>Switched to <code>console.debug</code> <strong>in the browser only</strong> when it is available (<a href="https://github-redirect.dependabot.com/debug-js/debug/issues/600">#600</a>)</li>
<li>Copied custom logger to namespace extension (<a href="https://github-redirect.dependabot.com/debug-js/debug/issues/646">#646</a>)</li>
<li>Added issue and pull request templates</li>
<li>Added <code>&quot;engines&quot;</code> key to package.json</li>
<li>Added ability to control <code>selectColor</code> (<a href="https://github-redirect.dependabot.com/debug-js/debug/issues/747">#747</a>)</li>
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
        Created At 2023-01-27 10:25:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2275" class=".btn">#2275</a>
            </td>
            <td>
                <b>
                    build(deps): bump ua-parser-js from 0.7.31 to 0.7.33
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [ua-parser-js](https://github.com/faisalman/ua-parser-js) from 0.7.31 to 0.7.33.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/faisalman/ua-parser-js/blob/master/changelog.md">ua-parser-js's changelog</a>.</em></p>
<blockquote>
<h2>Version 0.7.31 / 1.0.2</h2>
<ul>
<li>Fix OPPO Reno A5 incorrect detection</li>
<li>Fix TypeError Bug</li>
<li>Use AST to extract regexes and verify them with safe-regex</li>
</ul>
<h2>Version 0.7.32 / 1.0.32</h2>
<ul>
<li>Add new browser : DuckDuckGo, Huawei Browser, LinkedIn</li>
<li>Add new OS : HarmonyOS</li>
<li>Add some Huawei models</li>
<li>Add Sharp Aquos TV</li>
<li>Improve detection Xiaomi Mi CC9</li>
<li>Fix Sony Xperia 1 III misidentified as Acer tablet</li>
<li>Fix Detect Sony BRAVIA as SmartTV</li>
<li>Fix Detect Xiaomi Mi TV as SmartTV</li>
<li>Fix Detect Galaxy Tab S8 as tablet</li>
<li>Fix WeGame mistakenly identified as WeChat</li>
<li>Fix included commas in Safari / Mobile Safari version</li>
<li>Increase UA_MAX_LENGTH to 350</li>
</ul>
<h2>Version 0.7.33 / 1.0.33</h2>
<ul>
<li>Add new browser : Cobalt</li>
<li>Identify Macintosh as an Apple device</li>
<li>Fix ReDoS vulnerability</li>
</ul>
<h1>Version 0.8</h1>
<p>Version 0.8 was created by accident. This version is now deprecated and no longer maintained, please update to version 0.7 / 1.0.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/f2d0db001d87da15de7b9b1df7be9f2eacefd8c5"><code>f2d0db0</code></a> Bump version 0.7.33</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/a6140a17dd0300a35cfc9cff999545f267889411"><code>a6140a1</code></a> Remove unsafe regex in trim() function</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/a88660493568d6144a551424a8139d6c876635f6"><code>a886604</code></a> Fix <a href="https://github-redirect.dependabot.com/faisalman/ua-parser-js/issues/605">#605</a> - Identify Macintosh as Apple device</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/b814bcd79198e730936c82462e2d729eb5423e3c"><code>b814bcd</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/faisalman/ua-parser-js/issues/606">#606</a> from rileyjshaw/patch-1</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/7f71024161399b7aa5d5cd10dba9e059f0218262"><code>7f71024</code></a> Fix documentation</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/c239ac5167abd574a635cb809a2b4fa35810d23b"><code>c239ac5</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/faisalman/ua-parser-js/issues/604">#604</a> from obecerra3/master</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/8d3c2d327cf540ff2c050f1cc67bca8c6f8e4458"><code>8d3c2d3</code></a> Add new browser: Cobalt</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/d11fc47dc9b6acc0f89fc10c120cea08e10cd31a"><code>d11fc47</code></a> Bump version 0.7.32</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/b490110109de586deab96c775c9ef0dfc9c919c4"><code>b490110</code></a> Merge branch 'develop' of github.com:faisalman/ua-parser-js</li>
<li><a href="https://github.com/faisalman/ua-parser-js/commit/cb5da5ea4b220d5b60fe209e123b7f911d8e0d4a"><code>cb5da5e</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/faisalman/ua-parser-js/issues/600">#600</a> from moekm/develop</li>
<li>Additional commits viewable in <a href="https://github.com/faisalman/ua-parser-js/compare/0.7.31...0.7.33">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ua-parser-js&package-manager=npm_and_yarn&previous-version=0.7.31&new-version=0.7.33)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-01-27 09:32:01 +0000 UTC
    </div>
</div>

