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
                PR <a href="https://github.com/hyperledger/identus-docs/pull/123" class=".btn">#123</a>
            </td>
            <td>
                <b>
                    chore(deps): bump the npm_and_yarn group across 1 directory with 16 updates
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
| [async](https://github.com/caolan/async) | `3.2.1` | `3.2.4` |
| [docusaurus-plugin-openapi-docs](https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/tree/HEAD/packages/docusaurus-plugin-openapi-docs) | `1.7.3` | `3.0.1` |
| [docusaurus-theme-openapi-docs](https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/tree/HEAD/packages/docusaurus-theme-openapi-docs) | `1.7.3` | `2.2.1` |
| [axios](https://github.com/axios/axios) | `0.25.0` | `removed` |
| [@docusaurus/core](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus) | `2.4.3` | `3.4.0` |
| [@docusaurus/preset-classic](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-preset-classic) | `2.4.3` | `3.4.0` |
| [@docusaurus/theme-mermaid](https://github.com/facebook/docusaurus/tree/HEAD/packages/docusaurus-theme-mermaid) | `2.4.3` | `3.4.0` |
| [docusaurus-theme-openapi-docs](https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/tree/HEAD/packages/docusaurus-theme-openapi-docs) | `2.2.1` | `3.0.1` |
| [docusaurus-theme-redoc](https://github.com/rohit-gohri/redocusaurus) | `1.6.4` | `2.1.1` |
| [redocusaurus](https://github.com/rohit-gohri/redocusaurus) | `1.6.4` | `2.1.1` |
| [braces](https://github.com/micromatch/braces) | `3.0.2` | `3.0.3` |
| [express](https://github.com/expressjs/express) | `4.18.2` | `4.19.2` |
| [follow-redirects](https://github.com/follow-redirects/follow-redirects) | `1.15.4` | `1.15.6` |
| [webpack-dev-middleware](https://github.com/webpack/webpack-dev-middleware) | `5.3.3` | `5.3.4` |
| [ws](https://github.com/websockets/ws) | `7.5.9` | `7.5.10` |


Updates `async` from 3.2.1 to 3.2.4
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/caolan/async/blob/master/CHANGELOG.md">async's changelog</a>.</em></p>
<blockquote>
<h1>v3.2.4</h1>
<ul>
<li>Fix a bug in <code>priorityQueue</code> where it didn't wait for the result. (<a href="https://redirect.github.com/caolan/async/issues/1725">#1725</a>)</li>
<li>Fix a bug where <code>unshiftAsync</code> was included in <code>priorityQueue</code>. (<a href="https://redirect.github.com/caolan/async/issues/1790">#1790</a>)</li>
</ul>
<h1>v3.2.3</h1>
<ul>
<li>Fix bugs in comment parsing in <code>autoInject</code>. (<a href="https://redirect.github.com/caolan/async/issues/1767">#1767</a>, <a href="https://redirect.github.com/caolan/async/issues/1780">#1780</a>)</li>
</ul>
<h1>v3.2.2</h1>
<ul>
<li>Fix potential prototype pollution exploit</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/caolan/async/commit/f3ab51af76ca87ebe3ec67b3dd6dec4959e04816"><code>f3ab51a</code></a> Version 3.2.4</li>
<li><a href="https://github.com/caolan/async/commit/7ea2cec7398b33a15daf5c3bd9bda6ae78caf297"><code>7ea2cec</code></a> Update built files</li>
<li><a href="https://github.com/caolan/async/commit/bef7befc734e4b712ab6ffc82463cc40c1037056"><code>bef7bef</code></a> update changelog</li>
<li><a href="https://github.com/caolan/async/commit/03eeab36ae5a0454bbf67b881f087692e0b7c7e4"><code>03eeab3</code></a> Bump yargs from 17.4.1 to 17.5.1 (<a href="https://redirect.github.com/caolan/async/issues/1843">#1843</a>)</li>
<li><a href="https://github.com/caolan/async/commit/387efcf80f5b2c454effd2a64c75ff3c634ec3bd"><code>387efcf</code></a> Bump eslint from 8.14.0 to 8.17.0 (<a href="https://redirect.github.com/caolan/async/issues/1849">#1849</a>)</li>
<li><a href="https://github.com/caolan/async/commit/131225a8c82fda93010b8b82da46e9a23b6b1816"><code>131225a</code></a> Bump karma from 6.3.19 to 6.3.20 (<a href="https://redirect.github.com/caolan/async/issues/1844">#1844</a>)</li>
<li><a href="https://github.com/caolan/async/commit/4cfa89cb240d9748d5bfee0656fbed08cf80cc10"><code>4cfa89c</code></a> Bump eslint from 8.14.0 to 8.16.0 (<a href="https://redirect.github.com/caolan/async/issues/1845">#1845</a>)</li>
<li><a href="https://github.com/caolan/async/commit/90e940cbb5a051db7c2a28169769f97eef99fdd6"><code>90e940c</code></a> Bump rollup from 2.71.1 to 2.75.5 (<a href="https://redirect.github.com/caolan/async/issues/1846">#1846</a>)</li>
<li><a href="https://github.com/caolan/async/commit/dd72cf5f614bcf2b08ae2678f6e8ffbd28136804"><code>dd72cf5</code></a> Bump <code>@​babel/eslint-parser</code> from 7.17.0 to 7.18.2 (<a href="https://redirect.github.com/caolan/async/issues/1847">#1847</a>)</li>
<li><a href="https://github.com/caolan/async/commit/4ae026e8da11f817f274f264dd3a9ec7ef3307c5"><code>4ae026e</code></a> Bump babel-minify from 0.5.1 to 0.5.2 (<a href="https://redirect.github.com/caolan/async/issues/1848">#1848</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/caolan/async/compare/v3.2.1...v3.2.4">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~hargasinski">hargasinski</a>, a new releaser for async since your current version.</p>
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
<li>fix typo in attribute (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/864">#864</a>)</li>
<li>uncomment version dropdown styles (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/863">#863</a>)</li>
<li>Support flexible code snippet ordering and options (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/862">#862</a>)</li>
<li>migrate back to canonical postman deps (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/860">#860</a>)</li>
<li>Support custom downloadUrl for versions (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/859">#859</a>)</li>
<li>[V3] Fix tagGroup display when showSchemas is configured (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/852">#852</a>)</li>
<li>check to avoid tagGroup config before concat operation, api, schemas (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/853">#853</a>)</li>
<li>handle various additionalProperties cases (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/803">#803</a>)</li>
<li>cleanup legacy ApiDemoPanel component</li>
<li>cleanup legacy docusaurus config</li>
<li>upgrade to docusaurus 3.4.0 (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/850">#850</a>)</li>
<li>support empty object schema type (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/849">#849</a>)</li>
<li>ensure readOnly/writeOnly are evaluated first (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/848">#848</a>)</li>
<li>transparent bg color when showing placeholder (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/847">#847</a>)</li>
<li>Bug/set accept (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/846">#846</a>)</li>
<li>Implement the <code>x-tags</code> extension for schema objects (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/837">#837</a>)</li>
<li>fix col row padding footer&amp;pagination (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/810">#810</a>)</li>
<li>Update index.tsx (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/839">#839</a>)</li>
<li>fix: markdown table within the description attribute cannot be rendered correctly (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/831">#831</a>)</li>
<li>upgrade demo to docusaurus 3.3.2 (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/822">#822</a>)</li>
<li>add missing types and cast ref to LegacyRef (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/818">#818</a>)</li>
<li>Add option to disable frontmatter api prop compression (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/800">#800</a>)</li>
<li>preventing to send form onClick left/right arrows in SchemaTabs component (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/796">#796</a>)</li>
<li>Ensure sidebars.ts and schemas are properly cleaned (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/817">#817</a>)</li>
<li>changed theme and plugin to headings (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/786">#786</a>)</li>
<li>Allow custom plugin to render (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/784">#784</a>)</li>
<li>Remove scrollbar width for Tab components (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/785">#785</a>)</li>
</ul>
<h2>3.0.0-beta.10 (Mar 25, 2024)</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/commit/5f6e43a2b1fcc1c266941879cb73365eb3d68e5a"><code>5f6e43a</code></a> Prepare release v3.0.1 (<a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/tree/HEAD/packages/docusaurus-plugin-openapi-docs/issues/872">#872</a>)</li>
<li><a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/commit/d03859d67953de59558a3fa84e7cc690941dbd69"><code>d03859d</code></a> Prepare release v3.0.0 (<a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/tree/HEAD/packages/docusaurus-plugin-openapi-docs/issues/868">#868</a>)</li>
<li><a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/commit/3675c4e43e38c6509de8ebf1368156f0a6ee1b30"><code>3675c4e</code></a> Support absolute or relative downloadUrl (<a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/tree/HEAD/packages/docusaurus-plugin-openapi-docs/issues/865">#865</a>)</li>
<li><a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/commit/c618b4c3fad09ea2c95224e2cef68ca7827e24f9"><code>c618b4c</code></a> fix typo in attribute (<a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/tree/HEAD/packages/docusaurus-plugin-openapi-docs/issues/864">#864</a>)</li>
<li><a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/commit/03f3c9ae9d3465de57db971fb8f5e7c8607e2194"><code>03f3c9a</code></a> migrate back to canonical postman deps (<a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/tree/HEAD/packages/docusaurus-plugin-openapi-docs/issues/860">#860</a>)</li>
<li><a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/commit/8ea889eb778bee348e15e81079c79d04e054f369"><code>8ea889e</code></a> Support custom downloadUrl for versions (<a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/tree/HEAD/packages/docusaurus-plugin-openapi-docs/issues/859">#859</a>)</li>
<li><a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/commit/1122d94aa1ec6af0b83c8360a0a92eb28dbea223"><code>1122d94</code></a> [V3] Fix tagGroup display when showSchemas is configured (<a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/tree/HEAD/packages/docusaurus-plugin-openapi-docs/issues/852">#852</a>)</li>
<li><a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/commit/0a8aafc80514c95ffebf9531bc3b59813cf95b9f"><code>0a8aafc</code></a> check to avoid tagGroup config before concat operation, api, schemas (<a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/tree/HEAD/packages/docusaurus-plugin-openapi-docs/issues/853">#853</a>)</li>
<li><a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/commit/4e960fd8dc7f5c5dff2270792f474745a587fb63"><code>4e960fd</code></a> handle various additionalProperties cases (<a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/tree/HEAD/packages/docusaurus-plugin-openapi-docs/issues/803">#803</a>)</li>
<li><a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/commit/ea36cfa313ab825d9e0c1feb6833775a98aaeb68"><code>ea36cfa</code></a> support empty object schema type (<a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/tree/HEAD/packages/docusaurus-plugin-openapi-docs/issues/849">#849</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/commits/v3.0.1/packages/docusaurus-plugin-openapi-docs">compare view</a></li>
</ul>
</details>
<br />

Updates `docusaurus-theme-openapi-docs` from 1.7.3 to 2.2.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/releases">docusaurus-theme-openapi-docs's releases</a>.</em></p>
<blockquote>
<h2>v2.2.1</h2>
<h2>What's Changed</h2>
<ul>
<li>[UI Bug Fix] Firefox issue: Hide empty scrollbar track from Tab components  by <a href="https://github.com/blindaa121"><code>@​blindaa121</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/785">PaloAltoNetworks/docusaurus-openapi-docs#785</a></li>
<li>changed theme and plugin to headings by <a href="https://github.com/tjperry07"><code>@​tjperry07</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/786">PaloAltoNetworks/docusaurus-openapi-docs#786</a></li>
<li>preventing to send form onClick left/right arrows in SchemaTabs compo… by <a href="https://github.com/stakoov"><code>@​stakoov</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/796">PaloAltoNetworks/docusaurus-openapi-docs#796</a></li>
<li>Add option to disable frontmatter api prop compression by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/800">PaloAltoNetworks/docusaurus-openapi-docs#800</a></li>
<li>Fix clean-api-docs not deleting sidebar.ts by <a href="https://github.com/MarcL01"><code>@​MarcL01</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/829">PaloAltoNetworks/docusaurus-openapi-docs#829</a></li>
<li>Fix - <code>@​theme/ApiItem</code> causes undesired website-wide style changes by <a href="https://github.com/hadar-co"><code>@​hadar-co</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/839">PaloAltoNetworks/docusaurus-openapi-docs#839</a></li>
<li>fix col row padding footer&amp;pagination by <a href="https://github.com/entense"><code>@​entense</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/810">PaloAltoNetworks/docusaurus-openapi-docs#810</a></li>
<li>Implement the <code>x-tags</code> extension for schema objects by <a href="https://github.com/ElliotFriend"><code>@​ElliotFriend</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/837">PaloAltoNetworks/docusaurus-openapi-docs#837</a></li>
<li>Avoid concatenating all tags when grouped by tagGroups by <a href="https://github.com/ElliotFriend"><code>@​ElliotFriend</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/854">PaloAltoNetworks/docusaurus-openapi-docs#854</a></li>
<li>Fix tagGroup display when showSchemas is configured by <a href="https://github.com/ElliotFriend"><code>@​ElliotFriend</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/851">PaloAltoNetworks/docusaurus-openapi-docs#851</a></li>
<li>Revert to canonical postman libraries by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/861">PaloAltoNetworks/docusaurus-openapi-docs#861</a></li>
<li>fix typo in attribute by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/864">PaloAltoNetworks/docusaurus-openapi-docs#864</a></li>
<li>Prepare release v2.2.0 by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/866">PaloAltoNetworks/docusaurus-openapi-docs#866</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/tjperry07"><code>@​tjperry07</code></a> made their first contribution in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/786">PaloAltoNetworks/docusaurus-openapi-docs#786</a></li>
<li><a href="https://github.com/stakoov"><code>@​stakoov</code></a> made their first contribution in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/796">PaloAltoNetworks/docusaurus-openapi-docs#796</a></li>
<li><a href="https://github.com/hadar-co"><code>@​hadar-co</code></a> made their first contribution in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/839">PaloAltoNetworks/docusaurus-openapi-docs#839</a></li>
<li><a href="https://github.com/entense"><code>@​entense</code></a> made their first contribution in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/810">PaloAltoNetworks/docusaurus-openapi-docs#810</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/compare/v2.1.3...v2.2.0">https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/compare/v2.1.3...v2.2.0</a></p>
<h2>v2.1.3</h2>
<h2>What's Changed</h2>
<ul>
<li>Ensure correct eval of required properties with nested allOf by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/771">PaloAltoNetworks/docusaurus-openapi-docs#771</a></li>
<li>Prepare release v2.1.3 by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/772">PaloAltoNetworks/docusaurus-openapi-docs#772</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/compare/v2.1.2...v2.1.3">https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/compare/v2.1.2...v2.1.3</a></p>
<h2>v2.1.2</h2>
<h2>What's Changed</h2>
<ul>
<li>[bug] Ensure resize observer is calculated once per frame to avoid loops by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/763">PaloAltoNetworks/docusaurus-openapi-docs#763</a></li>
<li>Uncomment line preventing grouping by operation tags by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/764">PaloAltoNetworks/docusaurus-openapi-docs#764</a></li>
<li>Ensure qualifiers are rendered for polymorphic/primitive properties by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/765">PaloAltoNetworks/docusaurus-openapi-docs#765</a></li>
<li>Fix allOf schema qualifier and type by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/766">PaloAltoNetworks/docusaurus-openapi-docs#766</a></li>
<li>Prepare release v2.1.2 by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/768">PaloAltoNetworks/docusaurus-openapi-docs#768</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/compare/v2.1.1...v2.1.2">https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/compare/v2.1.1...v2.1.2</a></p>
<h2>v2.1.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Upgrade OpenAPI parsers by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/748">PaloAltoNetworks/docusaurus-openapi-docs#748</a></li>
<li>[bugfix] Ensure 0 and false are guarded correctly and add deprecated support to params by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/754">PaloAltoNetworks/docusaurus-openapi-docs#754</a></li>
<li>cleanup console log by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/755">PaloAltoNetworks/docusaurus-openapi-docs#755</a></li>
<li>Prepare release v2.1.1 by <a href="https://github.com/sserrata"><code>@​sserrata</code></a> in <a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/756">PaloAltoNetworks/docusaurus-openapi-docs#756</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/blob/v2.2.1/CHANGELOG.md">docusaurus-theme-openapi-docs's changelog</a>.</em></p>
<blockquote>
<h2>2.2.1 (Jul 3, 2024)</h2>
<p>High level enhancements</p>
<ul>
<li>Fixed regression bug</li>
</ul>
<p>Other enhancements and bug fixes</p>
<ul>
<li>Fall back to languageSet if no languageTabs provided (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/871">#871</a>)</li>
</ul>
<h2>2.2.0 (Jul 3, 2024)</h2>
<p>High level enhancements</p>
<ul>
<li>Improved support for customizing code snippets</li>
<li>Switched back to canonical postman depdendencies</li>
<li>Improved support for OpenAPI readOnly/writeOnly</li>
<li>Added support for OpenAPI <code>x-tags</code></li>
</ul>
<p>Other enhancements and bug fixes</p>
<ul>
<li>fix typo in attribute (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/864">#864</a>)</li>
<li>uncomment version dropdown styles (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/863">#863</a>)</li>
<li>revert to canonical postman libraries (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/861">#861</a>)</li>
<li>Fix tagGroup display when showSchemas is configured (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/851">#851</a>)</li>
<li>check to avoid tagGroup config before concat operation, api, schemas (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/854">#854</a>)</li>
<li>support empty object schema type (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/849">#849</a>)</li>
<li>ensure readOnly/writeOnly are evaluated first (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/848">#848</a>)</li>
<li>fix: markdown table within the description attribute cannot be rendered correctly (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/831">#831</a>)</li>
<li>Implement the <code>x-tags</code> extension for schema objects (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/837">#837</a>)</li>
<li>fix col row padding footer&amp;pagination (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/810">#810</a>)</li>
<li>Update index.tsx (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/839">#839</a>)</li>
<li>Fix clean-api-docs not deleting sidebar.ts (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/829">#829</a>)</li>
<li>Add option to disable frontmatter api prop compression (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/800">#800</a>)</li>
<li>preventing to send form onClick left/right arrows in SchemaTabs component (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/796">#796</a>)</li>
<li>changed theme and plugin to headings (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/786">#786</a>)</li>
<li>Allow custom plugin to render (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/784">#784</a>)</li>
<li>Remove scrollbar width for Tab components (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/785">#785</a>)</li>
</ul>
<h2>2.1.3 (Mar 22, 2024)</h2>
<p>High level enhancements</p>
<ul>
<li>bugfix</li>
</ul>
<p>Other enhancements and bug fixes</p>
<ul>
<li>ensure correct eval of required properties with allOf (<a href="https://redirect.github.com/PaloAltoNetworks/docusaurus-openapi-docs/pull/771">#771</a>)</li>
</ul>
<h2>2.1.2 (Mar 21, 2024)</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/commit/73b212d18343aa7a35ede5136f5353f06b89d25f"><code>73b212d</code></a> Prepare release v2.2.1 (<a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/tree/HEAD/packages/docusaurus-theme-openapi-docs/issues/876">#876</a>)</li>
<li><a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/commit/357edaf862b70b46417d6c487ee1574bb220571f"><code>357edaf</code></a> Fall back to languageSet if no languageTabs provided (<a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/tree/HEAD/packages/docusaurus-theme-openapi-docs/issues/871">#871</a>) (<a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/tree/HEAD/packages/docusaurus-theme-openapi-docs/issues/875">#875</a>)</li>
<li><a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/commit/060b5777c783abc23cd3744a6d43deb4df80cebd"><code>060b577</code></a> Prepare release v2.2.0 (<a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/tree/HEAD/packages/docusaurus-theme-openapi-docs/issues/866">#866</a>)</li>
<li><a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/commit/89675ca736901b07943d1fe8501080841c368e9f"><code>89675ca</code></a> uncomment version dropdown styles (<a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/tree/HEAD/packages/docusaurus-theme-openapi-docs/issues/863">#863</a>)</li>
<li><a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/commit/94d8e2ef21111df590bc9edc470ccc048df766be"><code>94d8e2e</code></a> fix formatting issues</li>
<li><a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/commit/9367911580ef23fe65dccf2ca433ea45d3c572ea"><code>9367911</code></a> cleanup ts config</li>
<li><a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/commit/45e9834ddb3bbbde575a5c43302982e74b4f737b"><code>45e9834</code></a> revert to canonical postman libraries (<a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/tree/HEAD/packages/docusaurus-theme-openapi-docs/issues/861">#861</a>)</li>
<li><a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/commit/bf5d1a3e8cc563367801048476a8b35aba87fdf7"><code>bf5d1a3</code></a> cleanup legacy ApiDemoPanel component</li>
<li><a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/commit/1ac868fb55096c0f26b17a5574925ad95efc756d"><code>1ac868f</code></a> fix col row padding footer&amp;pagination (<a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/tree/HEAD/packages/docusaurus-theme-openapi-docs/issues/810">#810</a>)</li>
<li><a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/commit/1de79c0449a95f2e51a9a6027365fa902be0d996"><code>1de79c0</code></a> Update index.tsx (<a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/tree/HEAD/packages/docusaurus-theme-openapi-docs/issues/839">#839</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/PaloAltoNetworks/docusaurus-openapi-docs/commits/v2.2.1/packages/docusaurus-theme-openapi-docs">compare view</a></li>
</ul>
</details>
<br />

Removes `axios`

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
<li><code>docusaurus-plugin-co...

_Description has been truncated_
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-05 10:32:24 +0000 UTC
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

