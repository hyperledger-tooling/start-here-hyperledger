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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3047" class=".btn">#3047</a>
            </td>
            <td>
                <b>
                    fix: Crytp signature verification using P384 key from JWK import 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since P-384 DER format was using Tink's default signature template which uses SHA512, it was causing keys imported from a JWK to fail.
This change uses a template with SHA384 instead to keep signature/verification consistent in all cases (native kms key vs JWK imported key).


Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 16:54:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3046" class=".btn">#3046</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.63.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.63.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
<h2>v5.63.0</h2>
<h1>Features</h1>
<ul>
<li>allow passing <code>chunkLoading: false</code> to disable on-demand loading</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>fix <code>import 'single-quote'</code> in esm build dependencies</li>
</ul>
<h2>v5.62.2</h2>
<h1>Bugfixes</h1>
<ul>
<li>fix <code>__system_context__</code> injection when using the <code>library</code> option on entrypoint</li>
<li>enable <code>exportsPresence: &quot;error&quot;</code> by default in <code>futureDefaults</code></li>
<li>fix bad performance for a RegExp in Stats printing (with large error messages)</li>
<li>fix <code>exportPresence</code> -&gt; <code>exportsPresence</code> typo</li>
<li>fix a bug with module invalidation when only module id changes with <code>experiments.cacheUnaffected</code></li>
</ul>
<h2>v5.62.1</h2>
<h1>Bugfix</h1>
<ul>
<li>fix invalid generated code when omitting <code>;</code></li>
</ul>
<h2>v5.62.0</h2>
<h1>Features</h1>
<ul>
<li>add options to configure export presence checking
<ul>
<li><code>parser.javascript.reexportExportsPresence: false</code> allows to disable warnings for non-existing exports during the migration from <code>export ... from &quot;...&quot;</code> to <code>export type ... from &quot;...&quot;</code> for type reexports in TypeScript</li>
</ul>
</li>
<li>add <code>experiments.backCompat: false</code> to disable some expensive deprecations for better performance</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>use <code>['catch']</code> instead of <code>.catch</code> for better ES3 support</li>
<li>fix removed parentheses when using <code>new (require(&quot;...&quot;)).Something()</code></li>
<li>fix <code>{ require }</code> object literals</li>
<li><code>splitChunks.chunks</code> option is now correctly used for <code>splitChunks.fallbackCacheGroup.maxSize</code> too</li>
<li>fix schema of <code>listen</code> option, allow to omit <code>port</code></li>
<li>add better support for Promises from different isolates</li>
</ul>
<h1>Developer Experience</h1>
<ul>
<li>add typings for the webpack API that is available within modules
<ul>
<li>use <code>/// &lt;reference types=&quot;webpack/module&quot; /&gt;</code> to use the typings in typescript modules</li>
<li>or <code>&quot;types&quot;: [..., &quot;webpack/module&quot;]</code> in tsconfig</li>
</ul>
</li>
</ul>
<h2>v5.61.0</h2>
<h1>Bugfixes</h1>
<ul>
<li>use a wasm md4 implementation for node 17 support</li>
<li>include the <code>path</code> submodules in the node.js default externals</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/f011c70aacbd4dd3c4e518b9b9d8ea945dce0a9a"><code>f011c70</code></a> 5.63.0</li>
<li><a href="https://github.com/webpack/webpack/commit/9cdd1674d0560f250eaeb90558ede2d8db8579ce"><code>9cdd167</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14692">#14692</a> from webpack/feature/chunk-loading-false</li>
<li><a href="https://github.com/webpack/webpack/commit/9570a12d6b7a5c5ecbeb2eb5c48f5a9abb901d96"><code>9570a12</code></a> add <code>chunkLoading: false</code> support</li>
<li><a href="https://github.com/webpack/webpack/commit/3c17f90bb3d811ba1643bf523cfedd92a68a4e12"><code>3c17f90</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14687">#14687</a> from webpack/bugfix/esm-single-quote</li>
<li><a href="https://github.com/webpack/webpack/commit/4edd0438cff92f047122bbb1a9e2a261f4d22c17"><code>4edd043</code></a> fix using single quotes with esm files</li>
<li><a href="https://github.com/webpack/webpack/commit/3aed1fe0249f8730a35fab62e3cdc3b399b0b6e9"><code>3aed1fe</code></a> 5.62.2</li>
<li><a href="https://github.com/webpack/webpack/commit/14582fc41504595b04f01561ea19d27391d6b9ac"><code>14582fc</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14684">#14684</a> from webpack/bugfix/cache-unaffected-module-id</li>
<li><a href="https://github.com/webpack/webpack/commit/393fb6e22c27cae0c6cffe19ba1a5ae710c0f9b5"><code>393fb6e</code></a> fix a bug with experiments.cacheUnaffected</li>
<li><a href="https://github.com/webpack/webpack/commit/86e3eb289f6ea9baf4bdc22748b9a9d8dff187b8"><code>86e3eb2</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14665">#14665</a> from markjm/markjm/option-names</li>
<li><a href="https://github.com/webpack/webpack/commit/12e028518a726c4ebf336ecfe823d27f51776b13"><code>12e0285</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14679">#14679</a> from webpack/fix-regexp</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.63.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.63.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-11-10 08:18:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3044" class=".btn">#3044</a>
            </td>
            <td>
                <b>
                    feat: Credential Manifest
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
        Created At 2021-11-09 04:12:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3042" class=".btn">#3042</a>
            </td>
            <td>
                <b>
                    feat: add issue credential V3 wasm test
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
        Created At 2021-11-08 08:24:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3040" class=".btn">#3040</a>
            </td>
            <td>
                <b>
                    chore: fix bdd test run flag
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
        Created At 2021-11-04 22:01:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3038" class=".btn">#3038</a>
            </td>
            <td>
                <b>
                    feat: OOB V2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change introduces OOB V2 service and client first draft.
It also injects the Accept oob property in the BDD tests.

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 14:56:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3037" class=".btn">#3037</a>
            </td>
            <td>
                <b>
                    feat: add bdd test for issue credential V3
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
        Created At 2021-11-04 13:41:19 +0000 UTC
    </div>
</div>

