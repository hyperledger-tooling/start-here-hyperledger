---
layout: default
title: besu-docs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu-docs
---

# besu-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1448" class=".btn">#1448</a>
            </td>
            <td>
                <b>
                    Bump got, @docusaurus/core, @docusaurus/plugin-client-redirects, @docusaurus/plugin-content-docs, @docusaurus/plugin-google-gtag, @docusaurus/plugin-google-tag-manager, @docusaurus/preset-classic, @docusaurus/theme-common, @easyops-cn/docusaurus-search-local and redocusaurus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [got](https://github.com/sindresorhus/got) to 12.6.1 and updates ancestor dependencies [got](https://github.com/sindresorhus/got), [@docusaurus/core](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus), [@docusaurus/plugin-client-redirects](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects), [@docusaurus/plugin-content-docs](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-content-docs), [@docusaurus/plugin-google-gtag](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-google-gtag), [@docusaurus/plugin-google-tag-manager](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-google-tag-manager), [@docusaurus/preset-classic](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-preset-classic), [@docusaurus/theme-common](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-theme-common), [@easyops-cn/docusaurus-search-local](https://github.com/easyops-cn/docusaurus-search-local) and [redocusaurus](https://github.com/rohit-gohri/redocusaurus). These dependencies need to be updated together.

Updates `got` from 9.6.0 to 12.6.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sindresorhus/got/releases">got's releases</a>.</em></p>
<blockquote>
<h2>v12.6.1</h2>
<ul>
<li>Fix <code>get-stream</code> import statement (<a href="https://redirect.github.com/sindresorhus/got/issues/2266">#2266</a>)  67d5039</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.6.0...v12.6.1">https://github.com/sindresorhus/got/compare/v12.6.0...v12.6.1</a></p>
<h2>v12.6.0</h2>
<ul>
<li>Update dependencies  88c88fb 979272e</li>
<li>Loosen URL validation strictness (<a href="https://redirect.github.com/sindresorhus/got/issues/2200">#2200</a>)  0ca0b7f</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.5.3...v12.6.0">https://github.com/sindresorhus/got/compare/v12.5.3...v12.6.0</a></p>
<h2>v12.5.3</h2>
<ul>
<li>Fix abort event listeners not always being cleaned up (<a href="https://redirect.github.com/sindresorhus/got/issues/2162">#2162</a>)  3cc40b5</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.5.2...v12.5.3">https://github.com/sindresorhus/got/compare/v12.5.2...v12.5.3</a></p>
<h2>v12.5.2</h2>
<ul>
<li>Improve TypeScript 4.9 compatibility (<a href="https://redirect.github.com/sindresorhus/got/issues/2163">#2163</a>)  39f83b6</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.5.1...v12.5.2">https://github.com/sindresorhus/got/compare/v12.5.1...v12.5.2</a></p>
<h2>v12.5.1</h2>
<ul>
<li>Fix compatibility with TypeScript and ESM  3b3ea67</li>
<li>Fix request body not being properly cached (<a href="https://redirect.github.com/sindresorhus/got/issues/2150">#2150</a>)  3e9d3af</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.5.0...v12.5.1">https://github.com/sindresorhus/got/compare/v12.5.0...v12.5.1</a></p>
<h2>v12.5.0</h2>
<ul>
<li>Disable method rewriting on 307 and 308 status codes (<a href="https://redirect.github.com/sindresorhus/got/issues/2145">#2145</a>)  e049e94</li>
<li>Upgrade dependencies  8630815 f0ac0b3 4c3762a</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.4.1...v12.5.0">https://github.com/sindresorhus/got/compare/v12.4.1...v12.5.0</a></p>
<h2>v12.4.1</h2>
<h3>Fixes</h3>
<ul>
<li>Fix <code>options.context</code> being not extensible b671480715dbbff908e9a385f5e714570c663cd7</li>
<li>Don't emit <code>uploadProgress</code> after promise cancelation 693de217b030816f574d6e4cb505ee2e77b21c29</li>
</ul>
<p><a href="https://github.com/sindresorhus/got/compare/v12.4.0...v12.4.1">https://github.com/sindresorhus/got/compare/v12.4.0...v12.4.1</a></p>
<h2>v12.4.0</h2>
<h3>Improvements</h3>
<ul>
<li>Support FormData without known length (<a href="https://redirect.github.com/sindresorhus/got/issues/2120">#2120</a>)  850773c</li>
</ul>
<h3>Fixes</h3>
<ul>
<li>Don&amp;<a href="https://redirect.github.com/sindresorhus/got/issues/39">#39</a>;t call <code>beforeError</code> hooks with <code>HTTPError</code> if the <code>throwHttpErrors</code> option is <code>false</code> (<a href="https://redirect.github.com/sindresorhus/got/issues/2104">#2104</a>)  3927348</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sindresorhus/got/commit/c405f5407863ef8faca3af397204d6f192a56320"><code>c405f54</code></a> 12.6.1</li>
<li><a href="https://github.com/sindresorhus/got/commit/67d5039ff5a5518489529f9706199234e9b64ad6"><code>67d5039</code></a> Fix <code>get-stream</code> import statement (<a href="https://redirect.github.com/sindresorhus/got/issues/2266">#2266</a>)</li>
<li><a href="https://github.com/sindresorhus/got/commit/469a45554ff29ca13050a2714eabaaec9f7160f7"><code>469a455</code></a> Meta tweaks</li>
<li><a href="https://github.com/sindresorhus/got/commit/8f77e8d07d8684cde95d351feafaa308b466dff4"><code>8f77e8d</code></a> Fix readme &quot;axios bugs&quot; urls (<a href="https://redirect.github.com/sindresorhus/got/issues/2253">#2253</a>)</li>
<li><a href="https://github.com/sindresorhus/got/commit/af928f6d3974d7106718d37acc6bd1d33d2cec70"><code>af928f6</code></a> Fix type error on build (<a href="https://redirect.github.com/sindresorhus/got/issues/2251">#2251</a>)</li>
<li><a href="https://github.com/sindresorhus/got/commit/702ed352ac5d8527deaf4a5821d0274afc56e9d8"><code>702ed35</code></a> Meta tweaks</li>
<li><a href="https://github.com/sindresorhus/got/commit/e4460f771b7acff845a2ca6f6de3f7693faa406d"><code>e4460f7</code></a> Add failing tests for <a href="https://redirect.github.com/sindresorhus/got/issues/2170">#2170</a> (<a href="https://redirect.github.com/sindresorhus/got/issues/2171">#2171</a>)</li>
<li><a href="https://github.com/sindresorhus/got/commit/13a68d36e0f6aed98cf39269e597489da5480c00"><code>13a68d3</code></a> 12.6.0</li>
<li><a href="https://github.com/sindresorhus/got/commit/88c88fbc469683dad33d418681cb7017d0e9fcbf"><code>88c88fb</code></a> Update dependencies</li>
<li><a href="https://github.com/sindresorhus/got/commit/0ca0b7f7134f41b45a51370154041cc97c28ca60"><code>0ca0b7f</code></a> Do not enforce newest URI rules on URLs (<a href="https://redirect.github.com/sindresorhus/got/issues/2200">#2200</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/sindresorhus/got/compare/v9.6.0...v12.6.1">compare view</a></li>
</ul>
</details>
<br />

Updates `@docusaurus/core` from 2.4.3 to 3.0.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/facebook/docusaurus/releases"><code>@​docusaurus/core</code>'s releases</a>.</em></p>
<blockquote>
<h2>3.0.0 (2023-10-31)</h2>
<ul>
<li>GitHub PR: <a href="https://redirect.github.com/facebook/docusaurus/pull/9478">facebook/docusaurus#9478</a></li>
<li>GitHub release notes: <a href="https://github.com/facebook/docusaurus/releases/tag/v3.0.0">https://github.com/facebook/docusaurus/releases/tag/v3.0.0</a></li>
<li>GitHub release discussion: <a href="https://github.com/facebook/docusaurus/discussions/9481">https://github.com/facebook/docusaurus/discussions/9481</a></li>
<li>Upgrade guide: <a href="https://docusaurus.io/docs/migration/v3">docusaurus.io/docs/migration/v3</a></li>
</ul>
<h4>:boom: Breaking Change</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9316">#9316</a> chore: upgrade syntax highlighting dependencies, <code>prism-react-renderer</code> to v2, <code>react-live</code> to v4 (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-cssnano-preset</code>, <code>docusaurus-logger</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-theme-translations</code>, <code>docusaurus-utils-common</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>, <code>eslint-plugin</code>, <code>lqip-loader</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9348">#9348</a> chore: update node engine version 18 (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9310">#9310</a> chore(plugin-docs): remove legacy versioned prefix on doc ids and sidebar names in versioned sidebars (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9308">#9308</a> fix(theme): make warning a first-class admonition, and deprecate caution admonition (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-tsconfig</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9258">#9258</a> feat: Docusaurus v3 upgrades and require TypeScript 5 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-blog</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9189">#9189</a> feat(blog-plugin): limit option for blog feedOptions (<a href="https://github.com/johnnyreilly"><code>@​johnnyreilly</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-tsconfig</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9050">#9050</a> feat: create official TypeScript base config <code>@​docusaurus/tsconfig</code> (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-module-type-aliases</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-types</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8961">#8961</a> feat: React 18 + automatic JSX runtime + build --dev (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9026">#9026</a> chore: remove facebook template (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-types</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8288">#8288</a> feat: upgrade to MDX v2 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/7966">#7966</a> fix(plugin-docs,theme): refactor docs plugin routes and component tree (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:rocket: New Feature</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-mdx-loader</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9394">#9394</a> feat(mdx-loader): Remark plugin to report unused MDX / Markdown directives (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9241">#9241</a> feat: support bun package manager in <code>create-docusaurus</code> (<a href="https://github.com/colinhacks"><code>@​colinhacks</code></a>)</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/facebook/docusaurus/blob/main/CHANGELOG.md"><code>@​docusaurus/core</code>'s changelog</a>.</em></p>
<blockquote>
<h2>3.0.0 (2023-10-31)</h2>
<h4>:boom: Breaking Change</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9316">#9316</a> chore: upgrade syntax highlighting dependencies, <code>prism-react-renderer</code> to v2, <code>react-live</code> to v4 (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-cssnano-preset</code>, <code>docusaurus-logger</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-theme-translations</code>, <code>docusaurus-utils-common</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>, <code>eslint-plugin</code>, <code>lqip-loader</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9348">#9348</a> chore: update node engine version 18 (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9310">#9310</a> chore(plugin-docs): remove legacy versioned prefix on doc ids and sidebar names in versioned sidebars (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9308">#9308</a> fix(theme): make warning a first-class admonition, and deprecate caution admonition (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-tsconfig</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9258">#9258</a> feat: Docusaurus v3 upgrades and require TypeScript 5 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-blog</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9189">#9189</a> feat(blog-plugin): limit option for blog feedOptions (<a href="https://github.com/johnnyreilly"><code>@​johnnyreilly</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-tsconfig</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9050">#9050</a> feat: create official TypeScript base config <code>@​docusaurus/tsconfig</code> (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-module-type-aliases</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-types</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8961">#8961</a> feat: React 18 + automatic JSX runtime + build --dev (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9026">#9026</a> chore: remove facebook template (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-types</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8288">#8288</a> feat: upgrade to MDX v2 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/7966">#7966</a> fix(plugin-docs,theme): refactor docs plugin routes and component tree (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:rocket: New Feature</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-mdx-loader</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9394">#9394</a> feat(mdx-loader): Remark plugin to report unused MDX / Markdown directives (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9241">#9241</a> feat: support bun package manager in <code>create-docusaurus</code> (<a href="https://github.com/colinhacks"><code>@​colinhacks</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-blog</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9189">#9189</a> feat(blog-plugin): limit option for blog feedOptions (<a href="https://github.com/johnnyreilly"><code>@​johnnyreilly</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9152">#9152</a> feat(theme): add support for meta og locale and alternates (<a href="https://github.com/FlorinaPacurar"><code>@​FlorinaPacurar</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9028">#9028</a> feat(theme): add ability to inject data attributes from query-string - possibility to create an iframe/embed variant of a page (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
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
<li><a href="https://github.com/facebook/docusaurus/commit/ca8b4638c47119d38838656c4a11ee3a5e7ba6f2"><code>ca8b463</code></a> v3.0.0</li>
<li><a href="https://github.com/facebook/docusaurus/commit/495c7936b605e6b8881f000d23a8463a9d6d850c"><code>495c793</code></a> chore: v3.0.0-rc.1 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/9453">#9453</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/7ee2f75ce1e645f75ae42b9f2f7f76cfc45b1743"><code>7ee2f75</code></a> chore: v3.0.0-rc.0 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/9418">#9418</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/45f1a669b5ab29a04365f20e88e37e085c0fb4de"><code>45f1a66</code></a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/9317">#9317</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/643a7fe5a325dacfd1d809a1f40a9688e9634fa7"><code>643a7fe</code></a> fix(core): log missing errorInfo in React 18 onRecoverableError callback (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/9387">#9387</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/1319996083a2becf38967a99f6db290c1d5c99cb"><code>1319996</code></a> feat(core): throw error when official docusaurus dependencies use different v...</li>
<li><a href="https://github.com/facebook/docusaurus/commit/dceaae41d7f3fc148a2d2240a3c89e0e9c22aa4c"><code>dceaae4</code></a> chore: upgrade syntax highlighting dependencies, <code>prism-react-renderer</code> to v2...</li>
<li><a href="https://github.com/facebook/docusaurus/commit/bde9cfd84d99ea1ca8fc59bf51f9d4001d6527f2"><code>bde9cfd</code></a> chore: update node engine version 18 (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/9348">#9348</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/52d79c4e0cf8876903aa079cf8cbcd46f265505a"><code>52d79c4</code></a> chore: v3.0.0-beta.0 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/9311">#9311</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/6e8e276e406e24c46bf34385dd47ebd2e44bc152"><code>6e8e276</code></a> fix(cli): disable vertical borders of the update notification (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/9309">#9309</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/facebook/docusaurus/commits/v3.0.0/packages/docusaurus">compare view</a></li>
</ul>
</details>
<br />

Updates `@docusaurus/plugin-client-redirects` from 2.4.3 to 3.0.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/facebook/docusaurus/releases"><code>@​docusaurus/plugin-client-redirects</code>'s releases</a>.</em></p>
<blockquote>
<h2>3.0.0 (2023-10-31)</h2>
<ul>
<li>GitHub PR: <a href="https://redirect.github.com/facebook/docusaurus/pull/9478">facebook/docusaurus#9478</a></li>
<li>GitHub release notes: <a href="https://github.com/facebook/docusaurus/releases/tag/v3.0.0">https://github.com/facebook/docusaurus/releases/tag/v3.0.0</a></li>
<li>GitHub release discussion: <a href="https://github.com/facebook/docusaurus/discussions/9481">https://github.com/facebook/docusaurus/discussions/9481</a></li>
<li>Upgrade guide: <a href="https://docusaurus.io/docs/migration/v3">docusaurus.io/docs/migration/v3</a></li>
</ul>
<h4>:boom: Breaking Change</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9316">#9316</a> chore: upgrade syntax highlighting dependencies, <code>prism-react-renderer</code> to v2, <code>react-live</code> to v4 (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-cssnano-preset</code>, <code>docusaurus-logger</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-theme-translations</code>, <code>docusaurus-utils-common</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>, <code>eslint-plugin</code>, <code>lqip-loader</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9348">#9348</a> chore: update node engine version 18 (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9310">#9310</a> chore(plugin-docs): remove legacy versioned prefix on doc ids and sidebar names in versioned sidebars (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9308">#9308</a> fix(theme): make warning a first-class admonition, and deprecate caution admonition (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-tsconfig</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9258">#9258</a> feat: Docusaurus v3 upgrades and require TypeScript 5 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-blog</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9189">#9189</a> feat(blog-plugin): limit option for blog feedOptions (<a href="https://github.com/johnnyreilly"><code>@​johnnyreilly</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-tsconfig</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9050">#9050</a> feat: create official TypeScript base config <code>@​docusaurus/tsconfig</code> (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-module-type-aliases</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-types</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8961">#8961</a> feat: React 18 + automatic JSX runtime + build --dev (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9026">#9026</a> chore: remove facebook template (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-types</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8288">#8288</a> feat: upgrade to MDX v2 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/7966">#7966</a> fix(plugin-docs,theme): refactor docs plugin routes and component tree (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:rocket: New Feature</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-mdx-loader</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9394">#9394</a> feat(mdx-loader): Remark plugin to report unused MDX / Markdown directives (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9241">#9241</a> feat: support bun package manager in <code>create-docusaurus</code> (<a href="https://github.com/colinhacks"><code>@​colinhacks</code></a>)</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/facebook/docusaurus/blob/main/CHANGELOG.md"><code>@​docusaurus/plugin-client-redirects</code>'s changelog</a>.</em></p>
<blockquote>
<h2>3.0.0 (2023-10-31)</h2>
<h4>:boom: Breaking Change</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9316">#9316</a> chore: upgrade syntax highlighting dependencies, <code>prism-react-renderer</code> to v2, <code>react-live</code> to v4 (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-cssnano-preset</code>, <code>docusaurus-logger</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-theme-translations</code>, <code>docusaurus-utils-common</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>, <code>eslint-plugin</code>, <code>lqip-loader</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9348">#9348</a> chore: update node engine version 18 (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9310">#9310</a> chore(plugin-docs): remove legacy versioned prefix on doc ids and sidebar names in versioned sidebars (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9308">#9308</a> fix(theme): make warning a first-class admonition, and deprecate caution admonition (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-tsconfig</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9258">#9258</a> feat: Docusaurus v3 upgrades and require TypeScript 5 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-blog</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9189">#9189</a> feat(blog-plugin): limit option for blog feedOptions (<a href="https://github.com/johnnyreilly"><code>@​johnnyreilly</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-tsconfig</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9050">#9050</a> feat: create official TypeScript base config <code>@​docusaurus/tsconfig</code> (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-module-type-aliases</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-types</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8961">#8961</a> feat: React 18 + automatic JSX runtime + build --dev (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9026">#9026</a> chore: remove facebook template (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-types</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8288">#8288</a> feat: upgrade to MDX v2 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/7966">#7966</a> fix(plugin-docs,theme): refactor docs plugin routes and component tree (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:rocket: New Feature</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-mdx-loader</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9394">#9394</a> feat(mdx-loader): Remark plugin to report unused MDX / Markdown directives (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9241">#9241</a> feat: support bun package manager in <code>create-docusaurus</code> (<a href="https://github.com/colinhacks"><code>@​colinhacks</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-blog</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9189">#9189</a> feat(blog-plugin): limit option for blog feedOptions (<a href="https://github.com/johnnyreilly"><code>@​johnnyreilly</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9152">#9152</a> feat(theme): add support for meta og locale and alternates (<a href="https://github.com/FlorinaPacurar"><code>@​FlorinaPacurar</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9028">#9028</a> feat(theme): add ability to inject data attributes from query-string - possibility to create an iframe/embed variant of a page (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
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
<li><a href="https://github.com/facebook/docusaurus/commit/ca8b4638c47119d38838656c4a11ee3a5e7ba6f2"><code>ca8b463</code></a> v3.0.0</li>
<li><a href="https://github.com/facebook/docusaurus/commit/495c7936b605e6b8881f000d23a8463a9d6d850c"><code>495c793</code></a> chore: v3.0.0-rc.1 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects/issues/9453">#9453</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/7ee2f75ce1e645f75ae42b9f2f7f76cfc45b1743"><code>7ee2f75</code></a> chore: v3.0.0-rc.0 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects/issues/9418">#9418</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/bde9cfd84d99ea1ca8fc59bf51f9d4001d6527f2"><code>bde9cfd</code></a> chore: update node engine version 18 (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects/issues/9348">#9348</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/52d79c4e0cf8876903aa079cf8cbcd46f265505a"><code>52d79c4</code></a> chore: v3.0.0-beta.0 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects/issues/9311">#9311</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/a59aead1e2732a6d7ceb83f881c0945abca4d696"><code>a59aead</code></a> chore: attempt to fix Crowdin issues (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects/issues/9220">#9220</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/09ea3bcfab029daebd75b057221e5339da28f00b"><code>09ea3bc</code></a> feat(client-redirects-plugin): support fully qualified urls and querystring/h...</li>
<li><a href="https://github.com/facebook/docusaurus/commit/ff227283d232acbde1fb902f4dbf0aec879956a2"><code>ff22728</code></a> chore: upgrade dependencies (non-major) (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects/issues/9148">#9148</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/7d033cc8c08e0c8fd57baff7390540def6eb6046"><code>7d033cc</code></a> chore: v3.0.0-alpha.0 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects/issues/9072">#9072</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/187e5aa218e764b06dcbbb50f22ced72159a8532"><code>187e5aa</code></a> feat: React 18 + automatic JSX runtime + build --dev (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects/issues/8961">#8961</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/facebook/docusaurus/commits/v3.0.0/packages/docusaurus-plugin-client-redirects">compare view</a></li>
</ul>
</details>
<br />

Updates `@docusaurus/plugin-content-docs` from 2.4.3 to 3.0.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/facebook/docusaurus/releases"><code>@​docusaurus/plugin-content-docs</code>'s releases</a>.</em></p>
<blockquote>
<h2>3.0.0 (2023-10-31)</h2>
<ul>
<li>GitHub PR: <a href="https://redirect.github.com/facebook/docusaurus/pull/9478">facebook/docusaurus#9478</a></li>
<li>GitHub release notes: <a href="https://github.com/facebook/docusaurus/releases/tag/v3.0.0">https://github.com/facebook/docusaurus/releases/tag/v3.0.0</a></li>
<li>GitHub release discussion: <a href="https://github.com/facebook/docusaurus/discussions/9481">https://github.com/facebook/docusaurus/discussions/9481</a></li>
<li>Upgrade guide: <a href="https://docusaurus.io/docs/migration/v3">docusaurus.io/docs/migration/v3</a></li>
</ul>
<h4>:boom: Breaking Change</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9316">#9316</a> chore: upgrade syntax highlighting dependencies, <code>prism-react-renderer</code> to v2, <code>react-live</code> to v4 (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-cssnano-preset</code>, <code>docusaurus-logger</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-theme-translations</code>, <code>docusaurus-utils-common</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>, <code>eslint-plugin</code>, <code>lqip-loader</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9348">#9348</a> chore: update node engine version 18 (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9310">#9310</a> chore(plugin-docs): remove legacy versioned prefix on doc ids and sidebar names in versioned sidebars (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9308">#9308</a> fix(theme): make warning a first-class admonition, and deprecate caution admonition (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-tsconfig</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9258">#9258</a> feat: Docusaurus v3 upgrades and require TypeScript 5 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-blog</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9189">#9189</a> feat(blog-plugin): limit option for blog feedOptions (<a href="https://github.com/johnnyreilly"><code>@​johnnyreilly</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-tsconfig</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9050">#9050</a> feat: create official TypeScript base config <code>@​docusaurus/tsconfig</code> (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-module-type-aliases</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-types</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8961">#8961</a> feat: React 18 + automatic JSX runtime + build --dev (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9026">#9026</a> chore: remove facebook template (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-types</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8288">#8288</a> feat: upgrade to MDX v2 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/7966">#7966</a> fix(plugin-docs,theme): refactor docs plugin routes and component tree (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:rocket: New Feature</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-mdx-loader</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9394">#9394</a> feat(mdx-loader): Remark plugin to report unused MDX / Markdown directives (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9241">#9241</a> feat: support bun package manager in <code>create-docusaurus</code> (<a href="https://github.com/colinhacks"><code>@​colinhacks</code></a>)</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/facebook/docusaurus/blob/main/CHANGELOG.md"><code>@​docusaurus/plugin-content-docs</code>'s changelog</a>.</em></p>
<blockquote>
<h2>3.0.0 (2023-10-31)</h2>
<h4>:boom: Breaking Change</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><...

_Description has been truncated_
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-16 15:04:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1447" class=".btn">#1447</a>
            </td>
            <td>
                <b>
                    Bump trim, @docusaurus/core, @docusaurus/plugin-client-redirects, @docusaurus/plugin-content-docs, @docusaurus/plugin-google-gtag, @docusaurus/plugin-google-tag-manager, @docusaurus/preset-classic, @docusaurus/theme-common, @easyops-cn/docusaurus-search-local and redocusaurus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Removes [trim](https://github.com/Trott/trim). It's no longer used after updating ancestor dependencies [trim](https://github.com/Trott/trim), [@docusaurus/core](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus), [@docusaurus/plugin-client-redirects](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects), [@docusaurus/plugin-content-docs](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-content-docs), [@docusaurus/plugin-google-gtag](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-google-gtag), [@docusaurus/plugin-google-tag-manager](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-google-tag-manager), [@docusaurus/preset-classic](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-preset-classic), [@docusaurus/theme-common](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-theme-common), [@easyops-cn/docusaurus-search-local](https://github.com/easyops-cn/docusaurus-search-local) and [redocusaurus](https://github.com/rohit-gohri/redocusaurus). These dependencies need to be updated together.

Removes `trim`

Updates `@docusaurus/core` from 2.4.3 to 3.0.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/facebook/docusaurus/releases"><code>@​docusaurus/core</code>'s releases</a>.</em></p>
<blockquote>
<h2>3.0.0 (2023-10-31)</h2>
<ul>
<li>GitHub PR: <a href="https://redirect.github.com/facebook/docusaurus/pull/9478">facebook/docusaurus#9478</a></li>
<li>GitHub release notes: <a href="https://github.com/facebook/docusaurus/releases/tag/v3.0.0">https://github.com/facebook/docusaurus/releases/tag/v3.0.0</a></li>
<li>GitHub release discussion: <a href="https://github.com/facebook/docusaurus/discussions/9481">https://github.com/facebook/docusaurus/discussions/9481</a></li>
<li>Upgrade guide: <a href="https://docusaurus.io/docs/migration/v3">docusaurus.io/docs/migration/v3</a></li>
</ul>
<h4>:boom: Breaking Change</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9316">#9316</a> chore: upgrade syntax highlighting dependencies, <code>prism-react-renderer</code> to v2, <code>react-live</code> to v4 (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-cssnano-preset</code>, <code>docusaurus-logger</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-theme-translations</code>, <code>docusaurus-utils-common</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>, <code>eslint-plugin</code>, <code>lqip-loader</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9348">#9348</a> chore: update node engine version 18 (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9310">#9310</a> chore(plugin-docs): remove legacy versioned prefix on doc ids and sidebar names in versioned sidebars (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9308">#9308</a> fix(theme): make warning a first-class admonition, and deprecate caution admonition (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-tsconfig</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9258">#9258</a> feat: Docusaurus v3 upgrades and require TypeScript 5 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-blog</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9189">#9189</a> feat(blog-plugin): limit option for blog feedOptions (<a href="https://github.com/johnnyreilly"><code>@​johnnyreilly</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-tsconfig</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9050">#9050</a> feat: create official TypeScript base config <code>@​docusaurus/tsconfig</code> (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-module-type-aliases</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-types</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8961">#8961</a> feat: React 18 + automatic JSX runtime + build --dev (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9026">#9026</a> chore: remove facebook template (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-types</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8288">#8288</a> feat: upgrade to MDX v2 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/7966">#7966</a> fix(plugin-docs,theme): refactor docs plugin routes and component tree (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:rocket: New Feature</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-mdx-loader</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9394">#9394</a> feat(mdx-loader): Remark plugin to report unused MDX / Markdown directives (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9241">#9241</a> feat: support bun package manager in <code>create-docusaurus</code> (<a href="https://github.com/colinhacks"><code>@​colinhacks</code></a>)</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/facebook/docusaurus/blob/main/CHANGELOG.md"><code>@​docusaurus/core</code>'s changelog</a>.</em></p>
<blockquote>
<h2>3.0.0 (2023-10-31)</h2>
<h4>:boom: Breaking Change</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9316">#9316</a> chore: upgrade syntax highlighting dependencies, <code>prism-react-renderer</code> to v2, <code>react-live</code> to v4 (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-cssnano-preset</code>, <code>docusaurus-logger</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-theme-translations</code>, <code>docusaurus-utils-common</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>, <code>eslint-plugin</code>, <code>lqip-loader</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9348">#9348</a> chore: update node engine version 18 (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9310">#9310</a> chore(plugin-docs): remove legacy versioned prefix on doc ids and sidebar names in versioned sidebars (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9308">#9308</a> fix(theme): make warning a first-class admonition, and deprecate caution admonition (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-tsconfig</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9258">#9258</a> feat: Docusaurus v3 upgrades and require TypeScript 5 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-blog</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9189">#9189</a> feat(blog-plugin): limit option for blog feedOptions (<a href="https://github.com/johnnyreilly"><code>@​johnnyreilly</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-tsconfig</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9050">#9050</a> feat: create official TypeScript base config <code>@​docusaurus/tsconfig</code> (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-module-type-aliases</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-types</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8961">#8961</a> feat: React 18 + automatic JSX runtime + build --dev (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9026">#9026</a> chore: remove facebook template (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-types</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8288">#8288</a> feat: upgrade to MDX v2 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/7966">#7966</a> fix(plugin-docs,theme): refactor docs plugin routes and component tree (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:rocket: New Feature</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-mdx-loader</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9394">#9394</a> feat(mdx-loader): Remark plugin to report unused MDX / Markdown directives (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9241">#9241</a> feat: support bun package manager in <code>create-docusaurus</code> (<a href="https://github.com/colinhacks"><code>@​colinhacks</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-blog</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9189">#9189</a> feat(blog-plugin): limit option for blog feedOptions (<a href="https://github.com/johnnyreilly"><code>@​johnnyreilly</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9152">#9152</a> feat(theme): add support for meta og locale and alternates (<a href="https://github.com/FlorinaPacurar"><code>@​FlorinaPacurar</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9028">#9028</a> feat(theme): add ability to inject data attributes from query-string - possibility to create an iframe/embed variant of a page (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
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
<li><a href="https://github.com/facebook/docusaurus/commit/ca8b4638c47119d38838656c4a11ee3a5e7ba6f2"><code>ca8b463</code></a> v3.0.0</li>
<li><a href="https://github.com/facebook/docusaurus/commit/495c7936b605e6b8881f000d23a8463a9d6d850c"><code>495c793</code></a> chore: v3.0.0-rc.1 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/9453">#9453</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/7ee2f75ce1e645f75ae42b9f2f7f76cfc45b1743"><code>7ee2f75</code></a> chore: v3.0.0-rc.0 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/9418">#9418</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/45f1a669b5ab29a04365f20e88e37e085c0fb4de"><code>45f1a66</code></a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/9317">#9317</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/643a7fe5a325dacfd1d809a1f40a9688e9634fa7"><code>643a7fe</code></a> fix(core): log missing errorInfo in React 18 onRecoverableError callback (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/9387">#9387</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/1319996083a2becf38967a99f6db290c1d5c99cb"><code>1319996</code></a> feat(core): throw error when official docusaurus dependencies use different v...</li>
<li><a href="https://github.com/facebook/docusaurus/commit/dceaae41d7f3fc148a2d2240a3c89e0e9c22aa4c"><code>dceaae4</code></a> chore: upgrade syntax highlighting dependencies, <code>prism-react-renderer</code> to v2...</li>
<li><a href="https://github.com/facebook/docusaurus/commit/bde9cfd84d99ea1ca8fc59bf51f9d4001d6527f2"><code>bde9cfd</code></a> chore: update node engine version 18 (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/9348">#9348</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/52d79c4e0cf8876903aa079cf8cbcd46f265505a"><code>52d79c4</code></a> chore: v3.0.0-beta.0 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/9311">#9311</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/6e8e276e406e24c46bf34385dd47ebd2e44bc152"><code>6e8e276</code></a> fix(cli): disable vertical borders of the update notification (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/9309">#9309</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/facebook/docusaurus/commits/v3.0.0/packages/docusaurus">compare view</a></li>
</ul>
</details>
<br />

Updates `@docusaurus/plugin-client-redirects` from 2.4.3 to 3.0.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/facebook/docusaurus/releases"><code>@​docusaurus/plugin-client-redirects</code>'s releases</a>.</em></p>
<blockquote>
<h2>3.0.0 (2023-10-31)</h2>
<ul>
<li>GitHub PR: <a href="https://redirect.github.com/facebook/docusaurus/pull/9478">facebook/docusaurus#9478</a></li>
<li>GitHub release notes: <a href="https://github.com/facebook/docusaurus/releases/tag/v3.0.0">https://github.com/facebook/docusaurus/releases/tag/v3.0.0</a></li>
<li>GitHub release discussion: <a href="https://github.com/facebook/docusaurus/discussions/9481">https://github.com/facebook/docusaurus/discussions/9481</a></li>
<li>Upgrade guide: <a href="https://docusaurus.io/docs/migration/v3">docusaurus.io/docs/migration/v3</a></li>
</ul>
<h4>:boom: Breaking Change</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9316">#9316</a> chore: upgrade syntax highlighting dependencies, <code>prism-react-renderer</code> to v2, <code>react-live</code> to v4 (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-cssnano-preset</code>, <code>docusaurus-logger</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-theme-translations</code>, <code>docusaurus-utils-common</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>, <code>eslint-plugin</code>, <code>lqip-loader</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9348">#9348</a> chore: update node engine version 18 (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9310">#9310</a> chore(plugin-docs): remove legacy versioned prefix on doc ids and sidebar names in versioned sidebars (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9308">#9308</a> fix(theme): make warning a first-class admonition, and deprecate caution admonition (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-tsconfig</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9258">#9258</a> feat: Docusaurus v3 upgrades and require TypeScript 5 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-blog</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9189">#9189</a> feat(blog-plugin): limit option for blog feedOptions (<a href="https://github.com/johnnyreilly"><code>@​johnnyreilly</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-tsconfig</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9050">#9050</a> feat: create official TypeScript base config <code>@​docusaurus/tsconfig</code> (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-module-type-aliases</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-types</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8961">#8961</a> feat: React 18 + automatic JSX runtime + build --dev (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9026">#9026</a> chore: remove facebook template (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-types</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8288">#8288</a> feat: upgrade to MDX v2 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/7966">#7966</a> fix(plugin-docs,theme): refactor docs plugin routes and component tree (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:rocket: New Feature</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-mdx-loader</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9394">#9394</a> feat(mdx-loader): Remark plugin to report unused MDX / Markdown directives (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9241">#9241</a> feat: support bun package manager in <code>create-docusaurus</code> (<a href="https://github.com/colinhacks"><code>@​colinhacks</code></a>)</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/facebook/docusaurus/blob/main/CHANGELOG.md"><code>@​docusaurus/plugin-client-redirects</code>'s changelog</a>.</em></p>
<blockquote>
<h2>3.0.0 (2023-10-31)</h2>
<h4>:boom: Breaking Change</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9316">#9316</a> chore: upgrade syntax highlighting dependencies, <code>prism-react-renderer</code> to v2, <code>react-live</code> to v4 (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-cssnano-preset</code>, <code>docusaurus-logger</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-theme-translations</code>, <code>docusaurus-utils-common</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>, <code>eslint-plugin</code>, <code>lqip-loader</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9348">#9348</a> chore: update node engine version 18 (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9310">#9310</a> chore(plugin-docs): remove legacy versioned prefix on doc ids and sidebar names in versioned sidebars (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9308">#9308</a> fix(theme): make warning a first-class admonition, and deprecate caution admonition (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-tsconfig</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9258">#9258</a> feat: Docusaurus v3 upgrades and require TypeScript 5 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-blog</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9189">#9189</a> feat(blog-plugin): limit option for blog feedOptions (<a href="https://github.com/johnnyreilly"><code>@​johnnyreilly</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-tsconfig</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9050">#9050</a> feat: create official TypeScript base config <code>@​docusaurus/tsconfig</code> (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-module-type-aliases</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-types</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8961">#8961</a> feat: React 18 + automatic JSX runtime + build --dev (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9026">#9026</a> chore: remove facebook template (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-types</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8288">#8288</a> feat: upgrade to MDX v2 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/7966">#7966</a> fix(plugin-docs,theme): refactor docs plugin routes and component tree (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:rocket: New Feature</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-mdx-loader</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9394">#9394</a> feat(mdx-loader): Remark plugin to report unused MDX / Markdown directives (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9241">#9241</a> feat: support bun package manager in <code>create-docusaurus</code> (<a href="https://github.com/colinhacks"><code>@​colinhacks</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-blog</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9189">#9189</a> feat(blog-plugin): limit option for blog feedOptions (<a href="https://github.com/johnnyreilly"><code>@​johnnyreilly</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9152">#9152</a> feat(theme): add support for meta og locale and alternates (<a href="https://github.com/FlorinaPacurar"><code>@​FlorinaPacurar</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9028">#9028</a> feat(theme): add ability to inject data attributes from query-string - possibility to create an iframe/embed variant of a page (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
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
<li><a href="https://github.com/facebook/docusaurus/commit/ca8b4638c47119d38838656c4a11ee3a5e7ba6f2"><code>ca8b463</code></a> v3.0.0</li>
<li><a href="https://github.com/facebook/docusaurus/commit/495c7936b605e6b8881f000d23a8463a9d6d850c"><code>495c793</code></a> chore: v3.0.0-rc.1 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects/issues/9453">#9453</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/7ee2f75ce1e645f75ae42b9f2f7f76cfc45b1743"><code>7ee2f75</code></a> chore: v3.0.0-rc.0 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects/issues/9418">#9418</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/bde9cfd84d99ea1ca8fc59bf51f9d4001d6527f2"><code>bde9cfd</code></a> chore: update node engine version 18 (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects/issues/9348">#9348</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/52d79c4e0cf8876903aa079cf8cbcd46f265505a"><code>52d79c4</code></a> chore: v3.0.0-beta.0 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects/issues/9311">#9311</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/a59aead1e2732a6d7ceb83f881c0945abca4d696"><code>a59aead</code></a> chore: attempt to fix Crowdin issues (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects/issues/9220">#9220</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/09ea3bcfab029daebd75b057221e5339da28f00b"><code>09ea3bc</code></a> feat(client-redirects-plugin): support fully qualified urls and querystring/h...</li>
<li><a href="https://github.com/facebook/docusaurus/commit/ff227283d232acbde1fb902f4dbf0aec879956a2"><code>ff22728</code></a> chore: upgrade dependencies (non-major) (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects/issues/9148">#9148</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/7d033cc8c08e0c8fd57baff7390540def6eb6046"><code>7d033cc</code></a> chore: v3.0.0-alpha.0 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects/issues/9072">#9072</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/187e5aa218e764b06dcbbb50f22ced72159a8532"><code>187e5aa</code></a> feat: React 18 + automatic JSX runtime + build --dev (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects/issues/8961">#8961</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/facebook/docusaurus/commits/v3.0.0/packages/docusaurus-plugin-client-redirects">compare view</a></li>
</ul>
</details>
<br />

Updates `@docusaurus/plugin-content-docs` from 2.4.3 to 3.0.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/facebook/docusaurus/releases"><code>@​docusaurus/plugin-content-docs</code>'s releases</a>.</em></p>
<blockquote>
<h2>3.0.0 (2023-10-31)</h2>
<ul>
<li>GitHub PR: <a href="https://redirect.github.com/facebook/docusaurus/pull/9478">facebook/docusaurus#9478</a></li>
<li>GitHub release notes: <a href="https://github.com/facebook/docusaurus/releases/tag/v3.0.0">https://github.com/facebook/docusaurus/releases/tag/v3.0.0</a></li>
<li>GitHub release discussion: <a href="https://github.com/facebook/docusaurus/discussions/9481">https://github.com/facebook/docusaurus/discussions/9481</a></li>
<li>Upgrade guide: <a href="https://docusaurus.io/docs/migration/v3">docusaurus.io/docs/migration/v3</a></li>
</ul>
<h4>:boom: Breaking Change</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9316">#9316</a> chore: upgrade syntax highlighting dependencies, <code>prism-react-renderer</code> to v2, <code>react-live</code> to v4 (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-cssnano-preset</code>, <code>docusaurus-logger</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-theme-translations</code>, <code>docusaurus-utils-common</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>, <code>eslint-plugin</code>, <code>lqip-loader</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9348">#9348</a> chore: update node engine version 18 (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9310">#9310</a> chore(plugin-docs): remove legacy versioned prefix on doc ids and sidebar names in versioned sidebars (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9308">#9308</a> fix(theme): make warning a first-class admonition, and deprecate caution admonition (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-tsconfig</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9258">#9258</a> feat: Docusaurus v3 upgrades and require TypeScript 5 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-blog</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9189">#9189</a> feat(blog-plugin): limit option for blog feedOptions (<a href="https://github.com/johnnyreilly"><code>@​johnnyreilly</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-tsconfig</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9050">#9050</a> feat: create official TypeScript base config <code>@​docusaurus/tsconfig</code> (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-module-type-aliases</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-types</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8961">#8961</a> feat: React 18 + automatic JSX runtime + build --dev (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9026">#9026</a> chore: remove facebook template (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-types</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8288">#8288</a> feat: upgrade to MDX v2 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/7966">#7966</a> fix(plugin-docs,theme): refactor docs plugin routes and component tree (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:rocket: New Feature</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-mdx-loader</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9394">#9394</a> feat(mdx-loader): Remark plugin to report unused MDX / Markdown directives (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9241">#9241</a> feat: support bun package manager in <code>create-docusaurus</code> (<a href="https://github.com/colinhacks"><code>@​colinhacks</code></a>)</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/facebook/docusaurus/blob/main/CHANGELOG.md"><code>@​docusaurus/plugin-content-docs</code>'s changelog</a>.</em></p>
<blockquote>
<h2>3.0.0 (2023-10-31)</h2>
<h4>:boom: Breaking Change</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9316">#9316</a> chore: upgrade syntax highlighting dependencies, <code>prism-react-renderer</code> to v2, <code>react-live</code> to v4 (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-cssnano-preset</code>, <code>docusaurus-logger</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-theme-translations</code>, <code>docusaurus-utils-common</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>, <code>eslint-plugin</code>, <code>lqip-loader</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9348">#9348</a> chore: update node engine version 18 (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9310">#9310</a> chore(plugin-docs): remove legacy versioned prefix on doc ids and sidebar names in versioned sidebars (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9308">#9308</a> fix(theme): make warning a first-class admonition, and deprecate caution admonition (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-tsconfig</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9258">#9258</a> feat: Docusaurus v3 upgrades and require TypeScript 5 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-blog</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9189">#9189</a> feat(blog-plugin): limit option for blog feedOptions (<a href="https://github.com/johnnyreilly"><code>@​johnnyreilly</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-tsconfig</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9050">#9050</a> feat: create official TypeScript base config <code>@​docusaurus/tsconfig</code> (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-module-type-aliases</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusau...

_Description has been truncated_
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-16 15:03:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1446" class=".btn">#1446</a>
            </td>
            <td>
                <b>
                    Bump axios, @docusaurus/core, @docusaurus/plugin-client-redirects, @docusaurus/plugin-content-docs, @docusaurus/plugin-google-gtag, @docusaurus/plugin-google-tag-manager, @docusaurus/preset-classic, @docusaurus/theme-common, @easyops-cn/docusaurus-search-local and redocusaurus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [axios](https://github.com/axios/axios) to 1.6.2 and updates ancestor dependencies [axios](https://github.com/axios/axios), [@docusaurus/core](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus), [@docusaurus/plugin-client-redirects](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects), [@docusaurus/plugin-content-docs](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-content-docs), [@docusaurus/plugin-google-gtag](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-google-gtag), [@docusaurus/plugin-google-tag-manager](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-google-tag-manager), [@docusaurus/preset-classic](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-preset-classic), [@docusaurus/theme-common](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-theme-common), [@easyops-cn/docusaurus-search-local](https://github.com/easyops-cn/docusaurus-search-local) and [redocusaurus](https://github.com/rohit-gohri/redocusaurus). These dependencies need to be updated together.

Updates `axios` from 0.25.0 to 1.6.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/releases">axios's releases</a>.</em></p>
<blockquote>
<h2>Release v1.6.2</h2>
<h2>Release notes:</h2>
<h3>Features</h3>
<ul>
<li><strong>withXSRFToken:</strong> added withXSRFToken option as a workaround to achieve the old <code>withCredentials</code> behavior; (<a href="https://redirect.github.com/axios/axios/issues/6046">#6046</a>) (<a href="https://github.com/axios/axios/commit/cff996779b272a5e94c2b52f5503ccf668bc42dc">cff9967</a>)</li>
</ul>
<h3>PRs</h3>
<ul>
<li>feat(withXSRFToken): added withXSRFToken option as a workaround to achieve the old `withCredentials` behavior; ( <a href="https://api.github.com/repos/axios/axios/pulls/6046">#6046</a> )</li>
</ul>
<pre><code>
📢 This PR added &amp;#x27;withXSRFToken&amp;#x27; option as a replacement for old withCredentials behaviour. 
You should now use withXSRFToken along with withCredential to get the old behavior.
This functionality is considered as a fix.
</code></pre>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+271/-146 ([#6081](https://github.com/axios/axios/issues/6081) [#6080](https://github.com/axios/axios/issues/6080) [#6079](https://github.com/axios/axios/issues/6079) [#6078](https://github.com/axios/axios/issues/6078) [#6046](https://github.com/axios/axios/issues/6046) [#6064](https://github.com/axios/axios/issues/6064) [#6063](https://github.com/axios/axios/issues/6063) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/ckng0221" title="+4/-4 ([#6073](https://github.com/axios/axios/issues/6073) )">Ng Choon Khon (CK)</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/mnomanmemon" title="+2/-2 ([#6048](https://github.com/axios/axios/issues/6048) )">Muhammad Noman</a></li>
</ul>
<h2>Release v1.6.1</h2>
<h2>Release notes:</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>formdata:</strong> fixed content-type header normalization for non-standard browser environments; (<a href="https://redirect.github.com/axios/axios/issues/6056">#6056</a>) (<a href="https://github.com/axios/axios/commit/dd465ab22bbfa262c6567be6574bf46a057d5288">dd465ab</a>)</li>
<li><strong>platform:</strong> fixed emulated browser detection in node.js environment; (<a href="https://redirect.github.com/axios/axios/issues/6055">#6055</a>) (<a href="https://github.com/axios/axios/commit/3dc8369e505e32a4e12c22f154c55fd63ac67fbb">3dc8369</a>)</li>
</ul>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+432/-65 ([#6059](https://github.com/axios/axios/issues/6059) [#6056](https://github.com/axios/axios/issues/6056) [#6055](https://github.com/axios/axios/issues/6055) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/meyfa" title="+5/-2 ([#5835](https://github.com/axios/axios/issues/5835) )">Fabian Meyer</a></li>
</ul>
<h2>Release v1.6.0</h2>
<h2>Release notes:</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>CSRF:</strong> fixed CSRF vulnerability CVE-2023-45857 (<a href="https://redirect.github.com/axios/axios/issues/6028">#6028</a>) (<a href="https://github.com/axios/axios/commit/96ee232bd3ee4de2e657333d4d2191cd389e14d0">96ee232</a>)</li>
<li><strong>dns:</strong> fixed lookup function decorator to work properly in node v20; (<a href="https://redirect.github.com/axios/axios/issues/6011">#6011</a>) (<a href="https://github.com/axios/axios/commit/5aaff532a6b820bb9ab6a8cd0f77131b47e2adb8">5aaff53</a>)</li>
<li><strong>types:</strong> fix AxiosHeaders types; (<a href="https://redirect.github.com/axios/axios/issues/5931">#5931</a>) (<a href="https://github.com/axios/axios/commit/a1c8ad008b3c13d53e135bbd0862587fb9d3fc09">a1c8ad0</a>)</li>
</ul>
<h3>PRs</h3>
<ul>
<li>CVE 2023 45857 ( <a href="https://api.github.com/repos/axios/axios/pulls/6028">#6028</a> )</li>
</ul>
<pre><code>
⚠️ Critical vulnerability fix. See https://security.snyk.io/vuln/SNYK-JS-AXIOS-6032459
</code></pre>
<h3>Contributors to this release</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/blob/v1.x/CHANGELOG.md">axios's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/axios/axios/compare/v1.6.1...v1.6.2">1.6.2</a> (2023-11-14)</h2>
<h3>Features</h3>
<ul>
<li><strong>withXSRFToken:</strong> added withXSRFToken option as a workaround to achieve the old <code>withCredentials</code> behavior; (<a href="https://redirect.github.com/axios/axios/issues/6046">#6046</a>) (<a href="https://github.com/axios/axios/commit/cff996779b272a5e94c2b52f5503ccf668bc42dc">cff9967</a>)</li>
</ul>
<h3>PRs</h3>
<ul>
<li>feat(withXSRFToken): added withXSRFToken option as a workaround to achieve the old `withCredentials` behavior; ( <a href="https://api.github.com/repos/axios/axios/pulls/6046">#6046</a> )</li>
</ul>
<pre><code>
📢 This PR added &amp;#x27;withXSRFToken&amp;#x27; option as a replacement for old withCredentials behaviour. 
You should now use withXSRFToken along with withCredential to get the old behavior.
This functionality is considered as a fix.
</code></pre>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+271/-146 ([#6081](https://github.com/axios/axios/issues/6081) [#6080](https://github.com/axios/axios/issues/6080) [#6079](https://github.com/axios/axios/issues/6079) [#6078](https://github.com/axios/axios/issues/6078) [#6046](https://github.com/axios/axios/issues/6046) [#6064](https://github.com/axios/axios/issues/6064) [#6063](https://github.com/axios/axios/issues/6063) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/ckng0221" title="+4/-4 ([#6073](https://github.com/axios/axios/issues/6073) )">Ng Choon Khon (CK)</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/mnomanmemon" title="+2/-2 ([#6048](https://github.com/axios/axios/issues/6048) )">Muhammad Noman</a></li>
</ul>
<h2><a href="https://github.com/axios/axios/compare/v1.6.0...v1.6.1">1.6.1</a> (2023-11-08)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>formdata:</strong> fixed content-type header normalization for non-standard browser environments; (<a href="https://redirect.github.com/axios/axios/issues/6056">#6056</a>) (<a href="https://github.com/axios/axios/commit/dd465ab22bbfa262c6567be6574bf46a057d5288">dd465ab</a>)</li>
<li><strong>platform:</strong> fixed emulated browser detection in node.js environment; (<a href="https://redirect.github.com/axios/axios/issues/6055">#6055</a>) (<a href="https://github.com/axios/axios/commit/3dc8369e505e32a4e12c22f154c55fd63ac67fbb">3dc8369</a>)</li>
</ul>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+432/-65 ([#6059](https://github.com/axios/axios/issues/6059) [#6056](https://github.com/axios/axios/issues/6056) [#6055](https://github.com/axios/axios/issues/6055) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/meyfa" title="+5/-2 ([#5835](https://github.com/axios/axios/issues/5835) )">Fabian Meyer</a></li>
</ul>
<h3>PRs</h3>
<ul>
<li>feat(withXSRFToken): added withXSRFToken option as a workaround to achieve the old `withCredentials` behavior; ( <a href="https://api.github.com/repos/axios/axios/pulls/6046">#6046</a> )</li>
</ul>
<pre><code>
📢 This PR added &amp;#x27;withXSRFToken&amp;#x27; option as a replacement for old withCredentials behaviour. 
You should now use withXSRFToken along with withCredential to get the old behavior.
This functionality is considered as a fix.
</code></pre>
<h1><a href="https://github.com/axios/axios/compare/v1.5.1...v1.6.0">1.6.0</a> (2023-10-26)</h1>
<h3>Bug Fixes</h3>
<ul>
<li><strong>CSRF:</strong> fixed CSRF vulnerability CVE-2023-45857 (<a href="https://redirect.github.com/axios/axios/issues/6028">#6028</a>) (<a href="https://github.com/axios/axios/commit/96ee232bd3ee4de2e657333d4d2191cd389e14d0">96ee232</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/axios/axios/commit/b3be36585884ba1e237fdd0eacf55f678aefc396"><code>b3be365</code></a> chore(release): v1.6.2 (<a href="https://redirect.github.com/axios/axios/issues/6082">#6082</a>)</li>
<li><a href="https://github.com/axios/axios/commit/8739acbd28eeb6b62c3565c8cf06309d15c5ed4b"><code>8739acb</code></a> chore(ci): removed redundant release action; (<a href="https://redirect.github.com/axios/axios/issues/6081">#6081</a>)</li>
<li><a href="https://github.com/axios/axios/commit/bfa9c305238bd14d1034af9af04b6749f9dba9b4"><code>bfa9c30</code></a> chore(docs): fix outdated grunt to npm scripts (<a href="https://redirect.github.com/axios/axios/issues/6073">#6073</a>)</li>
<li><a href="https://github.com/axios/axios/commit/a2b0fb314f5bd62deb4e9b3cb4d2e868734dd5bd"><code>a2b0fb3</code></a> chore(docs): update README.md (<a href="https://redirect.github.com/axios/axios/issues/6048">#6048</a>)</li>
<li><a href="https://github.com/axios/axios/commit/b12a6083f33539ac3883e5a9938e46a76f99305d"><code>b12a608</code></a> chore(ci): removed paths-ignore filter; (<a href="https://redirect.github.com/axios/axios/issues/6080">#6080</a>)</li>
<li><a href="https://github.com/axios/axios/commit/0c9d88602bf305926f8826bd6c1374465ddfd780"><code>0c9d886</code></a> chore(ci): reworked ignoring files logic; (<a href="https://redirect.github.com/axios/axios/issues/6079">#6079</a>)</li>
<li><a href="https://github.com/axios/axios/commit/30873ee5a8f35aef3eabcece9c81a18ae9bec7bf"><code>30873ee</code></a> chore(ci): add paths-ignore config to testing action; (<a href="https://redirect.github.com/axios/axios/issues/6078">#6078</a>)</li>
<li><a href="https://github.com/axios/axios/commit/cff996779b272a5e94c2b52f5503ccf668bc42dc"><code>cff9967</code></a> feat(withXSRFToken): added withXSRFToken option as a workaround to achieve th...</li>
<li><a href="https://github.com/axios/axios/commit/7009715369a50740ba2ce00534012c1caf269ad2"><code>7009715</code></a> chore(ci): fixed release notification action; (<a href="https://redirect.github.com/axios/axios/issues/6064">#6064</a>)</li>
<li><a href="https://github.com/axios/axios/commit/7144f10dc51a841527167b62b7d792e2989656c2"><code>7144f10</code></a> chore(ci): fixed release notification action; (<a href="https://redirect.github.com/axios/axios/issues/6063">#6063</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/axios/axios/compare/v0.25.0...v1.6.2">compare view</a></li>
</ul>
</details>
<br />

Updates `@docusaurus/core` from 2.4.3 to 3.0.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/facebook/docusaurus/releases"><code>@​docusaurus/core</code>'s releases</a>.</em></p>
<blockquote>
<h2>3.0.0 (2023-10-31)</h2>
<ul>
<li>GitHub PR: <a href="https://redirect.github.com/facebook/docusaurus/pull/9478">facebook/docusaurus#9478</a></li>
<li>GitHub release notes: <a href="https://github.com/facebook/docusaurus/releases/tag/v3.0.0">https://github.com/facebook/docusaurus/releases/tag/v3.0.0</a></li>
<li>GitHub release discussion: <a href="https://github.com/facebook/docusaurus/discussions/9481">https://github.com/facebook/docusaurus/discussions/9481</a></li>
<li>Upgrade guide: <a href="https://docusaurus.io/docs/migration/v3">docusaurus.io/docs/migration/v3</a></li>
</ul>
<h4>:boom: Breaking Change</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9316">#9316</a> chore: upgrade syntax highlighting dependencies, <code>prism-react-renderer</code> to v2, <code>react-live</code> to v4 (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-cssnano-preset</code>, <code>docusaurus-logger</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-theme-translations</code>, <code>docusaurus-utils-common</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>, <code>eslint-plugin</code>, <code>lqip-loader</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9348">#9348</a> chore: update node engine version 18 (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9310">#9310</a> chore(plugin-docs): remove legacy versioned prefix on doc ids and sidebar names in versioned sidebars (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9308">#9308</a> fix(theme): make warning a first-class admonition, and deprecate caution admonition (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-tsconfig</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9258">#9258</a> feat: Docusaurus v3 upgrades and require TypeScript 5 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-blog</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9189">#9189</a> feat(blog-plugin): limit option for blog feedOptions (<a href="https://github.com/johnnyreilly"><code>@​johnnyreilly</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-tsconfig</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9050">#9050</a> feat: create official TypeScript base config <code>@​docusaurus/tsconfig</code> (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-module-type-aliases</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-types</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8961">#8961</a> feat: React 18 + automatic JSX runtime + build --dev (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9026">#9026</a> chore: remove facebook template (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-types</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8288">#8288</a> feat: upgrade to MDX v2 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/7966">#7966</a> fix(plugin-docs,theme): refactor docs plugin routes and component tree (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:rocket: New Feature</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-mdx-loader</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9394">#9394</a> feat(mdx-loader): Remark plugin to report unused MDX / Markdown directives (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9241">#9241</a> feat: support bun package manager in <code>create-docusaurus</code> (<a href="https://github.com/colinhacks"><code>@​colinhacks</code></a>)</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/facebook/docusaurus/blob/main/CHANGELOG.md"><code>@​docusaurus/core</code>'s changelog</a>.</em></p>
<blockquote>
<h2>3.0.0 (2023-10-31)</h2>
<h4>:boom: Breaking Change</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9316">#9316</a> chore: upgrade syntax highlighting dependencies, <code>prism-react-renderer</code> to v2, <code>react-live</code> to v4 (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-cssnano-preset</code>, <code>docusaurus-logger</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-theme-translations</code>, <code>docusaurus-utils-common</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>, <code>eslint-plugin</code>, <code>lqip-loader</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9348">#9348</a> chore: update node engine version 18 (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9310">#9310</a> chore(plugin-docs): remove legacy versioned prefix on doc ids and sidebar names in versioned sidebars (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9308">#9308</a> fix(theme): make warning a first-class admonition, and deprecate caution admonition (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-tsconfig</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9258">#9258</a> feat: Docusaurus v3 upgrades and require TypeScript 5 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-blog</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9189">#9189</a> feat(blog-plugin): limit option for blog feedOptions (<a href="https://github.com/johnnyreilly"><code>@​johnnyreilly</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-tsconfig</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9050">#9050</a> feat: create official TypeScript base config <code>@​docusaurus/tsconfig</code> (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-module-type-aliases</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-types</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8961">#8961</a> feat: React 18 + automatic JSX runtime + build --dev (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9026">#9026</a> chore: remove facebook template (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-types</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8288">#8288</a> feat: upgrade to MDX v2 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/7966">#7966</a> fix(plugin-docs,theme): refactor docs plugin routes and component tree (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:rocket: New Feature</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-mdx-loader</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9394">#9394</a> feat(mdx-loader): Remark plugin to report unused MDX / Markdown directives (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9241">#9241</a> feat: support bun package manager in <code>create-docusaurus</code> (<a href="https://github.com/colinhacks"><code>@​colinhacks</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-blog</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9189">#9189</a> feat(blog-plugin): limit option for blog feedOptions (<a href="https://github.com/johnnyreilly"><code>@​johnnyreilly</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9152">#9152</a> feat(theme): add support for meta og locale and alternates (<a href="https://github.com/FlorinaPacurar"><code>@​FlorinaPacurar</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9028">#9028</a> feat(theme): add ability to inject data attributes from query-string - possibility to create an iframe/embed variant of a page (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
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
<li><a href="https://github.com/facebook/docusaurus/commit/ca8b4638c47119d38838656c4a11ee3a5e7ba6f2"><code>ca8b463</code></a> v3.0.0</li>
<li><a href="https://github.com/facebook/docusaurus/commit/495c7936b605e6b8881f000d23a8463a9d6d850c"><code>495c793</code></a> chore: v3.0.0-rc.1 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/9453">#9453</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/7ee2f75ce1e645f75ae42b9f2f7f76cfc45b1743"><code>7ee2f75</code></a> chore: v3.0.0-rc.0 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/9418">#9418</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/45f1a669b5ab29a04365f20e88e37e085c0fb4de"><code>45f1a66</code></a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/9317">#9317</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/643a7fe5a325dacfd1d809a1f40a9688e9634fa7"><code>643a7fe</code></a> fix(core): log missing errorInfo in React 18 onRecoverableError callback (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/9387">#9387</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/1319996083a2becf38967a99f6db290c1d5c99cb"><code>1319996</code></a> feat(core): throw error when official docusaurus dependencies use different v...</li>
<li><a href="https://github.com/facebook/docusaurus/commit/dceaae41d7f3fc148a2d2240a3c89e0e9c22aa4c"><code>dceaae4</code></a> chore: upgrade syntax highlighting dependencies, <code>prism-react-renderer</code> to v2...</li>
<li><a href="https://github.com/facebook/docusaurus/commit/bde9cfd84d99ea1ca8fc59bf51f9d4001d6527f2"><code>bde9cfd</code></a> chore: update node engine version 18 (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/9348">#9348</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/52d79c4e0cf8876903aa079cf8cbcd46f265505a"><code>52d79c4</code></a> chore: v3.0.0-beta.0 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/9311">#9311</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/6e8e276e406e24c46bf34385dd47ebd2e44bc152"><code>6e8e276</code></a> fix(cli): disable vertical borders of the update notification (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/9309">#9309</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/facebook/docusaurus/commits/v3.0.0/packages/docusaurus">compare view</a></li>
</ul>
</details>
<br />

Updates `@docusaurus/plugin-client-redirects` from 2.4.3 to 3.0.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/facebook/docusaurus/releases"><code>@​docusaurus/plugin-client-redirects</code>'s releases</a>.</em></p>
<blockquote>
<h2>3.0.0 (2023-10-31)</h2>
<ul>
<li>GitHub PR: <a href="https://redirect.github.com/facebook/docusaurus/pull/9478">facebook/docusaurus#9478</a></li>
<li>GitHub release notes: <a href="https://github.com/facebook/docusaurus/releases/tag/v3.0.0">https://github.com/facebook/docusaurus/releases/tag/v3.0.0</a></li>
<li>GitHub release discussion: <a href="https://github.com/facebook/docusaurus/discussions/9481">https://github.com/facebook/docusaurus/discussions/9481</a></li>
<li>Upgrade guide: <a href="https://docusaurus.io/docs/migration/v3">docusaurus.io/docs/migration/v3</a></li>
</ul>
<h4>:boom: Breaking Change</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9316">#9316</a> chore: upgrade syntax highlighting dependencies, <code>prism-react-renderer</code> to v2, <code>react-live</code> to v4 (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-cssnano-preset</code>, <code>docusaurus-logger</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-theme-translations</code>, <code>docusaurus-utils-common</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>, <code>eslint-plugin</code>, <code>lqip-loader</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9348">#9348</a> chore: update node engine version 18 (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9310">#9310</a> chore(plugin-docs): remove legacy versioned prefix on doc ids and sidebar names in versioned sidebars (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9308">#9308</a> fix(theme): make warning a first-class admonition, and deprecate caution admonition (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-tsconfig</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9258">#9258</a> feat: Docusaurus v3 upgrades and require TypeScript 5 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-blog</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9189">#9189</a> feat(blog-plugin): limit option for blog feedOptions (<a href="https://github.com/johnnyreilly"><code>@​johnnyreilly</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-tsconfig</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9050">#9050</a> feat: create official TypeScript base config <code>@​docusaurus/tsconfig</code> (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-module-type-aliases</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-types</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8961">#8961</a> feat: React 18 + automatic JSX runtime + build --dev (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9026">#9026</a> chore: remove facebook template (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-types</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8288">#8288</a> feat: upgrade to MDX v2 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/7966">#7966</a> fix(plugin-docs,theme): refactor docs plugin routes and component tree (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:rocket: New Feature</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-mdx-loader</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9394">#9394</a> feat(mdx-loader): Remark plugin to report unused MDX / Markdown directives (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9241">#9241</a> feat: support bun package manager in <code>create-docusaurus</code> (<a href="https://github.com/colinhacks"><code>@​colinhacks</code></a>)</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/facebook/docusaurus/blob/main/CHANGELOG.md"><code>@​docusaurus/plugin-client-redirects</code>'s changelog</a>.</em></p>
<blockquote>
<h2>3.0.0 (2023-10-31)</h2>
<h4>:boom: Breaking Change</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9316">#9316</a> chore: upgrade syntax highlighting dependencies, <code>prism-react-renderer</code> to v2, <code>react-live</code> to v4 (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-cssnano-preset</code>, <code>docusaurus-logger</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-theme-translations</code>, <code>docusaurus-utils-common</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>, <code>eslint-plugin</code>, <code>lqip-loader</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9348">#9348</a> chore: update node engine version 18 (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9310">#9310</a> chore(plugin-docs): remove legacy versioned prefix on doc ids and sidebar names in versioned sidebars (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9308">#9308</a> fix(theme): make warning a first-class admonition, and deprecate caution admonition (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-tsconfig</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9258">#9258</a> feat: Docusaurus v3 upgrades and require TypeScript 5 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-blog</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9189">#9189</a> feat(blog-plugin): limit option for blog feedOptions (<a href="https://github.com/johnnyreilly"><code>@​johnnyreilly</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-tsconfig</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9050">#9050</a> feat: create official TypeScript base config <code>@​docusaurus/tsconfig</code> (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-module-type-aliases</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-types</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8961">#8961</a> feat: React 18 + automatic JSX runtime + build --dev (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9026">#9026</a> chore: remove facebook template (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-types</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/8288">#8288</a> feat: upgrade to MDX v2 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/7966">#7966</a> fix(plugin-docs,theme): refactor docs plugin routes and component tree (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:rocket: New Feature</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-mdx-loader</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9394">#9394</a> feat(mdx-loader): Remark plugin to report unused MDX / Markdown directives (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9241">#9241</a> feat: support bun package manager in <code>create-docusaurus</code> (<a href="https://github.com/colinhacks"><code>@​colinhacks</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-blog</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9189">#9189</a> feat(blog-plugin): limit option for blog feedOptions (<a href="https://github.com/johnnyreilly"><code>@​johnnyreilly</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9152">#9152</a> feat(theme): add support for meta og locale and alternates (<a href="https://github.com/FlorinaPacurar"><code>@​FlorinaPacurar</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9028">#9028</a> feat(theme): add ability to inject data attributes from query-string - possibility to create an iframe/embed variant of a page (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
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
<li><a href="https://github.com/facebook/docusaurus/commit/ca8b4638c47119d38838656c4a11ee3a5e7ba6f2"><code>ca8b463</code></a> v3.0.0</li>
<li><a href="https://github.com/facebook/docusaurus/commit/495c7936b605e6b8881f000d23a8463a9d6d850c"><code>495c793</code></a> chore: v3.0.0-rc.1 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects/issues/9453">#9453</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/7ee2f75ce1e645f75ae42b9f2f7f76cfc45b1743"><code>7ee2f75</code></a> chore: v3.0.0-rc.0 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects/issues/9418">#9418</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/bde9cfd84d99ea1ca8fc59bf51f9d4001d6527f2"><code>bde9cfd</code></a> chore: update node engine version 18 (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects/issues/9348">#9348</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/52d79c4e0cf8876903aa079cf8cbcd46f265505a"><code>52d79c4</code></a> chore: v3.0.0-beta.0 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects/issues/9311">#9311</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/a59aead1e2732a6d7ceb83f881c0945abca4d696"><code>a59aead</code></a> chore: attempt to fix Crowdin issues (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects/issues/9220">#9220</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/09ea3bcfab029daebd75b057221e5339da28f00b"><code>09ea3bc</code></a> feat(client-redirects-plugin): support fully qualified urls and querystring/h...</li>
<li><a href="https://github.com/facebook/docusaurus/commit/ff227283d232acbde1fb902f4dbf0aec879956a2"><code>ff22728</code></a> chore: upgrade dependencies (non-major) (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects/issues/9148">#9148</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/7d033cc8c08e0c8fd57baff7390540def6eb6046"><code>7d033cc</code></a> chore: v3.0.0-alpha.0 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects/issues/9072">#9072</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/187e5aa218e764b06dcbbb50f22ced72159a8532"><code>187e5aa</code></a> feat: React 18 + automatic JSX runtime + build --dev (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-plugin-client-redirects/issues/8961">#8961</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/facebook/docusaurus/commits/v3.0.0/packages/docusaurus-plugin-client-redirects">compare view</a></li>
</ul>
</details>
<br />

Updates `@docusaurus/plugin-content-docs` from 2.4.3 to 3.0.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/facebook/docusaurus/releases"><code>@​docusaurus/plugin-content-docs</code>'s releases</a>.</em></p>
<blockquote>
<h2>3.0.0 (2023-10-31)</h2>
<ul>
<li>GitHub PR: <a href="https://redirect.github.com/facebook/docusaurus/pull/9478">facebook/docusaurus#9478</a></li>
<li>GitHub release notes: <a href="https://github.com/facebook/docusaurus/releases/tag/v3.0.0">https://github.com/facebook/docusaurus/releases/tag/v3.0.0</a></li>
<li>GitHub release discussion: <a href="https://github.com/facebook/docusaurus/discussions/9481">https://github.com/facebook/docusaurus/discussions/9481</a></li>
<li>Upgrade guide: <a href="https://docusaurus.io/docs/migration/v3">docusaurus.io/docs/migration/v3</a></li>
</ul>
<h4>:boom: Breaking Change</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9451">#9451</a> feat(mdx-loader): upgrade to MDX v3 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9317">#9317</a> feat(core): support TypeScript + ESM configuration (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9316">#9316</a> chore: upgrade syntax highlighting dependencies, <code>prism-react-renderer</code> to v2, <code>react-live</code> to v4 (<a href="https://github.com/harryzcy"><code>@​harryzcy</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-cssnano-preset</code>, <code>docusaurus-logger</code>, <code>docusaurus-mdx-loader</code>, <code>docusaurus-migrate</code>, <code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-preset-classic</code>, <code>docusaurus-remark-plugin-npm2yarn</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-theme-translations</code>, <code>docusaurus-utils-common</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>, <code>eslint-plugin</code>, <code>lqip-loader</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9348">#9348</a> chore: update node engine version 18 (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9310">#9310</a> chore(plugin-docs): remove legacy versioned prefix on doc ids and sidebar names in versioned sidebars (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9308">#9308</a> fix(theme): make warning a first-class admonition, and deprecate caution admonition (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9305">#9305</a> feat(theme-mermaid): upgrade Mermaid to v10.4 - handle async rendering (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-debug</code>, <code>docusaurus-plugin-google-analytics</code>, <code>docusaurus-plugin-google-gtag</code>, <code>docusaurus-plugin-google-tag-manager</code>, <code>docusaurus-plugin-ideal-image</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-theme-live-codeblock</code>, <code>docusaurus-theme-mermaid</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-tsconfig</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9258">#9258</a> feat: Docusaurus v3 upgrades and require TypeScript 5 (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-blog</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9189">#9189</a> feat(blog-plugin)...

_Description has been truncated_
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-16 15:02:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1444" class=".btn">#1444</a>
            </td>
            <td>
                <b>
                    Added option to skip empty blocks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1436 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-16 01:48:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1443" class=".btn">#1443</a>
            </td>
            <td>
                <b>
                    uprev to 23.10.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-15 17:11:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1442" class=".btn">#1442</a>
            </td>
            <td>
                <b>
                    Replaced EthSigner with Web3Signer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also removed the section on web3js-eea which was deprecated in 2021. 

Fixes #1412
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-15 08:39:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1441" class=".btn">#1441</a>
            </td>
            <td>
                <b>
                    Added input key to transaction call object
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1437 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-15 05:55:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1440" class=".btn">#1440</a>
            </td>
            <td>
                <b>
                    Added new JVM default options
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Decided not to go into details of when you'd want to use the `besu-untuned` start script - the rationale being that anyone who's going to need it will already be looking at the memory options and knows what they are doing. 

Fixes #1415 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-15 00:28:03 +0000 UTC
    </div>
</div>

