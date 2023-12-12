---
layout: default
title: open-enterprise-agent
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/open-enterprise-agent
---

# open-enterprise-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/open-enterprise-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/813" class=".btn">#813</a>
            </td>
            <td>
                <b>
                    fix: Option to disable apisix key auth
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">infra</span>
            </td>
            <td>
                # Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

Fixes ATL-xxxx

## Checklist

### My PR contains...
* [x] No code changes (changes to documentation, CI, metadata, etc.)
* [x] Bug fixes (non-breaking change which fixes an issue)
* [x] Improvements (misc. changes to existing features)
* [ ] Features (non-breaking change which adds functionality)

### My changes...
* [ ] are breaking changes
* [ ] are not breaking changes
* [ ] If yes to above: I have updated the documentation accordingly

### Documentation
* [ ] My changes do not require a change to the project documentation
* [ ] My changes require a change to the project documentation
* [ ] If yes to above: I have updated the documentation accordingly

### Tests
* [ ] My changes can not or do not need to be tested
* [ ] My changes can and should be tested by unit and/or integration tests
* [ ] If yes to above: I have added tests to cover my changes
* [ ] If yes to above: I have taken care to cover edge cases in my tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-12 17:55:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/811" class=".btn">#811</a>
            </td>
            <td>
                <b>
                    feat: env vars support through values file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">infra</span>
            </td>
            <td>
                # Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

Fixes ATL-xxxx

## Checklist

### My PR contains...
* [x] No code changes (changes to documentation, CI, metadata, etc.)
* [ ] Bug fixes (non-breaking change which fixes an issue)
* [x] Improvements (misc. changes to existing features)
* [ ] Features (non-breaking change which adds functionality)

### My changes...
* [ ] are breaking changes
* [ ] are not breaking changes
* [ ] If yes to above: I have updated the documentation accordingly

### Documentation
* [ ] My changes do not require a change to the project documentation
* [ ] My changes require a change to the project documentation
* [ ] If yes to above: I have updated the documentation accordingly

### Tests
* [ ] My changes can not or do not need to be tested
* [ ] My changes can and should be tested by unit and/or integration tests
* [ ] If yes to above: I have added tests to cover my changes
* [ ] If yes to above: I have taken care to cover edge cases in my tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-12 16:18:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/810" class=".btn">#810</a>
            </td>
            <td>
                <b>
                    fix: correct OAS examples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">prism-agent</span>
            </td>
            <td>
                # Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

Fixes ATL-4611

Verified by downloading `docs.yaml` from swagger-ui and `ctrl + f` for invalid examples.

## Checklist

### My PR contains...
* [x] No code changes (changes to documentation, CI, metadata, etc.)
* [ ] Bug fixes (non-breaking change which fixes an issue)
* [ ] Improvements (misc. changes to existing features)
* [ ] Features (non-breaking change which adds functionality)

### My changes...
* [ ] are breaking changes
* [x] are not breaking changes
* [ ] If yes to above: I have updated the documentation accordingly

### Documentation
* [x] My changes do not require a change to the project documentation
* [ ] My changes require a change to the project documentation
* [ ] If yes to above: I have updated the documentation accordingly

