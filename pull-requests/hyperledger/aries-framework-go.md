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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2917" class=".btn">#2917</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.49.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.49.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
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
<ul>
<li>upgrade webpack-sources for a bunch of bugfixes regarding source maps and missing chars in output</li>
</ul>
<h2>v5.47.0</h2>
<h1>Performance</h1>
<ul>
<li>improve source-map performance</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>avoid unnecessary <code>&quot;use strict&quot;</code>s in module mode</li>
</ul>
<h2>v5.46.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/d3868384c37f9d674d1db17a0198393bd213c763"><code>d386838</code></a> 5.49.0</li>
<li><a href="https://github.com/webpack/webpack/commit/150d370a2f682e0f549f331b38656ec4d577125e"><code>150d370</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13918">#13918</a> from privatenumber/hashes-typo</li>
<li><a href="https://github.com/webpack/webpack/commit/f8acab3f3b8708ba577c3e13b88ca12ade277f43"><code>f8acab3</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13944">#13944</a> from webpack/bugfix/11594</li>
<li><a href="https://github.com/webpack/webpack/commit/9e735a77e1de3e096f2927b1ab9f709c5ac9e183"><code>9e735a7</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13943">#13943</a> from webpack/bugfix/split-chunks-max-size-determini...</li>
<li><a href="https://github.com/webpack/webpack/commit/c6856e220446beb34feb449303f427f9cfcc252e"><code>c6856e2</code></a> optional modules will not fail the build when bail is set</li>
<li><a href="https://github.com/webpack/webpack/commit/0605b887c990099b391af304c9b8074fbc4787af"><code>0605b88</code></a> fix indeterminism with splitChunks.maxSize</li>
<li><a href="https://github.com/webpack/webpack/commit/a6e9f59dfc903b2e7ff947b524a9df646ef4e585"><code>a6e9f59</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13932">#13932</a> from webpack/bugfix/infinite-loop</li>
<li><a href="https://github.com/webpack/webpack/commit/d77d8636015ae71195b16b39dd0e6daebdcace83"><code>d77d863</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13925">#13925</a> from webpack/feature/http-urls</li>
<li><a href="https://github.com/webpack/webpack/commit/9bf67974167982435981b2d03f5cd9f4848408d4"><code>9bf6797</code></a> fix resolving context for redirects</li>
<li><a href="https://github.com/webpack/webpack/commit/30ebedd4ddf624bb5d5b7f8de2a8943a1c35ee2f"><code>30ebedd</code></a> fix handling of new URL() in remote resources</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.49.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.49.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-08-07 01:23:21 +0000 UTC
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2909" class=".btn">#2909</a>
            </td>
            <td>
                <b>
                    fix: Fixes DIDs resolution when inbound message received.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrii Soluk <isoluchok@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-05 06:38:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2908" class=".btn">#2908</a>
            </td>
            <td>
                <b>
                    chore(deps): bump tar from 6.1.0 to 6.1.6 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [tar](https://github.com/npm/node-tar) from 6.1.0 to 6.1.6.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/node-tar/commit/9bc1729939eec1c822b528385b1cc513b9888835"><code>9bc1729</code></a> 6.1.6</li>
<li><a href="https://github.com/npm/node-tar/commit/bdf4f5171340b890a62a5e578962ac143d34b3a9"><code>bdf4f51</code></a> fix: properly prefix hard links</li>
<li><a href="https://github.com/npm/node-tar/commit/94b2a740115fdce20f265a029b0404d53c0a18c6"><code>94b2a74</code></a> chore: remove benchmarks from git repo</li>
<li><a href="https://github.com/npm/node-tar/commit/ecaafb4777b7137421f2f0d6f40ab827654f9247"><code>ecaafb4</code></a> update deps</li>
<li><a href="https://github.com/npm/node-tar/commit/bd4691c90478f41b2649a97048199e34927dc046"><code>bd4691c</code></a> 6.1.5</li>
<li><a href="https://github.com/npm/node-tar/commit/d694c4f810d864badf223efa35d24a000d780179"><code>d694c4f</code></a> ci: test on node 16</li>
<li><a href="https://github.com/npm/node-tar/commit/84acbd31288541100910a528e437f901f8012214"><code>84acbd3</code></a> fix(unpack): fix hang on large file on open() fail</li>
<li><a href="https://github.com/npm/node-tar/commit/97c46fcee7e4e7849ea3432086c4537fb6197025"><code>97c46fc</code></a> fix(unpack): always resume parsing after an entry error</li>
<li><a href="https://github.com/npm/node-tar/commit/488ab8c01de69379406d937419fa3e5550e651c0"><code>488ab8c</code></a> chore: WriteEntry cleaner write() handling</li>
<li><a href="https://github.com/npm/node-tar/commit/be89aafd95296e9721e124b77eee7c745e1c1e97"><code>be89aaf</code></a> WriteEntry backpressure</li>
<li>Additional commits viewable in <a href="https://github.com/npm/node-tar/compare/v6.1.0...v6.1.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tar&package-manager=npm_and_yarn&previous-version=6.1.0&new-version=6.1.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-go/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-04 19:37:17 +0000 UTC
    </div>
</div>

