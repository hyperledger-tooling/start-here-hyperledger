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
                PR <a href="https://github.com/hyperledger/cacti/pull/2319" class=".btn">#2319</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump webpack from 5.50.0 to 5.76.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 5.50.0 to 5.76.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
<h2>v5.76.0</h2>
<h2>Bugfixes</h2>
<ul>
<li>Avoid cross-realm object access by <a href="https://github.com/Jack-Works"><code>@​Jack-Works</code></a> in <a href="https://redirect.github.com/webpack/webpack/pull/16500">webpack/webpack#16500</a></li>
<li>Improve hash performance via conditional initialization by <a href="https://github.com/lvivski"><code>@​lvivski</code></a> in <a href="https://redirect.github.com/webpack/webpack/pull/16491">webpack/webpack#16491</a></li>
<li>Serialize <code>generatedCode</code> info to fix bug in asset module cache restoration by <a href="https://github.com/ryanwilsonperkin"><code>@​ryanwilsonperkin</code></a> in <a href="https://redirect.github.com/webpack/webpack/pull/16703">webpack/webpack#16703</a></li>
<li>Improve performance of <code>hashRegExp</code> lookup by <a href="https://github.com/ryanwilsonperkin"><code>@​ryanwilsonperkin</code></a> in <a href="https://redirect.github.com/webpack/webpack/pull/16759">webpack/webpack#16759</a></li>
</ul>
<h2>Features</h2>
<ul>
<li>add <code>target</code> to <code>LoaderContext</code> type by <a href="https://github.com/askoufis"><code>@​askoufis</code></a> in <a href="https://redirect.github.com/webpack/webpack/pull/16781">webpack/webpack#16781</a></li>
</ul>
<h2>Security</h2>
<ul>
<li><a href="https://github.com/advisories/GHSA-3rfm-jhwj-7488">CVE-2022-37603</a> fixed by <a href="https://github.com/akhilgkrishnan"><code>@​akhilgkrishnan</code></a> in <a href="https://redirect.github.com/webpack/webpack/pull/16446">webpack/webpack#16446</a></li>
</ul>
<h2>Repo Changes</h2>
<ul>
<li>Fix HTML5 logo in README by <a href="https://github.com/jakebailey"><code>@​jakebailey</code></a> in <a href="https://redirect.github.com/webpack/webpack/pull/16614">webpack/webpack#16614</a></li>
<li>Replace TypeScript logo in README by <a href="https://github.com/jakebailey"><code>@​jakebailey</code></a> in <a href="https://redirect.github.com/webpack/webpack/pull/16613">webpack/webpack#16613</a></li>
<li>Update actions/cache dependencies by <a href="https://github.com/piwysocki"><code>@​piwysocki</code></a> in <a href="https://redirect.github.com/webpack/webpack/pull/16493">webpack/webpack#16493</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/Jack-Works"><code>@​Jack-Works</code></a> made their first contribution in <a href="https://redirect.github.com/webpack/webpack/pull/16500">webpack/webpack#16500</a></li>
<li><a href="https://github.com/lvivski"><code>@​lvivski</code></a> made their first contribution in <a href="https://redirect.github.com/webpack/webpack/pull/16491">webpack/webpack#16491</a></li>
<li><a href="https://github.com/jakebailey"><code>@​jakebailey</code></a> made their first contribution in <a href="https://redirect.github.com/webpack/webpack/pull/16614">webpack/webpack#16614</a></li>
<li><a href="https://github.com/akhilgkrishnan"><code>@​akhilgkrishnan</code></a> made their first contribution in <a href="https://redirect.github.com/webpack/webpack/pull/16446">webpack/webpack#16446</a></li>
<li><a href="https://github.com/ryanwilsonperkin"><code>@​ryanwilsonperkin</code></a> made their first contribution in <a href="https://redirect.github.com/webpack/webpack/pull/16703">webpack/webpack#16703</a></li>
<li><a href="https://github.com/piwysocki"><code>@​piwysocki</code></a> made their first contribution in <a href="https://redirect.github.com/webpack/webpack/pull/16493">webpack/webpack#16493</a></li>
<li><a href="https://github.com/askoufis"><code>@​askoufis</code></a> made their first contribution in <a href="https://redirect.github.com/webpack/webpack/pull/16781">webpack/webpack#16781</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/webpack/webpack/compare/v5.75.0...v5.76.0">https://github.com/webpack/webpack/compare/v5.75.0...v5.76.0</a></p>
<h2>v5.75.0</h2>
<h1>Bugfixes</h1>
<ul>
<li><code>experiments.*</code> normalize to <code>false</code> when opt-out</li>
<li>avoid <code>NaN%</code></li>
<li>show the correct error when using a conflicting chunk name in code</li>
<li>HMR code tests existance of <code>window</code> before trying to access it</li>
<li>fix <code>eval-nosources-*</code> actually exclude sources</li>
<li>fix race condition where no module is returned from processing module</li>
<li>fix position of standalong semicolon in runtime code</li>
</ul>
<h1>Features</h1>
<ul>
<li>add support for <code>@import</code> to extenal CSS when using experimental CSS in node</li>
<li>add <code>i64</code> support to the deprecated WASM implementation</li>
</ul>
<h1>Developer Experience</h1>
<ul>
<li>expose <code>EnableWasmLoadingPlugin</code></li>
<li>add more typings</li>
<li>generate getters instead of readonly properties in typings to allow overriding them</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/97b1718720c33f1b17302a74c5284b01e02ec001"><code>97b1718</code></a> Merge pull request <a href="https://redirect.github.com/webpack/webpack/issues/16781">#16781</a> from askoufis/loader-context-target-type</li>
<li><a href="https://github.com/webpack/webpack/commit/b84efe6224b276bf72e4c5e2f4e76acddfaeef07"><code>b84efe6</code></a> Merge pull request <a href="https://redirect.github.com/webpack/webpack/issues/16759">#16759</a> from ryanwilsonperkin/real-content-hash-regex-perf</li>
<li><a href="https://github.com/webpack/webpack/commit/c98e9e001441b165c7ed4845700839730b505833"><code>c98e9e0</code></a> Merge pull request <a href="https://redirect.github.com/webpack/webpack/issues/16493">#16493</a> from piwysocki/patch-1</li>
<li><a href="https://github.com/webpack/webpack/commit/5f34acfbc074da6cc09f48944d7f2b4273ffb3f8"><code>5f34acf</code></a> feat: Add <code>target</code> to <code>LoaderContext</code> type</li>
<li><a href="https://github.com/webpack/webpack/commit/b7fc4d876deb958d7ee81ecc00a312e39a354a44"><code>b7fc4d8</code></a> Merge pull request <a href="https://redirect.github.com/webpack/webpack/issues/16703">#16703</a> from ryanwilsonperkin/ryanwilsonperkin/fix-16160</li>
<li><a href="https://github.com/webpack/webpack/commit/63ea82da4d4e4242b6a6285fc937f0684f264fe8"><code>63ea82d</code></a> Merge branch 'webpack:main' into patch-1</li>
<li><a href="https://github.com/webpack/webpack/commit/4ba225225b1348c8776ca5b5fe53468519413bc0"><code>4ba2252</code></a> Merge pull request <a href="https://redirect.github.com/webpack/webpack/issues/16446">#16446</a> from akhilgkrishnan/patch-1</li>
<li><a href="https://github.com/webpack/webpack/commit/1acd6350be3d74d4ac70b64cbbc60f27724b618b"><code>1acd635</code></a> Merge pull request <a href="https://redirect.github.com/webpack/webpack/issues/16613">#16613</a> from jakebailey/ts-logo</li>
<li><a href="https://github.com/webpack/webpack/commit/302eb37fe19ed7ca60eaf895aca4f9da9dfd7931"><code>302eb37</code></a> Merge pull request <a href="https://redirect.github.com/webpack/webpack/issues/16614">#16614</a> from jakebailey/html5-logo</li>
<li><a href="https://github.com/webpack/webpack/commit/cfdb1dfe59b33bf7441b8a8e4fc58d75e4f54cee"><code>cfdb1df</code></a> Improve performance of hashRegExp lookup</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v5.50.0...v5.76.0">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~evilebottnawi">evilebottnawi</a>, a new releaser for webpack since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=5.50.0&new-version=5.76.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-03-14 17:07:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2318" class=".btn">#2318</a>
            </td>
            <td>
                <b>
                    build(yarn): migrate to CorePack
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2238