### Tests
* [ ] My changes can not or do not need to be tested
* [ ] My changes can and should be tested by unit and/or integration tests
* [ ] If yes to above: I have added tests to cover my changes
* [ ] If yes to above: I have taken care to cover edge cases in my tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-08 08:33:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/809" class=".btn">#809</a>
            </td>
            <td>
                <b>
                    build(deps): bump @babel/traverse from 7.22.11 to 7.23.5 in /tests/performance-tests/atala-performance-tests-k6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [@babel/traverse](https://github.com/babel/babel/tree/HEAD/packages/babel-traverse) from 7.22.11 to 7.23.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/babel/babel/releases"><code>@​babel/traverse</code>'s releases</a>.</em></p>
<blockquote>
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
<li><code>babel-eslint-plugin</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16023">#16023</a> Add <code>@babel/eslint-plugin/no-undef</code> to fix <code>no-undef</code> with accessor props (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h4>:microscope: Output optimization</h4>
<ul>
<li><code>babel-helpers</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16129">#16129</a> Optimize <code>decorator</code> helper size (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 4</h4>
<ul>
<li>Babel Bot (<a href="https://github.com/babel-bot"><code>@​babel-bot</code></a>)</li>
<li>Huáng Jùnliàng (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
<li>Nicolò Ribaudo (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
<li><a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a></li>
</ul>
<h2>v7.23.4 (2023-11-20)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-generator</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16104">#16104</a> fix: Pure comments missing parentheses (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 4</h4>
<ul>
<li>Babel Bot (<a href="https://github.com/babel-bot"><code>@​babel-bot</code></a>)</li>
<li>Huáng Jùnliàng (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
<li>Nicolò Ribaudo (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
<li><a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a></li>
</ul>
<h2>v7.23.3 (2023-11-09)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-plugin-transform-typescript</code></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/babel/babel/blob/main/CHANGELOG.md"><code>@​babel/traverse</code>'s changelog</a>.</em></p>
<blockquote>
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
<li><code>babel-eslint-plugin</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16023">#16023</a> Add <code>@babel/eslint-plugin/no-undef</code> to fix <code>no-undef</code> with accessor props (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h4>:microscope: Output optimization</h4>
<ul>
<li><code>babel-helpers</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16129">#16129</a> Optimize <code>decorator</code> helper size (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
</ul>
<h2>v7.23.4 (2023-11-20)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-generator</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16104">#16104</a> fix: Pure comments missing parentheses (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
</ul>
<h2>v7.23.3 (2023-11-09)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-plugin-transform-typescript</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16071">#16071</a> Strip type-only TS namespaces (<a href="https://github.com/colinaaa"><code>@​colinaaa</code></a>)</li>
</ul>
</li>
<li><code>babel-generator</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16078">#16078</a> Fix indentation when generating comments with <code>concise: true</code> (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-compat-data</code>, <code>babel-plugin-bugfix-v8-static-class-fields-redefine-readonly</code>, <code>babel-preset-env</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/14295">#14295</a> Add a bugfix plugin for <a href="https://crbug.com/v8/12421">https://crbug.com/v8/12421</a> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-transform-object-super</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/15948">#15948</a> fix: <code>super.x</code> in a loop (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-helper-module-transforms</code>, <code>babel-plugin-transform-modules-amd</code>, <code>babel-plugin-transform-modules-commonjs</code>, <code>babel-plugin-transform-modules-umd</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16015">#16015</a> fix: handle <code>__proto__</code> exports name in CJS/AMD/UMD (<a href="https://github.com/magic-akari"><code>@​magic-akari</code></a>)</li>
</ul>
</li>
</ul>
<h4>:memo: Documentation</h4>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16044">#16044</a> docs: Update links in <code>@​babel/eslint-parser</code> README (<a href="https://github.com/aryehb"><code>@​aryehb</code></a>)</li>
</ul>
<h4>:house: Internal</h4>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/babel/babel/commit/8479012ee722ffe316308c1789837e3836580de7"><code>8479012</code></a> v7.23.5</li>
<li><a href="https://github.com/babel/babel/commit/da7dc40fdab77e9c8e190e6ec1d80d4f5eedcfd5"><code>da7dc40</code></a> Do not remove bindings when removing assignment expression path (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16131">#16131</a>)</li>
<li><a href="https://github.com/babel/babel/commit/fadc081db163130903539e81c2384233882b0436"><code>fadc081</code></a> fix: Unexpected duplication of comments (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16110">#16110</a>)</li>
<li><a href="https://github.com/babel/babel/commit/13a5c83807ab755a1cfb3059a7370110b4c8370e"><code>13a5c83</code></a> v7.23.4</li>
<li><a href="https://github.com/babel/babel/commit/5e1c5f047cbcb3a47de5a09487818661bcce3743"><code>5e1c5f0</code></a> Use prettier 3.1 (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16098">#16098</a>)</li>
<li><a href="https://github.com/babel/babel/commit/1bce5c9d51abda279f374b54cef79939c3cc608d"><code>1bce5c9</code></a> v7.23.3</li>
<li><a href="https://github.com/babel/babel/commit/4fb4fa63e7d15b3993d466e79d5051ab1b1b8989"><code>4fb4fa6</code></a> Avoid dynamic dispatch when calling wrapCheck (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16060">#16060</a>)</li>
<li><a href="https://github.com/babel/babel/commit/6d9725cd62511816a1ac6a0ef6a4ef078fea6359"><code>6d9725c</code></a> [babel 8] Inline <code>toSequenceExpression</code> into <code>@babel/traverse</code> (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16057">#16057</a>)</li>
<li><a href="https://github.com/babel/babel/commit/b4b9942a6cde0685c222eb3412347880aae40ad5"><code>b4b9942</code></a> v7.23.2</li>
<li><a href="https://github.com/babel/babel/commit/b13376b346946e3f62fc0848c1d2a23223314c82"><code>b13376b</code></a> Only evaluate own String/Number/Math methods (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-traverse/issues/16033">#16033</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/babel/babel/commits/v7.23.5/packages/babel-traverse">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@babel/traverse&package-manager=npm_and_yarn&previous-version=7.22.11&new-version=7.23.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/open-enterprise-agent/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-07 17:17:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/808" class=".btn">#808</a>
            </td>
            <td>
                <b>
                    fix: tolerations and nodeAffinity for k8s
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">infra</span>
            </td>
            <td>
                # Overview
Fixing tolerations and nodeAffinity
Fixes ATL-xxxx

## Checklist

### My PR contains...
* [x] No code changes (changes to documentation, CI, metadata, etc.)
* [x] Bug fixes (non-breaking change which fixes an issue)
* [ ] Improvements (misc. changes to existing features)
* [ ] Features (non-breaking change which adds functionality)

### My changes...
* [ ] are breaking changes
* [ ] are not breaking changes
* [ ] If yes to above: I have updated the documentation accordingly

### Documentation
* [ ] My changes do not require a change to the project documentation
* [ ] My changes require a change to the project documentation
* [ ] If yes to above: I have updated the documentation accordingly

### Tests
* [ ] My changes can not or do not need to be tested
* [ ] My changes can and should be tested by unit and/or integration tests
* [ ] If yes to above: I have added tests to cover my changes
* [ ] If yes to above: I have taken care to cover edge cases in my tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-06 01:11:54 +0000 UTC
    </div>
</div>

