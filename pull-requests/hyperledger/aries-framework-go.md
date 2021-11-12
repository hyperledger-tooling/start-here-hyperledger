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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3053" class=".btn">#3053</a>
            </td>
            <td>
                <b>
                    feat: Add option to enable remote LD Document Loader from mobile bindings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Add option to enable remote LD Document Loader for mobile bindings

**Description:**
It was not possible to set the document loader before because gomobile removed the option to set DocumentLoader.

**Summary:**
Added a method in the Aries Mobile Options to set a DocumentLoader that has remote LD Document loading enabled.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-12 12:15:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3052" class=".btn">#3052</a>
            </td>
            <td>
                <b>
                    fix(vcwallet): correct path to profile existence endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**

VC wallet: REST endpoint /vcwallet/profile/{id} responds with 404

**Description:**

Closes #3051

**Summary:**

Adds a missing `/` to the rest endpoint.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-12 08:25:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3050" class=".btn">#3050</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump webpack from 4.46.0 to 5.64.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [webpack](https://github.com/webpack/webpack) from 4.46.0 to 5.64.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
<h2>v5.64.0</h2>
<h1>Features</h1>
<ul>
<li>add <code>asyncChunks: boolean</code> option to disable creation of async chunks</li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>fix ProfilingPlugin for <code>experiments.backCompat: false</code></li>
</ul>
<h1>Performance</h1>
<ul>
<li>avoid running regexp twice over the file list</li>
</ul>
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
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/789e58514b5747f6474bc247e4e104ce22892a2c"><code>789e585</code></a> 5.64.0</li>
<li><a href="https://github.com/webpack/webpack/commit/d96f23e9b09fa24a65721d8a304eb23cbf7426f4"><code>d96f23e</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14698">#14698</a> from webpack/bugfix/profiling-plugin-hook-check</li>
<li><a href="https://github.com/webpack/webpack/commit/ac7bd4052600ddc3bc255cf3da0186857190e3e0"><code>ac7bd40</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14701">#14701</a> from webpack/feature/no-async-chunk-loading</li>
<li><a href="https://github.com/webpack/webpack/commit/9bb5651e6a3a3f9d0b9939b96239c30680af8876"><code>9bb5651</code></a> add <code>asyncChunks: boolean</code> option to disable creation of async chunks</li>
<li><a href="https://github.com/webpack/webpack/commit/11bc877b42954b9912f0573e53416373e954cbd9"><code>11bc877</code></a> add test case</li>
<li><a href="https://github.com/webpack/webpack/commit/970b368bdaa43ee41a0ef158606922f6c19492a1"><code>970b368</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14686">#14686</a> from webpack/dependabot/npm_and_yarn/mime-types-2.1.34</li>
<li><a href="https://github.com/webpack/webpack/commit/6a12794b1107d06a903b258c84a7690ec1ef093e"><code>6a12794</code></a> check hooks for existance before using in ProfilingPlugin</li>
<li><a href="https://github.com/webpack/webpack/commit/e6da1d442045c36aef4d30aaa51ee56e14b87299"><code>e6da1d4</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/14694">#14694</a> from markjm/markjm/double-regexp</li>
<li><a href="https://github.com/webpack/webpack/commit/6d3cd42008ae4d31b05ea1af8161e5f0ad9fb4e6"><code>6d3cd42</code></a> perf: Prevent running regexs over the same strings twice</li>
<li><a href="https://github.com/webpack/webpack/commit/f011c70aacbd4dd3c4e518b9b9d8ea945dce0a9a"><code>f011c70</code></a> 5.63.0</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.64.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpack&package-manager=npm_and_yarn&previous-version=4.46.0&new-version=5.64.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-11-12 08:15:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3049" class=".btn">#3049</a>
            </td>
            <td>
                <b>
                    fix(vcwallet): convert key to kid before issuing vc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**

Fix VC wallet: Unable to issue credential

**Description:**

Fixes #3029

**Summary:**

Converts the verification method / public key to the key ID that's required by keyManager to retrieve the private key for signing. The conversion steps were taken from the standard VC issuing endpoint.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-12 07:42:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3048" class=".btn">#3048</a>
            </td>
            <td>
                <b>
                    docs: aries standards and specifications
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-12 02:57:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3047" class=".btn">#3047</a>
            </td>
            <td>
                <b>
                    fix: Crytpo signature verification using P384 key from JWK import 
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

