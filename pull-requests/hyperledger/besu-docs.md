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
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1358" class=".btn">#1358</a>
            </td>
            <td>
                <b>
                    Remove 'raft' from sample helm values.yml, replace 'ibft' with 'ibft2'
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I noticed that the Besu docs have `raft` in the example helm chart options, which Besu doesn't support. Also `ibft` is deprecated and has been replaced with `ibft2` so thought I'd update that as well.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-10 10:29:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1357" class=".btn">#1357</a>
            </td>
            <td>
                <b>
                    Bump stylelint from 14.16.1 to 15.10.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [stylelint](https://github.com/stylelint/stylelint) from 14.16.1 to 15.10.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/stylelint/stylelint/releases">stylelint's releases</a>.</em></p>
<blockquote>
<h2>15.10.1</h2>
<ul>
<li>Security: fix for <code>semver</code> vulnerability (<a href="https://redirect.github.com/stylelint/stylelint/issues/7043">#7043</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: invalid option regression on Windows 10 (<a href="https://redirect.github.com/stylelint/stylelint/issues/7043">#7043</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
</ul>
<h2>15.10.0</h2>
<ul>
<li>Added: <code>media-query-no-invalid</code> (<a href="https://redirect.github.com/stylelint/stylelint/issues/6963">#6963</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Added: support for JS objects with <code>extends</code> config option (<a href="https://redirect.github.com/stylelint/stylelint/issues/6998">#6998</a>) (<a href="https://github.com/fpetrakov"><code>@​fpetrakov</code></a>).</li>
<li>Fixed: inconsistent <code>errored</code> properties in <code>stylelint.lint()</code> return value (<a href="https://redirect.github.com/stylelint/stylelint/issues/6983">#6983</a>) (<a href="https://github.com/ybiquitous"><code>@​ybiquitous</code></a>).</li>
<li>Fixed: <code>{selector,value}-no-vendor-prefix</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/issues/7016">#7016</a>) (<a href="https://github.com/jeddy3"><code>@​jeddy3</code></a>).</li>
<li>Fixed: <code>custom-property-pattern</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/issues/7009">#7009</a>) (<a href="https://github.com/jeddy3"><code>@​jeddy3</code></a>).</li>
<li>Fixed: <code>function-linear-gradient-no-nonstandard-direction</code> false positives for <code>&lt;color-interpolation-method&gt;</code> (<a href="https://redirect.github.com/stylelint/stylelint/issues/6987">#6987</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>function-name-case</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/issues/7010">#7010</a>) (<a href="https://github.com/jeddy3"><code>@​jeddy3</code></a>).</li>
<li>Fixed: <code>function-no-unknown</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/issues/7004">#7004</a>) (<a href="https://github.com/jeddy3"><code>@​jeddy3</code></a>).</li>
<li>Fixed: <code>function-url-quotes</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/issues/7011">#7011</a>) (<a href="https://github.com/jeddy3"><code>@​jeddy3</code></a>).</li>
<li>Fixed: <code>hue-degree-notation</code> false negatives for <code>oklch</code> (<a href="https://redirect.github.com/stylelint/stylelint/issues/7015">#7015</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>hue-degree-notation</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/issues/7012">#7012</a>) (<a href="https://github.com/jeddy3"><code>@​jeddy3</code></a>).</li>
<li>Fixed: <code>media-feature-name-no-unknown</code> false positives for <code>environment-blending</code>, <code>nav-controls</code>, <code>prefers-reduced-data</code>, and <code>video-color-gamut</code> (<a href="https://redirect.github.com/stylelint/stylelint/issues/6978">#6978</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>media-feature-name-no-vendor-prefix</code> positions for <code>*-device-pixel-ratio</code> (<a href="https://redirect.github.com/stylelint/stylelint/issues/6977">#6977</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>no-descending-specificity</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/issues/7026">#7026</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>no-duplicate-at-import-rules</code> false negatives for imports with <code>supports</code> and <code>layer</code> conditions (<a href="https://redirect.github.com/stylelint/stylelint/issues/7001">#7001</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>selector-anb-no-unmatchable</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/issues/7042">#7042</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>selector-id-pattern</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/issues/7013">#7013</a>) (<a href="https://github.com/jeddy3"><code>@​jeddy3</code></a>).</li>
<li>Fixed: <code>selector-pseudo-class-no-unknown</code> false negatives for pseudo-elements with matching names (<a href="https://redirect.github.com/stylelint/stylelint/issues/6964">#6964</a>) (<a href="https://github.com/Mouvedia"><code>@​Mouvedia</code></a>).</li>
<li>Fixed: <code>selector-pseudo-element-no-unknown</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/issues/7007">#7007</a>) (<a href="https://github.com/jeddy3"><code>@​jeddy3</code></a>).</li>
<li>Fixed: <code>selector-type-case</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/issues/7041">#7041</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>selector-type-no-unknown</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/issues/7027">#7027</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>unit-disallowed-list</code> false negatives with percentages (<a href="https://redirect.github.com/stylelint/stylelint/issues/7018">#7018</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
</ul>
<h2>15.9.0</h2>
<ul>
<li>Added: <code>insideFunctions: {&quot;function&quot;: int}</code> to <code>number-max-precision</code> (<a href="https://redirect.github.com/stylelint/stylelint/issues/6932">#6932</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>declaration-block-no-redundant-longhand-properties</code> autofix for <code>border-radius</code> shorthand (<a href="https://redirect.github.com/stylelint/stylelint/issues/6958">#6958</a>) (<a href="https://github.com/mattxwang"><code>@​mattxwang</code></a>).</li>
<li>Fixed: <code>declaration-block-no-redundant-longhand-properties</code> autofix for <code>border-width</code> shorthand (<a href="https://redirect.github.com/stylelint/stylelint/issues/6956">#6956</a>) (<a href="https://github.com/mattxwang"><code>@​mattxwang</code></a>).</li>
<li>Fixed: <code>declaration-block-no-redundant-longhand-properties</code> autofix for <code>grid-column</code> and <code>grid-row</code> (<a href="https://redirect.github.com/stylelint/stylelint/issues/6957">#6957</a>) (<a href="https://github.com/mattxwang"><code>@​mattxwang</code></a>).</li>
</ul>
<h2>15.8.0</h2>
<ul>
<li>Added: <code>media-feature-name-value-no-unknown</code> (<a href="https://redirect.github.com/stylelint/stylelint/issues/6906">#6906</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Added: support for <code>.mjs</code> configuration files (<a href="https://redirect.github.com/stylelint/stylelint/issues/6910">#6910</a>) (<a href="https://github.com/ybiquitous"><code>@​ybiquitous</code></a>).</li>
<li>Fixed: <code>--print-config</code> description in CLI help (<a href="https://redirect.github.com/stylelint/stylelint/issues/6914">#6914</a>) (<a href="https://github.com/ybiquitous"><code>@​ybiquitous</code></a>).</li>
<li>Fixed: <code>allowEmptyInput</code> option in configuration files (<a href="https://redirect.github.com/stylelint/stylelint/issues/6929">#6929</a>) (<a href="https://github.com/ybiquitous"><code>@​ybiquitous</code></a>).</li>
<li>Fixed: <code>custom-property-no-missing-var-function</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/issues/6922">#6922</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>function-calc-no-unspaced-operator</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/issues/6923">#6923</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>function-linear-gradient-no-nonstandard-direction</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/issues/6924">#6924</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>function-no-unknown</code> false positives for SCSS functions with namespace (<a href="https://redirect.github.com/stylelint/stylelint/issues/6921">#6921</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>max-nesting-depth</code> error for at-rules in Sass syntax (<a href="https://redirect.github.com/stylelint/stylelint/issues/6909">#6909</a>) (<a href="https://github.com/ybiquitous"><code>@​ybiquitous</code></a>).</li>
<li>Fixed: <code>selector-anb-no-unmatchable</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/issues/6925">#6925</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: remove <code>v8-compile-cache</code> dependency (<a href="https://redirect.github.com/stylelint/stylelint/issues/6907">#6907</a>) (<a href="https://github.com/ybiquitous"><code>@​ybiquitous</code></a>).</li>
</ul>
<h2>15.7.0</h2>
<ul>
<li>Added: <code>splitList: boolean</code> to <code>selector-nested-pattern</code> (<a href="https://redirect.github.com/stylelint/stylelint/issues/6896">#6896</a>) (<a href="https://github.com/is2ei"><code>@​is2ei</code></a>).</li>
<li>Fixed: <code>unit-no-unknown</code> false positives for <code>unicode-range</code> descriptors (<a href="https://redirect.github.com/stylelint/stylelint/issues/6892">#6892</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/stylelint/stylelint/blob/main/CHANGELOG.md">stylelint's changelog</a>.</em></p>
<blockquote>
<h2>15.10.1</h2>
<ul>
<li>Security: fix for <code>semver</code> vulnerability (<a href="https://redirect.github.com/stylelint/stylelint/pull/7043">#7043</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: invalid option regression on Windows 10 (<a href="https://redirect.github.com/stylelint/stylelint/pull/7043">#7043</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
</ul>
<h2>15.10.0</h2>
<ul>
<li>Added: <code>media-query-no-invalid</code> (<a href="https://redirect.github.com/stylelint/stylelint/pull/6963">#6963</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Added: support for JS objects with <code>extends</code> config option (<a href="https://redirect.github.com/stylelint/stylelint/pull/6998">#6998</a>) (<a href="https://github.com/fpetrakov"><code>@​fpetrakov</code></a>).</li>
<li>Fixed: inconsistent <code>errored</code> properties in <code>stylelint.lint()</code> return value (<a href="https://redirect.github.com/stylelint/stylelint/pull/6983">#6983</a>) (<a href="https://github.com/ybiquitous"><code>@​ybiquitous</code></a>).</li>
<li>Fixed: <code>{selector,value}-no-vendor-prefix</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/pull/7016">#7016</a>) (<a href="https://github.com/jeddy3"><code>@​jeddy3</code></a>).</li>
<li>Fixed: <code>custom-property-pattern</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/pull/7009">#7009</a>) (<a href="https://github.com/jeddy3"><code>@​jeddy3</code></a>).</li>
<li>Fixed: <code>function-linear-gradient-no-nonstandard-direction</code> false positives for <code>&lt;color-interpolation-method&gt;</code> (<a href="https://redirect.github.com/stylelint/stylelint/pull/6987">#6987</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>function-name-case</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/pull/7010">#7010</a>) (<a href="https://github.com/jeddy3"><code>@​jeddy3</code></a>).</li>
<li>Fixed: <code>function-no-unknown</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/pull/7004">#7004</a>) (<a href="https://github.com/jeddy3"><code>@​jeddy3</code></a>).</li>
<li>Fixed: <code>function-url-quotes</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/pull/7011">#7011</a>) (<a href="https://github.com/jeddy3"><code>@​jeddy3</code></a>).</li>
<li>Fixed: <code>hue-degree-notation</code> false negatives for <code>oklch</code> (<a href="https://redirect.github.com/stylelint/stylelint/pull/7015">#7015</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>hue-degree-notation</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/pull/7012">#7012</a>) (<a href="https://github.com/jeddy3"><code>@​jeddy3</code></a>).</li>
<li>Fixed: <code>media-feature-name-no-unknown</code> false positives for <code>environment-blending</code>, <code>nav-controls</code>, <code>prefers-reduced-data</code>, and <code>video-color-gamut</code> (<a href="https://redirect.github.com/stylelint/stylelint/pull/6978">#6978</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>media-feature-name-no-vendor-prefix</code> positions for <code>*-device-pixel-ratio</code> (<a href="https://redirect.github.com/stylelint/stylelint/pull/6977">#6977</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>no-descending-specificity</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/pull/7026">#7026</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>no-duplicate-at-import-rules</code> false negatives for imports with <code>supports</code> and <code>layer</code> conditions (<a href="https://redirect.github.com/stylelint/stylelint/pull/7001">#7001</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>selector-anb-no-unmatchable</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/pull/7042">#7042</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>selector-id-pattern</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/pull/7013">#7013</a>) (<a href="https://github.com/jeddy3"><code>@​jeddy3</code></a>).</li>
<li>Fixed: <code>selector-pseudo-class-no-unknown</code> false negatives for pseudo-elements with matching names (<a href="https://redirect.github.com/stylelint/stylelint/pull/6964">#6964</a>) (<a href="https://github.com/Mouvedia"><code>@​Mouvedia</code></a>).</li>
<li>Fixed: <code>selector-pseudo-element-no-unknown</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/pull/7007">#7007</a>) (<a href="https://github.com/jeddy3"><code>@​jeddy3</code></a>).</li>
<li>Fixed: <code>selector-type-case</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/pull/7041">#7041</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>selector-type-no-unknown</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/pull/7027">#7027</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>unit-disallowed-list</code> false negatives with percentages (<a href="https://redirect.github.com/stylelint/stylelint/pull/7018">#7018</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
</ul>
<h2>15.9.0</h2>
<ul>
<li>Added: <code>insideFunctions: {&quot;function&quot;: int}</code> to <code>number-max-precision</code> (<a href="https://redirect.github.com/stylelint/stylelint/pull/6932">#6932</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>declaration-block-no-redundant-longhand-properties</code> autofix for <code>border-radius</code> shorthand (<a href="https://redirect.github.com/stylelint/stylelint/pull/6958">#6958</a>) (<a href="https://github.com/mattxwang"><code>@​mattxwang</code></a>).</li>
<li>Fixed: <code>declaration-block-no-redundant-longhand-properties</code> autofix for <code>border-width</code> shorthand (<a href="https://redirect.github.com/stylelint/stylelint/pull/6956">#6956</a>) (<a href="https://github.com/mattxwang"><code>@​mattxwang</code></a>).</li>
<li>Fixed: <code>declaration-block-no-redundant-longhand-properties</code> autofix for <code>grid-column</code> and <code>grid-row</code> (<a href="https://redirect.github.com/stylelint/stylelint/pull/6957">#6957</a>) (<a href="https://github.com/mattxwang"><code>@​mattxwang</code></a>).</li>
</ul>
<h2>15.8.0</h2>
<ul>
<li>Added: <code>media-feature-name-value-no-unknown</code> (<a href="https://redirect.github.com/stylelint/stylelint/pull/6906">#6906</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Added: support for <code>.mjs</code> configuration files (<a href="https://redirect.github.com/stylelint/stylelint/pull/6910">#6910</a>) (<a href="https://github.com/ybiquitous"><code>@​ybiquitous</code></a>).</li>
<li>Fixed: <code>--print-config</code> description in CLI help (<a href="https://redirect.github.com/stylelint/stylelint/pull/6914">#6914</a>) (<a href="https://github.com/ybiquitous"><code>@​ybiquitous</code></a>).</li>
<li>Fixed: <code>allowEmptyInput</code> option in configuration files (<a href="https://redirect.github.com/stylelint/stylelint/pull/6929">#6929</a>) (<a href="https://github.com/ybiquitous"><code>@​ybiquitous</code></a>).</li>
<li>Fixed: <code>custom-property-no-missing-var-function</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/pull/6922">#6922</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>function-calc-no-unspaced-operator</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/pull/6923">#6923</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>function-linear-gradient-no-nonstandard-direction</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/pull/6924">#6924</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>function-no-unknown</code> false positives for SCSS functions with namespace (<a href="https://redirect.github.com/stylelint/stylelint/pull/6921">#6921</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: <code>max-nesting-depth</code> error for at-rules in Sass syntax (<a href="https://redirect.github.com/stylelint/stylelint/pull/6909">#6909</a>) (<a href="https://github.com/ybiquitous"><code>@​ybiquitous</code></a>).</li>
<li>Fixed: <code>selector-anb-no-unmatchable</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/pull/6925">#6925</a>) (<a href="https://github.com/romainmenke"><code>@​romainmenke</code></a>).</li>
<li>Fixed: remove <code>v8-compile-cache</code> dependency (<a href="https://redirect.github.com/stylelint/stylelint/pull/6907">#6907</a>) (<a href="https://github.com/ybiquitous"><code>@​ybiquitous</code></a>).</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/stylelint/stylelint/commit/fb8cf35dae79e150ad17c75660bd93c4d4c0c9e0"><code>fb8cf35</code></a> 15.10.1</li>
<li><a href="https://github.com/stylelint/stylelint/commit/eeed72bdde9a368df0fa01952a1cfc94364c84ca"><code>eeed72b</code></a> Prepare release (<a href="https://redirect.github.com/stylelint/stylelint/issues/7048">#7048</a>)</li>
<li><a href="https://github.com/stylelint/stylelint/commit/80905538500d32a6f716fb1359e59de9fb418d02"><code>8090553</code></a> Document check of configs in release process (<a href="https://redirect.github.com/stylelint/stylelint/issues/7047">#7047</a>)</li>
<li><a href="https://github.com/stylelint/stylelint/commit/56a545e116e4f4bd52595a3eb3d131306ce02862"><code>56a545e</code></a> Security fix for <code>semver</code> vulnerability (<a href="https://redirect.github.com/stylelint/stylelint/issues/7043">#7043</a>)</li>
<li><a href="https://github.com/stylelint/stylelint/commit/a42f95582c2a928122fc1e59f9f8acc078fb9b91"><code>a42f955</code></a> Fix rules documentation for <code>media-query-no-invalid</code> (<a href="https://redirect.github.com/stylelint/stylelint/issues/7044">#7044</a>)</li>
<li><a href="https://github.com/stylelint/stylelint/commit/e56aa3001c3ef0070c6b2713a1554257f37472ab"><code>e56aa30</code></a> 15.10.0</li>
<li><a href="https://github.com/stylelint/stylelint/commit/c9e89ebcf6495d3935d8e6ee29eb6607f936caf3"><code>c9e89eb</code></a> Prepare release (<a href="https://redirect.github.com/stylelint/stylelint/issues/6974">#6974</a>)</li>
<li><a href="https://github.com/stylelint/stylelint/commit/b8e53176d42b496f84eaa520d9067c87e9080469"><code>b8e5317</code></a> Fix <code>selector-type-case</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/issues/7041">#7041</a>)</li>
<li><a href="https://github.com/stylelint/stylelint/commit/f82a24a6508f8a3a7d752b828cdb216e103cab63"><code>f82a24a</code></a> Fix <code>selector-anb-no-unmatchable</code> performance (<a href="https://redirect.github.com/stylelint/stylelint/issues/7042">#7042</a>)</li>
<li><a href="https://github.com/stylelint/stylelint/commit/16110fdde589caca7fafc0d2a167542bc5080d62"><code>16110fd</code></a> Revert removed changelog entry (<a href="https://redirect.github.com/stylelint/stylelint/issues/7039">#7039</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/stylelint/stylelint/compare/14.16.1...15.10.1">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~mattxwang">mattxwang</a>, a new releaser for stylelint since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=stylelint&package-manager=npm_and_yarn&previous-version=14.16.1&new-version=15.10.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/besu-docs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-07 22:07:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1355" class=".btn">#1355</a>
            </td>
            <td>
                <b>
                    Updated docs for TOML config files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updated docs for TOML config files.
Issue #1347 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-06 03:36:43 +0000 UTC
    </div>
</div>

