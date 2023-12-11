---
layout: default
title: TDIDN
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/TDIDN
---

# TDIDN <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/TDIDN){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/TDIDN/pull/7" class=".btn">#7</a>
            </td>
            <td>
                <b>
                    Bump @babel/traverse from 7.23.0 to 7.23.6 in /frontend/TDIN
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [@babel/traverse](https://github.com/babel/babel/tree/HEAD/packages/babel-traverse) from 7.23.0 to 7.23.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/babel/babel/releases"><code>@​babel/traverse</code>'s releases</a>.</em></p>
<blockquote>
<h2>v7.23.6 (2023-12-11)</h2>
<p>Thanks <a href="https://github.com/martinez-hugo"><code>@​martinez-hugo</code></a> and <a href="https://github.com/odinho"><code>@​odinho</code></a> for your first pull requests!</p>
<h4>:eyeglasses: Spec Compliance</h4>
<ul>
<li><code>babel-generator</code>, <code>babel-parser</code>, <code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16154">#16154</a> Remove <code>TSPropertySignature.initializer</code> (<a href="https://github.com/fisker"><code>@​fisker</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-decorators</code>, <code>babel-plugin-transform-class-properties</code>, <code>babel-plugin-transform-class-static-block</code>, <code>babel-plugin-transform-runtime</code>, <code>babel-preset-env</code>, <code>babel-runtime-corejs2</code>, <code>babel-runtime-corejs3</code>, <code>babel-runtime</code>, <code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16139">#16139</a> Apply <code>toPropertyKey</code> on decorator context name (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-generator</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16166">#16166</a> fix: Correctly indenting when <code>retainLines</code> is enabled (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-explicit-resource-management</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16150">#16150</a> <code>using</code>: Allow looking up <code>Symbol.dispose</code> on a function (<a href="https://github.com/odinho"><code>@​odinho</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-proposal-decorators</code>, <code>babel-plugin-transform-class-properties</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16161">#16161</a> Ensure the <code>[[@@toPrimitive]]</code> call of a decorated class member key is invoked once (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16148">#16148</a> Support named evaluation for decorated anonymous class exp (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-transform-for-of</code>, <code>babel-preset-env</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16011">#16011</a> fix: <code>for of</code> with <code>iterableIsArray</code> and shadowing variable  (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-decorators</code>, <code>babel-runtime-corejs2</code>, <code>babel-runtime-corejs3</code>, <code>babel-runtime</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16144">#16144</a> Set function name for decorated private non-field elements (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-transform-typescript</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16137">#16137</a> Fix references to enum values with merging (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h4>:microscope: Output optimization</h4>
<ul>
<li><code>babel-helper-create-class-features-plugin</code>, <code>babel-plugin-transform-class-properties</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16159">#16159</a> Reuse computed key memoiser (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-decorators</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16160">#16160</a> Optimize decorator helper size (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 7</h4>
<ul>
<li>Babel Bot (<a href="https://github.com/babel-bot"><code>@​babel-bot</code></a>)</li>
<li>Hugo Martinez (<a href="https://github.com/martinez-hugo"><code>@​martinez-hugo</code></a>)</li>
<li>Huáng Jùnliàng (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
<li>Nicolò Ribaudo (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
<li>Odin Hørthe-Omdal Urdland (<a href="https://github.com/odinho"><code>@​odinho</code></a>)</li>
<li><a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a></li>
<li>fisker Cheung (<a href="https://github.com/fisker"><code>@​fisker</code></a>)</li>
</ul>
<h2>v7.23.5 (2023-11-29)</h2>
<h4>:eyeglasses: Spec Compliance</h4>
<ul>
<li><code>babel-plugin-proposal-decorators</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16138">#16138</a> Class binding is in TDZ during decorators initialization (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-decorators</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16132">#16132</a> Allow addInitializer in field decorator context (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-traverse</code>, <code>babel-types</code></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/babel/babel/blob/main/CHANGELOG.md"><code>@​babel/traverse</code>'s changelog</a>.</em></p>
<blockquote>
<h2>v7.23.6 (2023-12-11)</h2>
<h4>:eyeglasses: Spec Compliance</h4>
<ul>
<li><code>babel-generator</code>, <code>babel-parser</code>, <code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16154">#16154</a> Remove <code>TSPropertySignature.initializer</code> (<a href="https://github.com/fisker"><code>@​fisker</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-decorators</code>, <code>babel-plugin-transform-class-properties</code>, <code>babel-plugin-transform-class-static-block</code>, <code>babel-plugin-transform-runtime</code>, <code>babel-preset-env</code>, <code>babel-runtime-corejs2</code>, <code>babel-runtime-corejs3</code>, <code>babel-runtime</code>, <code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16139">#16139</a> Apply <code>toPropertyKey</code> on decorator context name (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-generator</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16166">#16166</a> fix: Correctly indenting when <code>retainLines</code> is enabled (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-explicit-resource-management</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16150">#16150</a> <code>using</code>: Allow looking up <code>Symbol.dispose</code> on a function (<a href="https://github.com/odinho"><code>@​odinho</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-proposal-decorators</code>, <code>babel-plugin-transform-class-properties</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16161">#16161</a> Ensure the <code>[[@@toPrimitive]]</code> call of a decorated class member key is invoked once (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16148">#16148</a> Support named evaluation for decorated anonymous class exp (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-transform-for-of</code>, <code>babel-preset-env</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16011">#16011</a> fix: <code>for of</code> with <code>iterableIsArray</code> and shadowing variable  (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-decorators</code>, <code>babel-runtime-corejs2</code>, <code>babel-runtime-corejs3</code>, <code>babel-runtime</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16144">#16144</a> Set function name for decorated private non-field elements (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-transform-typescript</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16137">#16137</a> Fix references to enum values with merging (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h4>:microscope: Output optimization</h4>
<ul>
<li><code>babel-helper-create-class-features-plugin</code>, <code>babel-plugin-transform-class-properties</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16159">#16159</a> Reuse computed key memoiser (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-decorators</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16160">#16160</a> Optimize decorator helper size (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
</ul>
<h2>v7.23.5 (2023-11-29)</h2>
<h4>:eyeglasses: Spec Compliance</h4>
<ul>
<li><code>babel-plugin-proposal-decorators</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16138">#16138</a> Class binding is in TDZ during decorators initialization (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-decorators</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16132">#16132</a> Allow addInitializer in field decorator context (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-traverse</code>, <code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16131">#16131</a> Do not remove bindings when removing assignment expression path (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-transform-classes</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16135">#16135</a> Require class properties transform when compiling class with private fields (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-generator</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16122">#16122</a> fix: Missing parentheses after line break (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16130">#16130</a> Fix helpers internal fns names conflict resolution  (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-helper-create-class-features-plugin</code>, <code>babel-plugin-transform-class-properties</code>, <code>babel-plugin-transform-typescript</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16123">#16123</a> Simplify class fields injetion after <code>super()</code> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-generator</code>, <code>babel-plugin-transform-modules-commonjs</code>, <code>babel-plugin-transform-parameters</code>, <code>babel-plugin-transform-typescript</code>, <code>babel-traverse</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16110">#16110</a> fix: Unexpected duplication of comments (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-eslint-plugin</code></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/babel/babel/commit/d02c1f76ac441381b1ba3b5cad93bdd030b8fd63"><code>d02c1f7</code></a> v7.23.6</li>
<li><a href="https://github.com/babel/babel/commit/cce807f1eb638ee3030112dc190cbee032760888"><code>cce807f</code></a> Bump debug to ^4.3.1 (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16164">#16164</a>)</li>
<li><a href="https://github.com/babel/babel/commit/8479012ee722ffe316308c1789837e3836580de7"><code>8479012</code></a> v7.23.5</li>
<li><a href="https://github.com/babel/babel/commit/da7dc40fdab77e9c8e190e6ec1d80d4f5eedcfd5"><code>da7dc40</code></a> Do not remove bindings when removing assignment expression path (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16131">#16131</a>)</li>
<li><a href="https://github.com/babel/babel/commit/fadc081db163130903539e81c2384233882b0436"><code>fadc081</code></a> fix: Unexpected duplication of comments (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16110">#16110</a>)</li>
<li><a href="https://github.com/babel/babel/commit/13a5c83807ab755a1cfb3059a7370110b4c8370e"><code>13a5c83</code></a> v7.23.4</li>
<li><a href="https://github.com/babel/babel/commit/5e1c5f047cbcb3a47de5a09487818661bcce3743"><code>5e1c5f0</code></a> Use prettier 3.1 (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16098">#16098</a>)</li>
<li><a href="https://github.com/babel/babel/commit/1bce5c9d51abda279f374b54cef79939c3cc608d"><code>1bce5c9</code></a> v7.23.3</li>
<li><a href="https://github.com/babel/babel/commit/4fb4fa63e7d15b3993d466e79d5051ab1b1b8989"><code>4fb4fa6</code></a> Avoid dynamic dispatch when calling wrapCheck (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16060">#16060</a>)</li>
<li><a href="https://github.com/babel/babel/commit/6d9725cd62511816a1ac6a0ef6a4ef078fea6359"><code>6d9725c</code></a> [babel 8] Inline <code>toSequenceExpression</code> into <code>@babel/traverse</code> (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16057">#16057</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/babel/babel/commits/v7.23.6/packages/babel-traverse">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@babel/traverse&package-manager=npm_and_yarn&previous-version=7.23.0&new-version=7.23.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/TDIDN/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-11 16:06:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/TDIDN/pull/6" class=".btn">#6</a>
            </td>
            <td>
                <b>
                    Bump @babel/traverse from 7.23.0 to 7.23.6 in /frontend/web-wallet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [@babel/traverse](https://github.com/babel/babel/tree/HEAD/packages/babel-traverse) from 7.23.0 to 7.23.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/babel/babel/releases"><code>@​babel/traverse</code>'s releases</a>.</em></p>
<blockquote>
<h2>v7.23.6 (2023-12-11)</h2>
<p>Thanks <a href="https://github.com/martinez-hugo"><code>@​martinez-hugo</code></a> and <a href="https://github.com/odinho"><code>@​odinho</code></a> for your first pull requests!</p>
<h4>:eyeglasses: Spec Compliance</h4>
<ul>
<li><code>babel-generator</code>, <code>babel-parser</code>, <code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16154">#16154</a> Remove <code>TSPropertySignature.initializer</code> (<a href="https://github.com/fisker"><code>@​fisker</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-decorators</code>, <code>babel-plugin-transform-class-properties</code>, <code>babel-plugin-transform-class-static-block</code>, <code>babel-plugin-transform-runtime</code>, <code>babel-preset-env</code>, <code>babel-runtime-corejs2</code>, <code>babel-runtime-corejs3</code>, <code>babel-runtime</code>, <code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16139">#16139</a> Apply <code>toPropertyKey</code> on decorator context name (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-generator</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16166">#16166</a> fix: Correctly indenting when <code>retainLines</code> is enabled (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-explicit-resource-management</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16150">#16150</a> <code>using</code>: Allow looking up <code>Symbol.dispose</code> on a function (<a href="https://github.com/odinho"><code>@​odinho</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-proposal-decorators</code>, <code>babel-plugin-transform-class-properties</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16161">#16161</a> Ensure the <code>[[@@toPrimitive]]</code> call of a decorated class member key is invoked once (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16148">#16148</a> Support named evaluation for decorated anonymous class exp (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-transform-for-of</code>, <code>babel-preset-env</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16011">#16011</a> fix: <code>for of</code> with <code>iterableIsArray</code> and shadowing variable  (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-decorators</code>, <code>babel-runtime-corejs2</code>, <code>babel-runtime-corejs3</code>, <code>babel-runtime</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16144">#16144</a> Set function name for decorated private non-field elements (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-transform-typescript</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16137">#16137</a> Fix references to enum values with merging (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h4>:microscope: Output optimization</h4>
<ul>
<li><code>babel-helper-create-class-features-plugin</code>, <code>babel-plugin-transform-class-properties</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16159">#16159</a> Reuse computed key memoiser (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-decorators</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16160">#16160</a> Optimize decorator helper size (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 7</h4>
<ul>
<li>Babel Bot (<a href="https://github.com/babel-bot"><code>@​babel-bot</code></a>)</li>
<li>Hugo Martinez (<a href="https://github.com/martinez-hugo"><code>@​martinez-hugo</code></a>)</li>
<li>Huáng Jùnliàng (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
<li>Nicolò Ribaudo (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
<li>Odin Hørthe-Omdal Urdland (<a href="https://github.com/odinho"><code>@​odinho</code></a>)</li>
<li><a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a></li>
<li>fisker Cheung (<a href="https://github.com/fisker"><code>@​fisker</code></a>)</li>
</ul>
<h2>v7.23.5 (2023-11-29)</h2>
<h4>:eyeglasses: Spec Compliance</h4>
<ul>
<li><code>babel-plugin-proposal-decorators</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16138">#16138</a> Class binding is in TDZ during decorators initialization (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-decorators</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16132">#16132</a> Allow addInitializer in field decorator context (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-traverse</code>, <code>babel-types</code></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/babel/babel/blob/main/CHANGELOG.md"><code>@​babel/traverse</code>'s changelog</a>.</em></p>
<blockquote>
<h2>v7.23.6 (2023-12-11)</h2>
<h4>:eyeglasses: Spec Compliance</h4>
<ul>
<li><code>babel-generator</code>, <code>babel-parser</code>, <code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16154">#16154</a> Remove <code>TSPropertySignature.initializer</code> (<a href="https://github.com/fisker"><code>@​fisker</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-decorators</code>, <code>babel-plugin-transform-class-properties</code>, <code>babel-plugin-transform-class-static-block</code>, <code>babel-plugin-transform-runtime</code>, <code>babel-preset-env</code>, <code>babel-runtime-corejs2</code>, <code>babel-runtime-corejs3</code>, <code>babel-runtime</code>, <code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16139">#16139</a> Apply <code>toPropertyKey</code> on decorator context name (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-generator</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16166">#16166</a> fix: Correctly indenting when <code>retainLines</code> is enabled (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-explicit-resource-management</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16150">#16150</a> <code>using</code>: Allow looking up <code>Symbol.dispose</code> on a function (<a href="https://github.com/odinho"><code>@​odinho</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-proposal-decorators</code>, <code>babel-plugin-transform-class-properties</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16161">#16161</a> Ensure the <code>[[@@toPrimitive]]</code> call of a decorated class member key is invoked once (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16148">#16148</a> Support named evaluation for decorated anonymous class exp (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-transform-for-of</code>, <code>babel-preset-env</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16011">#16011</a> fix: <code>for of</code> with <code>iterableIsArray</code> and shadowing variable  (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-decorators</code>, <code>babel-runtime-corejs2</code>, <code>babel-runtime-corejs3</code>, <code>babel-runtime</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16144">#16144</a> Set function name for decorated private non-field elements (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-transform-typescript</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16137">#16137</a> Fix references to enum values with merging (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h4>:microscope: Output optimization</h4>
<ul>
<li><code>babel-helper-create-class-features-plugin</code>, <code>babel-plugin-transform-class-properties</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16159">#16159</a> Reuse computed key memoiser (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-decorators</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16160">#16160</a> Optimize decorator helper size (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
</ul>
<h2>v7.23.5 (2023-11-29)</h2>
<h4>:eyeglasses: Spec Compliance</h4>
<ul>
<li><code>babel-plugin-proposal-decorators</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16138">#16138</a> Class binding is in TDZ during decorators initialization (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-decorators</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16132">#16132</a> Allow addInitializer in field decorator context (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-traverse</code>, <code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16131">#16131</a> Do not remove bindings when removing assignment expression path (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-transform-classes</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16135">#16135</a> Require class properties transform when compiling class with private fields (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-generator</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16122">#16122</a> fix: Missing parentheses after line break (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16130">#16130</a> Fix helpers internal fns names conflict resolution  (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-helper-create-class-features-plugin</code>, <code>babel-plugin-transform-class-properties</code>, <code>babel-plugin-transform-typescript</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16123">#16123</a> Simplify class fields injetion after <code>super()</code> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-generator</code>, <code>babel-plugin-transform-modules-commonjs</code>, <code>babel-plugin-transform-parameters</code>, <code>babel-plugin-transform-typescript</code>, <code>babel-traverse</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16110">#16110</a> fix: Unexpected duplication of comments (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-eslint-plugin</code></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/babel/babel/commit/d02c1f76ac441381b1ba3b5cad93bdd030b8fd63"><code>d02c1f7</code></a> v7.23.6</li>
<li><a href="https://github.com/babel/babel/commit/cce807f1eb638ee3030112dc190cbee032760888"><code>cce807f</code></a> Bump debug to ^4.3.1 (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16164">#16164</a>)</li>
<li><a href="https://github.com/babel/babel/commit/8479012ee722ffe316308c1789837e3836580de7"><code>8479012</code></a> v7.23.5</li>
<li><a href="https://github.com/babel/babel/commit/da7dc40fdab77e9c8e190e6ec1d80d4f5eedcfd5"><code>da7dc40</code></a> Do not remove bindings when removing assignment expression path (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16131">#16131</a>)</li>
<li><a href="https://github.com/babel/babel/commit/fadc081db163130903539e81c2384233882b0436"><code>fadc081</code></a> fix: Unexpected duplication of comments (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16110">#16110</a>)</li>
<li><a href="https://github.com/babel/babel/commit/13a5c83807ab755a1cfb3059a7370110b4c8370e"><code>13a5c83</code></a> v7.23.4</li>
<li><a href="https://github.com/babel/babel/commit/5e1c5f047cbcb3a47de5a09487818661bcce3743"><code>5e1c5f0</code></a> Use prettier 3.1 (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16098">#16098</a>)</li>
<li><a href="https://github.com/babel/babel/commit/1bce5c9d51abda279f374b54cef79939c3cc608d"><code>1bce5c9</code></a> v7.23.3</li>
<li><a href="https://github.com/babel/babel/commit/4fb4fa63e7d15b3993d466e79d5051ab1b1b8989"><code>4fb4fa6</code></a> Avoid dynamic dispatch when calling wrapCheck (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16060">#16060</a>)</li>
<li><a href="https://github.com/babel/babel/commit/6d9725cd62511816a1ac6a0ef6a4ef078fea6359"><code>6d9725c</code></a> [babel 8] Inline <code>toSequenceExpression</code> into <code>@babel/traverse</code> (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16057">#16057</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/babel/babel/commits/v7.23.6/packages/babel-traverse">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@babel/traverse&package-manager=npm_and_yarn&previous-version=7.23.0&new-version=7.23.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/TDIDN/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-11 16:05:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/TDIDN/pull/5" class=".btn">#5</a>
            </td>
            <td>
                <b>
                    Bump @adobe/css-tools from 4.3.1 to 4.3.2 in /frontend/web-wallet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [@adobe/css-tools](https://github.com/adobe/css-tools) from 4.3.1 to 4.3.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/adobe/css-tools/blob/main/History.md"><code>@​adobe/css-tools</code>'s changelog</a>.</em></p>
<blockquote>
<h1>4.3.2 / 2023-11-28</h1>
<ul>
<li>Fix redos vulnerability with specific crafted css string - CVE-2023-48631</li>
<li>Fix Problem parsing with :is() and nested :nth-child() <a href="https://redirect.github.com/adobe/css-tools/issues/211">#211</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/adobe/css-tools/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@adobe/css-tools&package-manager=npm_and_yarn&previous-version=4.3.1&new-version=4.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/TDIDN/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-11 16:05:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/TDIDN/pull/4" class=".btn">#4</a>
            </td>
            <td>
                <b>
                    Bump @adobe/css-tools from 4.3.1 to 4.3.2 in /frontend/TDIN
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [@adobe/css-tools](https://github.com/adobe/css-tools) from 4.3.1 to 4.3.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/adobe/css-tools/blob/main/History.md"><code>@​adobe/css-tools</code>'s changelog</a>.</em></p>
<blockquote>
<h1>4.3.2 / 2023-11-28</h1>
<ul>
<li>Fix redos vulnerability with specific crafted css string - CVE-2023-48631</li>
<li>Fix Problem parsing with :is() and nested :nth-child() <a href="https://redirect.github.com/adobe/css-tools/issues/211">#211</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/adobe/css-tools/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@adobe/css-tools&package-manager=npm_and_yarn&previous-version=4.3.1&new-version=4.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/TDIDN/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-11 16:05:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/TDIDN/pull/3" class=".btn">#3</a>
            </td>
            <td>
                <b>
                    Bump axios from 1.5.1 to 1.6.0 in /frontend/TDIN
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [axios](https://github.com/axios/axios) from 1.5.1 to 1.6.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/releases">axios's releases</a>.</em></p>
<blockquote>
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
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+449/-114 ([#6032](https://github.com/axios/axios/issues/6032) [#6021](https://github.com/axios/axios/issues/6021) [#6011](https://github.com/axios/axios/issues/6011) [#5932](https://github.com/axios/axios/issues/5932) [#5931](https://github.com/axios/axios/issues/5931) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/valentin-panov" title="+4/-4 ([#6028](https://github.com/axios/axios/issues/6028) )">Valentin Panov</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/therealrinku" title="+1/-1 ([#5889](https://github.com/axios/axios/issues/5889) )">Rinku Chaudhari</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/blob/v1.x/CHANGELOG.md">axios's changelog</a>.</em></p>
<blockquote>
<h1><a href="https://github.com/axios/axios/compare/v1.5.1...v1.6.0">1.6.0</a> (2023-10-26)</h1>
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
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+449/-114 ([#6032](https://github.com/axios/axios/issues/6032) [#6021](https://github.com/axios/axios/issues/6021) [#6011](https://github.com/axios/axios/issues/6011) [#5932](https://github.com/axios/axios/issues/5932) [#5931](https://github.com/axios/axios/issues/5931) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/valentin-panov" title="+4/-4 ([#6028](https://github.com/axios/axios/issues/6028) )">Valentin Panov</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/therealrinku" title="+1/-1 ([#5889](https://github.com/axios/axios/issues/5889) )">Rinku Chaudhari</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/axios/axios/commit/f7adacdbaa569281253c8cfc623ad3f4dc909c60"><code>f7adacd</code></a> chore(release): v1.6.0 (<a href="https://redirect.github.com/axios/axios/issues/6031">#6031</a>)</li>
<li><a href="https://github.com/axios/axios/commit/9917e67cbb6c157382863bad8c741de58e3f3c2b"><code>9917e67</code></a> chore(ci): fix release-it arg; (<a href="https://redirect.github.com/axios/axios/issues/6032">#6032</a>)</li>
<li><a href="https://github.com/axios/axios/commit/96ee232bd3ee4de2e657333d4d2191cd389e14d0"><code>96ee232</code></a> fix(CSRF): fixed CSRF vulnerability CVE-2023-45857 (<a href="https://redirect.github.com/axios/axios/issues/6028">#6028</a>)</li>
<li><a href="https://github.com/axios/axios/commit/7d45ab2e2ad6e59f5475e39afd4b286b1f393fc0"><code>7d45ab2</code></a> chore(tests): fixed tests to pass in node v19 and v20 with <code>keep-alive</code> enabl...</li>
<li><a href="https://github.com/axios/axios/commit/5aaff532a6b820bb9ab6a8cd0f77131b47e2adb8"><code>5aaff53</code></a> fix(dns): fixed lookup function decorator to work properly in node v20; (<a href="https://redirect.github.com/axios/axios/issues/6011">#6011</a>)</li>
<li><a href="https://github.com/axios/axios/commit/a48a63ad823fc20e5a6a705f05f09842ca49f48c"><code>a48a63a</code></a> chore(docs): added AxiosHeaders docs; (<a href="https://redirect.github.com/axios/axios/issues/5932">#5932</a>)</li>
<li><a href="https://github.com/axios/axios/commit/a1c8ad008b3c13d53e135bbd0862587fb9d3fc09"><code>a1c8ad0</code></a> fix(types): fix AxiosHeaders types; (<a href="https://redirect.github.com/axios/axios/issues/5931">#5931</a>)</li>
<li><a href="https://github.com/axios/axios/commit/2ac731d60545ba5c4202c25fd2e732ddd8297d82"><code>2ac731d</code></a> chore(docs): update readme.md (<a href="https://redirect.github.com/axios/axios/issues/5889">#5889</a>)</li>
<li>See full diff in <a href="https://github.com/axios/axios/compare/v1.5.1...v1.6.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=axios&package-manager=npm_and_yarn&previous-version=1.5.1&new-version=1.6.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/TDIDN/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-11 16:05:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/TDIDN/pull/2" class=".btn">#2</a>
            </td>
            <td>
                <b>
                    Bump axios from 1.5.1 to 1.6.0 in /frontend/web-wallet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [axios](https://github.com/axios/axios) from 1.5.1 to 1.6.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/releases">axios's releases</a>.</em></p>
<blockquote>
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
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+449/-114 ([#6032](https://github.com/axios/axios/issues/6032) [#6021](https://github.com/axios/axios/issues/6021) [#6011](https://github.com/axios/axios/issues/6011) [#5932](https://github.com/axios/axios/issues/5932) [#5931](https://github.com/axios/axios/issues/5931) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/valentin-panov" title="+4/-4 ([#6028](https://github.com/axios/axios/issues/6028) )">Valentin Panov</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/therealrinku" title="+1/-1 ([#5889](https://github.com/axios/axios/issues/5889) )">Rinku Chaudhari</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/blob/v1.x/CHANGELOG.md">axios's changelog</a>.</em></p>
<blockquote>
<h1><a href="https://github.com/axios/axios/compare/v1.5.1...v1.6.0">1.6.0</a> (2023-10-26)</h1>
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
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+449/-114 ([#6032](https://github.com/axios/axios/issues/6032) [#6021](https://github.com/axios/axios/issues/6021) [#6011](https://github.com/axios/axios/issues/6011) [#5932](https://github.com/axios/axios/issues/5932) [#5931](https://github.com/axios/axios/issues/5931) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/valentin-panov" title="+4/-4 ([#6028](https://github.com/axios/axios/issues/6028) )">Valentin Panov</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/therealrinku" title="+1/-1 ([#5889](https://github.com/axios/axios/issues/5889) )">Rinku Chaudhari</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/axios/axios/commit/f7adacdbaa569281253c8cfc623ad3f4dc909c60"><code>f7adacd</code></a> chore(release): v1.6.0 (<a href="https://redirect.github.com/axios/axios/issues/6031">#6031</a>)</li>
<li><a href="https://github.com/axios/axios/commit/9917e67cbb6c157382863bad8c741de58e3f3c2b"><code>9917e67</code></a> chore(ci): fix release-it arg; (<a href="https://redirect.github.com/axios/axios/issues/6032">#6032</a>)</li>
<li><a href="https://github.com/axios/axios/commit/96ee232bd3ee4de2e657333d4d2191cd389e14d0"><code>96ee232</code></a> fix(CSRF): fixed CSRF vulnerability CVE-2023-45857 (<a href="https://redirect.github.com/axios/axios/issues/6028">#6028</a>)</li>
<li><a href="https://github.com/axios/axios/commit/7d45ab2e2ad6e59f5475e39afd4b286b1f393fc0"><code>7d45ab2</code></a> chore(tests): fixed tests to pass in node v19 and v20 with <code>keep-alive</code> enabl...</li>
<li><a href="https://github.com/axios/axios/commit/5aaff532a6b820bb9ab6a8cd0f77131b47e2adb8"><code>5aaff53</code></a> fix(dns): fixed lookup function decorator to work properly in node v20; (<a href="https://redirect.github.com/axios/axios/issues/6011">#6011</a>)</li>
<li><a href="https://github.com/axios/axios/commit/a48a63ad823fc20e5a6a705f05f09842ca49f48c"><code>a48a63a</code></a> chore(docs): added AxiosHeaders docs; (<a href="https://redirect.github.com/axios/axios/issues/5932">#5932</a>)</li>
<li><a href="https://github.com/axios/axios/commit/a1c8ad008b3c13d53e135bbd0862587fb9d3fc09"><code>a1c8ad0</code></a> fix(types): fix AxiosHeaders types; (<a href="https://redirect.github.com/axios/axios/issues/5931">#5931</a>)</li>
<li><a href="https://github.com/axios/axios/commit/2ac731d60545ba5c4202c25fd2e732ddd8297d82"><code>2ac731d</code></a> chore(docs): update readme.md (<a href="https://redirect.github.com/axios/axios/issues/5889">#5889</a>)</li>
<li>See full diff in <a href="https://github.com/axios/axios/compare/v1.5.1...v1.6.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=axios&package-manager=npm_and_yarn&previous-version=1.5.1&new-version=1.6.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/TDIDN/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-11 16:05:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/TDIDN/pull/1" class=".btn">#1</a>
            </td>
            <td>
                <b>
                    Initial Code
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
        Created At 2023-12-11 16:02:05 +0000 UTC
    </div>
</div>

