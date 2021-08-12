---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2929" class=".btn">#2929</a>
            </td>
            <td>
                <b>
                    feat: WACI holder APIs for vcwallet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Implemented Universal wallet interfaces discussed in
https://github.com/w3c-ccg/universal-wallet-interop-spec/issues/99
- Added bindings for SDK, REST, JS
- Closes #2928
- Part of #2433

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 15:24:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2927" class=".btn">#2927</a>
            </td>
            <td>
                <b>
                    docs: JSON-LD Context API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #2895

Signed-off-by: Andriy Holovko <andriy.holovko@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 13:58:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2926" class=".btn">#2926</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.50.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.50.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
<h2>v5.50.0</h2>
<h1>Features</h1>
<ul>
<li>hashbangs (<code>#! ...</code>) are now handled by webpack
<ul>
<li><a href="https://github.com/tc39/proposal-hashbang">https://github.com/tc39/proposal-hashbang</a></li>
</ul>
</li>
</ul>
<h1>Performance</h1>
<ul>
<li>disable cache compression by default as it tend to make performance worse
<ul>
<li>I could still be enabled again for specific scenarios</li>
</ul>
</li>
<li>reduce the number of allocations during cache serialization
<ul>
<li>This improves performance and memory usage</li>
</ul>
</li>
</ul>
<h2>v5.49.0</h2>
<h1>Features</h1>
<ul>
<li>add <code>experiments.buildHttp</code> to build <code>http(s)://</code> imports instead of keeping them external
<ul>
<li>keeps a <code>webpack.lock</code> file with integrity and <code>webpack.lock.data</code> with cached content that should be committed</li>
<li>Automatically upgrades lockfile during development when remote resources change
(might be disabled with <code>experiments.buildHttp.upgrade: false</code>)</li>
<li>Lockfile is frozen during production builds and usually no network requests are made
(exception: <code>Cache-Control: no-cache</code>).</li>
<li>The <code>webpack.lock.data</code> persisting can be disabled with <code>experiments.buildHttp.cacheLocation: false</code>.
That will will introduce a availability risk.
(webpack cache will be used to cache network responses)</li>
</ul>
</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>fix HMR infinite loop (again)</li>
<li>fix rare non-determinism with <code>splitChunks.maxSize</code> introduces in the last release</li>
<li>optional modules no longer cause the module to fail when <code>bail</code> is set</li>
<li>fix typo in records format: chunkHashs -&gt; chunkHashes</li>
</ul>
<h1>Performance</h1>
<ul>
<li>limit the number of parallel generated chunks for memory reasons</li>
</ul>
<h2>v5.48.0</h2>
<h1>Features</h1>
<ul>
<li>enable import assertions again</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>upgrade webpack-sources for fixes regarding source maps</li>
<li>fix infinite loop in HMR runtime code</li>
</ul>
<h2>v5.47.1</h2>
<h1>Bugfixes</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/400a0f94ab45ca20b10f219c8311e87d3d3f108c"><code>400a0f9</code></a> 5.50.0</li>
<li><a href="https://github.com/webpack/webpack/commit/7a032c0444894f2e1cb7958edc3deaf07b0e7fb6"><code>7a032c0</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13963">#13963</a> from webpack/perf/serialization</li>
<li><a href="https://github.com/webpack/webpack/commit/db9b2df6cdb33377ef8d832563522c926d12d4e6"><code>db9b2df</code></a> improve allocations needed in serialization</li>
<li><a href="https://github.com/webpack/webpack/commit/edfea41cfd46dfec8791b8e6fe99171d785f15fb"><code>edfea41</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13830">#13830</a> from webpack/dependabot/npm_and_yarn/babel/core-7.14.8</li>
<li><a href="https://github.com/webpack/webpack/commit/e2092010a6208ce4eb73c5814e0d1b0671155523"><code>e209201</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13864">#13864</a> from webpack/dependabot/npm_and_yarn/date-fns-2.23.0</li>
<li><a href="https://github.com/webpack/webpack/commit/856d3d220e50d99932698bfe1974c22f58956bc9"><code>856d3d2</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13904">#13904</a> from webpack/dependabot/npm_and_yarn/simple-git-2.42.0</li>
<li><a href="https://github.com/webpack/webpack/commit/a402d2002a8c84a4470fe3d9c0554981b0d0db38"><code>a402d20</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13882">#13882</a> from webpack/dependabot/npm_and_yarn/mime-types-2.1.32</li>
<li><a href="https://github.com/webpack/webpack/commit/648c8e3340996e338583a3109ffb4d5b8533c085"><code>648c8e3</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13939">#13939</a> from webpack/dependabot/npm_and_yarn/graceful-fs-4.2.8</li>
<li><a href="https://github.com/webpack/webpack/commit/d4410dbac82875e6c19dd47f35343bdb9203bb7f"><code>d4410db</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13919">#13919</a> from webpack/dependabot/npm_and_yarn/browserslist-4...</li>
<li><a href="https://github.com/webpack/webpack/commit/dbac9547564b3757fa7bc631263e938dc16eb436"><code>dbac954</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13906">#13906</a> from webpack/dependabot/npm_and_yarn/eslint-7.32.0</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.50.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.50.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 08:14:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2924" class=".btn">#2924</a>
            </td>
            <td>
                <b>
                    test: Additional common storage tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 15:05:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2923" class=".btn">#2923</a>
            </td>
            <td>
                <b>
                    feat: client for JSON-LD context API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #2912

Signed-off-by: Andriy Holovko <andriy.holovko@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 11:08:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2922" class=".btn">#2922</a>
            </td>
            <td>
                <b>
                    refactor: move jwk to its own package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">chore</span><span class="chip">refactor</span>
            </td>
            <td>
                To avoid cyclic dependency with did:key creation from kms keys, the jwk api needs to be in its own subpackage.

closes #2921

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-09 21:07:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2920" class=".btn">#2920</a>
            </td>
            <td>
                <b>
                    fix: schema uri matching handles IRIs expanded in nested contexts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-09 16:36:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2919" class=".btn">#2919</a>
            </td>
            <td>
                <b>
                    chore: Update storage implementations to pass new common tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-09 03:02:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2916" class=".btn">#2916</a>
            </td>
            <td>
                <b>
                    test: Updates and improvements to storage test suite
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Added new tests to ensure correct behaviour for the Store.Batch and Store.Close methods per the recently updated interface documentation.
- Added close calls for all of the stores that get created in the tests. This is important for storage implementations that maintain connections to databases. By closing these stores after each test, those implementations should be able to safely call TestAll without exhausting the connection limit and causing test failures.
- Updated storage implementations (as needed) to pass the new tests.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-06 21:17:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2915" class=".btn">#2915</a>
            </td>
            <td>
                <b>
                    docs: Update storage interface documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updated documentation to specify what happens in certain cases:

Batch: If the operations slice is empty or nil, an error is returned.
Close: It can be called repeatedly on the same store multiple times without causing an error.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-06 20:44:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2914" class=".btn">#2914</a>
            </td>
            <td>
                <b>
                    switch remote kms logs from info to debug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">chore</span>
            </td>
            <td>
                closes #2913

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-06 20:19:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2911" class=".btn">#2911</a>
            </td>
            <td>
                <b>
                    chore(deps): bump actions/setup-node from 2.3.0 to 2.4.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/setup-node](https://github.com/actions/setup-node) from 2.3.0 to 2.4.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/setup-node/releases">actions/setup-node's releases</a>.</em></p>
<blockquote>
<h2>Support caching for mono repos and repositories with complex structure</h2>
<p>This release introduces dependency caching support for mono repos and repositories with complex structure (<a href="https://github-redirect.dependabot.com/actions/setup-node/issues/305">#305</a>).</p>
<p>By default, the action searches for the dependency file (<code>package-lock.json</code> or <code>yarn.lock</code>) in the repository root. Use the <code>cache-dependency-path</code> input for cases when multiple dependency files are used, or they are located in different subdirectories. This input supports wildcards or a list of file names for caching multiple dependencies.</p>
<p>Yaml example:</p>
<pre lang="yml"><code>steps:
- uses: actions/checkout@v2
- uses: actions/setup-node@v2
  with:
    node-version: 14
    cache: npm
    cache-dependency-path: 'sub-project/package-lock.json'
</code></pre>
<p>For more examples of using <code>cache-dependency-path</code> input, see the <a href="https://github.com/actions/setup-node/blob/25316bbc1f10ac9d8798711f44914b1cf3c4e954/docs/advanced-usage.md#caching-packages-dependencies">Advanced usage</a> guide.</p>
<h2>Revert temporary fix</h2>
<p>We had to disable pre-cached Node.js usage in the previous version due to the broken image cache. Now cache is fixed, so we can safely enable its usage again.
Thank you for understanding.</p>
<h2>Temporary maintenance fix.</h2>
<p>Temporarily disabled usage of pre-cached Node.js.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/setup-node/commit/25316bbc1f10ac9d8798711f44914b1cf3c4e954"><code>25316bb</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/305">#305</a> from MaksimZhukov/mazhuk/adding-support-for-monorepos</li>
<li><a href="https://github.com/actions/setup-node/commit/76a4cff9ae9abd877db3173c31637296d870a25b"><code>76a4cff</code></a> update readme and dist files</li>
<li><a href="https://github.com/actions/setup-node/commit/a869e7cc2db593443fe4273b3566c2446337c3d1"><code>a869e7c</code></a> Merge branch 'main' of <a href="https://github.com/MaksimZhukov/setup-node">https://github.com/MaksimZhukov/setup-node</a> into mazhuk...</li>
<li><a href="https://github.com/actions/setup-node/commit/a0cdab1110ea1f0f4fb59851ef15f68231289f7b"><code>a0cdab1</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/299">#299</a> from actions/malob/adr-caching-monorepos</li>
<li><a href="https://github.com/actions/setup-node/commit/4d0182af5ead0b7bf53e87e49aa959476f5501d3"><code>4d0182a</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/310">#310</a> from actions/revert-308-v-alsvir/disable-cache-usage-...</li>
<li><a href="https://github.com/actions/setup-node/commit/896ee80599ea831592cc8484629043410040b226"><code>896ee80</code></a> Restore YARN flag</li>
<li><a href="https://github.com/actions/setup-node/commit/d21ecc7c5be116ff576d1e1dd67cf7eefbb22ed3"><code>d21ecc7</code></a> Revert &quot;Temporarily disabled cache usage for v2&quot;</li>
<li><a href="https://github.com/actions/setup-node/commit/d6e3b5539ed7e5ccd26c3459e26c7c817f4e9068"><code>d6e3b55</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/setup-node/issues/308">#308</a> from actions/v-alsvir/disable-cache-usage-temp-v2</li>
<li><a href="https://github.com/actions/setup-node/commit/db716f881ae727ff1c231028cc3926681f7d2e7b"><code>db716f8</code></a> Add yarn env variable</li>
<li><a href="https://github.com/actions/setup-node/commit/c24389f79e91ba615d93590929027ff3d63575ae"><code>c24389f</code></a> Staging unstaged</li>
<li>Additional commits viewable in <a href="https://github.com/actions/setup-node/compare/v2.3.0...v2.4.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/setup-node&package-manager=github_actions&previous-version=2.3.0&new-version=2.4.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-06 08:19:02 +0000 UTC
    </div>
</div>

