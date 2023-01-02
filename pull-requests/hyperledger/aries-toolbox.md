---
layout: default
title: aries-toolbox
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-toolbox
---

# aries-toolbox <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-toolbox){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-toolbox/pull/298" class=".btn">#298</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump json5, babel-loader and vue-loader
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [json5](https://github.com/json5/json5) to 2.2.3 and updates ancestor dependencies [json5](https://github.com/json5/json5), [babel-loader](https://github.com/babel/babel-loader) and [vue-loader](https://github.com/vuejs/vue-loader). These dependencies need to be updated together.

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

Updates `babel-loader` from 8.2.3 to 8.3.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/babel/babel-loader/releases">babel-loader's releases</a>.</em></p>
<blockquote>
<h2>v8.3.0</h2>
<h2>New features</h2>
<ul>
<li>Pass external dependencies from Babel to Webpack by <a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a> in <a href="https://github-redirect.dependabot.com/babel/babel-loader/pull/971">babel/babel-loader#971</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/babel/babel-loader/compare/v8.2.5...v8.3.0">https://github.com/babel/babel-loader/compare/v8.2.5...v8.3.0</a></p>
<h2>v8.2.5</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: respect <code>inputSourceMap</code> loader option by <a href="https://github.com/alan-agius4"><code>@​alan-agius4</code></a> in <a href="https://github-redirect.dependabot.com/babel/babel-loader/pull/896">babel/babel-loader#896</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/alan-agius4"><code>@​alan-agius4</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/babel/babel-loader/pull/896">babel/babel-loader#896</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/babel/babel-loader/compare/v8.2.4...v8.2.5">https://github.com/babel/babel-loader/compare/v8.2.4...v8.2.5</a></p>
<h2>v8.2.4</h2>
<h2>What's Changed</h2>
<ul>
<li>doc(README.md): fix a broken markdown link by <a href="https://github.com/loveDstyle"><code>@​loveDstyle</code></a> in <a href="https://github-redirect.dependabot.com/babel/babel-loader/pull/919">babel/babel-loader#919</a></li>
<li>Bump loader-utils to 2.x by <a href="https://github.com/stianjensen"><code>@​stianjensen</code></a> in <a href="https://github-redirect.dependabot.com/babel/babel-loader/pull/931">babel/babel-loader#931</a></li>
<li>Use md5 hashing for OpenSSL 3 by <a href="https://github.com/pathmapper"><code>@​pathmapper</code></a> in <a href="https://github-redirect.dependabot.com/babel/babel-loader/pull/924">babel/babel-loader#924</a></li>
</ul>
<p>Thanks <a href="https://github.com/loveDstyle"><code>@​loveDstyle</code></a>, <a href="https://github.com/stianjensen"><code>@​stianjensen</code></a> and <a href="https://github.com/pathmapper"><code>@​pathmapper</code></a> for your first PRs!</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/babel/babel-loader/commit/9bf5652c3b718971382c110c4b7f86212aa8cb52"><code>9bf5652</code></a> 8.3.0</li>
<li><a href="https://github.com/babel/babel-loader/commit/80ab7d013b1c2142516d9939c978cba82648c052"><code>80ab7d0</code></a> Update <code>@babel/</code> dependencies</li>
<li><a href="https://github.com/babel/babel-loader/commit/493ac6cfdb2763568b42e787b95ac3a05ebfd15b"><code>493ac6c</code></a> Pass external dependencies from Babel to Webpack (<a href="https://github-redirect.dependabot.com/babel/babel-loader/issues/971">#971</a>)</li>
<li><a href="https://github.com/babel/babel-loader/commit/df28fe312abba66cf72320e23268ad208fdf5006"><code>df28fe3</code></a> Fix broken main test (<a href="https://github-redirect.dependabot.com/babel/babel-loader/issues/950">#950</a>)</li>
<li><a href="https://github.com/babel/babel-loader/commit/0b338e4abb4e7c22a09c2cee39b1b1664226ecaf"><code>0b338e4</code></a> update hash method so it doesn't fail on a fips enabled machine (<a href="https://github-redirect.dependabot.com/babel/babel-loader/issues/939">#939</a>)</li>
<li><a href="https://github.com/babel/babel-loader/commit/1f98d3c7978a729becb2f27b42c44f4ac37fce83"><code>1f98d3c</code></a> 8.2.5</li>
<li><a href="https://github.com/babel/babel-loader/commit/c622868020a07cc4d632bb51afb3db1f4edaaae2"><code>c622868</code></a> fix: respect <code>inputSourceMap</code> loader option (<a href="https://github-redirect.dependabot.com/babel/babel-loader/issues/896">#896</a>)</li>
<li><a href="https://github.com/babel/babel-loader/commit/f7982c1a7ee34f25ce73cc4fd5771fca475b4447"><code>f7982c1</code></a> 8.2.4</li>
<li><a href="https://github.com/babel/babel-loader/commit/4bb9e21a36fa581c045121031717b90b5a77ef16"><code>4bb9e21</code></a> Use md5 hashing for OpenSSL 3 (<a href="https://github-redirect.dependabot.com/babel/babel-loader/issues/924">#924</a>)</li>
<li><a href="https://github.com/babel/babel-loader/commit/247c94ba90cd7311b17e18dea68349c727c28b6c"><code>247c94b</code></a> Bump loader-utils to 2.x (<a href="https://github-redirect.dependabot.com/babel/babel-loader/issues/931">#931</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/babel/babel-loader/compare/v8.2.3...v8.3.0">compare view</a></li>
</ul>
</details>
<br />

Updates `vue-loader` from 15.9.8 to 17.0.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-loader/releases">vue-loader's releases</a>.</em></p>
<blockquote>
<h2>v17.0.1</h2>
<h3>Bug Fixes</h3>
<ul>
<li>add <code>vue</code> and <code>@vue/compiler-sfc</code> to optional peerDependencies (<a href="https://github.com/vuejs/vue-loader/commit/df0ded5356864b9923da8f89ff33db1ae6c2402f">df0ded5</a>), closes <a href="https://github-redirect.dependabot.com/vuejs/vue-loader/issues/1944">#1944</a></li>
<li>merge custom queries rather than appending (<a href="https://github-redirect.dependabot.com/vuejs/vue-loader/issues/1911">#1911</a>) (<a href="https://github.com/vuejs/vue-loader/commit/9e4249a548ceb04ead46fff9b68e9b2676b4c692">9e4249a</a>)</li>
</ul>
<h2>v17.0.0</h2>
<h3>Features</h3>
<ul>
<li>support <code>reactivityTransform</code> option (<a href="https://github.com/vuejs/vue-loader/commit/e07490ec8b8ac9e00050251d6f0e697fb1f3bf3c">e07490e</a>)</li>
</ul>
<h3>BREAKING CHANGES</h3>
<ul>
<li>remove <code>refSugar</code> option, require <code>vue@^3.2.13</code></li>
</ul>
<h2>v16.8.3</h2>
<h3>Bug Fixes</h3>
<ul>
<li>HMR not working correctly with vue-class-component components (<a href="https://github-redirect.dependabot.com/vuejs/vue-loader/issues/1897">#1897</a>) (<a href="https://github.com/vuejs/vue-loader/commit/76b1448eb227c42e1791a691a86782b7a8cacfc0">76b1448</a>)</li>
</ul>
<h2>v16.8.2</h2>
<h3>Bug Fixes</h3>
<ul>
<li>should allow chaining with loaders for non-vue files (<a href="https://github-redirect.dependabot.com/vuejs/vue-loader/issues/1889">#1889</a>) (<a href="https://github.com/vuejs/vue-loader/commit/f32f9538ea34fc08e1a28622227896241847690f">f32f953</a>), closes <a href="https://github-redirect.dependabot.com/vuejs/vue-loader/issues/1879">#1879</a> <a href="https://github-redirect.dependabot.com/vuejs/vue-loader/issues/1883">#1883</a> <a href="https://github-redirect.dependabot.com/vuejs/vue-loader/issues/1890">#1890</a></li>
<li><strong>plugin:</strong> use compiler.webpack when possible (<a href="https://github-redirect.dependabot.com/vuejs/vue-loader/issues/1884">#1884</a>) (<a href="https://github.com/vuejs/vue-loader/commit/820d23cbf16013dae894e0d84ed9da6e58a37584">820d23c</a>)</li>
</ul>
<h2>v16.8.1</h2>
<h3>Bug Fixes</h3>
<ul>
<li>fix template options resolving for ts (<a href="https://github.com/vuejs/vue-loader/commit/91f581b99644119b68e586a0b642fff3811c8741">91f581b</a>)</li>
</ul>
<h2>v16.8.0</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>hmr:</strong> fix hmr regression (<a href="https://github.com/vuejs/vue-loader/commit/bacc6a9eeca40d6028a2d9a5f6ee02e6c8574abd">bacc6a9</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>
<p>enableTsInTemplate option (<a href="https://github.com/vuejs/vue-loader/commit/7613534954b83489a060860b9525a0d121023c5b">7613534</a>)</p>
<ul>
<li>
<p>When used with <code>ts-loader</code>, due to <code>ts-loader</code>'s cache invalidation behavior, it sometimes prevents the template from being hot-reloaded in isolation, causing the component to reload despite only the template being edited. If this is annoying, you can set this option to <code>false</code> (and avoid using TS expressions in templates).</p>
</li>
<li>
<p>Alternatively, leave this option on (by default) and use <a href="https://github.com/privatenumber/esbuild-loader"><code>esbuild-loader</code></a> to transpile TS instead, which doesn't suffer from this problem (it's also a lot faster). However, do note you will need to rely on TS type checking from other sources (e.g. IDE or <code>vue-tsc</code>).</p>
</li>
</ul>
</li>
</ul>
<h2>v16.7.1</h2>
<h3>Bug Fixes</h3>
<ul>
<li>remove pure annotation for custom blocks (<a href="https://github.com/vuejs/vue-loader/commit/cd891e593bf7f8aff852f1d47fda2337de661bea">cd891e5</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vuejs/vue-loader/blob/next/CHANGELOG.md">vue-loader's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/vuejs/vue-loader/compare/v16.8.3...v17.0.1">17.0.1</a> (2022-10-28)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>add <code>vue</code> and <code>@vue/compiler-sfc</code> to optional peerDependencies (<a href="https://github.com/vuejs/vue-loader/commit/df0ded5356864b9923da8f89ff33db1ae6c2402f">df0ded5</a>), closes <a href="https://github-redirect.dependabot.com/vuejs/vue-loader/issues/1944">#1944</a></li>
<li>merge custom queries rather than appending (<a href="https://github-redirect.dependabot.com/vuejs/vue-loader/issues/1911">#1911</a>) (<a href="https://github.com/vuejs/vue-loader/commit/9e4249a548ceb04ead46fff9b68e9b2676b4c692">9e4249a</a>)</li>
</ul>
<h1><a href="https://github.com/vuejs/vue-loader/compare/v16.8.3...v17.0.0">17.0.0</a> (2021-12-12)</h1>
<h3>Features</h3>
<ul>
<li>support <code>reactivityTransform</code> option (<a href="https://github.com/vuejs/vue-loader/commit/e07490ec8b8ac9e00050251d6f0e697fb1f3bf3c">e07490e</a>)</li>
</ul>
<h3>BREAKING CHANGES</h3>
<ul>
<li>remove <code>refSugar</code> option, require <code>vue@^3.2.13</code></li>
</ul>
<h2><a href="https://github.com/vuejs/vue-loader/compare/v16.8.2...v16.8.3">16.8.3</a> (2021-11-04)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>HMR not working correctly with vue-class-component components (<a href="https://github-redirect.dependabot.com/vuejs/vue-loader/issues/1897">#1897</a>) (<a href="https://github.com/vuejs/vue-loader/commit/76b1448eb227c42e1791a691a86782b7a8cacfc0">76b1448</a>)</li>
</ul>
<h2><a href="https://github.com/vuejs/vue-loader/compare/v16.8.2...v16.8.3">16.8.3</a> (2021-11-04)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>HMR not working correctly with vue-class-component components (<a href="https://github-redirect.dependabot.com/vuejs/vue-loader/issues/1897">#1897</a>) (<a href="https://github.com/vuejs/vue-loader/commit/76b1448eb227c42e1791a691a86782b7a8cacfc0">76b1448</a>)</li>
</ul>
<h2><a href="https://github.com/vuejs/vue-loader/compare/v16.8.1...v16.8.2">16.8.2</a> (2021-10-26)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>should allow chaining with loaders for non-vue files (<a href="https://github-redirect.dependabot.com/vuejs/vue-loader/issues/1889">#1889</a>) (<a href="https://github.com/vuejs/vue-loader/commit/f32f9538ea34fc08e1a28622227896241847690f">f32f953</a>), closes <a href="https://github-redirect.dependabot.com/vuejs/vue-loader/issues/1879">#1879</a> <a href="https://github-redirect.dependabot.com/vuejs/vue-loader/issues/1883">#1883</a> <a href="https://github-redirect.dependabot.com/vuejs/vue-loader/issues/1890">#1890</a></li>
<li><strong>plugin:</strong> use compiler.webpack when possible (<a href="https://github-redirect.dependabot.com/vuejs/vue-loader/issues/1884">#1884</a>) (<a href="https://github.com/vuejs/vue-loader/commit/820d23cbf16013dae894e0d84ed9da6e58a37584">820d23c</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vuejs/vue-loader/commit/75d2b5d5c7d5cc274f6f1440d6c107d6937d4f1f"><code>75d2b5d</code></a> 17.0.1</li>
<li><a href="https://github.com/vuejs/vue-loader/commit/df0ded5356864b9923da8f89ff33db1ae6c2402f"><code>df0ded5</code></a> fix: add <code>vue</code> and <code>@vue/compiler-sfc</code> to optional peerDependencies</li>
<li><a href="https://github.com/vuejs/vue-loader/commit/b3265c918a56f22c9282d97df589ef5f164c6fc1"><code>b3265c9</code></a> chore: add <code>repository</code> property to package.json (<a href="https://github-redirect.dependabot.com/vuejs/vue-loader/issues/1934">#1934</a>)</li>
<li><a href="https://github.com/vuejs/vue-loader/commit/0a023773fd79340492aeb2359c6c673e81cea54d"><code>0a02377</code></a> chore: fix typo (<a href="https://github-redirect.dependabot.com/vuejs/vue-loader/issues/2010">#2010</a>)</li>
<li><a href="https://github.com/vuejs/vue-loader/commit/9e4249a548ceb04ead46fff9b68e9b2676b4c692"><code>9e4249a</code></a> fix: merge custom queries rather than appending (<a href="https://github-redirect.dependabot.com/vuejs/vue-loader/issues/1911">#1911</a>)</li>
<li><a href="https://github.com/vuejs/vue-loader/commit/6a293dff5f2ed3167eb3b448f1d714091185a44e"><code>6a293df</code></a> chore: changelog [ci skip]</li>
<li><a href="https://github.com/vuejs/vue-loader/commit/e5c7ab41b77e193054b34b8b719e8cfce3b9e4f2"><code>e5c7ab4</code></a> v17.0.0</li>
<li><a href="https://github.com/vuejs/vue-loader/commit/e9314347d75a1b0e54f971272d23a669fc3e6965"><code>e931434</code></a> chore: lockfile</li>
<li><a href="https://github.com/vuejs/vue-loader/commit/e07490ec8b8ac9e00050251d6f0e697fb1f3bf3c"><code>e07490e</code></a> feat: support <code>reactivityTransform</code> option</li>
<li><a href="https://github.com/vuejs/vue-loader/commit/b391b04ed3335a2d2c9010101d98c2d9977626e8"><code>b391b04</code></a> chore: remove unncessary log</li>
<li>Additional commits viewable in <a href="https://github.com/vuejs/vue-loader/compare/v15.9.8...v17.0.1">compare view</a></li>
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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-toolbox/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-02 06:38:14 +0000 UTC
    </div>
</div>

