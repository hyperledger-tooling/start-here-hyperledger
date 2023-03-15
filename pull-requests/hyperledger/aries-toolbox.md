---
layout: default
title: aries-toolbox
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-toolbox
---

# aries-toolbox <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-toolbox){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-toolbox/pull/307" class=".btn">#307</a>
            </td>
            <td>
                <b>
                    Merge dependabot commits
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Merged as many of the dependabot commits as I could while still allowing the toolbox to build. The remaining commits failed to build.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 22:18:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-toolbox/pull/306" class=".btn">#306</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump webpack from 5.68.0 to 5.76.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 5.68.0 to 5.76.0.
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
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v5.68.0...v5.76.0">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~evilebottnawi">evilebottnawi</a>, a new releaser for webpack since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=5.68.0&new-version=5.76.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-toolbox/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 20:49:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-toolbox/pull/305" class=".btn">#305</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump terser from 5.10.0 to 5.16.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [terser](https://github.com/terser/terser) from 5.10.0 to 5.16.6.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/terser/terser/blob/master/CHANGELOG.md">terser's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<h2>v5.16.7</h2>
<ul>
<li>Become less conservative with analyzing function definitions for <code>reduce_vars</code></li>
<li>Parse <code>import.meta</code> as a real AST node and not an <code>object.property</code></li>
</ul>
<h2>v5.16.5</h2>
<ul>
<li>Correctly handle AST transform functions that mutate children arrays</li>
<li>Don't mutate the options object passed to Terser (<a href="https://redirect.github.com/terser/terser/issues/1342">#1342</a>)</li>
<li>Do not treat BigInt like a number</li>
</ul>
<h2>v5.16.4</h2>
<ul>
<li>Keep <code>(defaultArg = undefined) =&gt; ...</code>, because default args don't count for function length</li>
<li>Prevent inlining variables into <code>?.</code> optional chains</li>
<li>Avoid removing unused arguments while transforming</li>
<li>Optimize iterating AST node lists</li>
<li>Make sure <code>catch</code> and <code>finally</code> aren't children of <code>try</code> in the AST</li>
<li>Use modern unicode property escapes (<code>\p{...}</code>) to parse identifiers when available</li>
</ul>
<h2>v5.16.3</h2>
<ul>
<li>Ensure function definitions, don't assume the values of variables defined after them.</li>
</ul>
<h2>v5.16.2</h2>
<ul>
<li>Fix sourcemaps with non-ascii characters (<a href="https://redirect.github.com/terser/terser/issues/1318">#1318</a>)</li>
<li>Support string module name and export * as (<a href="https://redirect.github.com/terser/terser/issues/1336">#1336</a>)</li>
<li>Do not move <code>let</code> out of <code>for</code> initializers, as it can change scoping</li>
<li>Fix a corner case that would generate the invalid syntax <code>if (something) let x</code> (&quot;let&quot; in braceless if body)</li>
<li>Knowledge of more native object properties (<a href="https://redirect.github.com/terser/terser/issues/1330">#1330</a>)</li>
<li>Got rid of Travis (<a href="https://redirect.github.com/terser/terser/issues/1323">#1323</a>)</li>
<li>Added semi-secret <code>asObject</code> sourcemap option to typescript defs (<a href="https://redirect.github.com/terser/terser/issues/1321">#1321</a>)</li>
</ul>
<h2>v5.16.1</h2>
<ul>
<li>Properly handle references in destructurings (<code>const { [reference]: val } = ...</code>)</li>
<li>Allow parsing of <code>.#privatefield</code> in nested classes</li>
<li>Do not evaluate operations that return large strings if that would make the output code larger</li>
<li>Make <code>collapse_vars</code> handle block scope correctly</li>
<li>Internal improvements: Typos (<a href="https://redirect.github.com/terser/terser/issues/1311">#1311</a>), more tests, small-scale refactoring</li>
</ul>
<h2>v5.16.0</h2>
<ul>
<li>Disallow private fields in object bodies (<a href="https://redirect.github.com/terser/terser/issues/1011">#1011</a>)</li>
<li>Parse <code>#privatefield in object</code> (<a href="https://redirect.github.com/terser/terser/issues/1279">#1279</a>)</li>
<li>Compress <code>#privatefield in object</code></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/terser/terser/commit/91176951ec005f0b8f9b5498a33b5763dff7d8ab"><code>9117695</code></a> 5.16.6</li>
<li><a href="https://github.com/terser/terser/commit/96abde59dde46c520ea56aa20bd360a3c30012f3"><code>96abde5</code></a> update changelog</li>
<li><a href="https://github.com/terser/terser/commit/4d6c4f6db38c0de266256bc9834035189fb5a1b3"><code>4d6c4f6</code></a> Fix output increase by walking function definitions first. Closes <a href="https://redirect.github.com/terser/terser/issues/1338">#1338</a> while...</li>
<li><a href="https://github.com/terser/terser/commit/8a1b2400af130369cd4a44be526e5e58fb6cd58f"><code>8a1b240</code></a> Parse import.meta as a special expression. Closes <a href="https://redirect.github.com/terser/terser/issues/1349">#1349</a></li>
<li><a href="https://github.com/terser/terser/commit/c7d844b4a9dbf50c3471d5dd1115445b2ae5ed7a"><code>c7d844b</code></a> 5.16.5</li>
<li><a href="https://github.com/terser/terser/commit/4f447540897ded9be5621a7a19f13dc36e89ec9c"><code>4f44754</code></a> update changelog</li>
<li><a href="https://github.com/terser/terser/commit/324c63d961dea678dfb7eae95dd93dc0f2e0748a"><code>324c63d</code></a> add new test</li>
<li><a href="https://github.com/terser/terser/commit/fa6f16467165730aff45f6165afce33714c32dc8"><code>fa6f164</code></a> don't assume transform functions don't mutate AST arrays. Closes <a href="https://redirect.github.com/terser/terser/issues/1351">#1351</a></li>
<li><a href="https://github.com/terser/terser/commit/3c9fc4c53e325960cd97c6195a9e70a3d93439eb"><code>3c9fc4c</code></a> Don't mutate options object. Fixes <a href="https://redirect.github.com/terser/terser/issues/1341">#1341</a> (<a href="https://redirect.github.com/terser/terser/issues/1342">#1342</a>)</li>
<li><a href="https://github.com/terser/terser/commit/e062dc8ddf661d560d8778a0e408cb5e78360fd8"><code>e062dc8</code></a> Do not mark BigInt <code>is_number</code>. Closes <a href="https://redirect.github.com/terser/terser/issues/1315">#1315</a></li>
<li>Additional commits viewable in <a href="https://github.com/terser/terser/compare/v5.10.0...v5.16.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=terser&package-manager=npm_and_yarn&previous-version=5.10.0&new-version=5.16.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-toolbox/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 19:04:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-toolbox/pull/304" class=".btn">#304</a>
            </td>
            <td>
                <b>
                    update: merge main into dependabot branch, keep up to date
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                update: merge main into dependabot branch, keep up to date
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 18:00:22 +0000 UTC
    </div>
</div>

