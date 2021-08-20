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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2951" class=".btn">#2951</a>
            </td>
            <td>
                <b>
                    docs: Updates to storage interface documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Updated storage interface documentation to specify that some storage providers may require setting the tag name in a store configuration in order to do sorts in queries or get TotalItem counts.

- Added disclaimers to methods in the storage interface to indicate which ones are not currently used in aries-framework-go, but which may be useful for a custom solution. If someone is creating their own storage implementation and only needs it to work in aries-framework-go, this could help save them time.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-19 23:22:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2950" class=".btn">#2950</a>
            </td>
            <td>
                <b>
                    test: Additional common storage tests and new iterator test option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Added new storage tests to ensure that SetStoreConfig and GetStoreConfig are also case-insensitive with respect to the store name.
- Added an option to only check iterator total items counts when a store configuration has been set. This provides a workaround for testing storage providers that don't support getting total item counts without setting a store configuration.
- Removed aries-framework-go/test/component replace directive from aries-js-worker since it causes checks to break when the common test method signatures are updated... and since the indexeddb module lacks a replace, it also can't be updated to have the new method signature in a single commit.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-19 22:17:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2949" class=".btn">#2949</a>
            </td>
            <td>
                <b>
                    feat: Enhancements to LevelDB and IndexedDB storage providers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - LevelDB and IndexedDB storage providers now only create tag maps when needed. This saves space for stores that don't make use of tags+querying.
- Fixed an issue in the IndexedDB storage provider where the GetStoreConfig method doesn't properly convert store names to lowercase, resulting in issues when store names use capital letters.
- Updated storage implementations to use the storage module commits - this includes new common unit tests.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-19 20:46:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2946" class=".btn">#2946</a>
            </td>
            <td>
                <b>
                    test: Add unit tests for storing JSON strings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Bob Stasyszyn <Bob.Stasyszyn@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-19 16:24:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2945" class=".btn">#2945</a>
            </td>
            <td>
                <b>
                    Add support for X25519/Ed25519 keys in fingerprint.CreateDIDKeyByJwk()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                closes #2944

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-19 16:17:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2943" class=".btn">#2943</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.51.1 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.51.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
<h2>v5.51.1</h2>
<h1>Bugfixes</h1>
<ul>
<li><code>library: &quot;module&quot;</code> propages top-level-await correctly</li>
<li>fix crash in filesystem snapshotting when trying to snapshot a non-existing directory</li>
<li>fix some context-dependent logic in concatenated modules and source url handling</li>
</ul>
<h2>v5.51.0</h2>
<h1>Bugfixes</h1>
<ul>
<li>correctly keep chunk loading state when the chunk loading logic is HMR updated
<ul>
<li>This fixes some edge cases that e. g. occur when using lazy compilation for entrypoints. It is now able to HMR update that instead of needing a manual reload. Also see fixes in webpack-dev-server@4.</li>
</ul>
</li>
<li>track and resolve symlinks for filesystem snapshotting
<ul>
<li>This fixes some cases of circular <code>yarn link</code>ing of dependencies.</li>
<li>It also fixes some problems when using package managers that use symlinks to deduplicate (e. g. cnpm or pnpm)</li>
</ul>
</li>
<li>pass the resulting module in the callbacks of <code>Compilation.addModuleChain</code> and <code>Compilation.addModuleTree</code></li>
</ul>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/d3da48e7e3da3042b7142fe3deced0bcaac3e704"><code>d3da48e</code></a> 5.51.1</li>
<li><a href="https://github.com/webpack/webpack/commit/e73864c0367acdaad58c5129c1396410f986b392"><code>e73864c</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14031">#14031</a> from webpack/bugfix/concatenated-contextify</li>
<li><a href="https://github.com/webpack/webpack/commit/c76be4d7383f35b3260dafefbcd24cac245d9e42"><code>c76be4d</code></a> make some things context-independent</li>
<li><a href="https://github.com/webpack/webpack/commit/5239f2642738ea66b9a717d4164b06de4a867429"><code>5239f26</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14030">#14030</a> from webpack/bugfix/crash-fsinfo</li>
<li><a href="https://github.com/webpack/webpack/commit/ff69a4a631d0edf3c6086c70c79761929ae18fbb"><code>ff69a4a</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13997">#13997</a> from yujunjung/main</li>
<li><a href="https://github.com/webpack/webpack/commit/0088d5565c602fd28cd6145186a95ed08f119642"><code>0088d55</code></a> fix crash when trying to snapshot not existing directory</li>
<li><a href="https://github.com/webpack/webpack/commit/bd7cb37f1c0d872cfff9fc27c7db52a25e1ba6a3"><code>bd7cb37</code></a> 5.51.0</li>
<li><a href="https://github.com/webpack/webpack/commit/1a06a4517b326e23ab39b46b5d7d0040916ac2db"><code>1a06a45</code></a> update lazy-compilation example for webpack-dev-server@4</li>
<li><a href="https://github.com/webpack/webpack/commit/4e5e0aca41f0efaf7466c512095295421f17e4d5"><code>4e5e0ac</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14009">#14009</a> from henryqdineen/hqd-module-creation-callback</li>
<li><a href="https://github.com/webpack/webpack/commit/c61466e43895f84ff56fb98e69cbe3f3e19f47c2"><code>c61466e</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14019">#14019</a> from webpack/bugfix/symlink-snapshot</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.51.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.51.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-08-19 14:19:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2942" class=".btn">#2942</a>
            </td>
            <td>
                <b>
                    test: Added tests to ensure that store config is optional for queries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Updated common storage tests to check and make sure that stores can query without requiring a store configuration (indexes). The interface says that indexes are recommended for large stores, but it doesn't say that they're always required, so storage providers should ensure that they can function without them.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 18:49:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2941" class=".btn">#2941</a>
            </td>
            <td>
                <b>
                    fix: set config for remote provider store
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andriy Holovko <andriy.holovko@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 14:45:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2940" class=".btn">#2940</a>
            </td>
            <td>
                <b>
                    fix: integration issues in wallet DIDcomm interfaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Part of #2433

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 19:34:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2938" class=".btn">#2938</a>
            </td>
            <td>
                <b>
                    docs: Updates to storage interface documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Clarified expected behaviour of storage interface implementations
