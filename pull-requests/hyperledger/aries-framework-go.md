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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3153" class=".btn">#3153</a>
            </td>
            <td>
                <b>
                    feat: Function to validate Credential Application Attachment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Derek Trider <Derek.Trider@securekey.com>

closes #3150 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-03 20:58:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3152" class=".btn">#3152</a>
            </td>
            <td>
                <b>
                    feat: support for websocket read limit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #3147

Signed-off-by: Andrii Holovko <andriy.holovko@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-03 17:58:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3151" class=".btn">#3151</a>
            </td>
            <td>
                <b>
                    fix: issue-credential params support unmarshaling from DIDCommMsg
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also refactors present-proof params for consistency.

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-02 21:10:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3149" class=".btn">#3149</a>
            </td>
            <td>
                <b>
                    fix: vcwallet - collection data key collision
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixed problem with collections where 2 different content types share
same id

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-02 04:44:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3148" class=".btn">#3148</a>
            </td>
            <td>
                <b>
                    refactor: Reduce code duplication in WACI Issuance tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Refactored the WACI Issuance tests using V1 and V2 so that there's less code duplication.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>

closes #3143
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-02 03:52:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3146" class=".btn">#3146</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.68.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.68.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
<h2>v5.68.0</h2>
<h1>Features</h1>
<ul>
<li>allow to disable compile time evaluation of import.meta.url</li>
<li>add <code>__webpack_module__</code> and <code>__webpack_module__.id</code> to the api</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>fix handling of errors thrown in async modules</li>
</ul>
<h2>v5.67.0</h2>
<h1>Features</h1>
<ul>
<li>add 'outputPath' configuration option for resource asset modules</li>
<li>support Trusted Types in eval source maps</li>
<li><code>experiments.css</code>
<ul>
<li>allow to generate only exports for css in node</li>
<li>add <code>SyncModuleIdsPlugin</code> to sync module ids between server and client compilation</li>
<li>add more options to the <code>DeterministicModuleIdsPlugin</code> to allow to generate equal ids</li>
</ul>
</li>
</ul>
<h1>Developer Experience</h1>
<ul>
<li>limit data url module name in stats printer</li>
<li>allow specific description for CLI options</li>
<li>improve space limiting algorithm in stats printing to show partial lists</li>
<li>add <code>null</code> to errors in callbacks</li>
<li>fix call signature types of addChunkInGroup</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>avoid reporting non-existant package.jsons as dependencies</li>
<li><code>experiments.css</code>
<ul>
<li>fix missing css runtime when only initial css is used</li>
<li>fix css hmr support</li>
<li>bugfixes to css modules</li>
</ul>
</li>
<li>fix cache serialization for CreateScriptUrlDependency</li>
<li>fix data url content when processed by a loader</li>
<li>fix regexp in identifiers that include <code>|</code></li>
<li>fix ProfilingPlugin for watch scenarios</li>
<li>add layer to module names and identifiers
<ul>
<li>this avoid random module id changes when additional modules are added to another layer</li>
</ul>
</li>
<li>provide hashFunction parameter to DependencyTemplates to allow customizing it there</li>
<li>fix HMR when experiments.lazyCompilation is enabled</li>
<li>store url as Buffer to avoid serialization warnings</li>
<li>exclude <code>webpack-hot-middleware/client</code> from lazy compilation</li>
</ul>
<h1>Contributing</h1>
<ul>
<li>remove travis configuration</li>
<li>improve spell checking</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/f593d98453e7920bf65f24bf051cd67b5704b59d"><code>f593d98</code></a> 5.68.0</li>
<li><a href="https://github.com/webpack/webpack/commit/6f3735c54850960047cea1ece8194363b2401f29"><code>6f3735c</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/15279">#15279</a> from taranek/docs/array-helpers-docs</li>
<li><a href="https://github.com/webpack/webpack/commit/04039ca99c9a5575ecb041796c6a0858d7be591d"><code>04039ca</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/15284">#15284</a> from webpack/feature/<strong>webpack_module</strong></li>
<li><a href="https://github.com/webpack/webpack/commit/d7a87ab5bc3c6333dffb49af24990e7672643fcd"><code>d7a87ab</code></a> change <strong>webpack_module_id</strong> to <strong>webpack_module</strong>.id</li>
<li><a href="https://github.com/webpack/webpack/commit/612de998f186a9bb2fe8769a91678df689a0541e"><code>612de99</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/15282">#15282</a> from webpack/feature/<strong>webpack_module</strong></li>
<li><a href="https://github.com/webpack/webpack/commit/a962d2ceddc387354a4c4bc927f92e338babfd2c"><code>a962d2c</code></a> add <strong>webpack_module</strong> and <strong>webpack_module_id</strong> to the api</li>
<li><a href="https://github.com/webpack/webpack/commit/5a3760e6d47af6c2a9e70f2e08b7a0d02e6f78a5"><code>5a3760e</code></a> docs(util): added jsdoc annotations for ArrayHelpers.js</li>
<li><a href="https://github.com/webpack/webpack/commit/46e8639a6a1f5288e2f43229f39fc21aecb3c5e8"><code>46e8639</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/15246">#15246</a> from pavelsavara/import_meta_url</li>
<li><a href="https://github.com/webpack/webpack/commit/1e73ca79c4e01ab55e6e25f7991306050907ec66"><code>1e73ca7</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/15266">#15266</a> from webpack/bugfix/throwing-in-async-modules</li>
<li><a href="https://github.com/webpack/webpack/commit/232403c5e8fcfd733e4fff7f829aac6e51b5fb2a"><code>232403c</code></a> fix discussions</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.68.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.68.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-02-01 08:16:32 +0000 UTC
    </div>
</div>

