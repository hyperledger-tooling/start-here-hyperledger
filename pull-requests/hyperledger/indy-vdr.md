---
layout: default
title: indy-vdr
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-vdr
---

# indy-vdr <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-vdr){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/288" class=".btn">#288</a>
            </td>
            <td>
                <b>
                    fix: fixed binary for react native
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                the async_trait macro appeared to be crashing Bifold in react native. I've refactored the code to remove the `async_trait` macro and made some changes to the code to compensate
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-15 19:23:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/285" class=".btn">#285</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump eslint-plugin-import from 2.28.0 to 2.29.1 in /wrappers/javascript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [eslint-plugin-import](https://github.com/import-js/eslint-plugin-import) from 2.28.0 to 2.29.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/import-js/eslint-plugin-import/releases">eslint-plugin-import's releases</a>.</em></p>
<blockquote>
<h2>v2.29.1</h2>
<p><strong>Full Changelog</strong>: <a href="https://github.com/import-js/eslint-plugin-import/compare/v2.29.0...v2.29.1">https://github.com/import-js/eslint-plugin-import/compare/v2.29.0...v2.29.1</a></p>
<h2>v2.29.0</h2>
<p><strong>Full Changelog</strong>: <a href="https://github.com/import-js/eslint-plugin-import/compare/v2.28.1...v2.29.0">https://github.com/import-js/eslint-plugin-import/compare/v2.28.1...v2.29.0</a></p>
<h2>v2.28.1</h2>
<p><strong>Full Changelog</strong>: <a href="https://github.com/import-js/eslint-plugin-import/compare/v2.28.0...v2.28.1">https://github.com/import-js/eslint-plugin-import/compare/v2.28.0...v2.28.1</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/import-js/eslint-plugin-import/blob/main/CHANGELOG.md">eslint-plugin-import's changelog</a>.</em></p>
<blockquote>
<h2>[2.29.1] - 2023-12-14</h2>
<h3>Fixed</h3>
<ul>
<li>[<code>no-extraneous-dependencies</code>]: ignore <code>export type { ... } from '...'</code> when <code>includeTypes</code> is <code>false</code> (<a href="https://redirect.github.com/import-js/eslint-plugin-import/issues/2919">#2919</a>, thanks [<a href="https://github.com/Pandemic1617"><code>@​Pandemic1617</code></a>])</li>
<li>[<code>no-unused-modules</code>]: support export patterns with array destructuring (<a href="https://redirect.github.com/import-js/eslint-plugin-import/issues/2930">#2930</a>, thanks [<a href="https://github.com/ljharb"><code>@​ljharb</code></a>])</li>
<li>[Deps] update <code>tsconfig-paths</code> (<a href="https://redirect.github.com/import-js/eslint-plugin-import/issues/2447">#2447</a>, thanks [<a href="https://github.com/domdomegg"><code>@​domdomegg</code></a>])</li>
</ul>
<h2>[2.29.0] - 2023-10-22</h2>
<h3>Added</h3>
<ul>
<li>TypeScript config: add .cts and .mts extensions (<a href="https://redirect.github.com/import-js/eslint-plugin-import/issues/2851">#2851</a>, thanks [<a href="https://github.com/Zamiell"><code>@​Zamiell</code></a>])</li>
<li>[<code>newline-after-import</code>]: new option <code>exactCount</code> and docs update (<a href="https://redirect.github.com/import-js/eslint-plugin-import/issues/1933">#1933</a>, thanks [<a href="https://github.com/anikethsaha"><code>@​anikethsaha</code></a>] and [<a href="https://github.com/reosarevok"><code>@​reosarevok</code></a>])</li>
<li>[<code>newline-after-import</code>]: fix <code>exactCount</code> with <code>considerComments</code> false positive, when there is a leading comment (<a href="https://redirect.github.com/import-js/eslint-plugin-import/issues/2884">#2884</a>, thanks [<a href="https://github.com/kinland"><code>@​kinland</code></a>])</li>
</ul>
<h2>[2.28.1] - 2023-08-18</h2>
<h3>Fixed</h3>
<ul>
<li>[<code>order</code>]: revert breaking change to single nested group (<a href="https://redirect.github.com/import-js/eslint-plugin-import/issues/2854">#2854</a>, thanks [<a href="https://github.com/yndajas"><code>@​yndajas</code></a>])</li>
</ul>
<h3>Changed</h3>
<ul>
<li>[Docs] remove duplicate fixable notices in docs (<a href="https://redirect.github.com/import-js/eslint-plugin-import/issues/2850">#2850</a>, thanks [<a href="https://github.com/bmish"><code>@​bmish</code></a>])</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/import-js/eslint-plugin-import/commit/ee5fadeffff68f2300bed7f67a310496cb969d61"><code>ee5fade</code></a> Bump to 2.29.1</li>
<li><a href="https://github.com/import-js/eslint-plugin-import/commit/48fec35fbe9d20f5c859a02d0e4acef70759c875"><code>48fec35</code></a> [Deps] update <code>tsconfig-paths</code></li>
<li><a href="https://github.com/import-js/eslint-plugin-import/commit/80aee736721397cd073636950fef30aa65e165d3"><code>80aee73</code></a> [Dev Deps] update <code>chai</code>, <code>eslint-doc-generator</code>, <code>markdownlint-cli</code></li>
<li><a href="https://github.com/import-js/eslint-plugin-import/commit/8c83eafe4a709c0c275279a7bf99d92fa4e034a5"><code>8c83eaf</code></a> [Tests] node v21.3 has a broken <code>fs.writeFile</code></li>
<li><a href="https://github.com/import-js/eslint-plugin-import/commit/e67259e4c167d46e9cc5472d3afa32369fbf2eff"><code>e67259e</code></a> [Fix] <code>no-unused-modules</code>: support export patterns with array destructuring</li>
<li><a href="https://github.com/import-js/eslint-plugin-import/commit/9fd3c42707d71987e439a847f2e213f55c84f734"><code>9fd3c42</code></a> [Tests] <code>no-duplicates</code>: add passing test</li>
<li><a href="https://github.com/import-js/eslint-plugin-import/commit/12f0300100b9bb90c6a952d07c133f2d5842ad57"><code>12f0300</code></a> [Fix] <code>no-extraneous-dependencies</code>: ignore <code>export type { ... } from '...'</code> w...</li>
<li><a href="https://github.com/import-js/eslint-plugin-import/commit/6d34c88a91a9cb7556700b7cb83c8a27731ff302"><code>6d34c88</code></a> Bump to 2.29.0</li>
<li><a href="https://github.com/import-js/eslint-plugin-import/commit/ec6a8ea3c386241daaf208fe78da151b30415357"><code>ec6a8ea</code></a> [Refactor] use <code>hasown</code> instead of <code>has</code></li>
<li><a href="https://github.com/import-js/eslint-plugin-import/commit/78f50b852a0dc187ccbfd6b4592e4f59ba78d339"><code>78f50b8</code></a> [Deps] update <code>array-includes</code>, <code>array.prototype.findlastindex</code>, `array.proto...</li>
<li>Additional commits viewable in <a href="https://github.com/import-js/eslint-plugin-import/compare/v2.28.0...v2.29.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=eslint-plugin-import&package-manager=npm_and_yarn&previous-version=2.28.0&new-version=2.29.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 20:43:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/284" class=".btn">#284</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump @babel/core from 7.22.10 to 7.24.5 in /wrappers/javascript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@babel/core](https://github.com/babel/babel/tree/HEAD/packages/babel-core) from 7.22.10 to 7.24.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/babel/babel/releases"><code>@​babel/core</code>'s releases</a>.</em></p>
<blockquote>
<h2>v7.24.5 (2024-04-29)</h2>
<p>Thanks <a href="https://github.com/romgrk"><code>@​romgrk</code></a> and <a href="https://github.com/sossost"><code>@​sossost</code></a> for your first PRs!</p>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-plugin-transform-classes</code>, <code>babel-traverse</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16377">#16377</a> fix: TypeScript annotation affects output (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-explicit-resource-management</code>, <code>babel-runtime-corejs3</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16440">#16440</a> Fix suppressed error order (<a href="https://github.com/sossost"><code>@​sossost</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16408">#16408</a> Await nullish async disposable (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:nail_care: Polish</h4>
<ul>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16407">#16407</a> Recover from exported <code>using</code> declaration (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:house: Internal</h4>
<ul>
<li>Other
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16414">#16414</a> Relax ESLint peerDependency constraint to allow v9 (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16425">#16425</a> Improve <code>@babel/parser</code> AST types (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16417">#16417</a> Always pass type argument to <code>.startNode</code> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-helper-create-class-features-plugin</code>, <code>babel-helper-member-expression-to-functions</code>, <code>babel-helper-module-transforms</code>, <code>babel-helper-split-export-declaration</code>, <code>babel-helper-wrap-function</code>, <code>babel-helpers</code>, <code>babel-plugin-bugfix-firefox-class-in-computed-class-key</code>, <code>babel-plugin-proposal-explicit-resource-management</code>, <code>babel-plugin-transform-block-scoping</code>, <code>babel-plugin-transform-destructuring</code>, <code>babel-plugin-transform-object-rest-spread</code>, <code>babel-plugin-transform-optional-chaining</code>, <code>babel-plugin-transform-parameters</code>, <code>babel-plugin-transform-private-property-in-object</code>, <code>babel-plugin-transform-react-jsx-self</code>, <code>babel-plugin-transform-typeof-symbol</code>, <code>babel-plugin-transform-typescript</code>, <code>babel-traverse</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16439">#16439</a> Make <code>NodePath&lt;T | U&gt;</code> distributive (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-proposal-partial-application</code>, <code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16421">#16421</a> Remove <code>JSXNamespacedName</code> from valid <code>CallExpression</code> args (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-transform-class-properties</code>, <code>babel-preset-env</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16406">#16406</a> Do not load unnecessary Babel 7 syntax plugins in Babel 8 (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h4>:running_woman: Performance</h4>
<ul>
<li><code>babel-helpers</code>, <code>babel-preset-env</code>, <code>babel-runtime-corejs3</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16357">#16357</a> Performance: improve <code>objectWithoutPropertiesLoose</code> on V8 (<a href="https://github.com/romgrk"><code>@​romgrk</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 6</h4>
<ul>
<li>Babel Bot (<a href="https://github.com/babel-bot"><code>@​babel-bot</code></a>)</li>
<li>Huáng Jùnliàng (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
<li>Nicolò Ribaudo (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
<li>Rom Grk (<a href="https://github.com/romgrk"><code>@​romgrk</code></a>)</li>
<li><a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a></li>
<li>ynnsuis (<a href="https://github.com/sossost"><code>@​sossost</code></a>)</li>
</ul>
<h2>v7.24.4 (2024-04-03)</h2>
<p>Thanks <a href="https://github.com/Dunqing"><code>@​Dunqing</code></a>, <a href="https://github.com/luiscubal"><code>@​luiscubal</code></a>, and <a href="https://github.com/samualtnorman"><code>@​samualtnorman</code></a> for your first PRs!</p>
<h4>:eyeglasses: Spec Compliance</h4>
<ul>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16403">#16403</a> Forbid initializerless using (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-decorators</code>, <code>babel-runtime-corejs3</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16388">#16388</a> Ensure decorators are callable (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/babel/babel/blob/main/CHANGELOG.md"><code>@​babel/core</code>'s changelog</a>.</em></p>
<blockquote>
<h2>v7.24.5 (2024-04-29)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-plugin-transform-classes</code>, <code>babel-traverse</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16377">#16377</a> fix: TypeScript annotation affects output (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-explicit-resource-management</code>, <code>babel-runtime-corejs3</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16440">#16440</a> Fix suppressed error order (<a href="https://github.com/sossost"><code>@​sossost</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16408">#16408</a> Await nullish async disposable (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:nail_care: Polish</h4>
<ul>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16407">#16407</a> Recover from exported <code>using</code> declaration (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:house: Internal</h4>
<ul>
<li>Other
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16414">#16414</a> Relax ESLint peerDependency constraint to allow v9 (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16425">#16425</a> Improve <code>@babel/parser</code> AST types (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16417">#16417</a> Always pass type argument to <code>.startNode</code> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-helper-create-class-features-plugin</code>, <code>babel-helper-member-expression-to-functions</code>, <code>babel-helper-module-transforms</code>, <code>babel-helper-split-export-declaration</code>, <code>babel-helper-wrap-function</code>, <code>babel-helpers</code>, <code>babel-plugin-bugfix-firefox-class-in-computed-class-key</code>, <code>babel-plugin-proposal-explicit-resource-management</code>, <code>babel-plugin-transform-block-scoping</code>, <code>babel-plugin-transform-destructuring</code>, <code>babel-plugin-transform-object-rest-spread</code>, <code>babel-plugin-transform-optional-chaining</code>, <code>babel-plugin-transform-parameters</code>, <code>babel-plugin-transform-private-property-in-object</code>, <code>babel-plugin-transform-react-jsx-self</code>, <code>babel-plugin-transform-typeof-symbol</code>, <code>babel-plugin-transform-typescript</code>, <code>babel-traverse</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16439">#16439</a> Make <code>NodePath&lt;T | U&gt;</code> distributive (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-proposal-partial-application</code>, <code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16421">#16421</a> Remove <code>JSXNamespacedName</code> from valid <code>CallExpression</code> args (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-transform-class-properties</code>, <code>babel-preset-env</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16406">#16406</a> Do not load unnecessary Babel 7 syntax plugins in Babel 8 (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h4>:running_woman: Performance</h4>
<ul>
<li><code>babel-helpers</code>, <code>babel-preset-env</code>, <code>babel-runtime-corejs3</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16357">#16357</a> Performance: improve <code>objectWithoutPropertiesLoose</code> on V8 (<a href="https://github.com/romgrk"><code>@​romgrk</code></a>)</li>
</ul>
</li>
</ul>
<h2>v7.24.4 (2024-04-03)</h2>
<h4>:eyeglasses: Spec Compliance</h4>
<ul>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16403">#16403</a> Forbid initializerless using (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-decorators</code>, <code>babel-runtime-corejs3</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16388">#16388</a> Ensure decorators are callable (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-generator</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16402">#16402</a> fix: Correctly prints <code>{ [key in Bar]? }</code> (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16394">#16394</a> fix: Correctly generate <code>TSMappedType</code> (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-compat-data</code>, <code>babel-plugin-bugfix-firefox-class-in-computed-class-key</code>, <code>babel-preset-env</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16390">#16390</a> Create bugfix plugin for classes in computed keys in Firefox (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-helper-create-class-features-plugin</code>, <code>babel-plugin-proposal-decorators</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16387">#16387</a> fix: support mutated outer decorated class binding (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16385">#16385</a> fix: Decorators when <code>super()</code> exists and <code>protoInit</code> is not needed (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-transform-block-scoping</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16384">#16384</a> fix: Transform scoping for <code>for X</code> in loop (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16368">#16368</a> fix: Capture <code>let</code> when the <code>for</code> body is not a block (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-core</code>, <code>babel-plugin-transform-block-scoped-functions</code>, <code>babel-plugin-transform-block-scoping</code></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/babel/babel/commit/ddbea7d4e6314f799eb371cc10e16f96ac2c96b2"><code>ddbea7d</code></a> v7.24.5</li>
<li><a href="https://github.com/babel/babel/commit/ee4875443db7563b87ef8e11e1fb75582ac72ac1"><code>ee48754</code></a> Use multiple TypeScript projects (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-core/issues/16430">#16430</a>)</li>
<li><a href="https://github.com/babel/babel/commit/a8994f8b7d421dd17b076c2557c9d5bd0e3faef1"><code>a8994f8</code></a> Reduce platform-specific tests (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-core/issues/16436">#16436</a>)</li>
<li><a href="https://github.com/babel/babel/commit/5a8c69253e2ddaf214585ae4638e452f9e608fcc"><code>5a8c692</code></a> v7.24.4</li>
<li><a href="https://github.com/babel/babel/commit/d4ade61b47d0c2141de3dce0dadf051ad064e4c9"><code>d4ade61</code></a> Test Babel 7/8 compatibility for plugins from es2019 to es2024 (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-core/issues/16399">#16399</a>)</li>
<li><a href="https://github.com/babel/babel/commit/b8eb831f0a544a1912094be7722683d2a1c7e289"><code>b8eb831</code></a> Fix incorrect function hoisting in some case statements (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-core/issues/16363">#16363</a>)</li>
<li><a href="https://github.com/babel/babel/commit/0eac8cab4c7abfd2b2df259822a3b1b6a11a4d2e"><code>0eac8ca</code></a> v7.24.3</li>
<li><a href="https://github.com/babel/babel/commit/fb7cf6343704731802c2dac18999990d7d4ce484"><code>fb7cf63</code></a> [babel 8] Remove <code>import_</code> fallback (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-core/issues/16365">#16365</a>)</li>
<li><a href="https://github.com/babel/babel/commit/822b025fc9d43263e69aed8a9fc80e8c6b8ebf6d"><code>822b025</code></a> v7.24.1</li>
<li><a href="https://github.com/babel/babel/commit/19fdca5f622b7fd3c3fee77b6e82caee205cc5a2"><code>19fdca5</code></a> Reduce the use of class names (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-core/issues/16326">#16326</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/babel/babel/commits/v7.24.5/packages/babel-core">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@babel/core&package-manager=npm_and_yarn&previous-version=7.22.10&new-version=7.24.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 20:42:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/283" class=".btn">#283</a>
            </td>
            <td>
                <b>
                    chore(deps): update hyper requirement from 0.14 to 1.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Updates the requirements on [hyper](https://github.com/hyperium/hyper) to permit the latest version.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/hyper/releases">hyper's releases</a>.</em></p>
<blockquote>
<h2>v0.14.28</h2>
<h2>Features</h2>
<ul>
<li><strong>body:</strong> deprecate to_bytes() and aggregate() (<a href="https://redirect.github.com/hyperium/hyper/issues/3466">#3466</a>) (<a href="https://github.com/hyperium/hyper/commit/7f382ad64326e1470912feb310d348fd79099c44">7f382ad6</a>)</li>
<li><strong>client:</strong> add <code>conn::http1::Connection::without_shutdown()</code> method (<a href="https://redirect.github.com/hyperium/hyper/issues/3431">#3431</a>) (<a href="https://github.com/hyperium/hyper/commit/ad504977b520a9582e5516a08b2f1028ef1b5e45">ad504977</a>)</li>
<li><strong>server:</strong> add <code>Builder::local_addr()</code> (<a href="https://redirect.github.com/hyperium/hyper/issues/3278">#3278</a>) (<a href="https://github.com/hyperium/hyper/commit/d342c2c714498d33891fa285a3c9ae991dc34769">d342c2c7</a>)</li>
</ul>
<h2>Bug Fixes</h2>
<ul>
<li><strong>client:</strong>
<ul>
<li>panic when pool idle timeout set to zero (<a href="https://redirect.github.com/hyperium/hyper/issues/3365">#3365</a>) (<a href="https://github.com/hyperium/hyper/commit/34d38008499de37d9b5b65440b3123ccd05c7510">34d38008</a>)</li>
<li>divide by zero error when DNS returns no addrs (<a href="https://redirect.github.com/hyperium/hyper/issues/3355">#3355</a>) (<a href="https://github.com/hyperium/hyper/commit/41eaf2042b8169d3dd067d49cfdbdaaf36678903">41eaf204</a>)</li>
<li>Do not strip <code>path</code> and <code>scheme</code> components from URIs for HTTP/2 Extended CONNEC (<a href="https://github.com/hyperium/hyper/commit/45aa62494127066c63c987a57cc5eae2c5361886">45aa6249</a>)</li>
<li>early respond from server shouldn't propagate reset error (<a href="https://redirect.github.com/hyperium/hyper/issues/3274">#3274</a>) (<a href="https://github.com/hyperium/hyper/commit/aac6760e032050dd47f5dbd32f852bf1ede9312b">aac6760e</a>, closes <a href="https://redirect.github.com/hyperium/hyper/issues/2872">#2872</a>)</li>
</ul>
</li>
<li><strong>http1:</strong>
<ul>
<li>add internal limit for chunked extensions (<a href="https://redirect.github.com/hyperium/hyper/issues/3495">#3495</a>) (<a href="https://github.com/hyperium/hyper/commit/344a87822951a46d252843ccc0b48e62988fc85b">344a8782</a>)</li>
<li>reject chunked headers missing a digit (<a href="https://redirect.github.com/hyperium/hyper/issues/3494">#3494</a>) (<a href="https://github.com/hyperium/hyper/commit/5eca028f4142e3e73f6d6188a4076f4db292b252">5eca028f</a>)</li>
</ul>
</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/bdbai"><code>@​bdbai</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/hyper/pull/3242">hyperium/hyper#3242</a></li>
<li><a href="https://github.com/gngpp"><code>@​gngpp</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/hyper/pull/3355">hyperium/hyper#3355</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/hyper/blob/v0.14.28/CHANGELOG.md">hyper's changelog</a>.</em></p>
<blockquote>
<h3>v0.14.28 (2023-12-18)</h3>
<h4>Bug Fixes</h4>
<ul>
<li><strong>client:</strong>
<ul>
<li>panic when pool idle timeout set to zero (<a href="https://redirect.github.com/hyperium/hyper/issues/3365">#3365</a>) (<a href="https://github.com/hyperium/hyper/commit/34d38008499de37d9b5b65440b3123ccd05c7510">34d38008</a>)</li>
<li>divide by zero error when DNS returns no addrs (<a href="https://redirect.github.com/hyperium/hyper/issues/3355">#3355</a>) (<a href="https://github.com/hyperium/hyper/commit/41eaf2042b8169d3dd067d49cfdbdaaf36678903">41eaf204</a>)</li>
<li>Do not strip <code>path</code> and <code>scheme</code> components from URIs for HTTP/2 Extended CONNEC (<a href="https://github.com/hyperium/hyper/commit/45aa62494127066c63c987a57cc5eae2c5361886">45aa6249</a>)</li>
<li>early respond from server shouldn't propagate reset error (<a href="https://redirect.github.com/hyperium/hyper/issues/3274">#3274</a>) (<a href="https://github.com/hyperium/hyper/commit/aac6760e032050dd47f5dbd32f852bf1ede9312b">aac6760e</a>, closes <a href="https://redirect.github.com/hyperium/hyper/issues/2872">#2872</a>)</li>
</ul>
</li>
<li><strong>http1:</strong>
<ul>
<li>add internal limit for chunked extensions (<a href="https://redirect.github.com/hyperium/hyper/issues/3495">#3495</a>) (<a href="https://github.com/hyperium/hyper/commit/344a87822951a46d252843ccc0b48e62988fc85b">344a8782</a>)</li>
<li>reject chunked headers missing a digit (<a href="https://redirect.github.com/hyperium/hyper/issues/3494">#3494</a>) (<a href="https://github.com/hyperium/hyper/commit/5eca028f4142e3e73f6d6188a4076f4db292b252">5eca028f</a>)</li>
</ul>
</li>
</ul>
<h4>Features</h4>
<ul>
<li><strong>body:</strong> deprecate to_bytes() and aggregate() (<a href="https://redirect.github.com/hyperium/hyper/issues/3466">#3466</a>) (<a href="https://github.com/hyperium/hyper/commit/7f382ad64326e1470912feb310d348fd79099c44">7f382ad6</a>)</li>
<li><strong>client:</strong> add <code>conn::http1::Connection::without_shutdown()</code> method (<a href="https://redirect.github.com/hyperium/hyper/issues/3431">#3431</a>) (<a href="https://github.com/hyperium/hyper/commit/ad504977b520a9582e5516a08b2f1028ef1b5e45">ad504977</a>)</li>
<li><strong>server:</strong> add <code>Builder::local_addr()</code> (<a href="https://redirect.github.com/hyperium/hyper/issues/3278">#3278</a>) (<a href="https://github.com/hyperium/hyper/commit/d342c2c714498d33891fa285a3c9ae991dc34769">d342c2c7</a>)</li>
</ul>
<h3>v0.14.27 (2023-06-26)</h3>
<h4>Bug Fixes</h4>
<ul>
<li><strong>http1:</strong>
<ul>
<li>send error on Incoming body when connection errors (<a href="https://redirect.github.com/hyperium/hyper/issues/3256">#3256</a>) (<a href="https://github.com/hyperium/hyper/commit/b107655ff8557d001bb8e558752f5f2247381e98">b107655f</a>, closes <a href="https://redirect.github.com/hyperium/hyper/issues/3253">#3253</a>)</li>
<li>properly end chunked bodies when it was known to be empty (<a href="https://redirect.github.com/hyperium/hyper/issues/3254">#3254</a>) (<a href="https://github.com/hyperium/hyper/commit/32422c47ec35e7405873277c87de14c18dbb98bd">32422c47</a>, closes <a href="https://redirect.github.com/hyperium/hyper/issues/3252">#3252</a>)</li>
</ul>
</li>
</ul>
<h4>Features</h4>
<ul>
<li><strong>client:</strong> include connection info in <code>Client::send_request</code> errors (<a href="https://redirect.github.com/hyperium/hyper/issues/2749">#2749</a>)</li>
</ul>
<h3>v0.14.26 (2023-04-13)</h3>
<h4>Features</h4>
<ul>
<li><strong>http2:</strong> add <code>max_pending_accept_reset_streams</code> configuration option (<a href="https://redirect.github.com/hyperium/hyper/issues/3201">#3201</a>) (<a href="https://github.com/hyperium/hyper/commit/a6f7571a5299793aef8f1aa4194574438b9df64c">a6f7571a</a>)</li>
</ul>
<h3>v0.14.25 (2023-03-10)</h3>
<h4>Features</h4>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperium/hyper/commit/98a7ab039461cd859e835ae4d15413489fe5cf6b"><code>98a7ab0</code></a> v0.14.28</li>
<li><a href="https://github.com/hyperium/hyper/commit/344a87822951a46d252843ccc0b48e62988fc85b"><code>344a878</code></a> fix(http1): add internal limit for chunked extensions (<a href="https://redirect.github.com/hyperium/hyper/issues/3495">#3495</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/5eca028f4142e3e73f6d6188a4076f4db292b252"><code>5eca028</code></a> fix(http1): reject chunked headers missing a digit (<a href="https://redirect.github.com/hyperium/hyper/issues/3494">#3494</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/7f382ad64326e1470912feb310d348fd79099c44"><code>7f382ad</code></a> feat(body): deprecate to_bytes() and aggregate() (<a href="https://redirect.github.com/hyperium/hyper/issues/3466">#3466</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/ad504977b520a9582e5516a08b2f1028ef1b5e45"><code>ad50497</code></a> feat(client): add <code>conn::http1::Connection::without_shutdown()</code> method (<a href="https://redirect.github.com/hyperium/hyper/issues/3431">#3431</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/48997034ed388ae7e0cb083ab1d343df312919a2"><code>4899703</code></a> chore(ci): cache rust dependency</li>
<li><a href="https://github.com/hyperium/hyper/commit/e2c223a246c5ff859f37e6962f61c31ac7572caa"><code>e2c223a</code></a> chore(ffi): revamp gen_header using cargo-expand</li>
<li><a href="https://github.com/hyperium/hyper/commit/45fef3be27979b7e349ca4658052bcadb74dc4e2"><code>45fef3b</code></a> chore(ci): check C header file with stable rust</li>
<li><a href="https://github.com/hyperium/hyper/commit/5bddd5e4c4546a9984ff2709e0be7b871566ea72"><code>5bddd5e</code></a> chore(ci): use stable rust for building C API</li>
<li><a href="https://github.com/hyperium/hyper/commit/440f23a834b3f6a0901e02321f4a76af60640118"><code>440f23a</code></a> chore(ci): replace actions-rs with run and use taiki-e/install-action or taik...</li>
<li>Additional commits viewable in <a href="https://github.com/hyperium/hyper/compare/v0.14.0...v0.14.28">compare view</a></li>
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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 20:42:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/282" class=".btn">#282</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump react-native from 0.67.2 to 0.74.1 in /wrappers/javascript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [react-native](https://github.com/facebook/react-native/tree/HEAD/packages/react-native) from 0.67.2 to 0.74.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/facebook/react-native/releases">react-native's releases</a>.</em></p>
<blockquote>
<h2>0.74.1</h2>
<h3>Added</h3>
<h4>iOS Specific</h4>
<ul>
<li>Implement privacy manifest aggregation  (<a href="https://github.com/facebook/react-native/commit/4be1fafec8edca5da5ebe515ad359d4178db7d23">4be1fafec8</a> by <a href="https://github.com/@aleqsio"><code>@​aleqsio</code></a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Align debugger Chrome launch flags with Meta-internal version (<a href="https://github.com/facebook/react-native/commit/93956e267cd4f1a77adaa842a55ca6f2d0d1b9c5">93956e267c</a> by <a href="https://github.com/@motiz88"><code>@​motiz88</code></a>)</li>
<li>Update &quot;Open Debugger&quot; to print extended Flipper guidance (<a href="https://github.com/facebook/react-native/commit/261a58761c2e7e10cc5cf0a63ed9785e1cdf097c">261a58761c</a> by <a href="https://github.com/@huntie"><code>@​huntie</code></a>)</li>
<li>Enable event loop by default when bridgeless is enabled (<a href="https://github.com/facebook/react-native/commit/b440672468b6d1d99cd322a4348dd90150703f24">b440672468</a> by <a href="https://github.com/@rubennorte"><code>@​rubennorte</code></a>)</li>
<li>Upgrade <code>@react-native-community/cli</code> to 13.6.6 (<a href="https://github.com/facebook/react-native/commit/58b1f9b2d4f617290a3a535153ff1e93a4672038">58b1f9b2d4</a> by <a href="https://github.com/@szymonrybczak"><code>@​szymonrybczak</code></a>)</li>
</ul>
<h4>Android specific</h4>
<ul>
<li>Support more stubbed methods in <code>BridgelessCatalystInstance</code> (<a href="https://github.com/facebook/react-native/commit/cc1c69799e284b368e3eaaac0ccd8e238384857f">cc1c69799e</a> by <a href="https://github.com/@javache"><code>@​javache</code></a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Reset animation state in TouchableOpacity and TouchableBounce (<a href="https://github.com/facebook/react-native/commit/165cabb21f2419bde63acb4b52be2f4fb7a2ec2e">165cabb21f</a> by <a href=""><code>@​sammy-SChttps://github.com/@sammy-</code></a>)</li>
<li>Add missing struct member initialization in Props.h (<a href="https://github.com/facebook/react-native/commit/13739510fb1c2400fbae1df1635fb93dae55abaa">13739510fb</a> by <a href="https://github.com/@alanleedev"><code>@​alanleedev</code></a>)</li>
</ul>
<h4>Android Specific</h4>
<ul>
<li>Split scheduler commit and flush delegate methods (<a href="https://github.com/facebook/react-native/commit/ff4b20e823d2838b3f72e550e7a89daa08551a72">ff4b20e823</a> by <a href="https://github.com/@javache"><code>@​javache</code></a>)</li>
<li>Fixing exposing ReactDelegate through ReactActivity for reload (<a href="https://github.com/facebook/react-native/commit/7a841dbcd1b4eead77827eda2bd307f11babec1f">7a841dbcd1</a> by <a href="https://github.com/@arushikesarwani94"><code>@​arushikesarwani94</code></a>)</li>
<li>Fix ReactActivity.getReactDelegate().reload() (<a href="https://github.com/facebook/react-native/commit/56631cd471008c39fe6f771052c3f1af7085bd63">56631cd471</a> by <a href="https://github.com/@kudo"><code>@​kudo</code></a>)</li>
</ul>
<h4>iOS Specific</h4>
<ul>
<li>Fix Symbol not found: (_JSGlobalContextSetInspectable) which crashed iOS &lt;16.4 with JSC (<a href="https://github.com/facebook/react-native/commit/0a4d97362f5a40cff62edce5200c3e7e8622d912">0a4d97362f</a> by <a href="https://github.com/@cipolleschi"><code>@​cipolleschi</code></a>)</li>
<li>Fallback to the first foregroundInactive window when there are no <code>foregroundActive</code> windows in RCTKeyWindow (<a href="https://github.com/facebook/react-native/commit/eaaf865449e6b89cc2794b68f314d01aa775748e">eaaf865449</a> by <a href="https://github.com/@cipolleschi"><code>@​cipolleschi</code></a>)</li>
<li>Fix enable hermes debugger in Bridgeless mode (<a href="https://github.com/facebook/react-native/commit/3467f2f3a3319cc695bd729a8789c46d15ac8314">3467f2f3a3</a> by <a href="https://github.com/@Cipolleschi"><code>@​Cipolleschi</code></a>)</li>
<li>Maintain correct content offset when scroll view is suspended (<a href="https://github.com/facebook/react-native/commit/305249f9642da50bf680b1401644eaba9d5dce50">305249f964</a> by <a href=""><code>@​sammy-SChttps://github.com/@sammy-</code></a>)</li>
<li>Avoid calling abstract methods in RCTComposedViewRegistry (<a href="https://github.com/facebook/react-native/commit/59e7ed50386cdae8f4a10d9ebc70566b9b36d01c">59e7ed5038</a> by <a href="https://github.com/@cipolleschi"><code>@​cipolleschi</code></a>)</li>
<li>Honor requiresMainQueueSetup in bridgeless mode for ViewManagers (<a href="https://github.com/facebook/react-native/commit/88130612864b40adf9001efed9fae2d1ab80b30c">8813061286</a> by <a href="https://github.com/@cipolleschi"><code>@​cipolleschi</code></a>)</li>
</ul>
<hr />
<!-- raw HTML omitted -->
<p>Hermes dSYMS:</p>
<ul>
<li><a href="https://repo1.maven.org/maven2/com/facebook/react/react-native-artifacts/0.74.1/react-native-artifacts-0.74.1-hermes-framework-dSYM-debug.tar.gz">Debug</a></li>
<li><a href="https://repo1.maven.org/maven2/com/facebook/react/react-native-artifacts/0.74.1/react-native-artifacts-0.74.1-hermes-framework-dSYM-release.tar.gz">Release</a></li>
</ul>
<hr />
<p>You can file issues or pick requests against this release <a href="https://github.com/reactwg/react-native-releases/issues/new/choose">here</a>.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/facebook/react-native/blob/main/CHANGELOG-pre-070.md">react-native's changelog</a>.</em></p>
<blockquote>
<h1>Changelog (pre 0.70)</h1>
<p>This file contains all changelogs for releases in the 0.60-0.69 range. Please check out the other <code>CHANGELOG-*.md</code> files for newer and older versions.</p>
<h2>v0.69.12</h2>
<h3>Changed</h3>
<ul>
<li>[0.69] Bump CLI to ^8.0.7, Metro to 0.70.4 (<a href="https://github.com/facebook/react-native/commit/56807fadfacf3c5cc62a8d1948b3d72ca51a5e6b">56807fadfa</a> by <a href="https://github.com/robhogan"><code>@​robhogan</code></a>)</li>
</ul>
<h4>iOS specific</h4>
<ul>
<li>[0.69] Use <code>Content-Location</code> header in bundle response as JS source URL (<a href="https://github.com/facebook/react-native/tree/HEAD/packages/react-native/issues/37501">#37501</a>) (<a href="https://github.com/facebook/react-native/commit/367fc7ad5254c5dd2c8ef38248766173525cc77c">367fc7ad52</a> by <a href="https://github.com/robhogan"><code>@​robhogan</code></a>)</li>
</ul>
<h3>Fixed</h3>
<h4>Android specific</h4>
<ul>
<li>Prevent crash in runAnimationStep on OnePlus and Oppo devices (<a href="https://github.com/facebook/react-native/tree/HEAD/packages/react-native/issues/37487">#37487</a>) (<a href="https://github.com/facebook/react-native/commit/4db7a10e257c664aced8cd8a1737d7ed9ced14fe">4db7a10e25</a> by <a href="https://github.com/hsource"><code>@​hsource</code></a>)</li>
</ul>
<h2>v0.69.11</h2>
<h3>Fixed</h3>
<h4>iOS specific</h4>
<ul>
<li>Make 0.69 compatible with Xcode 15 (thanks to <a href="https://github.com/AlexanderEggers"><code>@​AlexanderEggers</code></a> for the commit in main) (<a href="https://github.com/facebook/react-native/commit/37e8df1cdce4a66763c720b1b0768d049def9518">37e8df1cdc</a>)</li>
</ul>
<h2>v0.69.10</h2>
<h3>Fixed</h3>
<h4>Android specific</h4>
<ul>
<li>Minimize EditText Spans 8/N: CustomStyleSpan (<a href="https://github.com/facebook/react-native/commit/b384bb613bf533aebf3271ba335c61946fcd3303">b384bb613b</a> by <a href="https://github.com/NickGerleman"><code>@​NickGerleman</code></a>)</li>
<li>Minimize EditText Spans 6/N: letterSpacing (<a href="https://github.com/facebook/react-native/commit/5791cf1f7b43aed1d98cad7bcc272d97ab659111">5791cf1f7b</a> by <a href="https://github.com/NickGerleman"><code>@​NickGerleman</code></a>)</li>
<li>Minimize Spans 5/N: Strikethrough and Underline (<a href="https://github.com/facebook/react-native/commit/0869ea29db6a4ca20b9043d592a2233ae1a0e7a2">0869ea29db</a> by <a href="https://github.com/NickGerleman"><code>@​NickGerleman</code></a>)</li>
<li>Minimize Spans 4/N: ReactForegroundColorSpan (<a href="https://github.com/facebook/react-native/commit/8c9c8ba5adb59f7f891a5307a0bce7200dd3ac7d">8c9c8ba5ad</a> by <a href="https://github.com/NickGerleman"><code>@​NickGerleman</code></a>)</li>
<li>Minimize Spans 3/N: ReactBackgroundColorSpan (<a href="https://github.com/facebook/react-native/commit/cc0ba57ea42d876155b2fd7d9ee78604ff8aa57a">cc0ba57ea4</a> by <a href="https://github.com/NickGerleman"><code>@​NickGerleman</code></a>)</li>
<li>Minimize Spans 1/N: Fix precedence (<a href="https://github.com/facebook/react-native/commit/1743dd7ab40998c4d3491e3b2c56c531daf5dc47">1743dd7ab4</a> by <a href="https://github.com/NickGerleman"><code>@​NickGerleman</code></a>)</li>
<li>Fix measurement of uncontrolled TextInput after edit (<a href="https://github.com/facebook/react-native/commit/8a0fe30591e21b90a3481c1ef3eeadd4b592f3ed">8a0fe30591</a> by <a href="https://github.com/NickGerleman"><code>@​NickGerleman</code></a>)</li>
</ul>
<h2>v0.69.9</h2>
<h3>Changed</h3>
<h4>iOS specific</h4>
<ul>
<li>Relax Ruby requirements (<a href="https://github.com/facebook/react-native/commit/4e015c69d646b320d58888f70af566c1d753eaed">4e015c69d6</a> by <a href="https://github.com/cipolleschi"><code>@​cipolleschi</code></a>)</li>
</ul>
<h3>Fixed</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/facebook/react-native/commit/31f9d45074f069151c155836335e0edff87f70bd"><code>31f9d45</code></a> Release 0.74.1</li>
<li><a href="https://github.com/facebook/react-native/commit/093a2adc07fe5d2879b1a5bca12940b4763a6b6c"><code>093a2ad</code></a> [LOCAL] Fix privacy manifest aggregator</li>
<li><a href="https://github.com/facebook/react-native/commit/a0ed073650cbdc3e1e08c11d18acf73e0952393a"><code>a0ed073</code></a> [LOCAL] Fix compilation error on ReactDelegate</li>
<li><a href="https://github.com/facebook/react-native/commit/4be1fafec8edca5da5ebe515ad359d4178db7d23"><code>4be1faf</code></a> Implement privacy manifest aggregation (<a href="https://github.com/facebook/react-native/tree/HEAD/packages/react-native/issues/44214">#44214</a>)</li>
<li><a href="https://github.com/facebook/react-native/commit/56631cd471008c39fe6f771052c3f1af7085bd63"><code>56631cd</code></a> fix ReactActivity.getReactDelegate().reload() (<a href="https://github.com/facebook/react-native/tree/HEAD/packages/react-native/issues/44223">#44223</a>)</li>
<li><a href="https://github.com/facebook/react-native/commit/cc1c69799e284b368e3eaaac0ccd8e238384857f"><code>cc1c697</code></a> Support more stubbed methods in BridgelessCatalystInstance (<a href="https://github.com/facebook/react-native/tree/HEAD/packages/react-native/issues/44091">#44091</a>)</li>
<li><a href="https://github.com/facebook/react-native/commit/58b1f9b2d4f617290a3a535153ff1e93a4672038"><code>58b1f9b</code></a> feat: upgrade <code>@react-native-community/cli</code> to <code>13.6.6</code> (<a href="https://github.com/facebook/react-native/tree/HEAD/packages/react-native/issues/44253">#44253</a>)</li>
<li><a href="https://github.com/facebook/react-native/commit/88130612864b40adf9001efed9fae2d1ab80b30c"><code>8813061</code></a> Honor <code>requiresMainQueueSetup</code> in bridgeless mode for ViewManagers</li>
<li><a href="https://github.com/facebook/react-native/commit/59e7ed50386cdae8f4a10d9ebc70566b9b36d01c"><code>59e7ed5</code></a> Avoid calling abstract methods in RCTComposedViewRegistry</li>
<li><a href="https://github.com/facebook/react-native/commit/305249f9642da50bf680b1401644eaba9d5dce50"><code>305249f</code></a> maintain correct content offset when scroll view is suspended (<a href="https://github.com/facebook/react-native/tree/HEAD/packages/react-native/issues/44256">#44256</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/facebook/react-native/commits/v0.74.1/packages/react-native">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~react-native-bot">react-native-bot</a>, a new releaser for react-native since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=react-native&package-manager=npm_and_yarn&previous-version=0.67.2&new-version=0.74.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 20:42:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/281" class=".btn">#281</a>
            </td>
            <td>
                <b>
                    chore(deps): update hyper-tls requirement from 0.5 to 0.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Updates the requirements on [hyper-tls](https://github.com/hyperium/hyper-tls) to permit the latest version.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperium/hyper-tls/commit/0265e166a8886f01253050516316a95900315b81"><code>0265e16</code></a> v0.6.0</li>
<li><a href="https://github.com/hyperium/hyper-tls/commit/373d1934537facd5f4300c57959453945d74c6e6"><code>373d193</code></a> add alpn support (<a href="https://redirect.github.com/hyperium/hyper-tls/issues/107">#107</a>)</li>
<li><a href="https://github.com/hyperium/hyper-tls/commit/95ebd8d3ac8785e552fc9fee0ffac141bb361423"><code>95ebd8d</code></a> tidy up dependency features (<a href="https://redirect.github.com/hyperium/hyper-tls/issues/106">#106</a>)</li>
<li><a href="https://github.com/hyperium/hyper-tls/commit/3fc97a044187db5813c50a17b2d8c9c856ae0893"><code>3fc97a0</code></a> Update hyper dependencies (<a href="https://redirect.github.com/hyperium/hyper-tls/issues/105">#105</a>)</li>
<li><a href="https://github.com/hyperium/hyper-tls/commit/9adf50b46e313a41987990a677cb487ebb3be393"><code>9adf50b</code></a> feat: upgrade to hyper-v1, use hyper-utils for now (<a href="https://redirect.github.com/hyperium/hyper-tls/issues/104">#104</a>)</li>
<li><a href="https://github.com/hyperium/hyper-tls/commit/5e4cb93e31065b979099f75bc8f38f250a838ff0"><code>5e4cb93</code></a> chore: port CI from hyper-util (<a href="https://redirect.github.com/hyperium/hyper-tls/issues/103">#103</a>)</li>
<li><a href="https://github.com/hyperium/hyper-tls/commit/74044e32b5eb6cdc8a70978a1f584dc7b0748932"><code>74044e3</code></a> Fix typo in documentation of client.rs (<a href="https://redirect.github.com/hyperium/hyper-tls/issues/87">#87</a>)</li>
<li>See full diff in <a href="https://github.com/hyperium/hyper-tls/compare/v0.5.0...v0.6.0">compare view</a></li>
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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 20:42:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/280" class=".btn">#280</a>
            </td>
            <td>
                <b>
                    chore(deps): update reqwest requirement from 0.11.17 to 0.12.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Updates the requirements on [reqwest](https://github.com/seanmonstar/reqwest) to permit the latest version.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/seanmonstar/reqwest/releases">reqwest's releases</a>.</em></p>
<blockquote>
<h2>v0.12.4</h2>
<h2>What's Changed</h2>
<ul>
<li>Add <code>zstd</code> support, enabled with <code>zstd</code> Cargo feature (thanks <a href="https://github.com/paolobarbolini"><code>@​paolobarbolini</code></a>!)</li>
<li>Add <code>ClientBuilder::read_timeout(Duration)</code>, which applies the duration for each read operation. The timeout resets after a successful read.</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/SamuelMarks"><code>@​SamuelMarks</code></a> made their first contribution in <a href="https://redirect.github.com/seanmonstar/reqwest/pull/2245">seanmonstar/reqwest#2245</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/seanmonstar/reqwest/blob/master/CHANGELOG.md">reqwest's changelog</a>.</em></p>
<blockquote>
<h2>v0.12.4</h2>
<ul>
<li>Add <code>zstd</code> support, enabled with <code>zstd</code> Cargo feature.</li>
<li>Add <code>ClientBuilder::read_timeout(Duration)</code>, which applies the duration for each read operation. The timeout resets after a successful read.</li>
</ul>
<h2>v0.12.3</h2>
<ul>
<li>Add <code>FromStr</code> for <code>dns::Name</code>.</li>
<li>Add <code>ClientBuilder::built_in_webpki_certs(bool)</code> to enable them separately.</li>
<li>Add <code>ClientBuilder::built_in_native_certs(bool)</code> to enable them separately.</li>
<li>Fix sending <code>content-length: 0</code> for GET requests.</li>
<li>Fix response body <code>content_length()</code> to return value when timeout is configured.</li>
<li>Fix <code>ClientBuilder::resolve()</code> to use lowercase domain names.</li>
</ul>
<h2>v0.12.2</h2>
<ul>
<li>Fix missing ALPN when connecting to socks5 proxy with rustls.</li>
<li>Fix TLS version limits with rustls.</li>
<li>Fix not detected ALPN h2 from server with native-tls.</li>
</ul>
<h2>v0.12.1</h2>
<ul>
<li>Fix <code>ClientBuilder::interface()</code> when no TLS is enabled.</li>
<li>Fix <code>TlsInfo::peer_certificate()</code> being truncated with rustls.</li>
<li>Fix panic if <code>http2</code> feature disabled but TLS negotiated h2 in ALPN.</li>
<li>Fix <code>Display</code> for <code>Error</code> to not include its source error.</li>
</ul>
<h1>v0.12.0</h1>
<ul>
<li>Upgrade to <code>hyper</code>, <code>http</code>, and <code>http-body</code> v1.</li>
<li>Add better support for converting to and from <code>http::Request</code> and <code>http::Response</code>.</li>
<li>Add <code>http2</code> optional cargo feature, default on.</li>
<li>Add <code>charset</code> optional cargo feature, default on.</li>
<li>Add <code>macos-system-configuration</code> cargo feature, default on.</li>
<li>Change all optional dependencies to no longer be exposed as implicit features.</li>
<li>Add <code>ClientBuilder::interface(str)</code> to specify the local interface to bind to.</li>
<li>Experimental: disables the <code>http3</code> feature temporarily.</li>
</ul>
<h2>v0.11.27</h2>
<ul>
<li>Add <code>hickory-dns</code> feature, deprecating <code>trust-dns</code>.</li>
<li>(wasm) Fix <code>Form::text()</code> to not set octet-stream for plain text fields.</li>
</ul>
<h2>v0.11.26</h2>
<ul>
<li>Revert <code>system-configuration</code> upgrade, which broke MSRV on macOS.</li>
</ul>
<h2>v0.11.25</h2>
<ul>
<li>Fix <code>Certificate::from_pem_bundle()</code> parsing.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/seanmonstar/reqwest/commit/de5dbb1ab849cc301dcefebaeabdf4ce2e0f1e53"><code>de5dbb1</code></a> v0.12.4</li>
<li><a href="https://github.com/seanmonstar/reqwest/commit/0f126f57abd09985526dbdf86777d209afbd7cc0"><code>0f126f5</code></a> tests: fix blocking test about empty bodies and content-length</li>
<li><a href="https://github.com/seanmonstar/reqwest/commit/107388134b7c1ea684cc76ed00efe2db12194610"><code>1073881</code></a> feat: add zstd support (<a href="https://redirect.github.com/seanmonstar/reqwest/issues/1866">#1866</a>)</li>
<li><a href="https://github.com/seanmonstar/reqwest/commit/1af8945143f0a4ba5563e2982b06fc303afea50b"><code>1af8945</code></a> feat: add ClientBuilder::read_timeout(dur) (<a href="https://redirect.github.com/seanmonstar/reqwest/issues/2241">#2241</a>)</li>
<li><a href="https://github.com/seanmonstar/reqwest/commit/e99da854a18ed6e968e0fff5bbf24a72983a0dc9"><code>e99da85</code></a> refactor: fix warnings related to mutability of <code>self</code> (<a href="https://redirect.github.com/seanmonstar/reqwest/issues/2245">#2245</a>)</li>
<li><a href="https://github.com/seanmonstar/reqwest/commit/0720159f6369f54e045a1fd315e0f24b7a0b4a39"><code>0720159</code></a> v0.12.3</li>
<li><a href="https://github.com/seanmonstar/reqwest/commit/92096952b7257af6a9eea6f94c5be04c418be0e3"><code>9209695</code></a> Remove duplicate example for ClientBuilder::default_headers (<a href="https://redirect.github.com/seanmonstar/reqwest/issues/2236">#2236</a>)</li>
<li><a href="https://github.com/seanmonstar/reqwest/commit/e3a15650d600f3ab1aa2c6f83dc7567a8677337e"><code>e3a1565</code></a> fix: use lower case domain string when using <code>resolve</code> and <code>resolve_to_addrs</code>...</li>
<li><a href="https://github.com/seanmonstar/reqwest/commit/b4c491a6ffa10418d8bfaa49fc38f2175312f90c"><code>b4c491a</code></a> feat: allow fine-grained root certs for rustls (<a href="https://redirect.github.com/seanmonstar/reqwest/issues/2232">#2232</a>)</li>
<li><a href="https://github.com/seanmonstar/reqwest/commit/cf4295d59d614b1b813cacfe97f186fba952a358"><code>cf4295d</code></a> chore: update winreg to 0.52.0 (<a href="https://redirect.github.com/seanmonstar/reqwest/issues/2226">#2226</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/seanmonstar/reqwest/compare/v0.11.17...v0.12.4">compare view</a></li>
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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 20:42:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/279" class=".btn">#279</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump @babel/runtime from 7.22.10 to 7.24.5 in /wrappers/javascript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@babel/runtime](https://github.com/babel/babel/tree/HEAD/packages/babel-runtime) from 7.22.10 to 7.24.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/babel/babel/releases"><code>@​babel/runtime</code>'s releases</a>.</em></p>
<blockquote>
<h2>v7.24.5 (2024-04-29)</h2>
<p>Thanks <a href="https://github.com/romgrk"><code>@​romgrk</code></a> and <a href="https://github.com/sossost"><code>@​sossost</code></a> for your first PRs!</p>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-plugin-transform-classes</code>, <code>babel-traverse</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16377">#16377</a> fix: TypeScript annotation affects output (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-explicit-resource-management</code>, <code>babel-runtime-corejs3</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16440">#16440</a> Fix suppressed error order (<a href="https://github.com/sossost"><code>@​sossost</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16408">#16408</a> Await nullish async disposable (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:nail_care: Polish</h4>
<ul>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16407">#16407</a> Recover from exported <code>using</code> declaration (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:house: Internal</h4>
<ul>
<li>Other
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16414">#16414</a> Relax ESLint peerDependency constraint to allow v9 (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16425">#16425</a> Improve <code>@babel/parser</code> AST types (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16417">#16417</a> Always pass type argument to <code>.startNode</code> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-helper-create-class-features-plugin</code>, <code>babel-helper-member-expression-to-functions</code>, <code>babel-helper-module-transforms</code>, <code>babel-helper-split-export-declaration</code>, <code>babel-helper-wrap-function</code>, <code>babel-helpers</code>, <code>babel-plugin-bugfix-firefox-class-in-computed-class-key</code>, <code>babel-plugin-proposal-explicit-resource-management</code>, <code>babel-plugin-transform-block-scoping</code>, <code>babel-plugin-transform-destructuring</code>, <code>babel-plugin-transform-object-rest-spread</code>, <code>babel-plugin-transform-optional-chaining</code>, <code>babel-plugin-transform-parameters</code>, <code>babel-plugin-transform-private-property-in-object</code>, <code>babel-plugin-transform-react-jsx-self</code>, <code>babel-plugin-transform-typeof-symbol</code>, <code>babel-plugin-transform-typescript</code>, <code>babel-traverse</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16439">#16439</a> Make <code>NodePath&lt;T | U&gt;</code> distributive (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-proposal-partial-application</code>, <code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16421">#16421</a> Remove <code>JSXNamespacedName</code> from valid <code>CallExpression</code> args (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-transform-class-properties</code>, <code>babel-preset-env</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16406">#16406</a> Do not load unnecessary Babel 7 syntax plugins in Babel 8 (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h4>:running_woman: Performance</h4>
<ul>
<li><code>babel-helpers</code>, <code>babel-preset-env</code>, <code>babel-runtime-corejs3</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16357">#16357</a> Performance: improve <code>objectWithoutPropertiesLoose</code> on V8 (<a href="https://github.com/romgrk"><code>@​romgrk</code></a>)</li>
</ul>
</li>
</ul>
<h4>Committers: 6</h4>
<ul>
<li>Babel Bot (<a href="https://github.com/babel-bot"><code>@​babel-bot</code></a>)</li>
<li>Huáng Jùnliàng (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
<li>Nicolò Ribaudo (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
<li>Rom Grk (<a href="https://github.com/romgrk"><code>@​romgrk</code></a>)</li>
<li><a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a></li>
<li>ynnsuis (<a href="https://github.com/sossost"><code>@​sossost</code></a>)</li>
</ul>
<h2>v7.24.4 (2024-04-03)</h2>
<p>Thanks <a href="https://github.com/Dunqing"><code>@​Dunqing</code></a>, <a href="https://github.com/luiscubal"><code>@​luiscubal</code></a>, and <a href="https://github.com/samualtnorman"><code>@​samualtnorman</code></a> for your first PRs!</p>
<h4>:eyeglasses: Spec Compliance</h4>
<ul>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16403">#16403</a> Forbid initializerless using (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-decorators</code>, <code>babel-runtime-corejs3</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16388">#16388</a> Ensure decorators are callable (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/babel/babel/blob/main/CHANGELOG.md"><code>@​babel/runtime</code>'s changelog</a>.</em></p>
<blockquote>
<h2>v7.24.5 (2024-04-29)</h2>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-plugin-transform-classes</code>, <code>babel-traverse</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16377">#16377</a> fix: TypeScript annotation affects output (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-explicit-resource-management</code>, <code>babel-runtime-corejs3</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16440">#16440</a> Fix suppressed error order (<a href="https://github.com/sossost"><code>@​sossost</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16408">#16408</a> Await nullish async disposable (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:nail_care: Polish</h4>
<ul>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16407">#16407</a> Recover from exported <code>using</code> declaration (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:house: Internal</h4>
<ul>
<li>Other
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16414">#16414</a> Relax ESLint peerDependency constraint to allow v9 (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16425">#16425</a> Improve <code>@babel/parser</code> AST types (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16417">#16417</a> Always pass type argument to <code>.startNode</code> (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-helper-create-class-features-plugin</code>, <code>babel-helper-member-expression-to-functions</code>, <code>babel-helper-module-transforms</code>, <code>babel-helper-split-export-declaration</code>, <code>babel-helper-wrap-function</code>, <code>babel-helpers</code>, <code>babel-plugin-bugfix-firefox-class-in-computed-class-key</code>, <code>babel-plugin-proposal-explicit-resource-management</code>, <code>babel-plugin-transform-block-scoping</code>, <code>babel-plugin-transform-destructuring</code>, <code>babel-plugin-transform-object-rest-spread</code>, <code>babel-plugin-transform-optional-chaining</code>, <code>babel-plugin-transform-parameters</code>, <code>babel-plugin-transform-private-property-in-object</code>, <code>babel-plugin-transform-react-jsx-self</code>, <code>babel-plugin-transform-typeof-symbol</code>, <code>babel-plugin-transform-typescript</code>, <code>babel-traverse</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16439">#16439</a> Make <code>NodePath&lt;T | U&gt;</code> distributive (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-proposal-partial-application</code>, <code>babel-types</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16421">#16421</a> Remove <code>JSXNamespacedName</code> from valid <code>CallExpression</code> args (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-transform-class-properties</code>, <code>babel-preset-env</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16406">#16406</a> Do not load unnecessary Babel 7 syntax plugins in Babel 8 (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
</ul>
<h4>:running_woman: Performance</h4>
<ul>
<li><code>babel-helpers</code>, <code>babel-preset-env</code>, <code>babel-runtime-corejs3</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16357">#16357</a> Performance: improve <code>objectWithoutPropertiesLoose</code> on V8 (<a href="https://github.com/romgrk"><code>@​romgrk</code></a>)</li>
</ul>
</li>
</ul>
<h2>v7.24.4 (2024-04-03)</h2>
<h4>:eyeglasses: Spec Compliance</h4>
<ul>
<li><code>babel-parser</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16403">#16403</a> Forbid initializerless using (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
<li><code>babel-helpers</code>, <code>babel-plugin-proposal-decorators</code>, <code>babel-runtime-corejs3</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16388">#16388</a> Ensure decorators are callable (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
</ul>
</li>
</ul>
<h4>:bug: Bug Fix</h4>
<ul>
<li><code>babel-generator</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16402">#16402</a> fix: Correctly prints <code>{ [key in Bar]? }</code> (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16394">#16394</a> fix: Correctly generate <code>TSMappedType</code> (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-compat-data</code>, <code>babel-plugin-bugfix-firefox-class-in-computed-class-key</code>, <code>babel-preset-env</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16390">#16390</a> Create bugfix plugin for classes in computed keys in Firefox (<a href="https://github.com/nicolo-ribaudo"><code>@​nicolo-ribaudo</code></a>)</li>
</ul>
</li>
<li><code>babel-helper-create-class-features-plugin</code>, <code>babel-plugin-proposal-decorators</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16387">#16387</a> fix: support mutated outer decorated class binding (<a href="https://github.com/JLHwung"><code>@​JLHwung</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16385">#16385</a> fix: Decorators when <code>super()</code> exists and <code>protoInit</code> is not needed (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-plugin-transform-block-scoping</code>
<ul>
<li><a href="https://redirect.github.com/babel/babel/pull/16384">#16384</a> fix: Transform scoping for <code>for X</code> in loop (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
<li><a href="https://redirect.github.com/babel/babel/pull/16368">#16368</a> fix: Capture <code>let</code> when the <code>for</code> body is not a block (<a href="https://github.com/liuxingbaoyu"><code>@​liuxingbaoyu</code></a>)</li>
</ul>
</li>
<li><code>babel-core</code>, <code>babel-plugin-transform-block-scoped-functions</code>, <code>babel-plugin-transform-block-scoping</code></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/babel/babel/commit/ddbea7d4e6314f799eb371cc10e16f96ac2c96b2"><code>ddbea7d</code></a> v7.24.5</li>
<li><a href="https://github.com/babel/babel/commit/5a8c69253e2ddaf214585ae4638e452f9e608fcc"><code>5a8c692</code></a> v7.24.4</li>
<li><a href="https://github.com/babel/babel/commit/822b025fc9d43263e69aed8a9fc80e8c6b8ebf6d"><code>822b025</code></a> v7.24.1</li>
<li><a href="https://github.com/babel/babel/commit/c6cf0d706cf3b8418902d49dcf8236c1785d156d"><code>c6cf0d7</code></a> Allow separate helpers to be excluded in Babel 8 (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-runtime/issues/16323">#16323</a>)</li>
<li><a href="https://github.com/babel/babel/commit/ce59160e34e21e8f1ac2fc55ae037f7b043e8d20"><code>ce59160</code></a> v7.24.0</li>
<li><a href="https://github.com/babel/babel/commit/24fb6f880f43c079476985f7f042caf5dab4a202"><code>24fb6f8</code></a> Do not use descriptors for private class elements (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-runtime/issues/16261">#16261</a>)</li>
<li><a href="https://github.com/babel/babel/commit/e2649b13dd5cbeab4a7840b801c0ab893ab05308"><code>e2649b1</code></a> Support decorator 2023-11 normative updates (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-runtime/issues/16242">#16242</a>)</li>
<li><a href="https://github.com/babel/babel/commit/a0dd614d1271dd69db1ce908e5171d4ccfec8691"><code>a0dd614</code></a> v7.23.9</li>
<li><a href="https://github.com/babel/babel/commit/218faee4351345415b40b23a9e0102f628d45108"><code>218faee</code></a> Improve output of <code>using</code> (<a href="https://github.com/babel/babel/tree/HEAD/packages/babel-runtime/issues/15959">#15959</a>)</li>
<li><a href="https://github.com/babel/babel/commit/80c554fdbc6636683c51d580947384d3ce7f26ad"><code>80c554f</code></a> v7.23.8</li>
<li>Additional commits viewable in <a href="https://github.com/babel/babel/commits/v7.24.5/packages/babel-runtime">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@babel/runtime&package-manager=npm_and_yarn&previous-version=7.22.10&new-version=7.24.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 20:42:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/278" class=".btn">#278</a>
            </td>
            <td>
                <b>
                    chore(deps): update time requirement from =0.3.20 to =0.3.36
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Updates the requirements on [time](https://github.com/time-rs/time) to permit the latest version.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/time-rs/time/releases">time's releases</a>.</em></p>
<blockquote>
<h2>v0.3.36</h2>
<p>See the <a href="https://github.com/time-rs/time/blob/main/CHANGELOG.md">changelog</a> for details.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/time-rs/time/blob/main/CHANGELOG.md">time's changelog</a>.</em></p>
<blockquote>
<h2>0.3.36 [2024-04-10]</h2>
<h3># Fixed</h3>
<ul>
<li><code>FormatItem</code> can be used as part of an import path. See <a href="https://redirect.github.com/time-rs/time/issues/675">#675</a> for details.</li>
</ul>
<p><a href="https://redirect.github.com/time-rs/time/issues/675">#675</a>: <a href="https://redirect.github.com/time-rs/time/issues/675">time-rs/time#675</a></p>
<h2>0.3.35 [2024-04-10]</h2>
<h3>Added</h3>
<ul>
<li><code>Duration::checked_neg</code></li>
<li><code>ext::InstantExt</code>, which provides methods for using <code>time::Duration</code> with <code>std::time::Instant</code></li>
</ul>
<h3>Changed</h3>
<ul>
<li><code>Instant</code> is deprecated. It is recommended to use <code>std::time::Instant</code> directly, importing
<code>time::ext::InstantExt</code> for interoperability with <code>time::Duration</code>.</li>
<li><code>FormatItem</code> has been renamed to <code>BorrowedFormatItem</code>, avoiding confusion with <code>OwnedFormatItem</code>.
An alias has been added for backwards compatibility.</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>The weekday is optional when parsing RFC2822.</li>
<li>The range of sub-second values in <code>Duration</code> is documented correctly. The previous documentation
contained an off-by-one error.</li>
<li>Leap seconds are now correctly handled when parsing ISO 8601.</li>
</ul>
<h2>0.3.34 [2024-02-03]</h2>
<h3>Fixed</h3>
<p>Computing the local offset on Windows works again. It was broken in some cases in v0.3.32 and
v0.3.33.</p>
<h2>0.3.33 [2024-02-03]</h2>
<h3>Fixed</h3>
<p>Builds targeting <code>wasm32-unknown-unknown</code> now work again.</p>
<h2>0.3.32 [2024-02-01]</h2>
<h3>Added</h3>
<ul>
<li>Methods to replace the day of the year.
<ul>
<li><code>Date::replace_ordinal</code></li>
<li><code>PrimitiveDateTime::replace_ordinal</code></li>
<li><code>OffsetDateTime::replace_ordinal</code></li>
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
<li><a href="https://github.com/time-rs/time/commit/3c3c546a661ac59e1a586a4edc65adff04fd1335"><code>3c3c546</code></a> <code>pub use</code> instead of <code>pub type</code> re-exporting</li>
<li><a href="https://github.com/time-rs/time/commit/266178da674121982d4d79404380c9bf7ed7236f"><code>266178d</code></a> Update code coverage CI</li>
<li><a href="https://github.com/time-rs/time/commit/131049ea15d9a445fee306f87707d6751637f9fd"><code>131049e</code></a> v0.3.35 release</li>
<li><a href="https://github.com/time-rs/time/commit/9c15ee34668fc99c918656fb2895b6d0bfdf7d75"><code>9c15ee3</code></a> Permit leap seconds when parsing ISO 8601</li>
<li><a href="https://github.com/time-rs/time/commit/d279d8d38f5932ce8d0483df15f9df2e572dd026"><code>d279d8d</code></a> Fix invalid offset hour diagnostic test</li>
<li><a href="https://github.com/time-rs/time/commit/f04a28feecd42e5e0657bdad2a4cf0f93c9ee749"><code>f04a28f</code></a> Eliminate unreachable branch</li>
<li><a href="https://github.com/time-rs/time/commit/06a096d821c9137e7a81f7e360cdd8323d19339f"><code>06a096d</code></a> Rename <code>FormatItem</code> to <code>BorrowedFormatItem</code></li>
<li><a href="https://github.com/time-rs/time/commit/fd664eef0dd6bf4ca729ece9f4bfd8c4bd96ef82"><code>fd664ee</code></a> Include diagnostics regression</li>
<li><a href="https://github.com/time-rs/time/commit/b8d09a7bccbd3ea300fe30bf12b5f0a11ba1d539"><code>b8d09a7</code></a> Address nightly lints</li>
<li><a href="https://github.com/time-rs/time/commit/330865ac9065978664eb49d906b2f0d251426720"><code>330865a</code></a> Update deny.toml</li>
<li>Additional commits viewable in <a href="https://github.com/time-rs/time/compare/v0.3.20...v0.3.36">compare view</a></li>
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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 20:42:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/277" class=".btn">#277</a>
            </td>
            <td>
                <b>
                    chore(deps): update rstest requirement from 0.18 to 0.19
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Updates the requirements on [rstest](https://github.com/la10736/rstest) to permit the latest version.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/la10736/rstest/releases">rstest's releases</a>.</em></p>
<blockquote>
<p>Introduce MSRV and minor fixes</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/la10736/rstest/blob/master/CHANGELOG.md">rstest's changelog</a>.</em></p>
<blockquote>
<h2>[0.19.0] 2024/4/9</h2>
<h3>Changed</h3>
<ul>
<li>Defined <code>rust-version</code> for each crate (see <a href="https://redirect.github.com/la10736/rstest/issues/227">#227</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>
<p><code>#[once]</code> fixtures now require the returned type to be
<a href="https://doc.rust-lang.org/std/marker/trait.Sync.html"><code>Sync</code></a> to prevent UB
when tests are executed in parallel. (see <a href="https://redirect.github.com/la10736/rstest/issues/235">#235</a>
for more details)</p>
</li>
<li>
<p><code>#[future(awt)]</code> and <code>#[awt]</code> now properly handle mutable (<code>mut</code>) parameters by treating futures as immutable and
treating the awaited rebinding as mutable.</p>
</li>
</ul>
<h2>[0.18.2] 2023/8/13</h2>
<h3>Changed</h3>
<ul>
<li>Now <code>#[files]</code> accept also parent folders (see <a href="https://redirect.github.com/la10736/rstest/issues/205">#205</a>
for more details).</li>
</ul>
<h2>[0.18.1] 2023/7/5</h2>
<h3>Fixed</h3>
<ul>
<li>Wrong doc test</li>
<li>Docs</li>
</ul>
<h2>[0.18.0] 2023/7/4</h2>
<h3>Add</h3>
<ul>
<li>Add support for <code>RSTEST_TIMEOUT</code> environment variable to define a max timeout
for each function (see <a href="https://redirect.github.com/la10736/rstest/issues/190">#190</a> for details).
Thanks to <a href="https://github.com/aviramha"><code>@​aviramha</code></a> for idea and PR</li>
<li><code>#[files(&quot;glob path&quot;)]</code> attribute to generate tests based on files that
satisfy the given glob path (see <a href="https://redirect.github.com/la10736/rstest/issues/163">#163</a> for details).</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Switch to <code>syn</code> 2.0 and edition 2021 : minimal Rust version now is 1.56.0
both for <code>rstest</code> and <code>rstest_reuse</code> (see <a href="https://redirect.github.com/la10736/rstest/issues/187">#187</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Fixed wired behavior on extraction <code>#[awt]</code> function attrs (See
<a href="https://redirect.github.com/la10736/rstest/issues/189">#189</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/la10736/rstest/commit/3ffd682568b49bcd77bc69742da0fc59c1e3ea37"><code>3ffd682</code></a> Fix license links</li>
<li><a href="https://github.com/la10736/rstest/commit/36ab06d68eff527fa325ce5464f378001ac7a161"><code>36ab06d</code></a> Fix license link</li>
<li><a href="https://github.com/la10736/rstest/commit/941d8ac7ae08ddec7a184f219e6449e065679732"><code>941d8ac</code></a> Update changelog</li>
<li><a href="https://github.com/la10736/rstest/commit/cdff674d16521d71f8aa2a4bb52ad934540ad692"><code>cdff674</code></a> Bump version</li>
<li><a href="https://github.com/la10736/rstest/commit/e0624fe19846ead048135dd1f34faa71319e0748"><code>e0624fe</code></a> Fix clippy warning</li>
<li><a href="https://github.com/la10736/rstest/commit/f7b4b57922e0dd671c793acab424b6bf858737a4"><code>f7b4b57</code></a> Shutup warning on nightly (tests)</li>
<li><a href="https://github.com/la10736/rstest/commit/49a7d3816e51ca9137a8df8985e5abf21548add9"><code>49a7d38</code></a> Shutup warning in night</li>
<li><a href="https://github.com/la10736/rstest/commit/b58ce22ef1cd1a24e78f8ce31b69cf43a3ddf6a3"><code>b58ce22</code></a> Set resolver in virtual manifest</li>
<li><a href="https://github.com/la10736/rstest/commit/3c2fb9c33c0d6fbc7b173f9e9477cea60e3fd59a"><code>3c2fb9c</code></a> Properly handle mutability for awaited futures (<a href="https://redirect.github.com/la10736/rstest/issues/239">#239</a>)</li>
<li><a href="https://github.com/la10736/rstest/commit/61a7007f666803138b2146a41804a375b3bb12cd"><code>61a7007</code></a> We're not interested about msrv for tests</li>
<li>Additional commits viewable in <a href="https://github.com/la10736/rstest/compare/v0.18.0...v0.19.0">compare view</a></li>
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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 20:41:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/276" class=".btn">#276</a>
            </td>
            <td>
                <b>
                    chore(deps): bump github.com/google/uuid from 1.1.1 to 1.6.0 in /wrappers/golang
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/google/uuid](https://github.com/google/uuid) from 1.1.1 to 1.6.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/google/uuid/releases">github.com/google/uuid's releases</a>.</em></p>
<blockquote>
<h2>v1.6.0</h2>
<h2><a href="https://github.com/google/uuid/compare/v1.5.0...v1.6.0">1.6.0</a> (2024-01-16)</h2>
<h3>Features</h3>
<ul>
<li>add Max UUID constant (<a href="https://redirect.github.com/google/uuid/issues/149">#149</a>) (<a href="https://github.com/google/uuid/commit/c58770eb495f55fe2ced6284f93c5158a62e53e3">c58770e</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>fix typo in version 7 uuid documentation (<a href="https://redirect.github.com/google/uuid/issues/153">#153</a>) (<a href="https://github.com/google/uuid/commit/016b199544692f745ffc8867b914129ecb47ef06">016b199</a>)</li>
<li>Monotonicity in UUIDv7 (<a href="https://redirect.github.com/google/uuid/issues/150">#150</a>) (<a href="https://github.com/google/uuid/commit/a2b2b32373ff0b1a312b7fdf6d38a977099698a6">a2b2b32</a>)</li>
</ul>
<h2>v1.5.0</h2>
<h2><a href="https://github.com/google/uuid/compare/v1.4.0...v1.5.0">1.5.0</a> (2023-12-12)</h2>
<h3>Features</h3>
<ul>
<li>Validate UUID without creating new UUID (<a href="https://redirect.github.com/google/uuid/issues/141">#141</a>) (<a href="https://github.com/google/uuid/commit/9ee7366e66c9ad96bab89139418a713dc584ae29">9ee7366</a>)</li>
</ul>
<h2>v1.4.0</h2>
<h2><a href="https://github.com/google/uuid/compare/v1.3.1...v1.4.0">1.4.0</a> (2023-10-26)</h2>
<h3>Features</h3>
<ul>
<li>UUIDs slice type with Strings() convenience method (<a href="https://redirect.github.com/google/uuid/issues/133">#133</a>) (<a href="https://github.com/google/uuid/commit/cd5fbbdd02f3e3467ac18940e07e062be1f864b4">cd5fbbd</a>)</li>
</ul>
<h3>Fixes</h3>
<ul>
<li>Clarify that Parse's job is to parse but not necessarily validate strings. (Documents current behavior)</li>
</ul>
<h2>v1.3.1</h2>
<h2><a href="https://github.com/google/uuid/compare/v1.3.0...v1.3.1">1.3.1</a> (2023-08-18)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>Use .EqualFold() to parse urn prefixed UUIDs (<a href="https://redirect.github.com/google/uuid/issues/118">#118</a>) (<a href="https://github.com/google/uuid/commit/574e6874943741fb99d41764c705173ada5293f0">574e687</a>)</li>
</ul>
<h2>Add randomness pool mode for V4 UUID and NullUUID for SQL Scanners.</h2>
<p>From Andrey Pechkurov:</p>
<p>Adds an optional randomness pool mode for Random (Version 4) UUID generation. The pool contains random bytes read from the random number generator on demand in batches. Enabling the pool may improve the UUID generation throughput significantly.</p>
<p>Since the pool is stored on the Go heap, this feature may be a bad fit for security sensitive applications. That's why it's implemented as an opt-in feature.</p>
<p>From Samuel Roth:</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/google/uuid/blob/master/CHANGELOG.md">github.com/google/uuid's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/google/uuid/compare/v1.5.0...v1.6.0">1.6.0</a> (2024-01-16)</h2>
<h3>Features</h3>
<ul>
<li>add Max UUID constant (<a href="https://redirect.github.com/google/uuid/issues/149">#149</a>) (<a href="https://github.com/google/uuid/commit/c58770eb495f55fe2ced6284f93c5158a62e53e3">c58770e</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>fix typo in version 7 uuid documentation (<a href="https://redirect.github.com/google/uuid/issues/153">#153</a>) (<a href="https://github.com/google/uuid/commit/016b199544692f745ffc8867b914129ecb47ef06">016b199</a>)</li>
<li>Monotonicity in UUIDv7 (<a href="https://redirect.github.com/google/uuid/issues/150">#150</a>) (<a href="https://github.com/google/uuid/commit/a2b2b32373ff0b1a312b7fdf6d38a977099698a6">a2b2b32</a>)</li>
</ul>
<h2><a href="https://github.com/google/uuid/compare/v1.4.0...v1.5.0">1.5.0</a> (2023-12-12)</h2>
<h3>Features</h3>
<ul>
<li>Validate UUID without creating new UUID (<a href="https://redirect.github.com/google/uuid/issues/141">#141</a>) (<a href="https://github.com/google/uuid/commit/9ee7366e66c9ad96bab89139418a713dc584ae29">9ee7366</a>)</li>
</ul>
<h2><a href="https://github.com/google/uuid/compare/v1.3.1...v1.4.0">1.4.0</a> (2023-10-26)</h2>
<h3>Features</h3>
<ul>
<li>UUIDs slice type with Strings() convenience method (<a href="https://redirect.github.com/google/uuid/issues/133">#133</a>) (<a href="https://github.com/google/uuid/commit/cd5fbbdd02f3e3467ac18940e07e062be1f864b4">cd5fbbd</a>)</li>
</ul>
<h3>Fixes</h3>
<ul>
<li>Clarify that Parse's job is to parse but not necessarily validate strings. (Documents current behavior)</li>
</ul>
<h2><a href="https://github.com/google/uuid/compare/v1.3.0...v1.3.1">1.3.1</a> (2023-08-18)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>Use .EqualFold() to parse urn prefixed UUIDs (<a href="https://redirect.github.com/google/uuid/issues/118">#118</a>) (<a href="https://github.com/google/uuid/commit/574e6874943741fb99d41764c705173ada5293f0">574e687</a>)</li>
</ul>
<h2>Changelog</h2>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/google/uuid/commit/0f11ee6918f41a04c201eceeadf612a377bc7fbc"><code>0f11ee6</code></a> chore(master): release 1.6.0 (<a href="https://redirect.github.com/google/uuid/issues/151">#151</a>)</li>
<li><a href="https://github.com/google/uuid/commit/16939dafc37a38d2743810a8bdf60fdad6a0f3a3"><code>16939da</code></a> chore(tests):  add strict monotonicity test case for uuid v7. (<a href="https://redirect.github.com/google/uuid/issues/154">#154</a>)</li>
<li><a href="https://github.com/google/uuid/commit/016b199544692f745ffc8867b914129ecb47ef06"><code>016b199</code></a> fix: fix typo in version 7 uuid documentation (<a href="https://redirect.github.com/google/uuid/issues/153">#153</a>)</li>
<li><a href="https://github.com/google/uuid/commit/1d8b6ea0990d688105843a9a67b1d07222350502"><code>1d8b6ea</code></a> ci: set token permissions to github workflows (<a href="https://redirect.github.com/google/uuid/issues/143">#143</a>)</li>
<li><a href="https://github.com/google/uuid/commit/a2b2b32373ff0b1a312b7fdf6d38a977099698a6"><code>a2b2b32</code></a> fix: Monotonicity in UUIDv7 (<a href="https://redirect.github.com/google/uuid/issues/150">#150</a>)</li>
<li><a href="https://github.com/google/uuid/commit/c58770eb495f55fe2ced6284f93c5158a62e53e3"><code>c58770e</code></a> feat: add Max UUID constant (<a href="https://redirect.github.com/google/uuid/issues/149">#149</a>)</li>
<li><a href="https://github.com/google/uuid/commit/4d47f8eb066f43cfaedd728a543479d9c9dfa8f6"><code>4d47f8e</code></a> chore(master): release 1.5.0 (<a href="https://redirect.github.com/google/uuid/issues/145">#145</a>)</li>
<li><a href="https://github.com/google/uuid/commit/9ee7366e66c9ad96bab89139418a713dc584ae29"><code>9ee7366</code></a> feat: Validate UUID without creating new UUID (<a href="https://redirect.github.com/google/uuid/issues/141">#141</a>)</li>
<li><a href="https://github.com/google/uuid/commit/b35aa6a595277504b1ec94c520d4091ec050b9d5"><code>b35aa6a</code></a> add uuid version 6 and 7 (<a href="https://redirect.github.com/google/uuid/issues/139">#139</a>)</li>
<li><a href="https://github.com/google/uuid/commit/8de8764e294f072b7a2f1a209e88fdcdb1ebc875"><code>8de8764</code></a> chore(master): release 1.4.0 (<a href="https://redirect.github.com/google/uuid/issues/134">#134</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/google/uuid/compare/v1.1.1...v1.6.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/google/uuid&package-manager=go_modules&previous-version=1.1.1&new-version=1.6.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 20:41:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/275" class=".btn">#275</a>
            </td>
            <td>
                <b>
                    chore(deps): bump github.com/mitchellh/mapstructure from 1.3.2 to 1.5.0 in /wrappers/golang
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/mitchellh/mapstructure](https://github.com/mitchellh/mapstructure) from 1.3.2 to 1.5.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/mitchellh/mapstructure/blob/main/CHANGELOG.md">github.com/mitchellh/mapstructure's changelog</a>.</em></p>
<blockquote>
<h2>1.5.0</h2>
<ul>
<li>New option <code>IgnoreUntaggedFields</code> to ignore decoding to any fields
without <code>mapstructure</code> (or the configured tag name) set <a href="https://redirect.github.com/mitchellh/mapstructure/issues/277">GH-277</a></li>
<li>New option <code>ErrorUnset</code> which makes it an error if any fields
in a target struct are not set by the decoding process. <a href="https://redirect.github.com/mitchellh/mapstructure/issues/225">GH-225</a></li>
<li>New function <code>OrComposeDecodeHookFunc</code> to help compose decode hooks. <a href="https://redirect.github.com/mitchellh/mapstructure/issues/240">GH-240</a></li>
<li>Decoding to slice from array no longer crashes <a href="https://redirect.github.com/mitchellh/mapstructure/issues/265">GH-265</a></li>
<li>Decode nested struct pointers to map <a href="https://redirect.github.com/mitchellh/mapstructure/issues/271">GH-271</a></li>
<li>Fix issue where <code>,squash</code> was ignored if <code>Squash</code> option was set. <a href="https://redirect.github.com/mitchellh/mapstructure/issues/280">GH-280</a></li>
<li>Fix issue where fields with <code>,omitempty</code> would sometimes decode
into a map with an empty string key <a href="https://redirect.github.com/mitchellh/mapstructure/issues/281">GH-281</a></li>
</ul>
<h2>1.4.3</h2>
<ul>
<li>Fix cases where <code>json.Number</code> didn't decode properly <a href="https://redirect.github.com/mitchellh/mapstructure/issues/261">GH-261</a></li>
</ul>
<h2>1.4.2</h2>
<ul>
<li>Custom name matchers to support any sort of casing, formatting, etc. for
field names. <a href="https://redirect.github.com/mitchellh/mapstructure/issues/250">GH-250</a></li>
<li>Fix possible panic in ComposeDecodeHookFunc <a href="https://redirect.github.com/mitchellh/mapstructure/issues/251">GH-251</a></li>
</ul>
<h2>1.4.1</h2>
<ul>
<li>Fix regression where <code>*time.Time</code> value would be set to empty and not be sent
to decode hooks properly <a href="https://redirect.github.com/mitchellh/mapstructure/issues/232">GH-232</a></li>
</ul>
<h2>1.4.0</h2>
<ul>
<li>A new decode hook type <code>DecodeHookFuncValue</code> has been added that has
access to the full values. <a href="https://redirect.github.com/mitchellh/mapstructure/issues/183">GH-183</a></li>
<li>Squash is now supported with embedded fields that are struct pointers <a href="https://redirect.github.com/mitchellh/mapstructure/issues/205">GH-205</a></li>
<li>Empty strings will convert to 0 for all numeric types when weakly decoding <a href="https://redirect.github.com/mitchellh/mapstructure/issues/206">GH-206</a></li>
</ul>
<h2>1.3.3</h2>
<ul>
<li>Decoding maps from maps creates a settable value for decode hooks <a href="https://redirect.github.com/mitchellh/mapstructure/issues/203">GH-203</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/mitchellh/mapstructure/commit/ab69d8d93410fce4361f4912bb1ff88110a81311"><code>ab69d8d</code></a> update CHANGELOG to 1.5.0</li>
<li><a href="https://github.com/mitchellh/mapstructure/commit/bd687ea300c090473812a1a5730c3a335fbb5b72"><code>bd687ea</code></a> update CHANGELOG</li>
<li><a href="https://github.com/mitchellh/mapstructure/commit/c9b585b7a79987f1364852f1e2a287c96f16a938"><code>c9b585b</code></a> update test to not rely on fmt</li>
<li><a href="https://github.com/mitchellh/mapstructure/commit/5a2eb615e9aa01976c587b346a0d125072d85256"><code>5a2eb61</code></a> Merge pull request <a href="https://redirect.github.com/mitchellh/mapstructure/issues/281">#281</a> from semrekkers/issue-238</li>
<li><a href="https://github.com/mitchellh/mapstructure/commit/74e07d1cd0c857b2f0736e99e54a27e717d30544"><code>74e07d1</code></a> update CHANGELOG</li>
<li><a href="https://github.com/mitchellh/mapstructure/commit/3a684c784c7e538b03ab7a28dc77cfcf76afb654"><code>3a684c7</code></a> Merge pull request <a href="https://redirect.github.com/mitchellh/mapstructure/issues/240">#240</a> from julnicolas/feature/add_or_compose_decode_hook_func</li>
<li><a href="https://github.com/mitchellh/mapstructure/commit/0bb6a2ebbd99e6d7d6f04c405e7e012adb2947cd"><code>0bb6a2e</code></a> Merge branch 'master' into feature/add_or_compose_decode_hook_func</li>
<li><a href="https://github.com/mitchellh/mapstructure/commit/ac10e2295c8477c1d3467c400450b6c1db6299f0"><code>ac10e22</code></a> update CHANGELOG</li>
<li><a href="https://github.com/mitchellh/mapstructure/commit/8385cfade656c903b73c3c30afd7a3c1fa905008"><code>8385cfa</code></a> Merge pull request <a href="https://redirect.github.com/mitchellh/mapstructure/issues/225">#225</a> from SaschaRoland/unset-fields</li>
<li><a href="https://github.com/mitchellh/mapstructure/commit/17e49ec5580fac6eab31ac606f49270f5590454a"><code>17e49ec</code></a> update CHANGELOG</li>
<li>Additional commits viewable in <a href="https://github.com/mitchellh/mapstructure/compare/v1.3.2...v1.5.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/mitchellh/mapstructure&package-manager=go_modules&previous-version=1.3.2&new-version=1.5.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 20:41:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/274" class=".btn">#274</a>
            </td>
            <td>
                <b>
                    chore(deps): bump rust from 1.41-slim to 1.78-slim in /docker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps rust from 1.41-slim to 1.78-slim.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=rust&package-manager=docker&previous-version=1.41-slim&new-version=1.78-slim)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 20:41:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/273" class=".btn">#273</a>
            </td>
            <td>
                <b>
                    chore(deps): bump github.com/stretchr/testify from 1.6.1 to 1.9.0 in /wrappers/golang
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/stretchr/testify](https://github.com/stretchr/testify) from 1.6.1 to 1.9.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/stretchr/testify/releases">github.com/stretchr/testify's releases</a>.</em></p>
<blockquote>
<h2>v1.9.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix Go modules version by <a href="https://github.com/SuperQ"><code>@​SuperQ</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1394">stretchr/testify#1394</a></li>
<li>Document that require is not safe to call in created goroutines by <a href="https://github.com/programmer04"><code>@​programmer04</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1392">stretchr/testify#1392</a></li>
<li>Remove myself from MAINTAINERS.md by <a href="https://github.com/mvdkleijn"><code>@​mvdkleijn</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1367">stretchr/testify#1367</a></li>
<li>Correct spelling/grammar by <a href="https://github.com/echarrod"><code>@​echarrod</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1389">stretchr/testify#1389</a></li>
<li>docs: Update URLs in README by <a href="https://github.com/davidjb"><code>@​davidjb</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1349">stretchr/testify#1349</a></li>
<li>Update mockery link to Github Pages in README by <a href="https://github.com/LandonTClipp"><code>@​LandonTClipp</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1346">stretchr/testify#1346</a></li>
<li>docs: Fix typos in tests and comments by <a href="https://github.com/alexandear"><code>@​alexandear</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1410">stretchr/testify#1410</a></li>
<li>CI: tests from go1.17 by <a href="https://github.com/SuperQ"><code>@​SuperQ</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1409">stretchr/testify#1409</a></li>
<li>Fix adding ? when no values passed by <a href="https://github.com/lesichkovm"><code>@​lesichkovm</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1320">stretchr/testify#1320</a></li>
<li>codegen: use standard header for generated files by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1406">stretchr/testify#1406</a></li>
<li>mock: AssertExpectations log reason only on failure by <a href="https://github.com/hikyaru-suzuki"><code>@​hikyaru-suzuki</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1360">stretchr/testify#1360</a></li>
<li>assert: fix flaky TestNeverTrue by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1417">stretchr/testify#1417</a></li>
<li>README: fix typos &quot;set up&quot; vs &quot;setup&quot; by <a href="https://github.com/ossan-dev"><code>@​ossan-dev</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1428">stretchr/testify#1428</a></li>
<li>mock: move regexp compilation outside of <code>Called</code> by <a href="https://github.com/aud10slave"><code>@​aud10slave</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/631">stretchr/testify#631</a></li>
<li>assert: refactor internal func getLen() by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1445">stretchr/testify#1445</a></li>
<li>mock: deprecate type AnythingOfTypeArgument (<a href="https://redirect.github.com/stretchr/testify/issues/1434">#1434</a>) by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1441">stretchr/testify#1441</a></li>
<li>Remove no longer needed assert.canConvert by <a href="https://github.com/alexandear"><code>@​alexandear</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1470">stretchr/testify#1470</a></li>
<li>assert: ObjectsAreEqual: use time.Equal for time.Time types by <a href="https://github.com/tscales"><code>@​tscales</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1464">stretchr/testify#1464</a></li>
<li>Bump actions/checkout from 3 to 4 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1466">stretchr/testify#1466</a></li>
<li>Bump actions/setup-go from 3.2.0 to 4.1.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1451">stretchr/testify#1451</a></li>
<li>fix: make EventuallyWithT concurrency safe by <a href="https://github.com/czeslavo"><code>@​czeslavo</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1395">stretchr/testify#1395</a></li>
<li>assert: fix httpCode and HTTPBody occur panic when http.Handler read Body by <a href="https://github.com/hidu"><code>@​hidu</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1484">stretchr/testify#1484</a></li>
<li>assert.EqualExportedValues: fix handling of arrays by <a href="https://github.com/zrbecker"><code>@​zrbecker</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1473">stretchr/testify#1473</a></li>
<li>.github: use latest Go versions by <a href="https://github.com/kevinburkesegment"><code>@​kevinburkesegment</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1489">stretchr/testify#1489</a></li>
<li>assert: Deprecate EqualExportedValues by <a href="https://github.com/HaraldNordgren"><code>@​HaraldNordgren</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1488">stretchr/testify#1488</a></li>
<li>suite: refactor test assertions by <a href="https://github.com/alexandear"><code>@​alexandear</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1474">stretchr/testify#1474</a></li>
<li>suite: fix SetupSubTest and TearDownSubTest execution order by <a href="https://github.com/linusbarth"><code>@​linusbarth</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1471">stretchr/testify#1471</a></li>
<li>docs: Fix deprecation comments for http package by <a href="https://github.com/alexandear"><code>@​alexandear</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1335">stretchr/testify#1335</a></li>
<li>Add map support doc comments to Subset and NotSubset by <a href="https://github.com/jedevc"><code>@​jedevc</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1306">stretchr/testify#1306</a></li>
<li>TestErrorIs/TestNotErrorIs: check error message contents by <a href="https://github.com/craig65535"><code>@​craig65535</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1435">stretchr/testify#1435</a></li>
<li>suite: fix subtest names (fix <a href="https://redirect.github.com/stretchr/testify/issues/1501">#1501</a>) by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1504">stretchr/testify#1504</a></li>
<li>assert: improve unsafe.Pointer tests by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1505">stretchr/testify#1505</a></li>
<li>assert: simplify isNil implementation by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1506">stretchr/testify#1506</a></li>
<li>assert.InEpsilonSlice: fix expected/actual order and other improvements by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1483">stretchr/testify#1483</a></li>
<li>Fix dependency cycle with objx <a href="https://redirect.github.com/stretchr/testify/issues/1292">#1292</a> by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1453">stretchr/testify#1453</a></li>
<li>mock: refactor TestIsArgsEqual by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1444">stretchr/testify#1444</a></li>
<li>mock: optimize argument matching checks by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1416">stretchr/testify#1416</a></li>
<li>assert: fix TestEventuallyTimeout by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1412">stretchr/testify#1412</a></li>
<li>CI: add go 1.21 in GitHub Actions by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1450">stretchr/testify#1450</a></li>
<li>suite: fix recoverAndFailOnPanic to report test failure at the right location by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1502">stretchr/testify#1502</a></li>
<li>Update maintainers by <a href="https://github.com/brackendawson"><code>@​brackendawson</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1533">stretchr/testify#1533</a></li>
<li>assert: Fix EqualValues to handle overflow/underflow by <a href="https://github.com/arjunmahishi"><code>@​arjunmahishi</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1531">stretchr/testify#1531</a></li>
<li>assert: better formatting for Len() error by <a href="https://github.com/kevinburkesegment"><code>@​kevinburkesegment</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1485">stretchr/testify#1485</a></li>
<li>Ensure AssertExpectations does not fail in skipped tests by <a href="https://github.com/ianrose14"><code>@​ianrose14</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1331">stretchr/testify#1331</a></li>
<li>suite: fix deadlock in suite.Require()/Assert() by <a href="https://github.com/arjunmahishi"><code>@​arjunmahishi</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1535">stretchr/testify#1535</a></li>
<li>Revert &quot;assert: ObjectsAreEqual: use time.Equal for time.Time type&quot; by <a href="https://github.com/brackendawson"><code>@​brackendawson</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1537">stretchr/testify#1537</a></li>
<li>[chore] Add issue templates by <a href="https://github.com/arjunmahishi"><code>@​arjunmahishi</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1538">stretchr/testify#1538</a></li>
<li>Update the build status badge by <a href="https://github.com/brackendawson"><code>@​brackendawson</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1540">stretchr/testify#1540</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/stretchr/testify/commit/bb548d0473d4e1c9b7bbfd6602c7bf12f7a84dd2"><code>bb548d0</code></a> Merge pull request <a href="https://redirect.github.com/stretchr/testify/issues/1552">#1552</a> from stretchr/dependabot/go_modules/github.com/stret...</li>
<li><a href="https://github.com/stretchr/testify/commit/814075f391adffd2bf2b5110a74c51827ba132c4"><code>814075f</code></a> build(deps): bump github.com/stretchr/objx from 0.5.1 to 0.5.2</li>
<li><a href="https://github.com/stretchr/testify/commit/e0456122451b1839c8d58d32df6364e4d0f0a709"><code>e045612</code></a> Merge pull request <a href="https://redirect.github.com/stretchr/testify/issues/1339">#1339</a> from bogdandrutu/uintptr</li>
<li><a href="https://github.com/stretchr/testify/commit/5b6926d686d412518f50e888b9ae9b938355e011"><code>5b6926d</code></a> Merge pull request <a href="https://redirect.github.com/stretchr/testify/issues/1385">#1385</a> from hslatman/not-implements</li>
<li><a href="https://github.com/stretchr/testify/commit/9f97d67703eff02136d487e6c907e76fdea31a8b"><code>9f97d67</code></a> Merge pull request <a href="https://redirect.github.com/stretchr/testify/issues/1550">#1550</a> from stretchr/release-notes</li>
<li><a href="https://github.com/stretchr/testify/commit/bcb0d3fe49ff300fb78288cc144bc61a881f58ec"><code>bcb0d3f</code></a> Include the auto-release notes in releases</li>
<li><a href="https://github.com/stretchr/testify/commit/fb770f8238261aa22f8e0c56f18168ccb90f4a09"><code>fb770f8</code></a> Merge pull request <a href="https://redirect.github.com/stretchr/testify/issues/1247">#1247</a> from ccoVeille/typos</li>
<li><a href="https://github.com/stretchr/testify/commit/85d8bb6eea715dcbbb68f7c87b50e1956e20f892"><code>85d8bb6</code></a> fix typos in comments, tests and github templates</li>
<li><a href="https://github.com/stretchr/testify/commit/e2741fa4e9bf2fdfe3ed48d976a7eeebe76c5009"><code>e2741fa</code></a> Merge pull request <a href="https://redirect.github.com/stretchr/testify/issues/1548">#1548</a> from arjunmahishi/msgAndArgs</li>
<li><a href="https://github.com/stretchr/testify/commit/6e59f20c0d3883d2bdc589a9e48374ea30601851"><code>6e59f20</code></a> http_assertions: assert that the msgAndArgs actually works in tests</li>
<li>Additional commits viewable in <a href="https://github.com/stretchr/testify/compare/v1.6.1...v1.9.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/stretchr/testify&package-manager=go_modules&previous-version=1.6.1&new-version=1.9.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 20:41:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/272" class=".btn">#272</a>
            </td>
            <td>
                <b>
                    chore: update minSdkVersion to get the project version or fallback to 21
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the react-native wrapper to get the minSdkVersion from the project config or fallback to the current hardcoded version. @TimoGlastra @berendsliedrecht 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 08:53:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/271" class=".btn">#271</a>
            </td>
            <td>
                <b>
                    chore: updating dependabot file to support gha, TS, JS, gradle, Go lang, cargo and docker packages
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
        Created At 2024-05-10 15:59:32 +0000 UTC
    </div>
</div>

