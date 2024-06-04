---
layout: default
title: aries-agent-test-harness
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-agent-test-harness
---

# aries-agent-test-harness <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-agent-test-harness){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/830" class=".btn">#830</a>
            </td>
            <td>
                <b>
                    Bump prettier from 2.8.8 to 3.3.0 in /aries-backchannels/javascript/server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [prettier](https://github.com/prettier/prettier) from 2.8.8 to 3.3.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/prettier/prettier/releases">prettier's releases</a>.</em></p>
<blockquote>
<h2>3.3.0</h2>
<p><a href="https://github.com/prettier/prettier/compare/3.2.5...3.3.0">diff</a></p>
<p>🔗 <a href="https://prettier.io/blog/2024/06/01/3.3.0.html">Release note</a></p>
<h2>3.2.5</h2>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#325">Changelog</a></p>
<h2>3.2.4</h2>
<ul>
<li>Fix <code>.eslintrc.json</code> format <a href="https://redirect.github.com/prettier/prettier/issues/15947">#15947</a></li>
</ul>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#324">Changelog</a></p>
<h2>3.2.3</h2>
<ul>
<li>Format <code>tsconfig.json</code> file with <code>jsonc</code> parser <a href="https://redirect.github.com/prettier/prettier/issues/15927">#15927</a></li>
</ul>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#323">Changelog</a></p>
<h2>3.2.2</h2>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#322">Changelog</a></p>
<h2>3.2.1</h2>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#321">Changelog</a></p>
<h2>3.2.0</h2>
<p><a href="https://github.com/prettier/prettier/compare/3.1.1...3.2.0">diff</a></p>
<p>🔗 <a href="https://prettier.io/blog/2024/01/12/3.2.0.html">Release note</a></p>
<h2>3.1.1</h2>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#311">Changelog</a></p>
<h2>3.1.0</h2>
<p><a href="https://github.com/prettier/prettier/compare/3.0.3...3.1.0">diff</a></p>
<p>🔗 <a href="https://prettier.io/blog/2023/11/13/3.1.0.html">Release note</a></p>
<h2>3.0.3</h2>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#303">Changelog</a></p>
<h2>3.0.2</h2>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#302">Changelog</a></p>
<h2>3.0.1</h2>
<p>🔗 <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md#301">Changelog</a></p>
<h2>3.0.0</h2>
<p><a href="https://github.com/prettier/prettier/compare/3.0.0-alpha.6...3.0.0">diff</a></p>
<p>🔗 <a href="https://prettier.io/blog/2023/07/05/3.0.0.html">Release note</a></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/prettier/prettier/blob/main/CHANGELOG.md">prettier's changelog</a>.</em></p>
<blockquote>
<h1>3.3.0</h1>
<p><a href="https://github.com/prettier/prettier/compare/3.2.5...3.3.0">diff</a></p>
<p>🔗 <a href="https://prettier.io/blog/2024/06/01/3.3.0.html">Release Notes</a></p>
<h1>3.2.5</h1>
<p><a href="https://github.com/prettier/prettier/compare/3.2.4...3.2.5">diff</a></p>
<h4>Support Angular inline styles as single template literal (<a href="https://redirect.github.com/prettier/prettier/pull/15968">#15968</a> by <a href="https://github.com/sosukesuzuki"><code>@​sosukesuzuki</code></a>)</h4>
<p><a href="https://blog.angular.io/introducing-angular-v17-4d7033312e4b">Angular v17</a> supports single string inline styles.</p>
<!-- raw HTML omitted -->
<pre lang="ts"><code>// Input
@Component({
  template: `&lt;div&gt;...&lt;/div&gt;`,
  styles: `h1 { color: blue; }`,
})
export class AppComponent {}
<p>// Prettier 3.2.4
<a href="https://github.com/Component"><code>@​Component</code></a>({
template: <code>&amp;lt;div&amp;gt;...&amp;lt;/div&amp;gt;</code>,
styles: <code>h1 { color: blue; }</code>,
})
export class AppComponent {}</p>
<p>// Prettier 3.2.5
<a href="https://github.com/Component"><code>@​Component</code></a>({
template: <code>&amp;lt;div&amp;gt;...&amp;lt;/div&amp;gt;</code>,
styles: <code>h1 { color: blue; }</code>,
})
export class AppComponent {}</p>
<p></code></pre></p>
<h4>Unexpected embedded formatting for Angular template (<a href="https://redirect.github.com/prettier/prettier/pull/15969">#15969</a> by <a href="https://github.com/JounQin"><code>@​JounQin</code></a>)</h4>
<p>Computed template should not be considered as Angular component template</p>
<!-- raw HTML omitted -->
<pre lang="ts"><code>// Input
&lt;/tr&gt;&lt;/table&gt; 
</code></pre>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/prettier/prettier/commit/c4ab460357478d2b847c60a1efb40098b1181931"><code>c4ab460</code></a> Release 3.3.0</li>
<li><a href="https://github.com/prettier/prettier/commit/8a88cdce6d4605f206305ebb9204a0cabf96a070"><code>8a88cdc</code></a> Respect <code>trailingComma</code> in angular templates (<a href="https://redirect.github.com/prettier/prettier/issues/15926">#15926</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/c2e20fbae8ce1800ac0c8242c176d9379db5c001"><code>c2e20fb</code></a> chore(deps): update babel to v7.24.6 (<a href="https://redirect.github.com/prettier/prettier/issues/16326">#16326</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/41f1dffed08b33fe6d43da1e82d798b23ba0b57c"><code>41f1dff</code></a> Add newline between markdown footnote definitions (<a href="https://redirect.github.com/prettier/prettier/issues/16063">#16063</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/da5ad84bf441afd5c157bf83840814b1deaa39b1"><code>da5ad84</code></a> chore(deps): update babel to v7.24.6 (<a href="https://redirect.github.com/prettier/prettier/issues/16325">#16325</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/f790be81319a70f08942b1e3c12d68ee392d3269"><code>f790be8</code></a> chore(deps): update dependency file-entry-cache to v9 (<a href="https://redirect.github.com/prettier/prettier/issues/16324">#16324</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/7250556e287922508d9f28c12a82165a60bab5d7"><code>7250556</code></a> chore(deps): update dependency meriyah to v4.4.3 (<a href="https://redirect.github.com/prettier/prettier/issues/16323">#16323</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/96e057a0dc1efa7247b1c50843c9422a0ed66900"><code>96e057a</code></a> chore(deps): update dependency <code>@​angular/compiler</code> to v18 (<a href="https://redirect.github.com/prettier/prettier/issues/16322">#16322</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/a4ea5a2e2fcebe72315c9c0523b35bc79fe91405"><code>a4ea5a2</code></a> chore(deps): update dependency eslint-plugin-regexp to v2.6.0 (<a href="https://redirect.github.com/prettier/prettier/issues/16320">#16320</a>)</li>
<li><a href="https://github.com/prettier/prettier/commit/229006cd5b5178c195e5d66ce924d2b58bfde4ef"><code>229006c</code></a> chore(deps): update dependency micromatch to v4.0.7 (<a href="https://redirect.github.com/prettier/prettier/issues/16319">#16319</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/prettier/prettier/compare/2.8.8...3.3.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=prettier&package-manager=npm_and_yarn&previous-version=2.8.8&new-version=3.3.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-03 11:19:05 +0000 UTC
    </div>
</div>