Signed-off-by: charellesandig [charelle.wrk@gmail.com](mailto:charelle.wrk@gmail.com)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 09:52:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2316" class=".btn">#2316</a>
            </td>
            <td>
                <b>
                    build(deps): bump sqlite3 from 5.0.3 to 5.1.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [sqlite3](https://github.com/TryGhost/node-sqlite3) from 5.0.3 to 5.1.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/TryGhost/node-sqlite3/releases">sqlite3's releases</a>.</em></p>
<blockquote>
<h2>v5.1.5</h2>
<h2>What's Changed</h2>
<ul>
<li>🔒 Fixed code execution vulnerability due to Object coercion by <a href="https://github.com/daniellockyer"><code>@​daniellockyer</code></a></li>
<li>Updated bundled SQLite to v3.41.1 by <a href="https://github.com/daniellockyer"><code>@​daniellockyer</code></a></li>
<li>Fixed rpath linker option when using a custom sqlite by <a href="https://github.com/jeromew"><code>@​jeromew</code></a> in <a href="https://redirect.github.com/TryGhost/node-sqlite3/pull/1654">TryGhost/node-sqlite3#1654</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/TryGhost/node-sqlite3/compare/v5.1.4...v5.1.5">https://github.com/TryGhost/node-sqlite3/compare/v5.1.4...v5.1.5</a></p>
<h2>v5.1.4</h2>
<h2>What's Changed</h2>
<ul>
<li>Fixed glibc compatibility by downgrading CI to Ubuntu 20 by <a href="https://github.com/daniellockyer"><code>@​daniellockyer</code></a> in <a href="https://redirect.github.com/TryGhost/node-sqlite3/pull/1664">TryGhost/node-sqlite3#1664</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/TryGhost/node-sqlite3/compare/v5.1.3...v5.1.4">https://github.com/TryGhost/node-sqlite3/compare/v5.1.3...v5.1.4</a></p>
<h2>v5.1.3</h2>
<h2>What's Changed</h2>
<ul>
<li>Updated bundled SQLite to v3.40.0 by <a href="https://github.com/daniellockyer"><code>@​daniellockyer</code></a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/TryGhost/node-sqlite3/compare/v5.1.2...v5.1.3">https://github.com/TryGhost/node-sqlite3/compare/v5.1.2...v5.1.3</a></p>
<h2>v5.1.2</h2>
<h2>What's Changed</h2>
<ul>
<li>Updated bundled SQLite to v3.39.4 by <a href="https://github.com/daniellockyer"><code>@​daniellockyer</code></a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/TryGhost/node-sqlite3/compare/v5.1.1...v5.1.2">https://github.com/TryGhost/node-sqlite3/compare/v5.1.1...v5.1.2</a></p>
<h2>v5.1.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Added Darwin ARM64 binaries by <a href="https://github.com/daniellockyer"><code>@​daniellockyer</code></a> in <a href="https://redirect.github.com/TryGhost/node-sqlite3/pull/1594">TryGhost/node-sqlite3#1594</a></li>
</ul>
<p>A huge thanks to <a href="https://www.macstadium.com/">MacStadium</a> for providing an M1 Mac Mini so we can offer ARM64 binaries.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/TryGhost/node-sqlite3/compare/v5.1.0...v5.1.1">https://github.com/TryGhost/node-sqlite3/compare/v5.1.0...v5.1.1</a></p>
<h2>v5.1.0</h2>
<p>✨ We're very excited to announce node-sqlite3's first minor release of v5, packed with features and improvements.</p>
<p>If you encounter any problems, please open a detailed issue using the <a href="https://github.com/TryGhost/node-sqlite3/issues/new/choose">templates</a>.</p>
<h2>What's Changed</h2>
<ul>
<li>Updated bundled SQLite to v3.39.3 by <a href="https://github.com/daniellockyer"><code>@​daniellockyer</code></a></li>
<li>Added ability to receive updates from <code>sqlite3_update_hook</code> by <a href="https://github.com/soukand"><code>@​soukand</code></a> in <a href="https://redirect.github.com/TryGhost/node-sqlite3/pull/1267">TryGhost/node-sqlite3#1267</a></li>
<li>Added support for setting SQLite limits by <a href="https://github.com/paulfitz"><code>@​paulfitz</code></a> in <a href="https://redirect.github.com/TryGhost/node-sqlite3/pull/1548">TryGhost/node-sqlite3#1548</a></li>
<li>Added library types file by <a href="https://github.com/bpasero"><code>@​bpasero</code></a> in <a href="https://redirect.github.com/TryGhost/node-sqlite3/pull/1527">TryGhost/node-sqlite3#1527</a></li>
<li>Added <code>package-lock.json</code> to <code>.gitignore</code> by <a href="https://github.com/JoelEinbinder"><code>@​JoelEinbinder</code></a> in <a href="https://redirect.github.com/TryGhost/node-sqlite3/pull/1628">TryGhost/node-sqlite3#1628</a></li>
<li>Fixed remaining method declarations by <a href="https://github.com/alexanderfloh"><code>@​alexanderfloh</code></a> in <a href="https://redirect.github.com/TryGhost/node-sqlite3/pull/1633">TryGhost/node-sqlite3#1633</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/TryGhost/node-sqlite3/commit/6a806f87903d778d520bce09f6e893752619383b"><code>6a806f8</code></a> v5.1.5</li>
<li><a href="https://github.com/TryGhost/node-sqlite3/commit/edb1934dd222ae55632e120d8f64552d5191c781"><code>edb1934</code></a> Fixed code execution vulnerability due to Object coercion</li>
<li><a href="https://github.com/TryGhost/node-sqlite3/commit/3a4888894dd0e0463d3bf4dc833fdcc995b614af"><code>3a48888</code></a> Updated bundled SQLite to v3.41.1</li>
<li><a href="https://github.com/TryGhost/node-sqlite3/commit/c1440bdaa47ffdda852ff576ac543114c4f0fb4b"><code>c1440bd</code></a> Fixed rpath linker option when using a custom sqlite (<a href="https://redirect.github.com/TryGhost/node-sqlite3/issues/1654">#1654</a>)</li>
<li><a href="https://github.com/TryGhost/node-sqlite3/commit/93affa425958f479150b699f08eb67af3e5b522c"><code>93affa4</code></a> Update microsoft/setup-msbuild action to v1.3</li>
<li><a href="https://github.com/TryGhost/node-sqlite3/commit/6f6318e929367ae05f395c5e0e5e4b09c62e87f4"><code>6f6318e</code></a> v5.1.4</li>
<li><a href="https://github.com/TryGhost/node-sqlite3/commit/aeafe2591d664fcf6c70e7ddadc7875c8f691a4d"><code>aeafe25</code></a> Revert &quot;Renamed <code>master</code> references to <code>main</code>&quot;</li>
<li><a href="https://github.com/TryGhost/node-sqlite3/commit/57ce2d4519d0fe1c801081389d20cc7f357cdc02"><code>57ce2d4</code></a> Fixed glib compatibility by downgrading to Ubuntu 20</li>
<li><a href="https://github.com/TryGhost/node-sqlite3/commit/af8e567f25f9da7e0c14f90ede688efe56486ce4"><code>af8e567</code></a> Renamed <code>master</code> references to <code>main</code></li>
<li><a href="https://github.com/TryGhost/node-sqlite3/commit/8fd18a392c4844288811330dddfcf171c18ed93f"><code>8fd18a3</code></a> Extracted function checking code into macro</li>
<li>Additional commits viewable in <a href="https://github.com/TryGhost/node-sqlite3/compare/v5.0.3...v5.1.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=sqlite3&package-manager=npm_and_yarn&previous-version=5.0.3&new-version=5.1.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-03-13 21:47:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2313" class=".btn">#2313</a>
            </td>
            <td>
                <b>
                    chore: adding custom gitguardian check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                related to #720

this includes gitguardian workflow + configuration file
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-10 03:29:22 +0000 UTC
    </div>
</div>