- Added missing call to Provider.SetStoreConfig for the context store.
- Removed the workaround for MySQL, which is no longer needed.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 19:12:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2937" class=".btn">#2937</a>
            </td>
            <td>
                <b>
                    refactor: use did:key in packagers (for didcomm v1)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">refactor</span><span class="chip">aip 2.0</span>
            </td>
            <td>
                This change removes Base58 key encoding for recipients and sender for did:key (execept for legacy packer which will remain using bsae58 encoding).
It also includes vdr peer did creation with all VM and KeyAgreement keys, not only the first key.
This change adds key resolvers for the packers, one for did:key resolution and another one used for the 1PU test vector verification purposes using a thirdparty store resolution.
Finally, this change also moves did:key fingerprint code referencing did.Doc into a separate subpackage (pkg/vdr/fingerprint/didfp) to avoid cyclic dependency with jwk fingerprint.

closes #1604
closes #1207
closes #1659
closes #1847

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 18:17:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2936" class=".btn">#2936</a>
            </td>
            <td>
                <b>
                    fix: add close request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Firas Qutishat <firas.qutishat@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-16 16:58:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2934" class=".btn">#2934</a>
            </td>
            <td>
                <b>
                    fix: context store Import when underlying storage is mysql
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andriy Holovko <andriy.holovko@gmail.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-16 09:42:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2933" class=".btn">#2933</a>
            </td>
            <td>
                <b>
                    chore(deps): bump tar from 6.1.0 to 6.1.8 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [tar](https://github.com/npm/node-tar) from 6.1.0 to 6.1.8.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/node-tar/commit/6a9c51da31a2c9b67d266d8ce7119e1e2c0d1e5d"><code>6a9c51d</code></a> 6.1.8</li>
<li><a href="https://github.com/npm/node-tar/commit/dfc5923b965aff780d0d8eb4dd657195ee095c41"><code>dfc5923</code></a> fix: skip extract if linkpath is stripped entirely</li>
<li><a href="https://github.com/npm/node-tar/commit/575a511cda6fe3ad201d8a576caaf30abea808a4"><code>575a511</code></a> fix: reserve paths case-insensitively</li>
<li><a href="https://github.com/npm/node-tar/commit/d61628cb40381d89f119431a16a4aab2fbecb056"><code>d61628c</code></a> 6.1.7</li>
<li><a href="https://github.com/npm/node-tar/commit/9e018cf2a5e289d6b34d1a0157980070b3a14c75"><code>9e018cf</code></a> tests: run (and pass) on windows</li>
<li><a href="https://github.com/npm/node-tar/commit/c2a0948fb7b70862f92828e7b37b622566ed367e"><code>c2a0948</code></a> fix: refactoring to pass tests on Windows</li>
<li><a href="https://github.com/npm/node-tar/commit/d0ce670bdb7eed5861837538a0d18c7864ff71c6"><code>d0ce670</code></a> update deps</li>
<li><a href="https://github.com/npm/node-tar/commit/53602669f58ddbeb3294d7196b3320aaaed22728"><code>5360266</code></a> fix: normalize paths on Windows systems</li>
<li><a href="https://github.com/npm/node-tar/commit/9bc1729939eec1c822b528385b1cc513b9888835"><code>9bc1729</code></a> 6.1.6</li>
<li><a href="https://github.com/npm/node-tar/commit/bdf4f5171340b890a62a5e578962ac143d34b3a9"><code>bdf4f51</code></a> fix: properly prefix hard links</li>
<li>Additional commits viewable in <a href="https://github.com/npm/node-tar/compare/v6.1.0...v6.1.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tar&package-manager=npm_and_yarn&previous-version=6.1.0&new-version=6.1.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-08-13 12:29:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2932" class=".btn">#2932</a>
            </td>
            <td>
                <b>
                    chore: Updated json-gold module
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
        Created At 2021-08-13 12:03:45 +0000 UTC
    </div>
</div>

