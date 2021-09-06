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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2970" class=".btn">#2970</a>
            </td>
            <td>
                <b>
                    feat: Present proof v3 service implementation
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
        Created At 2021-09-06 10:25:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2969" class=".btn">#2969</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.52.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.52.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
<h2>v5.52.0</h2>
<h1>Feature</h1>
<ul>
<li><code>experiments.executeModule</code> is enabled by default and the option is removed
<ul>
<li>loaders are now free to use <code>this.importModule</code></li>
</ul>
</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>fix generated <code>__WEBPACK_EXTERNAL_MODULE_null__</code>, which leads to merged externals</li>
<li><code>.webpack[...]</code> extension is not part of matching and module name</li>
</ul>
<h2>v5.51.2</h2>
<h1>Bugfixes</h1>
<ul>
<li>fix crash in FileSystemInfo when errors occur</li>
<li>avoid property access of reserved properties</li>
<li>fix reexports from async modules</li>
<li>automatically close an active watching when closing the compiler</li>
<li>when filenames of other runtimes are referenced that need a full hash, upgrade referencing runtime moduel to full hash mode too
<ul>
<li>fixes a bug where <code>[contenthash]</code> is undefined when using <code>new Worker</code></li>
</ul>
</li>
</ul>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/4edd3800567f279edd7091af14b3385552a8972f"><code>4edd380</code></a> 5.52.0</li>
<li><a href="https://github.com/webpack/webpack/commit/d05648611aa6f554860a08940c3bf784b499c3a9"><code>d056486</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14134">#14134</a> from webpack/bugfix/webpack-extension</li>
<li><a href="https://github.com/webpack/webpack/commit/a513b1381a6e0248d1b44446a471b0bd6711a9b2"><code>a513b13</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14118">#14118</a> from webpack/bugfix/multiple-module-externals</li>
<li><a href="https://github.com/webpack/webpack/commit/825bbc1b61d562774dbe74ee3a84b4c0920b0a53"><code>825bbc1</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14004">#14004</a> from webpack/dependabot/npm_and_yarn/webpack-cli-4.8.0</li>
<li><a href="https://github.com/webpack/webpack/commit/0d25c2f6889e8dd6199eca94e3a69ae5fee28474"><code>0d25c2f</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14100">#14100</a> from webpack/dependabot/npm_and_yarn/eslint-plugin-...</li>
<li><a href="https://github.com/webpack/webpack/commit/1220f75bc52ed30e4eaee9f887182414d0b64c2a"><code>1220f75</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14126">#14126</a> from webpack/dependabot/npm_and_yarn/core-js-3.17.2</li>
<li><a href="https://github.com/webpack/webpack/commit/8cc4bda0b3f9b0f3241b4c5e0864239d6a306b14"><code>8cc4bda</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14127">#14127</a> from webpack/dependabot/npm_and_yarn/memfs-3.2.4</li>
<li><a href="https://github.com/webpack/webpack/commit/bc117e1e9782c7a267d97f9079816f77108c0c02"><code>bc117e1</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14129">#14129</a> from webpack/dependabot/npm_and_yarn/fork-ts-checke...</li>
<li><a href="https://github.com/webpack/webpack/commit/765101bded6bf9dc9693fac6af18771d11b37eed"><code>765101b</code></a> match resource should not include special <code>.webpack[...]</code> extension</li>
<li><a href="https://github.com/webpack/webpack/commit/2ce5458404fa2db2bf91cec57f91142a2216fbfe"><code>2ce5458</code></a> chore(deps-dev): bump fork-ts-checker-webpack-plugin from 6.3.2 to 6.3.3</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.52.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.52.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-09-04 07:05:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2967" class=".btn">#2967</a>
            </td>
            <td>
                <b>
                    test: Additional and improved JSON storage tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Added additional JSON storage tests that check for more types.
