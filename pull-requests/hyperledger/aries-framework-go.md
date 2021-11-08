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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3041" class=".btn">#3041</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.62.1 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.62.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
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
<h1>Performance</h1>
<ul>
<li>improve string to binary conversion performance for hashing</li>
</ul>
<h1>Contribution</h1>
<ul>
<li>CI runs on node.js 17</li>
</ul>
<h2>v5.60.0</h2>
<h1>Features</h1>
<ul>
<li>Allow to pass more options to <code>experiments.lazyCompilation</code>. e. g. port, https stuff</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>fix <code>output.hashFunction</code> used to persistent caching too</li>
<li>Initialize <code>buildDependencies</code> Set correctly when loaders are added in <code>beforeLoaders</code> hook</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/daba59b3d60e7895543b6563682c209e4ad6b8b8"><code>daba59b</code></a> 5.62.1</li>
<li><a href="https://github.com/webpack/webpack/commit/707a6d360f39419ea158a1e174a8ecd6483d9188"><code>707a6d3</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14663">#14663</a> from webpack/hotfix/14662</li>
<li><a href="https://github.com/webpack/webpack/commit/610d4356607eb74409e29954dd35945fdb2eb42b"><code>610d435</code></a> fix <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14662">#14662</a></li>
<li><a href="https://github.com/webpack/webpack/commit/04640dcc757c8b3e78c6cbf6e4dda7cbbde33fe2"><code>04640dc</code></a> 5.62.0</li>
<li><a href="https://github.com/webpack/webpack/commit/122db57e7bb0ddb8327b37eeaa0adb9bd5135962"><code>122db57</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14653">#14653</a> from webpack/feature/no-back-compat</li>
<li><a href="https://github.com/webpack/webpack/commit/43f6109957cc31f8bc8a98c0a82061dac185a2b8"><code>43f6109</code></a> update snapshot</li>
<li><a href="https://github.com/webpack/webpack/commit/e06c2c0ac5859077a2d8fa8610505a7ea888075b"><code>e06c2c0</code></a> update snapshot and move cli test to basic tests</li>
<li><a href="https://github.com/webpack/webpack/commit/7afcc5d4ff4ecaa371a2f82d7428dabd3728c63e"><code>7afcc5d</code></a> allow to disable some deprecations</li>
<li><a href="https://github.com/webpack/webpack/commit/95b101fc8ea719b57e94370e35fb8f417b299158"><code>95b101f</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14641">#14641</a> from webpack/dependabot/npm_and_yarn/jest-junit-13.0.0</li>
<li><a href="https://github.com/webpack/webpack/commit/26482ea249507e8143d3a43f79272ce7c147360e"><code>26482ea</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14640">#14640</a> from webpack/dependabot/npm_and_yarn/mini-svg-data-...</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.62.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.62.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-11-08 08:17:28 +0000 UTC
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3036" class=".btn">#3036</a>
            </td>
            <td>
                <b>
                    feat: add issue credential V3 to command
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
        Created At 2021-11-03 08:30:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3035" class=".btn">#3035</a>
            </td>
            <td>
                <b>
                    feat: two-stage protocol service initialization & inbound dispatcher package
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
        Created At 2021-11-03 00:36:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3034" class=".btn">#3034</a>
            </td>
            <td>
                <b>
                    fix: present proof issues in REST controllers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - fixed issues where request body payloads are being ignored by present
proof REST controllers

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 22:40:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3033" class=".btn">#3033</a>
            </td>
            <td>
                <b>
                    feat: add issue credential V3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                V3 spec: https://github.com/trustbloc/wallet/tree/main/docs/waci-credential-manifest/issue_credential

Signed-off-by: Firas Qutishat <firas.qutishat@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 18:08:41 +0000 UTC
    </div>
</div>

