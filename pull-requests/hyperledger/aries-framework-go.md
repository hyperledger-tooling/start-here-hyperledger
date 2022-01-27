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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3140" class=".btn">#3140</a>
            </td>
            <td>
                <b>
                    feat: include router connections in oobv2 acceptinvitation peer DID
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
        Created At 2022-01-26 15:19:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3139" class=".btn">#3139</a>
            </td>
            <td>
                <b>
                    feat: vc wallet resolve manifest by credential ID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - added new option in vcwallet to resolve credential saved in wallet
content store just by providing credential ID
- refcatored credential mabnifest API to accept raw credential to avoid
repeated marshal/unmarshaling of credential object
- Part of #3120

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-26 04:15:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3138" class=".btn">#3138</a>
            </td>
            <td>
                <b>
                    test: Enhancements to WACI issuance BDD tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Attachments are now generated on the fly using pre-defined Credential Manifest, Credential Application, and Credential Fulfillment objects.
- Added constants to Credential Manifest package for attachment formats and contexts.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 21:10:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3137" class=".btn">#3137</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.67.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.67.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
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
<h2>v5.66.0</h2>
<h1>Features</h1>
<ul>
<li>add <code>output.library.type: &quot;commonjs-static&quot;</code> to emit a statically analyse-able commonjs module (for node.js esm interop support)</li>
<li>add <code>experiments.css</code> (very experimental)
<ul>
<li>see <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14893">webpack/webpack#14893</a></li>
</ul>
</li>
</ul>
<h1>Bugfixes</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/4abe329dcdaea60371c03c0d85c3a3994d875138"><code>4abe329</code></a> 5.67.0</li>
<li><a href="https://github.com/webpack/webpack/commit/6fa6e30254f0eb2673a3525739da1df0a5f51791"><code>6fa6e30</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/13110">#13110</a> from eltociear/patch-1</li>
<li><a href="https://github.com/webpack/webpack/commit/9dbf3ca8999fd85402be21dc8e2db5a592d58d82"><code>9dbf3ca</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14721">#14721</a> from Schweinepriester/patch-1</li>
<li><a href="https://github.com/webpack/webpack/commit/f22a31425f66fc0f31a82561d171518c07d0e9e6"><code>f22a314</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/15202">#15202</a> from tmeasday/webpack-hot-middleware-lazy-compilation</li>
<li><a href="https://github.com/webpack/webpack/commit/3014a3b8246f4ac1b3c5d27dd68120df88f04b17"><code>3014a3b</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/15222">#15222</a> from webpack/bugfix/serialization-warning</li>
<li><a href="https://github.com/webpack/webpack/commit/17f317bef2b567f73890c4201f37f09a740ada33"><code>17f317b</code></a> store url as Buffer to avoid serialization warnings</li>
<li><a href="https://github.com/webpack/webpack/commit/e2d214a1ce8a78b3bb58ab7ba59f181b7f85cd7d"><code>e2d214a</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/15200">#15200</a> from webpack/feature/css-exports-in-node</li>
<li><a href="https://github.com/webpack/webpack/commit/1ed8aaf2e291fc0b14597ef452e6224ad10ccbc9"><code>1ed8aaf</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14173">#14173</a> from tosmolka/tosmolka/14075</li>
<li><a href="https://github.com/webpack/webpack/commit/181a2f032ac57d7efda67c2b2fd0dccd14790588"><code>181a2f0</code></a> remove broken concatenation for now</li>
<li><a href="https://github.com/webpack/webpack/commit/70da0dd0432299c674e603fd1efd4d321ad1fa60"><code>70da0dd</code></a> improve test case</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.67.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.67.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-01-24 08:17:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3136" class=".btn">#3136</a>
            </td>
            <td>
                <b>
                    feat: credential manifest support in vcwallet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - added new resolve credential manifest interface to resolve
fulfillments and credentials
- refactores testdata files to avoid duplicate testdata files across
various packages
- Closes #3120

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-22 19:51:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3135" class=".btn">#3135</a>
            </td>
            <td>
                <b>
                    feat: credential manifest resolve - specify schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - specify schema along with resolved values which will be helpful for
rendering resolved values

- Part of #3092

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 01:30:13 +0000 UTC
    </div>
</div>