- Updated tests to check unmarshalled data instead of directly comparing bytes, in agreement with the updated storage interface documentation. This will avoid potential issues where some storage providers may change the order of the fields around, which could cause the tests to fail unnecessarily.
- Removed replace of test module from aries-agent-mobile and aries-agent-rest, since it can cause some issues when the test signatures are updated.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-02 22:06:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2966" class=".btn">#2966</a>
            </td>
            <td>
                <b>
                    feat: support DID Doc KeyAgreement.ID as kid/skid for DIDCommV2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                This change adds DIDCommV2 support to use KeyAgreement.ID when a DID doc is available.
Default behaviour is to use did:key for pre DIDCommV2 or where DID doc is not available to the recipient.
The Peer VDR creator now uses DIDCommV2 service type matching the media porfile version: DIDCommMessaging (for V2).
Default is did-communication (for pre V2) if media profile is missing or is not DIDCommV2.

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-02 21:07:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2965" class=".btn">#2965</a>
            </td>
            <td>
                <b>
                    docs: Update to SPI documentation for Store Put method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added clarification about how JSON-formatted objects are treated.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-02 19:23:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2964" class=".btn">#2964</a>
            </td>
            <td>
                <b>
                    feat: mobile bindings for vcwallet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Florin Birsan <71101813+skflorin@users.noreply.github.com>

Added VCWalletController to be used in native code
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-01 14:05:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2963" class=".btn">#2963</a>
            </td>
            <td>
                <b>
                    chore(deps): bump tar from 6.1.8 to 6.1.11 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [tar](https://github.com/npm/node-tar) from 6.1.8 to 6.1.11.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/node-tar/commit/e573aeea19d4d650908b7f6bf0a1ad8dce9f1736"><code>e573aee</code></a> 6.1.11</li>
<li><a href="https://github.com/npm/node-tar/commit/edb8e9a3fa5869cfb935479a262f6f61b0a2ec57"><code>edb8e9a</code></a> fix: perf regression on hot string munging path</li>
<li><a href="https://github.com/npm/node-tar/commit/a9d9b05fc974425089922bf66e8e7751ea8bfbbc"><code>a9d9b05</code></a> chore(test): Avoid spurious failures packing node_modules/.cache</li>
<li><a href="https://github.com/npm/node-tar/commit/24b8bdadf37118182496ecf81fa7a872196fb38b"><code>24b8bda</code></a> fix(test): use posix path for testing path reservations</li>
<li><a href="https://github.com/npm/node-tar/commit/e5a223c6b293f1cb2ebb2dd97668f787e8983ca4"><code>e5a223c</code></a> fix(test): make unpack test pass on case-sensitive fs</li>
<li><a href="https://github.com/npm/node-tar/commit/188baddc1d0e6ef5140c7a788f03fc2a6c3df2ea"><code>188badd</code></a> 6.1.10</li>
<li><a href="https://github.com/npm/node-tar/commit/23312ce7db8a12c78d0fba96d7664a01619266a3"><code>23312ce</code></a> drop dirCache for symlink on all platforms</li>
<li><a href="https://github.com/npm/node-tar/commit/4f1f4a21fca64f3089da0e83ceea775c66b55052"><code>4f1f4a2</code></a> 6.1.9</li>
<li><a href="https://github.com/npm/node-tar/commit/875a37e3ec031186fc6599f6807341f56c584598"><code>875a37e</code></a> fix: prevent path escape using drive-relative paths</li>
<li><a href="https://github.com/npm/node-tar/commit/b6162c7fafe797f856564ef37f4b82747f051455"><code>b6162c7</code></a> fix: reserve paths properly for unicode, windows</li>
<li>Additional commits viewable in <a href="https://github.com/npm/node-tar/compare/v6.1.8...v6.1.11">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tar&package-manager=npm_and_yarn&previous-version=6.1.8&new-version=6.1.11)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-09-01 00:33:42 +0000 UTC
    </div>
</div>

