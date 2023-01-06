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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3462" class=".btn">#3462</a>
            </td>
            <td>
                <b>
                    feat: Unit test for SD-JWT Flow (Issuer, Holder, Verifier)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Unit test for SD-JWT Flow.

Closes #3461

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-05 21:33:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3460" class=".btn">#3460</a>
            </td>
            <td>
                <b>
                    feat: SD-JWT Holder/Verifier - Process Disclosures
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added utility function to decode disclosures (used by both holder and verifier) Created disclose claims function for holder that re-creates SD-JWT with disclosures for selected claims only.

Created get verified payload function for verifier (removes _sd and _sd_alg from claims and inserts into payload disclosed claims).

Closes #3459

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-05 03:07:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3458" class=".btn">#3458</a>
            </td>
            <td>
                <b>
                    chore(deps): bump json5 and webpack in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [json5](https://github.com/json5/json5) to 2.2.3 and updates ancestor dependency [webpack](https://github.com/webpack/webpack). These dependencies need to be updated together.

Updates `json5` from 2.2.0 to 2.2.3
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/releases">json5's releases</a>.</em></p>
<blockquote>
<h2>v2.2.3</h2>
<ul>
<li>Fix: json5@2.2.3 is now the 'latest' release according to npm instead of v1.0.2. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/299">#299</a>)</li>
</ul>
<h2>v2.2.2</h2>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays.
(<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by
Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>).</li>
</ul>
<h2>v2.2.1</h2>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/blob/main/CHANGELOG.md">json5's changelog</a>.</em></p>
<blockquote>
<h3>v2.2.3 [<a href="https://github.com/json5/json5/tree/v2.2.3">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.2...v2.2.3">diff</a>]</h3>
<ul>
<li>Fix: json5@2.2.3 is now the 'latest' release according to npm instead of
v1.0.2. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/299">#299</a>)</li>
</ul>
<h3>v2.2.2 [<a href="https://github.com/json5/json5/tree/v2.2.2">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.1...v2.2.2">diff</a>]</h3>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays.
(<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by
Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>).</li>
</ul>
<h3>v2.2.1 [<a href="https://github.com/json5/json5/tree/v2.2.1">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.0...v2.2.1">diff</a>]</h3>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/json5/json5/commit/c3a75242772a5026a49c4017a16d9b3543b62776"><code>c3a7524</code></a> 2.2.3</li>
<li><a href="https://github.com/json5/json5/commit/94fd06d82eeed225fa172f6fb2ca27375cbd2e39"><code>94fd06d</code></a> docs: update CHANGELOG for v2.2.3</li>
<li><a href="https://github.com/json5/json5/commit/3b8cebf0c474a8b20c78bd75c89cca0c4dce84ce"><code>3b8cebf</code></a> docs(security): use GitHub security advisories</li>
<li><a href="https://github.com/json5/json5/commit/f0fd9e194dde282caff114a110f4fac635f3a62c"><code>f0fd9e1</code></a> docs: publish a security policy</li>
<li><a href="https://github.com/json5/json5/commit/6a91a05fffeda16ff6b3b5008b6b340d42d31ec0"><code>6a91a05</code></a> docs(template): bug -&gt; bug report</li>
<li><a href="https://github.com/json5/json5/commit/14f8cb186e8abdfaccf6527171da7b1224374650"><code>14f8cb1</code></a> 2.2.2</li>
<li><a href="https://github.com/json5/json5/commit/10cc7ca9169b59c5e0f5afc03dbd870cd06bcc46"><code>10cc7ca</code></a> docs: update CHANGELOG for v2.2.2</li>
<li><a href="https://github.com/json5/json5/commit/7774c1097993bc3ce9f0ac4b722a32bf7d6871c8"><code>7774c10</code></a> fix: add <strong>proto</strong> to objects and arrays</li>
<li><a href="https://github.com/json5/json5/commit/edde30abd8b22facf2c06c72586b9f6edf12700d"><code>edde30a</code></a> Readme: slight tweak to intro</li>
<li><a href="https://github.com/json5/json5/commit/97286f8bd542c89dcee096bc05dd28ed2dfc1e16"><code>97286f8</code></a> Improve example in readme</li>
<li>Additional commits viewable in <a href="https://github.com/json5/json5/compare/v2.2.0...v2.2.3">compare view</a></li>
</ul>
</details>
<br />

Updates `webpack` from 4.46.0 to 5.75.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/webpack/webpack/releases">webpack's releases</a>.</em></p>
<blockquote>
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
<h2>v5.74.0</h2>
<h1>Features</h1>
<ul>
<li>add <code>resolve.extensionAlias</code> option which allows to alias extensions
<ul>
<li>This is useful when you are forced to add the <code>.js</code> extension to imports when the file really has a <code>.ts</code> extension (typescript + <code>&quot;type&quot;: &quot;module&quot;</code>)</li>
</ul>
</li>
<li>add support for ES2022 features like static blocks</li>
<li>add Tree Shaking support for <code>ProvidePlugin</code></li>
</ul>
<h1>Bugfixes</h1>
<ul>
<li>fix persistent cache when some build dependencies are on a different windows drive</li>
<li>make order of evaluation of side-effect-free modules deterministic between concatenated and non-concatenated modules</li>
<li>remove left-over from debugging in TLA/async modules runtime code</li>
<li>remove unneeded extra 1s timestamp offset during watching when files are actually untouched
<ul>
<li>This sometimes caused an additional second build which are not really needed</li>
</ul>
</li>
<li>fix <code>shareScope</code> option for <code>ModuleFederationPlugin</code></li>
<li>set <code>&quot;use-credentials&quot;</code> also for same origin scripts</li>
</ul>
<h1>Performance</h1>
<ul>
<li>Improve memory usage and performance of aggregating needed files/directories for watching
<ul>
<li>This affects rebuild performance</li>
</ul>
</li>
</ul>
<h1>Extensibility</h1>
<ul>
<li>export <code>HarmonyImportDependency</code> for plugins</li>
</ul>
<h2>v5.73.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/webpack/webpack/commit/8241da7f1e75c5581ba535d127fa66aeb9eb2ac8"><code>8241da7</code></a> 5.75.0</li>
<li><a href="https://github.com/webpack/webpack/commit/a91d9232ea87eedbe9077366395748f156730a2d"><code>a91d923</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/16458">#16458</a> from webpack/bugfix/semi</li>
<li><a href="https://github.com/webpack/webpack/commit/4608b114168f25eef4cfe9a27645cec40e7a68b5"><code>4608b11</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/16457">#16457</a> from webpack/tooling/update</li>
<li><a href="https://github.com/webpack/webpack/commit/dfdd0b0e42a479f60c1f84ced2fc4e3bdb2b2456"><code>dfdd0b0</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/16122">#16122</a> from AnmolBansalDEV/bug/compilationCallback</li>
<li><a href="https://github.com/webpack/webpack/commit/23b9a1c01ff5bb4570aece5a99d703aa564a8f3a"><code>23b9a1c</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/16167">#16167</a> from exposir/fixts</li>
<li><a href="https://github.com/webpack/webpack/commit/6f2c5e852a502a049ed8e37cfdc428305573b6b1"><code>6f2c5e8</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/16257">#16257</a> from alexzhang1030/calc_deterministic_verbose</li>
<li><a href="https://github.com/webpack/webpack/commit/f7f36ad412760c29cf727a4e952eeeba23570d36"><code>f7f36ad</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/16339">#16339</a> from Liamolucko/wasm-i64</li>
<li><a href="https://github.com/webpack/webpack/commit/761a54285e7b4e24727e7bb17e9291e264fe5351"><code>761a542</code></a> fix semicolon position</li>
<li><a href="https://github.com/webpack/webpack/commit/2403a36326248f7f515959a479baa257288bef4d"><code>2403a36</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/webpack/webpack/issues/16345">#16345</a> from ahabhgk/fix-eval-nosources</li>
<li><a href="https://github.com/webpack/webpack/commit/c18203c89447cd6728aa1f9d77b03aff7ae6e03f"><code>c18203c</code></a> update tooling</li>
<li>Additional commits viewable in <a href="https://github.com/webpack/webpack/compare/v4.46.0...v5.75.0">compare view</a></li>
</ul>
</details>
<br />


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
        Created At 2023-01-01 16:05:39 +0000 UTC
    </div>
</div>

