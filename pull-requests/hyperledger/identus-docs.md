---
layout: default
title: identus-docs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/identus-docs
---

# identus-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/identus-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-docs/pull/124" class=".btn">#124</a>
            </td>
            <td>
                <b>
                    chore(deps): bump the npm_and_yarn group across 1 directory with 17 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps the npm_and_yarn group with 14 updates in the / directory:

| Package | From | To |
| --- | --- | --- |
| [@docusaurus/core](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus) | `2.4.3` | `3.4.0` |
| [@docusaurus/preset-classic](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-preset-classic) | `2.4.3` | `3.4.0` |
| [@docusaurus/theme-mermaid](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-theme-mermaid) | `2.4.3` | `3.4.0` |
| [docusaurus-plugin-openapi-docs](https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/tree/HEAD/packages/docusaurus-plugin-openapi-docs) | `1.7.3` | `3.0.1` |
| [docusaurus-theme-openapi-docs](https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/tree/HEAD/packages/docusaurus-theme-openapi-docs) | `1.7.3` | `2.2.1` |
| [docusaurus-theme-redoc](https://github.com/rohit-gohri/redocusaurus) | `1.6.4` | `2.1.1` |
| [redocusaurus](https://github.com/rohit-gohri/redocusaurus) | `1.6.4` | `2.1.1` |
| [axios](https://github.com/axios/axios) | `0.25.0` | `removed` |
| [docusaurus-theme-openapi-docs](https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/tree/HEAD/packages/docusaurus-theme-openapi-docs) | `2.2.1` | `3.0.1` |
| [@docusaurus/theme-common](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-theme-common) | `2.4.3` | `3.4.0` |
| [braces](https://github.com/micromatch/braces) | `3.0.2` | `3.0.3` |
| [express](https://github.com/expressjs/express) | `4.18.2` | `4.19.2` |
| [follow-redirects](https://github.com/follow-redirects/follow-redirects) | `1.15.4` | `1.15.6` |
| [webpack-dev-middleware](https://github.com/webpack/webpack-dev-middleware) | `5.3.3` | `5.3.4` |
| [ws](https://github.com/websockets/ws) | `7.5.9` | `7.5.10` |


Updates `@docusaurus/core` from 2.4.3 to 3.4.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/facebook/docusaurus/releases"><code>@​docusaurus/core</code>'s releases</a>.</em></p>
<blockquote>
<h2>3.4.0 (2024-05-31)</h2>
<h4>:rocket: New Feature</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10137">#10137</a> feat(docs, blog): add support for <code>tags.yml</code>, predefined list of tags (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10151">#10151</a> feat(theme-translations): Added Turkmen (tk) default theme translations (<a href="https://github.com/ilmedova"><code>@​ilmedova</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10111">#10111</a> feat(theme-translations): Add Bulgarian default theme translations (bg) (<a href="https://github.com/PetarMc1"><code>@​PetarMc1</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9859">#9859</a> feat(core): hash router option - browse site offline (experimental) (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-module-type-aliases</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-types</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10121">#10121</a> feat(core): site storage config options (experimental) (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10185">#10185</a> fix(docs, blog): Markdown link resolution does not support hot reload (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-search-algolia</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10178">#10178</a> fix(theme): SearchPage should respect <code>contextualSearch: false</code> setting (<a href="https://github.com/ncoughlin"><code>@​ncoughlin</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10164">#10164</a> fix(search): fix algolia search container bug (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10168">#10168</a> fix(mdx-loader): resolve Markdown/MDX links with Remark instead of RegExp (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10165">#10165</a> fix(theme-translation): add missing Korean (ko) theme translations (<a href="https://github.com/revi"><code>@​revi</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10157">#10157</a> fix(theme-translations): complete Vietnamese theme translations (<a href="https://github.com/namnguyenthanhwork"><code>@​namnguyenthanhwork</code></a>)</li>
</ul>
</li>
<li><code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10145">#10145</a> fix(core): fix serve workaround regexp (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10142">#10142</a> fix(core): fix <code>docusaurus serve</code> broken for assets when using trailingSlash (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10130">#10130</a> fix(core): the broken anchor checker should not be sensitive pathname trailing slashes (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10144">#10144</a> fix(theme): fix announcement bar layout shift due to missing storage key namespace (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10132">#10132</a> fix(core): <code>configurePostCss()</code> should run after <code>configureWebpack()</code> (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10131">#10131</a> fix(core): codegen should generate unique route prop filenames (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10118">#10118</a> fix(theme-translations): fix missing pluralization for label DocCard.categoryDescription.plurals (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:memo: Documentation</h4>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10176">#10176</a> docs: add community plugin docusaurus-graph (<a href="https://github.com/Arsero"><code>@​Arsero</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10173">#10173</a> docs: improve how to use <code>&lt;details&gt;</code> (<a href="https://github.com/tats-u"><code>@​tats-u</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10167">#10167</a> docs: suggest using <code>{&lt;...&gt;...&lt;/...&gt;}</code> if don't use Markdown in migra… (<a href="https://github.com/tats-u"><code>@​tats-u</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10143">#10143</a> docs: recommend users to remove hast-util-is-element in migration to v3 (<a href="https://github.com/tats-u"><code>@​tats-u</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10124">#10124</a> docs: v3 prepare your site blog post should point users to the upgrade guide (<a href="https://github.com/homotechsual"><code>@​homotechsual</code></a>)</li>
</ul>
<h4>:robot: Dependencies</h4>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10155">#10155</a> chore(deps): bump peaceiris/actions-gh-pages from 3 to 4 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/facebook/docusaurus/blob/main/CHANGELOG.md"><code>@​docusaurus/core</code>'s changelog</a>.</em></p>
<blockquote>
<h2>3.4.0 (2024-05-31)</h2>
<h4>:rocket: New Feature</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10137">#10137</a> feat(docs, blog): add support for <code>tags.yml</code>, predefined list of tags (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10151">#10151</a> feat(theme-translations): Added Turkmen (tk) default theme translations (<a href="https://github.com/ilmedova"><code>@​ilmedova</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10111">#10111</a> feat(theme-translations): Add Bulgarian default theme translations (bg) (<a href="https://github.com/PetarMc1"><code>@​PetarMc1</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9859">#9859</a> feat(core): hash router option - browse site offline (experimental) (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-module-type-aliases</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-types</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10121">#10121</a> feat(core): site storage config options (experimental) (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10185">#10185</a> fix(docs, blog): Markdown link resolution does not support hot reload (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-search-algolia</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10178">#10178</a> fix(theme): SearchPage should respect <code>contextualSearch: false</code> setting (<a href="https://github.com/ncoughlin"><code>@​ncoughlin</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10164">#10164</a> fix(search): fix algolia search container bug (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10168">#10168</a> fix(mdx-loader): resolve Markdown/MDX links with Remark instead of RegExp (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10165">#10165</a> fix(theme-translation): add missing Korean (ko) theme translations (<a href="https://github.com/revi"><code>@​revi</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10157">#10157</a> fix(theme-translations): complete Vietnamese theme translations (<a href="https://github.com/namnguyenthanhwork"><code>@​namnguyenthanhwork</code></a>)</li>
</ul>
</li>
<li><code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10145">#10145</a> fix(core): fix serve workaround regexp (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10142">#10142</a> fix(core): fix <code>docusaurus serve</code> broken for assets when using trailingSlash (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10130">#10130</a> fix(core): the broken anchor checker should not be sensitive pathname trailing slashes (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10144">#10144</a> fix(theme): fix announcement bar layout shift due to missing storage key namespace (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10132">#10132</a> fix(core): <code>configurePostCss()</code> should run after <code>configureWebpack()</code> (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10131">#10131</a> fix(core): codegen should generate unique route prop filenames (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10118">#10118</a> fix(theme-translations): fix missing pluralization for label DocCard.categoryDescription.plurals (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:memo: Documentation</h4>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10176">#10176</a> docs: add community plugin docusaurus-graph (<a href="https://github.com/Arsero"><code>@​Arsero</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10173">#10173</a> docs: improve how to use <code>&lt;details&gt;</code> (<a href="https://github.com/tats-u"><code>@​tats-u</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10167">#10167</a> docs: suggest using <code>{&lt;...&gt;...&lt;/...&gt;}</code> if don't use Markdown in migra… (<a href="https://github.com/tats-u"><code>@​tats-u</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10143">#10143</a> docs: recommend users to remove hast-util-is-element in migration to v3 (<a href="https://github.com/tats-u"><code>@​tats-u</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10124">#10124</a> docs: v3 prepare your site blog post should point users to the upgrade guide (<a href="https://github.com/homotechsual"><code>@​homotechsual</code></a>)</li>
</ul>
<h4>:robot: Dependencies</h4>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10155">#10155</a> chore(deps): bump peaceiris/actions-gh-pages from 3 to 4 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/facebook/docusaurus/commit/49e9a2143274a8dd795659b417b470bc42abbd6e"><code>49e9a21</code></a> v3.4.0</li>
<li><a href="https://github.com/facebook/docusaurus/commit/17f3e02a4244b1893b7624ec3c948bfa926feacd"><code>17f3e02</code></a> feat(core): hash router option - browse site offline (experimental) (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/9859">#9859</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/b73ad1ece5540654618240dd95425ba950bf015f"><code>b73ad1e</code></a> fix(core): fix serve workaround regexp (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/10145">#10145</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/87f0023eb349575725010509f6abedcb4878c059"><code>87f0023</code></a> fix(core): fix <code>docusaurus serve</code> broken for assets when using trailingSlash ...</li>
<li><a href="https://github.com/facebook/docusaurus/commit/ff5039f4137c80de010308d775b5f0bc74be9f2f"><code>ff5039f</code></a> fix(core): <code>configurePostCss()</code> should run after <code>configureWebpack()</code> (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/10132">#10132</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/29b7a4ddbbd057372d10370fc062075d79c98b46"><code>29b7a4d</code></a> fix(core): codegen should generate unique route prop filenames (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/10131">#10131</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/394ce84691ff3993d584de4e7c8ae2df30659dda"><code>394ce84</code></a> fix(core): the broken anchor checker should not be sensitive pathname trailin...</li>
<li><a href="https://github.com/facebook/docusaurus/commit/02e38d8ccf7811af27a9c15ddbadf4d26cfc0eab"><code>02e38d8</code></a> refactor: fix i18n bug in node v22 (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/10129">#10129</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/620e46350a57bf1588fb20ce8622a3c871a366de"><code>620e463</code></a> feat(core): site storage config options (experimental) (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/10121">#10121</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/c125f7a27252cfbd4e8a65e4ee6ba2dee7f5f5c1"><code>c125f7a</code></a> chore: release Docusaurus 3.3.0 + 3.3.1 + 3.3.2 (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus/issues/10101">#10101</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/facebook/docusaurus/commits/v3.4.0/packages/docusaurus">compare view</a></li>
</ul>
</details>
<br />

Updates `@docusaurus/preset-classic` from 2.4.3 to 3.4.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/facebook/docusaurus/releases"><code>@​docusaurus/preset-classic</code>'s releases</a>.</em></p>
<blockquote>
<h2>3.4.0 (2024-05-31)</h2>
<h4>:rocket: New Feature</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10137">#10137</a> feat(docs, blog): add support for <code>tags.yml</code>, predefined list of tags (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10151">#10151</a> feat(theme-translations): Added Turkmen (tk) default theme translations (<a href="https://github.com/ilmedova"><code>@​ilmedova</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10111">#10111</a> feat(theme-translations): Add Bulgarian default theme translations (bg) (<a href="https://github.com/PetarMc1"><code>@​PetarMc1</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9859">#9859</a> feat(core): hash router option - browse site offline (experimental) (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-module-type-aliases</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-types</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10121">#10121</a> feat(core): site storage config options (experimental) (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10185">#10185</a> fix(docs, blog): Markdown link resolution does not support hot reload (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-search-algolia</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10178">#10178</a> fix(theme): SearchPage should respect <code>contextualSearch: false</code> setting (<a href="https://github.com/ncoughlin"><code>@​ncoughlin</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10164">#10164</a> fix(search): fix algolia search container bug (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10168">#10168</a> fix(mdx-loader): resolve Markdown/MDX links with Remark instead of RegExp (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10165">#10165</a> fix(theme-translation): add missing Korean (ko) theme translations (<a href="https://github.com/revi"><code>@​revi</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10157">#10157</a> fix(theme-translations): complete Vietnamese theme translations (<a href="https://github.com/namnguyenthanhwork"><code>@​namnguyenthanhwork</code></a>)</li>
</ul>
</li>
<li><code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10145">#10145</a> fix(core): fix serve workaround regexp (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10142">#10142</a> fix(core): fix <code>docusaurus serve</code> broken for assets when using trailingSlash (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10130">#10130</a> fix(core): the broken anchor checker should not be sensitive pathname trailing slashes (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10144">#10144</a> fix(theme): fix announcement bar layout shift due to missing storage key namespace (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10132">#10132</a> fix(core): <code>configurePostCss()</code> should run after <code>configureWebpack()</code> (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10131">#10131</a> fix(core): codegen should generate unique route prop filenames (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10118">#10118</a> fix(theme-translations): fix missing pluralization for label DocCard.categoryDescription.plurals (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:memo: Documentation</h4>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10176">#10176</a> docs: add community plugin docusaurus-graph (<a href="https://github.com/Arsero"><code>@​Arsero</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10173">#10173</a> docs: improve how to use <code>&lt;details&gt;</code> (<a href="https://github.com/tats-u"><code>@​tats-u</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10167">#10167</a> docs: suggest using <code>{&lt;...&gt;...&lt;/...&gt;}</code> if don't use Markdown in migra… (<a href="https://github.com/tats-u"><code>@​tats-u</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10143">#10143</a> docs: recommend users to remove hast-util-is-element in migration to v3 (<a href="https://github.com/tats-u"><code>@​tats-u</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10124">#10124</a> docs: v3 prepare your site blog post should point users to the upgrade guide (<a href="https://github.com/homotechsual"><code>@​homotechsual</code></a>)</li>
</ul>
<h4>:robot: Dependencies</h4>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10155">#10155</a> chore(deps): bump peaceiris/actions-gh-pages from 3 to 4 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/facebook/docusaurus/blob/main/CHANGELOG.md"><code>@​docusaurus/preset-classic</code>'s changelog</a>.</em></p>
<blockquote>
<h2>3.4.0 (2024-05-31)</h2>
<h4>:rocket: New Feature</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10137">#10137</a> feat(docs, blog): add support for <code>tags.yml</code>, predefined list of tags (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10151">#10151</a> feat(theme-translations): Added Turkmen (tk) default theme translations (<a href="https://github.com/ilmedova"><code>@​ilmedova</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10111">#10111</a> feat(theme-translations): Add Bulgarian default theme translations (bg) (<a href="https://github.com/PetarMc1"><code>@​PetarMc1</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9859">#9859</a> feat(core): hash router option - browse site offline (experimental) (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-module-type-aliases</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-types</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10121">#10121</a> feat(core): site storage config options (experimental) (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10185">#10185</a> fix(docs, blog): Markdown link resolution does not support hot reload (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-search-algolia</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10178">#10178</a> fix(theme): SearchPage should respect <code>contextualSearch: false</code> setting (<a href="https://github.com/ncoughlin"><code>@​ncoughlin</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10164">#10164</a> fix(search): fix algolia search container bug (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10168">#10168</a> fix(mdx-loader): resolve Markdown/MDX links with Remark instead of RegExp (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10165">#10165</a> fix(theme-translation): add missing Korean (ko) theme translations (<a href="https://github.com/revi"><code>@​revi</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10157">#10157</a> fix(theme-translations): complete Vietnamese theme translations (<a href="https://github.com/namnguyenthanhwork"><code>@​namnguyenthanhwork</code></a>)</li>
</ul>
</li>
<li><code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10145">#10145</a> fix(core): fix serve workaround regexp (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10142">#10142</a> fix(core): fix <code>docusaurus serve</code> broken for assets when using trailingSlash (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10130">#10130</a> fix(core): the broken anchor checker should not be sensitive pathname trailing slashes (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10144">#10144</a> fix(theme): fix announcement bar layout shift due to missing storage key namespace (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10132">#10132</a> fix(core): <code>configurePostCss()</code> should run after <code>configureWebpack()</code> (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10131">#10131</a> fix(core): codegen should generate unique route prop filenames (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10118">#10118</a> fix(theme-translations): fix missing pluralization for label DocCard.categoryDescription.plurals (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:memo: Documentation</h4>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10176">#10176</a> docs: add community plugin docusaurus-graph (<a href="https://github.com/Arsero"><code>@​Arsero</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10173">#10173</a> docs: improve how to use <code>&lt;details&gt;</code> (<a href="https://github.com/tats-u"><code>@​tats-u</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10167">#10167</a> docs: suggest using <code>{&lt;...&gt;...&lt;/...&gt;}</code> if don't use Markdown in migra… (<a href="https://github.com/tats-u"><code>@​tats-u</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10143">#10143</a> docs: recommend users to remove hast-util-is-element in migration to v3 (<a href="https://github.com/tats-u"><code>@​tats-u</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10124">#10124</a> docs: v3 prepare your site blog post should point users to the upgrade guide (<a href="https://github.com/homotechsual"><code>@​homotechsual</code></a>)</li>
</ul>
<h4>:robot: Dependencies</h4>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10155">#10155</a> chore(deps): bump peaceiris/actions-gh-pages from 3 to 4 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/facebook/docusaurus/commit/49e9a2143274a8dd795659b417b470bc42abbd6e"><code>49e9a21</code></a> v3.4.0</li>
<li><a href="https://github.com/facebook/docusaurus/commit/c125f7a27252cfbd4e8a65e4ee6ba2dee7f5f5c1"><code>c125f7a</code></a> chore: release Docusaurus 3.3.0 + 3.3.1 + 3.3.2 (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-preset-classic/issues/10101">#10101</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/ca33858ca0140ee1a97646a7b0e787e68d7afcd7"><code>ca33858</code></a> fix: handle React v18.3 warnings (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-preset-classic/issues/10079">#10079</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/f88da6c66d578f11960a1301e72ffdc4a59dd78b"><code>f88da6c</code></a> refactor: extract base TS client config + upgrade TS + refactor TS setup (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-preset-classic/issues/10">#10</a>...</li>
<li><a href="https://github.com/facebook/docusaurus/commit/e012e0315862b2ca02cad40c58d11d31c319ff75"><code>e012e03</code></a> chore: release Docusaurus 3.2.1 (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-preset-classic/issues/10016">#10016</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/debfc87d34c8b475fe4d76b64fe9c791c2dfd90b"><code>debfc87</code></a> chore: release Docusaurus v3.2.0 (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-preset-classic/issues/10000">#10000</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/85e5e552cbd237dc562e982d7fae346b730c3557"><code>85e5e55</code></a> chore: release Docusaurus 3.0.0 (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-preset-classic/issues/9478">#9478</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/495c7936b605e6b8881f000d23a8463a9d6d850c"><code>495c793</code></a> chore: v3.0.0-rc.1 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-preset-classic/issues/9453">#9453</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/7ee2f75ce1e645f75ae42b9f2f7f76cfc45b1743"><code>7ee2f75</code></a> chore: v3.0.0-rc.0 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-preset-classic/issues/9418">#9418</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/bde9cfd84d99ea1ca8fc59bf51f9d4001d6527f2"><code>bde9cfd</code></a> chore: update node engine version 18 (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-preset-classic/issues/9348">#9348</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/facebook/docusaurus/commits/v3.4.0/packages/docusaurus-preset-classic">compare view</a></li>
</ul>
</details>
<br />

Updates `@docusaurus/theme-mermaid` from 2.4.3 to 3.4.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/facebook/docusaurus/releases"><code>@​docusaurus/theme-mermaid</code>'s releases</a>.</em></p>
<blockquote>
<h2>3.4.0 (2024-05-31)</h2>
<h4>:rocket: New Feature</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10137">#10137</a> feat(docs, blog): add support for <code>tags.yml</code>, predefined list of tags (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10151">#10151</a> feat(theme-translations): Added Turkmen (tk) default theme translations (<a href="https://github.com/ilmedova"><code>@​ilmedova</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10111">#10111</a> feat(theme-translations): Add Bulgarian default theme translations (bg) (<a href="https://github.com/PetarMc1"><code>@​PetarMc1</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9859">#9859</a> feat(core): hash router option - browse site offline (experimental) (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-module-type-aliases</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-types</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10121">#10121</a> feat(core): site storage config options (experimental) (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10185">#10185</a> fix(docs, blog): Markdown link resolution does not support hot reload (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-search-algolia</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10178">#10178</a> fix(theme): SearchPage should respect <code>contextualSearch: false</code> setting (<a href="https://github.com/ncoughlin"><code>@​ncoughlin</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10164">#10164</a> fix(search): fix algolia search container bug (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10168">#10168</a> fix(mdx-loader): resolve Markdown/MDX links with Remark instead of RegExp (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10165">#10165</a> fix(theme-translation): add missing Korean (ko) theme translations (<a href="https://github.com/revi"><code>@​revi</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10157">#10157</a> fix(theme-translations): complete Vietnamese theme translations (<a href="https://github.com/namnguyenthanhwork"><code>@​namnguyenthanhwork</code></a>)</li>
</ul>
</li>
<li><code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10145">#10145</a> fix(core): fix serve workaround regexp (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10142">#10142</a> fix(core): fix <code>docusaurus serve</code> broken for assets when using trailingSlash (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10130">#10130</a> fix(core): the broken anchor checker should not be sensitive pathname trailing slashes (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10144">#10144</a> fix(theme): fix announcement bar layout shift due to missing storage key namespace (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10132">#10132</a> fix(core): <code>configurePostCss()</code> should run after <code>configureWebpack()</code> (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10131">#10131</a> fix(core): codegen should generate unique route prop filenames (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10118">#10118</a> fix(theme-translations): fix missing pluralization for label DocCard.categoryDescription.plurals (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:memo: Documentation</h4>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10176">#10176</a> docs: add community plugin docusaurus-graph (<a href="https://github.com/Arsero"><code>@​Arsero</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10173">#10173</a> docs: improve how to use <code>&lt;details&gt;</code> (<a href="https://github.com/tats-u"><code>@​tats-u</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10167">#10167</a> docs: suggest using <code>{&lt;...&gt;...&lt;/...&gt;}</code> if don't use Markdown in migra… (<a href="https://github.com/tats-u"><code>@​tats-u</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10143">#10143</a> docs: recommend users to remove hast-util-is-element in migration to v3 (<a href="https://github.com/tats-u"><code>@​tats-u</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10124">#10124</a> docs: v3 prepare your site blog post should point users to the upgrade guide (<a href="https://github.com/homotechsual"><code>@​homotechsual</code></a>)</li>
</ul>
<h4>:robot: Dependencies</h4>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10155">#10155</a> chore(deps): bump peaceiris/actions-gh-pages from 3 to 4 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/facebook/docusaurus/blob/main/CHANGELOG.md"><code>@​docusaurus/theme-mermaid</code>'s changelog</a>.</em></p>
<blockquote>
<h2>3.4.0 (2024-05-31)</h2>
<h4>:rocket: New Feature</h4>
<ul>
<li><code>create-docusaurus</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-utils-validation</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10137">#10137</a> feat(docs, blog): add support for <code>tags.yml</code>, predefined list of tags (<a href="https://github.com/OzakIOne"><code>@​OzakIOne</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10151">#10151</a> feat(theme-translations): Added Turkmen (tk) default theme translations (<a href="https://github.com/ilmedova"><code>@​ilmedova</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10111">#10111</a> feat(theme-translations): Add Bulgarian default theme translations (bg) (<a href="https://github.com/PetarMc1"><code>@​PetarMc1</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-client-redirects</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-pwa</code>, <code>docusaurus-plugin-sitemap</code>, <code>docusaurus-theme-search-algolia</code>, <code>docusaurus-types</code>, <code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/9859">#9859</a> feat(core): hash router option - browse site offline (experimental) (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-module-type-aliases</code>, <code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>, <code>docusaurus-types</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10121">#10121</a> feat(core): site storage config options (experimental) (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10185">#10185</a> fix(docs, blog): Markdown link resolution does not support hot reload (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-search-algolia</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10178">#10178</a> fix(theme): SearchPage should respect <code>contextualSearch: false</code> setting (<a href="https://github.com/ncoughlin"><code>@​ncoughlin</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10164">#10164</a> fix(search): fix algolia search container bug (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-mdx-loader</code>, <code>docusaurus-plugin-content-blog</code>, <code>docusaurus-plugin-content-docs</code>, <code>docusaurus-plugin-content-pages</code>, <code>docusaurus-utils</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10168">#10168</a> fix(mdx-loader): resolve Markdown/MDX links with Remark instead of RegExp (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10165">#10165</a> fix(theme-translation): add missing Korean (ko) theme translations (<a href="https://github.com/revi"><code>@​revi</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10157">#10157</a> fix(theme-translations): complete Vietnamese theme translations (<a href="https://github.com/namnguyenthanhwork"><code>@​namnguyenthanhwork</code></a>)</li>
</ul>
</li>
<li><code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10145">#10145</a> fix(core): fix serve workaround regexp (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10142">#10142</a> fix(core): fix <code>docusaurus serve</code> broken for assets when using trailingSlash (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10130">#10130</a> fix(core): the broken anchor checker should not be sensitive pathname trailing slashes (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-common</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10144">#10144</a> fix(theme): fix announcement bar layout shift due to missing storage key namespace (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-plugin-content-docs</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10132">#10132</a> fix(core): <code>configurePostCss()</code> should run after <code>configureWebpack()</code> (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-utils</code>, <code>docusaurus</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10131">#10131</a> fix(core): codegen should generate unique route prop filenames (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
<li><code>docusaurus-theme-classic</code>, <code>docusaurus-theme-translations</code>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10118">#10118</a> fix(theme-translations): fix missing pluralization for label DocCard.categoryDescription.plurals (<a href="https://github.com/slorber"><code>@​slorber</code></a>)</li>
</ul>
</li>
</ul>
<h4>:memo: Documentation</h4>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10176">#10176</a> docs: add community plugin docusaurus-graph (<a href="https://github.com/Arsero"><code>@​Arsero</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10173">#10173</a> docs: improve how to use <code>&lt;details&gt;</code> (<a href="https://github.com/tats-u"><code>@​tats-u</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10167">#10167</a> docs: suggest using <code>{&lt;...&gt;...&lt;/...&gt;}</code> if don't use Markdown in migra… (<a href="https://github.com/tats-u"><code>@​tats-u</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10143">#10143</a> docs: recommend users to remove hast-util-is-element in migration to v3 (<a href="https://github.com/tats-u"><code>@​tats-u</code></a>)</li>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10124">#10124</a> docs: v3 prepare your site blog post should point users to the upgrade guide (<a href="https://github.com/homotechsual"><code>@​homotechsual</code></a>)</li>
</ul>
<h4>:robot: Dependencies</h4>
<ul>
<li><a href="https://redirect.github.com/facebook/docusaurus/pull/10155">#10155</a> chore(deps): bump peaceiris/actions-gh-pages from 3 to 4 (<a href="https://github.com/apps/dependabot"><code>@​dependabot[bot]</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/facebook/docusaurus/commit/49e9a2143274a8dd795659b417b470bc42abbd6e"><code>49e9a21</code></a> v3.4.0</li>
<li><a href="https://github.com/facebook/docusaurus/commit/c125f7a27252cfbd4e8a65e4ee6ba2dee7f5f5c1"><code>c125f7a</code></a> chore: release Docusaurus 3.3.0 + 3.3.1 + 3.3.2 (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-theme-mermaid/issues/10101">#10101</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/f88da6c66d578f11960a1301e72ffdc4a59dd78b"><code>f88da6c</code></a> refactor: extract base TS client config + upgrade TS + refactor TS setup (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-theme-mermaid/issues/10">#10</a>...</li>
<li><a href="https://github.com/facebook/docusaurus/commit/e012e0315862b2ca02cad40c58d11d31c319ff75"><code>e012e03</code></a> chore: release Docusaurus 3.2.1 (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-theme-mermaid/issues/10016">#10016</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/debfc87d34c8b475fe4d76b64fe9c791c2dfd90b"><code>debfc87</code></a> chore: release Docusaurus v3.2.0 (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-theme-mermaid/issues/10000">#10000</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/0a2e6e67d36a4129b20810fbaebf2d0e970d5ce9"><code>0a2e6e6</code></a> fix: remove old useless mdx typedefs (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-theme-mermaid/issues/9733">#9733</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/85e5e552cbd237dc562e982d7fae346b730c3557"><code>85e5e55</code></a> chore: release Docusaurus 3.0.0 (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-theme-mermaid/issues/9478">#9478</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/495c7936b605e6b8881f000d23a8463a9d6d850c"><code>495c793</code></a> chore: v3.0.0-rc.1 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-theme-mermaid/issues/9453">#9453</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/7ee2f75ce1e645f75ae42b9f2f7f76cfc45b1743"><code>7ee2f75</code></a> chore: v3.0.0-rc.0 release (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-theme-mermaid/issues/9418">#9418</a>)</li>
<li><a href="https://github.com/facebook/docusaurus/commit/bde9cfd84d99ea1ca8fc59bf51f9d4001d6527f2"><code>bde9cfd</code></a> chore: update node engine version 18 (<a href="https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-theme-mermaid/issues/9348">#9348</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/facebook/docusaurus/commits/v3.4.0/packages/docusaurus-theme-mermaid">compare view</a></li>
</ul>
</details>
<br />

Updates `docusaurus-plugin-openapi-docs` from 1.7.3 to 3.0.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/releases">docusaurus-plugin-openapi-docs's releases</a>.</em></p>
<blockquote>
<h2>v3.0.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Fall back to languageSet if no languageTabs provided by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/871">PaloAltoNetworks/docusaurus-openapi-docs#871</a></li>
<li>Prepare release v3.0.1 by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/872">PaloAltoNetworks/docusaurus-openapi-docs#872</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/compare/v3.0.0...v3.0.1">https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/compare/v3.0.0...v3.0.1</a></p>
<h2>v3.0.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Allow custom plugin to render by <a href="https://github.com/jlvandenhout"><code>@​jlvandenhout</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/784">PaloAltoNetworks/docusaurus-openapi-docs#784</a></li>
<li>Ensure sidebars.ts and schemas are properly cleaned by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/817">PaloAltoNetworks/docusaurus-openapi-docs#817</a></li>
<li>Add missing types and cast ref to LegacyRef by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/818">PaloAltoNetworks/docusaurus-openapi-docs#818</a></li>
<li>Upgrade demo to docusaurus 3.3.2 by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/822">PaloAltoNetworks/docusaurus-openapi-docs#822</a></li>
<li>fix: markdown table within the description attribute cannot be rendered correctly by <a href="https://github.com/htmlin"><code>@​htmlin</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/831">PaloAltoNetworks/docusaurus-openapi-docs#831</a></li>
<li>Bug/set accept by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/846">PaloAltoNetworks/docusaurus-openapi-docs#846</a></li>
<li>Transparent background when displaying response placeholder by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/847">PaloAltoNetworks/docusaurus-openapi-docs#847</a></li>
<li>ensure readOnly/writeOnly are evaluated first by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/848">PaloAltoNetworks/docusaurus-openapi-docs#848</a></li>
<li>Support empty object schemas by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/849">PaloAltoNetworks/docusaurus-openapi-docs#849</a></li>
<li>upgrade to docusaurus 3.4.0 by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/850">PaloAltoNetworks/docusaurus-openapi-docs#850</a></li>
<li>handle various additionalProperties cases by <a href="https://github.com/Ugzuzg"><code>@​Ugzuzg</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/803">PaloAltoNetworks/docusaurus-openapi-docs#803</a></li>
<li>[V3] Avoid concatenating all tags when grouped by tagGroups by <a href="https://github.com/ElliotFriend"><code>@​ElliotFriend</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/853">PaloAltoNetworks/docusaurus-openapi-docs#853</a></li>
<li>[V3] Fix tagGroup display when showSchemas is configured by <a href="https://github.com/ElliotFriend"><code>@​ElliotFriend</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/852">PaloAltoNetworks/docusaurus-openapi-docs#852</a></li>
<li>Support custom downloadUrl for versions by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/859">PaloAltoNetworks/docusaurus-openapi-docs#859</a></li>
<li>Migrate to canonical postman dependencies by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/860">PaloAltoNetworks/docusaurus-openapi-docs#860</a></li>
<li>Support flexible code snippet ordering and options by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/862">PaloAltoNetworks/docusaurus-openapi-docs#862</a></li>
<li>Version dropdown styles by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/863">PaloAltoNetworks/docusaurus-openapi-docs#863</a></li>
<li>Support absolute or relative downloadUrl by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/865">PaloAltoNetworks/docusaurus-openapi-docs#865</a></li>
<li>Prepare release v3.0.0 by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/868">PaloAltoNetworks/docusaurus-openapi-docs#868</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/jlvandenhout"><code>@​jlvandenhout</code></a> made their first contribution in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/784">PaloAltoNetworks/docusaurus-openapi-docs#784</a></li>
<li><a href="https://github.com/htmlin"><code>@​htmlin</code></a> made their first contribution in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/831">PaloAltoNetworks/docusaurus-openapi-docs#831</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/compare/v3.0.0-beta.10...v3.0.0">https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/compare/v3.0.0-beta.10...v3.0.0</a></p>
<h2>v3.0.0-beta.10</h2>
<p>No release notes provided.</p>
<h2>v3.0.0-beta.9</h2>
<p>No release notes provided.</p>
<h2>v3.0.0-beta.8</h2>
<p>No release notes provided.</p>
<h2>v3.0.0-beta.7</h2>
<h2>What's Changed</h2>
<ul>
<li>Prepare release v3.0.0-beta.1 by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/661">PaloAltoNetworks/docusaurus-openapi-docs#661</a></li>
<li>Port v2 changes/fixes into v3 by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/667">PaloAltoNetworks/docusaurus-openapi-docs#667</a></li>
<li>Prepare release v3.0.0-beta.2 by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/668">PaloAltoNetworks/docusaurus-openapi-docs#668</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/blob/main/CHANGELOG.md">docusaurus-plugin-openapi-docs's changelog</a>.</em></p>
<blockquote>
<h2>3.0.1 (Jul 3, 2024)</h2>
<p>High level enhancements</p>
<ul>
<li>Fixed regression bug</li>
</ul>
<p>Other enhancements and bug fixes</p>
<ul>
<li>Fall back to languageSet if no languageTabs provided (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/871">#871</a>)</li>
</ul>
<h2>3.0.0 (Jul 3, 2024)</h2>
<p>First official v3 release!</p>
<ul>
<li>Added support for Docusaurus v3.0.1 - v3.4.0 (and hopefully beyond)</li>
<li>Complete feature parity with v2.2.0 including bug fixes</li>
</ul>
<p>Other enhancements and bug fixes</p>
<ul>
<li>Support absolute or relative downloadUrl (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/865">#865</a>)</li>
<li>fix...

_Description has been truncated_
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-07 00:36:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-docs/pull/122" class=".btn">#122</a>
            </td>
            <td>
                <b>
                    fix: update QSG after transferring repositories under the Hyperledger org
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
        Created At 2024-07-05 09:31:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-docs/pull/121" class=".btn">#121</a>
            </td>
            <td>
                <b>
                    ci: switch to PAT for checkout action
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
        Created At 2024-07-04 16:52:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-docs/pull/120" class=".btn">#120</a>
            </td>
            <td>
                <b>
                    ci: fix release flow
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
        Created At 2024-07-04 15:10:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-docs/pull/119" class=".btn">#119</a>
            </td>
            <td>
                <b>
                    feat: add submodule directories
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
        Created At 2024-07-04 14:57:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-docs/pull/118" class=".btn">#118</a>
            </td>
            <td>
                <b>
                    ci: fix ghcr login
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
        Created At 2024-07-04 14:52:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-docs/pull/117" class=".btn">#117</a>
            </td>
            <td>
                <b>
                    ci: fix release flow
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
        Created At 2024-07-04 14:45:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-docs/pull/116" class=".btn">#116</a>
            </td>
            <td>
                <b>
                    ci: fix deployment.yml
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
        Created At 2024-07-04 14:41:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-docs/pull/115" class=".btn">#115</a>
            </td>
            <td>
                <b>
                    ci: use PAT for commit the changes
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
        Created At 2024-07-04 14:36:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-docs/pull/114" class=".btn">#114</a>
            </td>
            <td>
                <b>
                    ci: fix autocommit action
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
        Created At 2024-07-04 14:26:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-docs/pull/113" class=".btn">#113</a>
            </td>
            <td>
                <b>
                    ci: fix gpg github action
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
        Created At 2024-07-04 14:19:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-docs/pull/112" class=".btn">#112</a>
            </td>
            <td>
                <b>
                    chore: reinit submodules from atala to identus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR:
- removed atala repositories submodules
- added identus repositories submodules
- fixed the paths in the CI
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-04 13:03:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-docs/pull/111" class=".btn">#111</a>
            </td>
            <td>
                <b>
                    ci: switch to the Hyperledger secrets in the GitHub actions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The PR contains the following changes:
- replace ATALA_GITHUB_TOKEN whenever it's possible
- switch from `atala-dev` bot to `hyperledger-bot`
- update GPG keys to sign the commits
- upgrade the GitHub actions to newer versions
- IDENTUS_CI token is added to the repository, but should be tested
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-04 10:53:49 +0000 UTC
    </div>
</div>

